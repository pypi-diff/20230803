# Comparing `tmp/xiaomitv-0.9.1.tar.gz` & `tmp/xiaomitv-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaomitv-0.9.1.tar", last modified: Wed Aug  2 11:34:09 2023, max compression
+gzip compressed data, was "xiaomitv-0.9.2.tar", last modified: Thu Aug  3 02:51:38 2023, max compression
```

## Comparing `xiaomitv-0.9.1.tar` & `xiaomitv-0.9.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 11:34:09.349886 xiaomitv-0.9.1/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 xiaomitv-0.9.1/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      555 2023-08-02 11:34:09.349886 xiaomitv-0.9.1/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       12 2023-08-02 03:55:35.000000 xiaomitv-0.9.1/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      676 2023-08-02 11:33:38.000000 xiaomitv-0.9.1/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-08-02 11:34:09.349886 xiaomitv-0.9.1/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 11:34:09.345886 xiaomitv-0.9.1/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 11:34:09.345886 xiaomitv-0.9.1/src/xiaomitv/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4508 2023-08-02 09:41:56.000000 xiaomitv-0.9.1/src/xiaomitv/__init__.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-02 11:34:09.349886 xiaomitv-0.9.1/src/xiaomitv.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      555 2023-08-02 11:34:09.000000 xiaomitv-0.9.1/src/xiaomitv.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      236 2023-08-02 11:34:09.000000 xiaomitv-0.9.1/src/xiaomitv.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-08-02 11:34:09.000000 xiaomitv-0.9.1/src/xiaomitv.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       15 2023-08-02 11:34:09.000000 xiaomitv-0.9.1/src/xiaomitv.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        9 2023-08-02 11:34:09.000000 xiaomitv-0.9.1/src/xiaomitv.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-03 02:51:38.626547 xiaomitv-0.9.2/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 xiaomitv-0.9.2/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      555 2023-08-03 02:51:38.626547 xiaomitv-0.9.2/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       12 2023-08-02 03:55:35.000000 xiaomitv-0.9.2/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      676 2023-08-03 02:46:34.000000 xiaomitv-0.9.2/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-08-03 02:51:38.626547 xiaomitv-0.9.2/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-03 02:51:38.618548 xiaomitv-0.9.2/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-03 02:51:38.622547 xiaomitv-0.9.2/src/xiaomitv/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     4422 2023-08-03 02:47:46.000000 xiaomitv-0.9.2/src/xiaomitv/__init__.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-08-03 02:51:38.622547 xiaomitv-0.9.2/src/xiaomitv.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      555 2023-08-03 02:51:38.000000 xiaomitv-0.9.2/src/xiaomitv.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      236 2023-08-03 02:51:38.000000 xiaomitv-0.9.2/src/xiaomitv.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-08-03 02:51:38.000000 xiaomitv-0.9.2/src/xiaomitv.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       15 2023-08-03 02:51:38.000000 xiaomitv-0.9.2/src/xiaomitv.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        9 2023-08-03 02:51:38.000000 xiaomitv-0.9.2/src/xiaomitv.egg-info/top_level.txt
```

### Comparing `xiaomitv-0.9.1/LICENSE` & `xiaomitv-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaomitv-0.9.1/PKG-INFO` & `xiaomitv-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaomitv
-Version: 0.9.1
+Version: 0.9.2
 Summary: Remote control for Xiaomi TVs
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/xiaomitv
 Project-URL: Bug Tracker, https://github.com/zhbjsh/xiaomitv/issues
 Keywords: xiaomi tv,mi tv,xiaomi,remote control
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xiaomitv-0.9.1/pyproject.toml` & `xiaomitv-0.9.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xiaomitv"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Remote control for Xiaomi TVs"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,13 +19,13 @@
 keywords = [
   "xiaomi tv",
   "mi tv",
   "xiaomi",
   "remote control",
 ]
 dependencies = [
-  "aiohttp >= 3.0.0",
+  "aiohttp >= 3.8.5",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/xiaomitv"
 "Bug Tracker" = "https://github.com/zhbjsh/xiaomitv/issues"
```

### Comparing `xiaomitv-0.9.1/src/xiaomitv/__init__.py` & `xiaomitv-0.9.2/src/xiaomitv/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 class Key:
     POWER = "power"
     UP = "up"
     DOWN = "down"
     LEFT = "left"
     RIGHT = "right"
     ENTER = "enter"
-    HOME = "home"
-    BACK = "back"
     MENU = "menu"
+    BACK = "back"
+    HOME = "home"
     VOLUME_UP = "volumeup"
     VOLUME_DOWN = "volumedown"
 
 
 class SystemState:
     def __init__(self, data: dict) -> None:
         self.name: str = data["devicename"]
@@ -62,30 +62,36 @@
     def __init__(
         self,
         host: str,
         *,
         port: int = PORT,
         timeout: int = TIMEOUT,
     ) -> None:
-        self._host = host
-        self._port = port
-        self._timeout = timeout
+        self._session = aiohttp.ClientSession(
+            f"http://{host}:{port}",
+            timeout=aiohttp.ClientTimeout(timeout),
+        )
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, *args):
+        await self.async_close()
 
     async def _async_send_request(self, string: str) -> dict:
-        if not self._session:
-            self._session = aiohttp.ClientSession(
-                f"http://{self._host}:{self._port}",
-                timeout=aiohttp.ClientTimeout(self._timeout),
-            )
         try:
             async with self._session.get(string) as response:
                 return json.loads(await response.text())["data"]
         except Exception as exc:
             raise RequestError("Request failed") from exc
 
+    async def async_close(self):
+        """Close."""
+        await self._session.close()
+
     async def async_get_system_state(self) -> SystemState:
         """Get the system state."""
         data = await self._async_send_request("/request?action=isalive")
         return SystemState(data)
 
     async def async_get_system_info(self) -> SystemInfo:
         """Get the system info."""
@@ -128,16 +134,10 @@
             if diff < 0:
                 await self.async_press_key(Key.VOLUME_UP)
                 diff += 1
             else:
                 await self.async_press_key(Key.VOLUME_DOWN)
                 diff -= 1
 
-    async def async_close(self):
-        """Close."""
-        if self._session:
-            await self._session.close()
-            self._session = None
-
 
 class RequestError(Exception):
     """Error to indicate a request failed."""
```

### Comparing `xiaomitv-0.9.1/src/xiaomitv.egg-info/PKG-INFO` & `xiaomitv-0.9.2/src/xiaomitv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaomitv
-Version: 0.9.1
+Version: 0.9.2
 Summary: Remote control for Xiaomi TVs
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/xiaomitv
 Project-URL: Bug Tracker, https://github.com/zhbjsh/xiaomitv/issues
 Keywords: xiaomi tv,mi tv,xiaomi,remote control
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

