# Comparing `tmp/asgi-cors-middleware-0.0.1.tar.gz` & `tmp/asgi-cors-middleware-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/kiura/dev/lab/asgi-cors-middleware/dist/tmpnbt4iiti/asgi-cors-middleware-0.0.1.tar", last modified: Tue May 18 16:38:38 2021, max compression
+gzip compressed data, was "asgi-cors-middleware-0.0.2.tar", last modified: Thu Aug  3 11:53:50 2023, max compression
```

## Comparing `asgi-cors-middleware-0.0.1.tar` & `asgi-cors-middleware-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 kiura      (501) staff       (20)        0 2021-05-18 16:38:38.000000 asgi-cors-middleware-0.0.1/
--rw-r--r--   0 kiura      (501) staff       (20)     1067 2021-05-18 11:16:25.000000 asgi-cors-middleware-0.0.1/LICENSE
--rw-r--r--   0 kiura      (501) staff       (20)     4195 2021-05-18 16:38:38.000000 asgi-cors-middleware-0.0.1/PKG-INFO
--rw-r--r--   0 kiura      (501) staff       (20)     2825 2021-05-18 15:42:29.000000 asgi-cors-middleware-0.0.1/README.md
-drwxr-xr-x   0 kiura      (501) staff       (20)        0 2021-05-18 16:38:38.000000 asgi-cors-middleware-0.0.1/asgi_cors_middleware/
--rw-r--r--   0 kiura      (501) staff       (20)       36 2021-05-18 11:47:12.000000 asgi-cors-middleware-0.0.1/asgi_cors_middleware/__init__.py
--rw-r--r--   0 kiura      (501) staff       (20)     6138 2021-05-18 11:46:34.000000 asgi-cors-middleware-0.0.1/asgi_cors_middleware/middleware.py
-drwxr-xr-x   0 kiura      (501) staff       (20)        0 2021-05-18 16:38:38.000000 asgi-cors-middleware-0.0.1/asgi_cors_middleware.egg-info/
--rw-r--r--   0 kiura      (501) staff       (20)     4195 2021-05-18 16:38:38.000000 asgi-cors-middleware-0.0.1/asgi_cors_middleware.egg-info/PKG-INFO
--rw-r--r--   0 kiura      (501) staff       (20)      328 2021-05-18 16:38:38.000000 asgi-cors-middleware-0.0.1/asgi_cors_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 kiura      (501) staff       (20)        1 2021-05-18 16:38:38.000000 asgi-cors-middleware-0.0.1/asgi_cors_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 kiura      (501) staff       (20)       10 2021-05-18 16:38:38.000000 asgi-cors-middleware-0.0.1/asgi_cors_middleware.egg-info/requires.txt
--rw-r--r--   0 kiura      (501) staff       (20)       21 2021-05-18 16:38:38.000000 asgi-cors-middleware-0.0.1/asgi_cors_middleware.egg-info/top_level.txt
--rw-r--r--   0 kiura      (501) staff       (20)      103 2021-05-18 16:04:31.000000 asgi-cors-middleware-0.0.1/pyproject.toml
--rw-r--r--   0 kiura      (501) staff       (20)       38 2021-05-18 16:38:38.000000 asgi-cors-middleware-0.0.1/setup.cfg
--rw-r--r--   0 kiura      (501) staff       (20)      797 2021-05-18 16:38:08.000000 asgi-cors-middleware-0.0.1/setup.py
+drwxr-xr-x   0 kiura      (502) staff       (20)        0 2023-08-03 11:53:50.511386 asgi-cors-middleware-0.0.2/
+-rw-r--r--   0 kiura      (502) staff       (20)     1067 2023-08-03 11:38:36.000000 asgi-cors-middleware-0.0.2/LICENSE
+-rw-r--r--   0 kiura      (502) staff       (20)     3306 2023-08-03 11:53:50.511271 asgi-cors-middleware-0.0.2/PKG-INFO
+-rw-r--r--   0 kiura      (502) staff       (20)     2825 2023-08-03 11:38:36.000000 asgi-cors-middleware-0.0.2/README.md
+drwxr-xr-x   0 kiura      (502) staff       (20)        0 2023-08-03 11:53:50.510092 asgi-cors-middleware-0.0.2/asgi_cors_middleware/
+-rw-r--r--   0 kiura      (502) staff       (20)       36 2023-08-03 11:38:36.000000 asgi-cors-middleware-0.0.2/asgi_cors_middleware/__init__.py
+-rw-r--r--   0 kiura      (502) staff       (20)     6882 2023-08-03 11:38:36.000000 asgi-cors-middleware-0.0.2/asgi_cors_middleware/middleware.py
+drwxr-xr-x   0 kiura      (502) staff       (20)        0 2023-08-03 11:53:50.510726 asgi-cors-middleware-0.0.2/asgi_cors_middleware.egg-info/
+-rw-r--r--   0 kiura      (502) staff       (20)     3306 2023-08-03 11:53:50.000000 asgi-cors-middleware-0.0.2/asgi_cors_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 kiura      (502) staff       (20)      353 2023-08-03 11:53:50.000000 asgi-cors-middleware-0.0.2/asgi_cors_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 kiura      (502) staff       (20)        1 2023-08-03 11:53:50.000000 asgi-cors-middleware-0.0.2/asgi_cors_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 kiura      (502) staff       (20)       25 2023-08-03 11:53:50.000000 asgi-cors-middleware-0.0.2/asgi_cors_middleware.egg-info/requires.txt
+-rw-r--r--   0 kiura      (502) staff       (20)       21 2023-08-03 11:53:50.000000 asgi-cors-middleware-0.0.2/asgi_cors_middleware.egg-info/top_level.txt
+-rw-r--r--   0 kiura      (502) staff       (20)      105 2023-08-03 11:52:28.000000 asgi-cors-middleware-0.0.2/pyproject.toml
+-rw-r--r--   0 kiura      (502) staff       (20)       38 2023-08-03 11:53:50.511418 asgi-cors-middleware-0.0.2/setup.cfg
+-rw-r--r--   0 kiura      (502) staff       (20)      815 2023-08-03 11:52:59.000000 asgi-cors-middleware-0.0.2/setup.py
+drwxr-xr-x   0 kiura      (502) staff       (20)        0 2023-08-03 11:53:50.510846 asgi-cors-middleware-0.0.2/tests/
+-rw-r--r--   0 kiura      (502) staff       (20)    26146 2023-08-03 11:38:36.000000 asgi-cors-middleware-0.0.2/tests/test_middleware.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `asgi-cors-middleware-0.0.1/LICENSE` & `asgi-cors-middleware-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi-cors-middleware-0.0.1/PKG-INFO` & `asgi-cors-middleware-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,124 @@
 Metadata-Version: 2.1
 Name: asgi-cors-middleware
-Version: 0.0.1
+Version: 0.0.2
 Summary: Whitelist urls on ASGI applications allowing for cross origin requests
 Home-page: https://github.com/mrkiura/asgi-cors-middleware
 Author: Alex Kiura
 Author-email: kiuraalex@gmail.com
 License: MIT
-Description: # asgi-cors-middleware
-        
-        Python package that allows whitelisting of urls on ASGI applications making it possible to perform cross origin requests from the browser.
-        
-        ## CORS in a nutshell
-        
-        **Cross-Origin Resource Sharing (CORS)** allows a server to define any
-         origins other than its own that are safe for the browser to load resources from.
-        
-        Mozilla does a good job of explaining CORS [here](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS).
-        
-        ## Background
-        
-        Assuming you have a web application that follows a client-server architecture, it's possible the frontend would be running on a server
-        different from the API. If the frontend application made a request to the API, this kind of request would be blocked by the browser.
-        
-        For security reasons, browsers block cross origin requests by default.
-        
-        A cross origin request is a request made to a server with a different url/ origin. To mitigate around this, we could simply add the url of the frontend application as an allowed origin on the API server.
-        Most web frameworks provide a way to do this or have third party libraries that achieve the same.
-        
-        **asgi-cors-middleware** aims to provide a simple way to achieve the above for ASGI applications.
-        
-        ## Features
-        
-        * Simple
-        * Works with most ASGI frameworks (Django, Starlette, FastAPI, channels)
-        * Works with Ariadne
-        
-        ## Installation
-        
-        Can be installed via pip
-        
-        ```bash
-        pip install asgi-cors-middleware
-        ```
-        
-        ## Usage
-        
-        To use the middleware, just import it like so:
-        
-        ```python
-        from asgi_cors_middleware import CorsASGIApp
-        ```
-        
-        To start whitelisting origins, just wrap your asgi application instance with
-        `CorsASGIApp`.
-        
-        ```python
-        
-        app = CorsASGIApp(
-            app=asgi_app_instance,
-            origins=["www.example.com"]
-        )
-        ```
-        
-        ## Example
-        
-        A simple HelloWorld application that whitelists the origins below:
-        * www.example.com
-        * localhost:9000
-        
-        ### Install an ASGI server
-        
-        ```bash
-        pip install uvicorn
-        ```
-        
-        Create a file called example.py and update it with the code below:
-        
-        ```python
-        from asgi_cors_middleware import CorsASGIApp
-        
-        class HelloWorld:
-            def __init__(self, scope):
-                pass
-        
-            async def __call__(self, receive, send):
-                await send({
-                    'type': 'http.response.start',
-                    'status': 200,
-                    'headers': [
-                        [b'content-type', b'text/plain'],
-                    ]
-                })
-                await send({
-                    'type': 'http.response.body',
-                    'body': b'Hello, world!',
-                })
-        
-        app = CorsASGIApp(
-            app=HelloWorld,
-            origins=[
-                "www.example.com",
-                "localhost:9000"
-            ]
-        )
-        ```
-        
-        That's it. For real, that's really it. Now your application is all set to allow requests from www.example.com and localhost:9000.
-        
-        ### Run the app
-        
-        ```bash
-        uvicorn example:app
-        ```
-        
-        ## Contributing
-        
-        For guidance and instructions, please see [CONTRIBUTING.md](CONTRIBUTING.md)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# asgi-cors-middleware
+
+Python package that allows whitelisting of urls on ASGI applications making it possible to perform cross origin requests from the browser.
+
+## CORS in a nutshell
+
+**Cross-Origin Resource Sharing (CORS)** allows a server to define any
+ origins other than its own that are safe for the browser to load resources from.
+
+Mozilla does a good job of explaining CORS [here](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS).
+
+## Background
+
+Assuming you have a web application that follows a client-server architecture, it's possible the frontend would be running on a server
+different from the API. If the frontend application made a request to the API, this kind of request would be blocked by the browser.
+
+For security reasons, browsers block cross origin requests by default.
+
+A cross origin request is a request made to a server with a different url/ origin. To mitigate around this, we could simply add the url of the frontend application as an allowed origin on the API server.
+Most web frameworks provide a way to do this or have third party libraries that achieve the same.
+
+**asgi-cors-middleware** aims to provide a simple way to achieve the above for ASGI applications.
+
+## Features
+
+* Simple
+* Works with most ASGI frameworks (Django, Starlette, FastAPI, channels)
+* Works with Ariadne
+
+## Installation
+
+Can be installed via pip
+
+```bash
+pip install asgi-cors-middleware
+```
+
+## Usage
+
+To use the middleware, just import it like so:
+
+```python
+from asgi_cors_middleware import CorsASGIApp
+```
+
+To start whitelisting origins, just wrap your asgi application instance with
+`CorsASGIApp`.
+
+```python
+
+app = CorsASGIApp(
+    app=asgi_app_instance,
+    origins=["www.example.com"]
+)
+```
+
+## Example
+
+A simple HelloWorld application that whitelists the origins below:
+* www.example.com
+* localhost:9000
+
+### Install an ASGI server
+
+```bash
+pip install uvicorn
+```
+
+Create a file called example.py and update it with the code below:
+
+```python
+from asgi_cors_middleware import CorsASGIApp
+
+class HelloWorld:
+    def __init__(self, scope):
+        pass
+
+    async def __call__(self, receive, send):
+        await send({
+            'type': 'http.response.start',
+            'status': 200,
+            'headers': [
+                [b'content-type', b'text/plain'],
+            ]
+        })
+        await send({
+            'type': 'http.response.body',
+            'body': b'Hello, world!',
+        })
+
+app = CorsASGIApp(
+    app=HelloWorld,
+    origins=[
+        "www.example.com",
+        "localhost:9000"
+    ]
+)
+```
+
+That's it. For real, that's really it. Now your application is all set to allow requests from www.example.com and localhost:9000.
+
+### Run the app
+
+```bash
+uvicorn example:app
+```
+
+## Contributing
+
+For guidance and instructions, please see [CONTRIBUTING.md](CONTRIBUTING.md)
```

### Comparing `asgi-cors-middleware-0.0.1/README.md` & `asgi-cors-middleware-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `asgi-cors-middleware-0.0.1/asgi_cors_middleware/middleware.py` & `asgi-cors-middleware-0.0.2/asgi_cors_middleware/middleware.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,19 +3,23 @@
     * CORS middleware
 """
 
 import functools
 import re
 import typing
 
+from asgiref.compatibility import guarantee_single_callable
 from starlette.datastructures import Headers, MutableHeaders
 
 from starlette.responses import PlainTextResponse
+from starlette.responses import Response
 
-ALL_METHODS = ("DELETE", "GET", "OPTIONS", "PATCH", "POST", "PUT")
+# OPTIONS doesn't make sense to return as an allowed method for CORS.
+# See https://stackoverflow.com/a/68529748
+ALL_METHODS = ("DELETE", "GET", "PATCH", "POST", "PUT")
 SAFELISTED_HEADERS = {
     "Accept", "Accept-Language", "Content-Language", "Content-Type"
 }
 
 
 class CorsASGIApp:
     def __init__(
@@ -45,60 +49,63 @@
         if expose_headers:
             simple_headers["Access-Control-Expose-Headers"] = \
                 ", ".join(expose_headers)
 
         preflight_headers = {}
         if "*" in origins:
             preflight_headers["Access-Control-Allow-Origin"] = "*"
-        else:
+        elif len(origins) > 1 or compiled_allow_origin_regex is not None:
             preflight_headers["Vary"] = "Origin"
         preflight_headers.update(
             {
                 "Access-Control-Allow-Methods": ", ".join(allow_methods),
                 "Access-Control-Max-Age": str(max_age),
             }
         )
-        allow_headers = sorted(SAFELISTED_HEADERS | set(allow_headers))
+        # re-including normally safelisted headers implies that you want to lift the browsers
+        #  additional restrictions on those headers. we don't want to do that by default.
+        # See https://developer.mozilla.org/en-US/docs/Glossary/CORS-safelisted_request_header#additional_restrictions
+        allow_headers = sorted(set(allow_headers))
         if allow_headers and "*" not in allow_headers:
             preflight_headers["Access-Control-Allow-Headers"] = \
                 ", ".join(allow_headers)
         if allow_credentials:
             preflight_headers["Access-Control-Allow-Credentials"] = "true"
 
-        self.app = app
+        self.app = guarantee_single_callable(app)
         self.origins = origins
         self.allow_methods = allow_methods
         self.allow_headers = [h.lower() for h in allow_headers]
         self.allow_all_origins = "*" in origins
         self.allow_all_headers = "*" in allow_headers
         self.allow_origin_regex = compiled_allow_origin_regex
         self.simple_headers = simple_headers
         self.preflight_headers = preflight_headers
 
     async def __call__(
             self, scope, receive, send
     ) -> None:
-        if scope["type"] != "http":  # pragma: no cover
-            handler = await self.app(scope, receive, send)
-            await handler.__call__(receive, send)
-            return
+        if scope["type"] != "http":
+            return await self.app(scope, receive, send)
 
         method = scope["method"]
         headers = Headers(scope=scope)
         origin = headers.get("origin")
 
         if origin is None:
-            handler = await self.app(scope, receive, send)
-            await handler.__call__(receive, send)
-            return
+            return await self.app(scope, receive, send)
 
-        if method == "OPTIONS" and "access-control-request-method" in headers:
-            response = self.preflight_response(request_headers=headers)
-            await response(scope, receive, send)
-            return
+        if method == "OPTIONS":
+            if "access-control-request-method" in headers:
+                response = self.preflight_response(request_headers=headers)
+                await response(scope, receive, send)
+                return
+            # if this is an options request but was not a cors preflight,
+            #  we should skip the simple response processing.
+            return await self.app(scope, receive, send)
 
         await self.simple_response(
             scope, receive, send, request_headers=headers
         )
 
     def is_allowed_origin(self, origin: str) -> bool:
         if self.allow_all_origins:
@@ -106,15 +113,15 @@
 
         if self.allow_origin_regex is not None and \
                 self.allow_origin_regex.fullmatch(origin):
             return True
 
         return any(host in origin for host in self.origins)
 
-    def preflight_response(self, request_headers) -> PlainTextResponse:
+    def preflight_response(self, request_headers) -> Response:
         requested_origin = request_headers["origin"]
         requested_method = request_headers["access-control-request-method"]
         requested_headers = request_headers.get(
             "access-control-request-headers"
         )
 
         headers = dict(self.preflight_headers)
@@ -129,37 +136,37 @@
         if requested_method not in self.allow_methods:
             failures.append("method")
 
         if self.allow_all_headers and requested_headers is not None:
             headers["Access-Control-Allow-Headers"] = requested_headers
         elif requested_headers is not None:
             for header in [h.lower() for h in requested_headers.split(",")]:
-                if header.strip() not in self.allow_headers:
+                requested_header = header.strip()
+                if requested_header not in self.allow_headers and requested_method not in SAFELISTED_HEADERS:
                     failures.append("headers")
 
         if failures:
             failure_text = "Disallowed CORS " + ", ".join(failures)
             return PlainTextResponse(
-                failure_text, status_code=400, headers=headers
+                failure_text, status_code=403, headers=headers
             )
 
-        return PlainTextResponse("OK", status_code=200, headers=headers)
+        return Response("", status_code=204, headers=headers)
 
     async def simple_response(
             self,
             scope,
             receive,
             send,
             request_headers
     ) -> None:
         send = functools.partial(
             self.send, send=send, request_headers=request_headers
         )
-        handler = await self.app(scope, receive, send)
-        await handler(receive, send)
+        return await self.app(scope, receive, send)
 
     async def send(self, message, send, request_headers) -> None:
         if message["type"] != "http.response.start":
             await send(message)
             return
 
         message.setdefault("headers", [])
@@ -170,9 +177,10 @@
 
         if self.allow_all_origins and has_cookie:
             headers["Access-Control-Allow-Origin"] = origin
 
         elif not self.allow_all_origins and \
                 self.is_allowed_origin(origin=origin):
             headers["Access-Control-Allow-Origin"] = origin
-            headers.add_vary_header("Origin")
+            if len(self.origins) > 1 or self.allow_origin_regex is not None:
+                headers.add_vary_header("Origin")
         await send(message)
```

### Comparing `asgi-cors-middleware-0.0.1/asgi_cors_middleware.egg-info/PKG-INFO` & `asgi-cors-middleware-0.0.2/asgi_cors_middleware.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,124 @@
 Metadata-Version: 2.1
 Name: asgi-cors-middleware
-Version: 0.0.1
+Version: 0.0.2
 Summary: Whitelist urls on ASGI applications allowing for cross origin requests
 Home-page: https://github.com/mrkiura/asgi-cors-middleware
 Author: Alex Kiura
 Author-email: kiuraalex@gmail.com
 License: MIT
-Description: # asgi-cors-middleware
-        
-        Python package that allows whitelisting of urls on ASGI applications making it possible to perform cross origin requests from the browser.
-        
-        ## CORS in a nutshell
-        
-        **Cross-Origin Resource Sharing (CORS)** allows a server to define any
-         origins other than its own that are safe for the browser to load resources from.
-        
-        Mozilla does a good job of explaining CORS [here](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS).
-        
-        ## Background
-        
-        Assuming you have a web application that follows a client-server architecture, it's possible the frontend would be running on a server
-        different from the API. If the frontend application made a request to the API, this kind of request would be blocked by the browser.
-        
-        For security reasons, browsers block cross origin requests by default.
-        
-        A cross origin request is a request made to a server with a different url/ origin. To mitigate around this, we could simply add the url of the frontend application as an allowed origin on the API server.
-        Most web frameworks provide a way to do this or have third party libraries that achieve the same.
-        
-        **asgi-cors-middleware** aims to provide a simple way to achieve the above for ASGI applications.
-        
-        ## Features
-        
-        * Simple
-        * Works with most ASGI frameworks (Django, Starlette, FastAPI, channels)
-        * Works with Ariadne
-        
-        ## Installation
-        
-        Can be installed via pip
-        
-        ```bash
-        pip install asgi-cors-middleware
-        ```
-        
-        ## Usage
-        
-        To use the middleware, just import it like so:
-        
-        ```python
-        from asgi_cors_middleware import CorsASGIApp
-        ```
-        
-        To start whitelisting origins, just wrap your asgi application instance with
-        `CorsASGIApp`.
-        
-        ```python
-        
-        app = CorsASGIApp(
-            app=asgi_app_instance,
-            origins=["www.example.com"]
-        )
-        ```
-        
-        ## Example
-        
-        A simple HelloWorld application that whitelists the origins below:
-        * www.example.com
-        * localhost:9000
-        
-        ### Install an ASGI server
-        
-        ```bash
-        pip install uvicorn
-        ```
-        
-        Create a file called example.py and update it with the code below:
-        
-        ```python
-        from asgi_cors_middleware import CorsASGIApp
-        
-        class HelloWorld:
-            def __init__(self, scope):
-                pass
-        
-            async def __call__(self, receive, send):
-                await send({
-                    'type': 'http.response.start',
-                    'status': 200,
-                    'headers': [
-                        [b'content-type', b'text/plain'],
-                    ]
-                })
-                await send({
-                    'type': 'http.response.body',
-                    'body': b'Hello, world!',
-                })
-        
-        app = CorsASGIApp(
-            app=HelloWorld,
-            origins=[
-                "www.example.com",
-                "localhost:9000"
-            ]
-        )
-        ```
-        
-        That's it. For real, that's really it. Now your application is all set to allow requests from www.example.com and localhost:9000.
-        
-        ### Run the app
-        
-        ```bash
-        uvicorn example:app
-        ```
-        
-        ## Contributing
-        
-        For guidance and instructions, please see [CONTRIBUTING.md](CONTRIBUTING.md)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# asgi-cors-middleware
+
+Python package that allows whitelisting of urls on ASGI applications making it possible to perform cross origin requests from the browser.
+
+## CORS in a nutshell
+
+**Cross-Origin Resource Sharing (CORS)** allows a server to define any
+ origins other than its own that are safe for the browser to load resources from.
+
+Mozilla does a good job of explaining CORS [here](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS).
+
+## Background
+
+Assuming you have a web application that follows a client-server architecture, it's possible the frontend would be running on a server
+different from the API. If the frontend application made a request to the API, this kind of request would be blocked by the browser.
+
+For security reasons, browsers block cross origin requests by default.
+
+A cross origin request is a request made to a server with a different url/ origin. To mitigate around this, we could simply add the url of the frontend application as an allowed origin on the API server.
+Most web frameworks provide a way to do this or have third party libraries that achieve the same.
+
+**asgi-cors-middleware** aims to provide a simple way to achieve the above for ASGI applications.
+
+## Features
+
+* Simple
+* Works with most ASGI frameworks (Django, Starlette, FastAPI, channels)
+* Works with Ariadne
+
+## Installation
+
+Can be installed via pip
+
+```bash
+pip install asgi-cors-middleware
+```
+
+## Usage
+
+To use the middleware, just import it like so:
+
+```python
+from asgi_cors_middleware import CorsASGIApp
+```
+
+To start whitelisting origins, just wrap your asgi application instance with
+`CorsASGIApp`.
+
+```python
+
+app = CorsASGIApp(
+    app=asgi_app_instance,
+    origins=["www.example.com"]
+)
+```
+
+## Example
+
+A simple HelloWorld application that whitelists the origins below:
+* www.example.com
+* localhost:9000
+
+### Install an ASGI server
+
+```bash
+pip install uvicorn
+```
+
+Create a file called example.py and update it with the code below:
+
+```python
+from asgi_cors_middleware import CorsASGIApp
+
+class HelloWorld:
+    def __init__(self, scope):
+        pass
+
+    async def __call__(self, receive, send):
+        await send({
+            'type': 'http.response.start',
+            'status': 200,
+            'headers': [
+                [b'content-type', b'text/plain'],
+            ]
+        })
+        await send({
+            'type': 'http.response.body',
+            'body': b'Hello, world!',
+        })
+
+app = CorsASGIApp(
+    app=HelloWorld,
+    origins=[
+        "www.example.com",
+        "localhost:9000"
+    ]
+)
+```
+
+That's it. For real, that's really it. Now your application is all set to allow requests from www.example.com and localhost:9000.
+
+### Run the app
+
+```bash
+uvicorn example:app
+```
+
+## Contributing
+
+For guidance and instructions, please see [CONTRIBUTING.md](CONTRIBUTING.md)
```

### Comparing `asgi-cors-middleware-0.0.1/setup.py` & `asgi-cors-middleware-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="asgi-cors-middleware",
-    version="0.0.1",
+    version="0.0.2",
     description="Whitelist urls on ASGI applications allowing for cross origin "
                 "requests",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mrkiura/asgi-cors-middleware",
     author="Alex Kiura",
     author_email="kiuraalex@gmail.com",
@@ -19,9 +19,9 @@
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
     ],
     packages=["asgi_cors_middleware"],
     include_package_data=True,
-    install_requires=["starlette"]
+    install_requires=["starlette", "asgiref>=3.5.0"]
 )
```

