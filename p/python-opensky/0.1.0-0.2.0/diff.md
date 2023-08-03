# Comparing `tmp/python_opensky-0.1.0.tar.gz` & `tmp/python_opensky-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_opensky-0.1.0.tar", max compression
+gzip compressed data, was "python_opensky-0.2.0.tar", max compression
```

## Comparing `python_opensky-0.1.0.tar` & `python_opensky-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-07-28 10:26:54.231170 python_opensky-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     5321 2023-07-28 10:26:54.231170 python_opensky-0.1.0/README.md
--rw-r--r--   0        0        0     3661 2023-07-28 10:27:11.628697 python_opensky-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      444 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/__init__.py
--rw-r--r--   0        0        0      849 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/const.py
--rw-r--r--   0        0        0      384 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/exceptions.py
--rw-r--r--   0        0        0     3714 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/models.py
--rw-r--r--   0        0        0     9397 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/opensky.py
--rw-r--r--   0        0        0        0 2023-07-28 10:26:54.235170 python_opensky-0.1.0/src/python_opensky/py.typed
--rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 python_opensky-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-08-03 12:34:32.065166 python_opensky-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     5321 2023-08-03 12:34:32.065166 python_opensky-0.2.0/README.md
+-rw-r--r--   0        0        0     3661 2023-08-03 12:34:51.214326 python_opensky-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      444 2023-08-03 12:34:32.069167 python_opensky-0.2.0/src/python_opensky/__init__.py
+-rw-r--r--   0        0        0      849 2023-08-03 12:34:32.069167 python_opensky-0.2.0/src/python_opensky/const.py
+-rw-r--r--   0        0        0      384 2023-08-03 12:34:32.069167 python_opensky-0.2.0/src/python_opensky/exceptions.py
+-rw-r--r--   0        0        0     3714 2023-08-03 12:34:32.069167 python_opensky-0.2.0/src/python_opensky/models.py
+-rw-r--r--   0        0        0    10092 2023-08-03 12:34:32.069167 python_opensky-0.2.0/src/python_opensky/opensky.py
+-rw-r--r--   0        0        0        0 2023-08-03 12:34:32.069167 python_opensky-0.2.0/src/python_opensky/py.typed
+-rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 python_opensky-0.2.0/PKG-INFO
```

### Comparing `python_opensky-0.1.0/LICENSE.md` & `python_opensky-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.1.0/README.md` & `python_opensky-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.1.0/pyproject.toml` & `python_opensky-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python_opensky"
-version = "0.1.0"
+version = "0.2.0"
 description = "Asynchronous Python client for Opensky API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-opensky"
 repository = "https://github.com/joostlek/python-opensky"
@@ -40,15 +40,15 @@
 mypy = "1.4.1"
 pre-commit = "3.3.3"
 pre-commit-hooks = "4.4.0"
 pylint = "2.17.5"
 pytest = "7.4.0"
 pytest-asyncio = "0.21.1"
 pytest-cov = "4.1.0"
-ruff = "0.0.280"
+ruff = "0.0.282"
 safety = "2.4.0b1"
 yamllint = "1.32.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/joostlek/python-opensky/issues"
 Changelog = "https://github.com/joostlek/python-opensky/releases"
```

### Comparing `python_opensky-0.1.0/src/python_opensky/const.py` & `python_opensky-0.2.0/src/python_opensky/const.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.1.0/src/python_opensky/models.py` & `python_opensky-0.2.0/src/python_opensky/models.py`

 * *Files identical despite different names*

### Comparing `python_opensky-0.1.0/src/python_opensky/opensky.py` & `python_opensky-0.2.0/src/python_opensky/opensky.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,23 +33,43 @@
     opensky_credits: int = 400
     timezone = timezone.utc
     _close_session: bool = False
     _credit_usage: dict[datetime, int] = field(default_factory=dict)
     _auth: BasicAuth | None = None
     _contributing_user: bool = False
 
-    def authenticate(self, auth: BasicAuth, *, contributing_user: bool = False) -> None:
+    async def authenticate(
+        self,
+        auth: BasicAuth,
+        *,
+        contributing_user: bool = False,
+    ) -> None:
         """Authenticate the user."""
         self._auth = auth
+        try:
+            await self.get_states()
+        except OpenSkyUnauthenticatedError as exc:
+            self._auth = None
+            raise OpenSkyUnauthenticatedError from exc
         self._contributing_user = contributing_user
         if contributing_user:
             self.opensky_credits = 8000
         else:
             self.opensky_credits = 4000
 
+    @property
+    def is_contributing_user(self) -> bool:
+        """Return if the user is contributing to OpenSky."""
+        return self._contributing_user
+
+    @property
+    def is_authenticated(self) -> bool:
+        """Return if the user is correctly authenticated."""
+        return self._auth is not None
+
     async def _request(
         self,
         uri: str,
         *,
         data: dict[str, Any] | None = None,
     ) -> dict[str, Any]:
         """Handle a request to OpenSky.
@@ -103,14 +123,16 @@
             msg = "Timeout occurred while connecting to the OpenSky API"
             raise OpenSkyConnectionError(msg) from exception
         except (
             ClientError,
             ClientResponseError,
             socket.gaierror,
         ) as exception:
+            if isinstance(exception, ClientResponseError) and exception.status == 401:
+                raise OpenSkyUnauthenticatedError from exception
             msg = "Error occurred while communicating with OpenSky API"
             raise OpenSkyConnectionError(msg) from exception
 
         content_type = response.headers.get("Content-Type", "")
 
         if "application/json" not in content_type:
             text = await response.text()
```

### Comparing `python_opensky-0.1.0/PKG-INFO` & `python_opensky-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-opensky
-Version: 0.1.0
+Version: 0.2.0
 Summary: Asynchronous Python client for Opensky API.
 Home-page: https://github.com/joostlek/python-opensky
 License: MIT
 Keywords: opensky,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
```

