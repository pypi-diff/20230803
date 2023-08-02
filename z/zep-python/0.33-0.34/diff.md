# Comparing `tmp/zep_python-0.33.tar.gz` & `tmp/zep_python-0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.33.tar", max compression
+gzip compressed data, was "zep_python-0.34.tar", max compression
```

## Comparing `zep_python-0.33.tar` & `zep_python-0.34.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-07-12 15:27:19.852473 zep_python-0.33/LICENSE
--rw-r--r--   0        0        0     2402 2023-07-12 15:27:19.852473 zep_python-0.33/README.md
--rw-r--r--   0        0        0      872 2023-07-12 15:27:19.856473 zep_python-0.33/pyproject.toml
--rw-r--r--   0        0        0      389 2023-07-12 15:27:19.856473 zep_python-0.33/zep_python/__init__.py
--rw-r--r--   0        0        0     2234 2023-07-12 15:27:19.856473 zep_python-0.33/zep_python/exceptions.py
--rw-r--r--   0        0        0     5855 2023-07-12 15:27:19.856473 zep_python-0.33/zep_python/models.py
--rw-r--r--   0        0        0        0 2023-07-12 15:27:19.856473 zep_python-0.33/zep_python/py.typed
--rw-r--r--   0        0        0    18158 2023-07-12 15:27:19.856473 zep_python-0.33/zep_python/zep_client.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 zep_python-0.33/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 23:15:07.689601 zep_python-0.34/LICENSE
+-rw-r--r--   0        0        0     2402 2023-08-02 23:15:07.689601 zep_python-0.34/README.md
+-rw-r--r--   0        0        0      872 2023-08-02 23:15:07.693601 zep_python-0.34/pyproject.toml
+-rw-r--r--   0        0        0      417 2023-08-02 23:15:07.693601 zep_python-0.34/zep_python/__init__.py
+-rw-r--r--   0        0        0     2234 2023-08-02 23:15:07.693601 zep_python-0.34/zep_python/exceptions.py
+-rw-r--r--   0        0        0     5855 2023-08-02 23:15:07.693601 zep_python-0.34/zep_python/models.py
+-rw-r--r--   0        0        0        0 2023-08-02 23:15:07.693601 zep_python-0.34/zep_python/py.typed
+-rw-r--r--   0        0        0    19426 2023-08-02 23:15:07.693601 zep_python-0.34/zep_python/zep_client.py
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 zep_python-0.34/PKG-INFO
```

### Comparing `zep_python-0.33/LICENSE` & `zep_python-0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.33/README.md` & `zep_python-0.34/README.md`

 * *Files identical despite different names*

### Comparing `zep_python-0.33/pyproject.toml` & `zep_python-0.34/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zep-python"
-version = "0.33"
+version = "0.34"
 description = "Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service."
 authors = ["Daniel Chalef <daniel.chalef@private.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.24.0"
```

### Comparing `zep_python-0.33/zep_python/exceptions.py` & `zep_python-0.34/zep_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.33/zep_python/models.py` & `zep_python-0.34/zep_python/models.py`

 * *Files identical despite different names*

### Comparing `zep_python-0.33/zep_python/zep_client.py` & `zep_python-0.34/zep_python/zep_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,22 +59,24 @@
             The API key to use for authentication. (optional)
         """
 
         headers: Dict[str, str] = {}
         if api_key is not None:
             headers["Authorization"] = f"Bearer {api_key}"
 
-        self.base_url = urljoin(base_url, API_BASE_PATH)
+        self.base_url = concat_url(base_url, API_BASE_PATH)
         self.aclient = httpx.AsyncClient(
             base_url=self.base_url, headers=headers, timeout=API_TIMEOUT
         )
         self.client = httpx.Client(
             base_url=self.base_url, headers=headers, timeout=API_TIMEOUT
         )
 
+        self._healthcheck(base_url)
+
     async def __aenter__(self) -> "ZepClient":
         """Asynchronous context manager entry point"""
         return self
 
     async def __aexit__(
         self,
         exc_type: Type[Exception],
@@ -137,14 +139,42 @@
 
     def _gen_get_params(self, lastn: Optional[int] = None) -> Dict[str, Any]:
         params = {}
         if lastn is not None:
             params["lastn"] = lastn
         return params
 
+    def _healthcheck(self, base_url: str) -> None:
+        """
+        Check that the Zep server is running and the API URL is correct.
+
+        Raises
+        ------
+        ConnectionError
+            If the server is not running or the API URL is incorrect.
+        """
+
+        url = concat_url(base_url, "/healthz")
+
+        error_msg = """Failed to connect to Zep server. Please check that:
+         - the server is running 
+         - the API URL is correct
+         - No other process is using the same port"""
+
+        try:
+            response = httpx.get(url)
+
+            self._handle_response(response, error_msg)
+
+            if response.status_code == 200 and response.text != ".":
+                raise APIError(response, error_msg)
+
+        except (httpx.ConnectError, httpx.NetworkError, httpx.TimeoutException) as e:
+            raise APIError(None, error_msg) from e
+
     def get_session(self, session_id: str) -> Session:
         """
         Retrieve the session with the specified ID.
 
         Parameters
         ----------
         session_id : str
@@ -599,7 +629,26 @@
         """
         Close the HTTP client.
 
         [Optional] This method may be called when the ZepClient is no longer needed to
         release resources.
         """
         self.client.close()
+
+
+def concat_url(base_url: str, path: str) -> str:
+    """
+    Join the specified base URL and path.
+
+    Parameters
+    ----------
+    base_url : str
+        The base URL to join.
+    path : str
+        The path to join.
+
+    Returns
+    -------
+    str
+        The joined URL.
+    """
+    return urljoin(base_url + "/", path.lstrip("/"))
```

### Comparing `zep_python-0.33/PKG-INFO` & `zep_python-0.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zep-python
-Version: 0.33
+Version: 0.34
 Summary: Zep stores, manages, enriches, indexes, and searches long-term memory for conversational AI applications. This is the Python client for the Zep service.
 Author: Daniel Chalef
 Author-email: daniel.chalef@private.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

