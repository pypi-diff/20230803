# Comparing `tmp/aiohutils-0.7.1.tar.gz` & `tmp/aiohutils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohutils-0.7.1.tar", last modified: Thu Aug  3 07:50:35 2023, max compression
+gzip compressed data, was "aiohutils-0.8.0.tar", last modified: Thu Aug  3 10:41:48 2023, max compression
```

## Comparing `aiohutils-0.7.1.tar` & `aiohutils-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:50:35.333392 aiohutils-0.7.1/
--rw-rw-rw-   0        0        0      503 2023-08-03 07:50:35.332394 aiohutils-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-08-03 06:55:23.000000 aiohutils-0.7.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-03 07:50:35.312448 aiohutils-0.7.1/aiohutils/
--rw-rw-rw-   0        0        0       22 2023-08-03 07:50:32.000000 aiohutils-0.7.1/aiohutils/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-08-03 07:39:47.000000 aiohutils-0.7.1/aiohutils/session.py
--rw-rw-rw-   0        0        0     2946 2023-08-03 07:49:19.000000 aiohutils-0.7.1/aiohutils/tests.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:50:35.331397 aiohutils-0.7.1/aiohutils.egg-info/
--rw-rw-rw-   0        0        0      503 2023-08-03 07:50:35.000000 aiohutils-0.7.1/aiohutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-03 07:50:35.000000 aiohutils-0.7.1/aiohutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:50:35.000000 aiohutils-0.7.1/aiohutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-08-03 07:50:35.000000 aiohutils-0.7.1/aiohutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-03 07:50:35.000000 aiohutils-0.7.1/aiohutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-08-03 06:59:05.000000 aiohutils-0.7.1/aiohutils.egg-info/zip-safe
--rw-rw-rw-   0        0        0      967 2023-08-03 07:01:19.000000 aiohutils-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 07:50:35.333392 aiohutils-0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 10:41:48.888435 aiohutils-0.8.0/
+-rw-rw-rw-   0        0        0      503 2023-08-03 10:41:48.888435 aiohutils-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-08-03 06:55:23.000000 aiohutils-0.8.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-03 10:41:48.878461 aiohutils-0.8.0/aiohutils/
+-rw-rw-rw-   0        0        0       22 2023-08-03 10:41:46.000000 aiohutils-0.8.0/aiohutils/__init__.py
+-rw-rw-rw-   0        0        0     1223 2023-08-03 10:39:06.000000 aiohutils-0.8.0/aiohutils/session.py
+-rw-rw-rw-   0        0        0     2946 2023-08-03 07:49:19.000000 aiohutils-0.8.0/aiohutils/tests.py
+drwxrwxrwx   0        0        0        0 2023-08-03 10:41:48.886439 aiohutils-0.8.0/aiohutils.egg-info/
+-rw-rw-rw-   0        0        0      503 2023-08-03 10:41:48.000000 aiohutils-0.8.0/aiohutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-03 10:41:48.000000 aiohutils-0.8.0/aiohutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 10:41:48.000000 aiohutils-0.8.0/aiohutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-08-03 10:41:48.000000 aiohutils-0.8.0/aiohutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 10:41:48.000000 aiohutils-0.8.0/aiohutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-03 06:59:05.000000 aiohutils-0.8.0/aiohutils.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      967 2023-08-03 07:01:19.000000 aiohutils-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 10:41:48.889433 aiohutils-0.8.0/setup.cfg
```

### Comparing `aiohutils-0.7.1/aiohutils/session.py` & `aiohutils-0.8.0/aiohutils/session.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,47 @@
+import asyncio
 import atexit
-from asyncio import run
 from warnings import warn
 
 from aiohttp import ClientResponse, ClientSession, ClientTimeout
 
 
 class SessionManager:
     __slots__ = ('_session', '_args', '_kwargs')
 
     def __init__(
         self,
         args=(),
-        kwargs={},
+        kwargs=None,
     ):
         self._args = args
+
+        if kwargs is None:
+            kwargs = {}
         self._kwargs = {
             'timeout': ClientTimeout(
                 total=60.0, sock_connect=30.0, sock_read=30.0
             ),
         } | kwargs
 
     @property
     def session(self) -> ClientSession:
         try:
             session = self._session
         except AttributeError:
             session = self._session = ClientSession(
                 *self._args, **self._kwargs
             )
-            atexit.register(self.close)
+            atexit.register(asyncio.run, session.close())
         return session
 
-    def _check_response(self, response: ClientResponse):
+    @staticmethod
+    def _check_response(response: ClientResponse):
         if response.history:
-            warn(f'r.history is not empty (possible redirection): {r.history}')
+            warn(
+                f'r.history is not empty (possible redirection): {response.history}'
+            )
 
     async def get(self, *args, **kwargs) -> ClientResponse:
         resp = await self.session.get(*args, **kwargs)
         self._check_response(resp)
         return resp
-
-    def close(self):
-        run(self.session.close())
```

### Comparing `aiohutils-0.7.1/aiohutils/tests.py` & `aiohutils-0.8.0/aiohutils/tests.py`

 * *Files identical despite different names*

### Comparing `aiohutils-0.7.1/pyproject.toml` & `aiohutils-0.8.0/pyproject.toml`

 * *Files identical despite different names*

