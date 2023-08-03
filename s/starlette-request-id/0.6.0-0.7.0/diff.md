# Comparing `tmp/starlette-request-id-0.6.0.tar.gz` & `tmp/starlette-request-id-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette-request-id-0.6.0.tar", last modified: Mon Jul 26 09:33:12 2021, max compression
+gzip compressed data, was "starlette-request-id-0.7.0.tar", last modified: Thu Aug  3 12:10:56 2023, max compression
```

## Comparing `starlette-request-id-0.6.0.tar` & `starlette-request-id-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:33:12.951906 starlette-request-id-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11466 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4974 2021-07-26 09:33:12.951906 starlette-request-id-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3222 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      429 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-26 09:33:12.951906 starlette-request-id-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:33:12.951906 starlette-request-id-0.6.0/starlette_request_id/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/starlette_request_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/starlette_request_id/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/starlette_request_id/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/starlette_request_id/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/starlette_request_id/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/starlette_request_id/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-07-26 09:33:03.000000 starlette-request-id-0.6.0/starlette_request_id/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:33:12.951906 starlette-request-id-0.6.0/starlette_request_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4974 2021-07-26 09:33:12.000000 starlette-request-id-0.6.0/starlette_request_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      543 2021-07-26 09:33:12.000000 starlette-request-id-0.6.0/starlette_request_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 09:33:12.000000 starlette-request-id-0.6.0/starlette_request_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 09:33:12.000000 starlette-request-id-0.6.0/starlette_request_id.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-07-26 09:33:12.000000 starlette-request-id-0.6.0/starlette_request_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-07-26 09:33:12.000000 starlette-request-id-0.6.0/starlette_request_id.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:10:56.513551 starlette-request-id-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-03 12:10:56.513551 starlette-request-id-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:10:56.513551 starlette-request-id-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:10:56.513551 starlette-request-id-0.7.0/starlette_request_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/starlette_request_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/starlette_request_id/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/starlette_request_id/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/starlette_request_id/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/starlette_request_id/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/starlette_request_id/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 12:10:45.000000 starlette-request-id-0.7.0/starlette_request_id/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:10:56.513551 starlette-request-id-0.7.0/starlette_request_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-03 12:10:56.000000 starlette-request-id-0.7.0/starlette_request_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-03 12:10:56.000000 starlette-request-id-0.7.0/starlette_request_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:10:56.000000 starlette-request-id-0.7.0/starlette_request_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:10:56.000000 starlette-request-id-0.7.0/starlette_request_id.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 12:10:56.000000 starlette-request-id-0.7.0/starlette_request_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 12:10:56.000000 starlette-request-id-0.7.0/starlette_request_id.egg-info/top_level.txt
```

### Comparing `starlette-request-id-0.6.0/LICENSE` & `starlette-request-id-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette-request-id-0.6.0/PKG-INFO` & `starlette-request-id-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,120 +1,123 @@
 Metadata-Version: 2.1
 Name: starlette-request-id
-Version: 0.6.0
+Version: 0.7.0
 Summary: Helper for starlette to add request id in logger
 Home-page: https://github.com/bigbag/starlette-request-id
+Download-URL: https://pypi.python.org/pypi/starlette-request-id
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/starlette-request-id
-Description: # starlette-request-id
-        
-        [![CI](https://github.com/bigbag/starlette-request-id/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-request-id/actions?query=workflow%3ACI)
-        [![codecov](https://codecov.io/gh/bigbag/starlette-request-id/branch/main/graph/badge.svg?token=ZRUN7SUKB2)](https://codecov.io/gh/bigbag/starlette-request-id)
-        [![pypi](https://img.shields.io/pypi/v/starlette-request-id.svg)](https://pypi.python.org/pypi/starlette-request-id)
-        [![downloads](https://img.shields.io/pypi/dm/starlette-request-id.svg)](https://pypistats.org/packages/starlette-request-id)
-        [![versions](https://img.shields.io/pypi/pyversions/starlette-request-id.svg)](https://github.com/bigbag/starlette-request-id)
-        [![license](https://img.shields.io/github/license/bigbag/starlette-request-id.svg)](https://github.com/bigbag/starlette-request-id/blob/master/LICENSE)
-        
-        
-        **starlette-request-id** is a helper for starlette to add request id in logger.
-        
-        ## Installation
-        
-        starlette-request-id is available on PyPI.
-        Use pip to install:
-        
-            $ pip install starlette-request-id
-        
-        ## Basic Usage
-        
-        ```py
-        import httpx
-        import uvicorn
-        from starlette.applications import Starlette
-        from starlette.responses import PlainTextResponse
-        from starlette_request_id import REQUEST_ID_HEADER, RequestIdMiddleware, init_logger, request_id_ctx
-        
-        LOGGING = {
-            "version": 1,
-            "disable_existing_loggers": 0,
-            "formatters": {
-                "default": {
-                    "format": "[%(asctime)s] %(levelname)s [%(request_id)s] %(name)s | %(message)s",
-                    "datefmt": "%d/%b/%Y %H:%M:%S",
-                }
-            },
-            "handlers": {
-                "stdout": {
-                    "level": "INFO",
-                    "class": "logging.StreamHandler",
-                    "formatter": "default",
-                },
-            },
-            "loggers": {
-                "": {
-                    "handlers": ["stdout"],
-                    "propagate": True,
-                    "level": "INFO",
-                },
-            },
-        }
-        
-        
-        def init_app():
-            init_logger(LOGGING)
-        
-            app_ = Starlette()
-            app_.add_middleware(RequestIdMiddleware)
-        
-            @app_.route("/")
-            def success(request):
-                httpx.post("https://www.example.org/", headers={REQUEST_ID_HEADER: request_id_ctx.get()})
-                return PlainTextResponse("OK", status_code=200)
-        
-            return app_
-        
-        
-        app = init_app()
-        
-        if __name__ == "__main__":
-            uvicorn.run(
-                app=app,
-                log_config=LOGGING,
-            )
-        
-        ```
-        
-        curl 127.0.0.1:8000
-        
-        ```bash
-            [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Started server process [576540]
-            [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Waiting for application startup.
-            [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Application startup complete.
-            [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
-            [17/Jan/2021 18:31:22] INFO [22395fa2-e296-420e-93a1-5537e1ba0a62] uvicorn.access | 127.0.0.1:50372 - "GET / HTTP/1.1" 200
-            [17/Jan/2021 18:31:25] INFO [9ac6fa25-5048-4222-ac54-dd2c70e3e042] uvicorn.access | 127.0.0.1:50374 - "GET / HTTP/1.1" 200
-        ```
-        ## License
-        
-        starlette-request-id is developed and distributed under the Apache 2.0 license.
-        
-        ## Reporting a Security Vulnerability
-        
-        See our [security policy](https://github.com/bigbag/starlette-request-id/security/policy).
-        
 Platform: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# starlette-request-id
+
+[![CI](https://github.com/bigbag/starlette-request-id/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-request-id/actions?query=workflow%3ACI)
+[![codecov](https://codecov.io/gh/bigbag/starlette-request-id/branch/main/graph/badge.svg?token=ZRUN7SUKB2)](https://codecov.io/gh/bigbag/starlette-request-id)
+[![pypi](https://img.shields.io/pypi/v/starlette-request-id.svg)](https://pypi.python.org/pypi/starlette-request-id)
+[![downloads](https://img.shields.io/pypi/dm/starlette-request-id.svg)](https://pypistats.org/packages/starlette-request-id)
+[![versions](https://img.shields.io/pypi/pyversions/starlette-request-id.svg)](https://github.com/bigbag/starlette-request-id)
+[![license](https://img.shields.io/github/license/bigbag/starlette-request-id.svg)](https://github.com/bigbag/starlette-request-id/blob/master/LICENSE)
+
+
+**starlette-request-id** is a helper for starlette to add request id in logger.
+
+## Installation
+
+starlette-request-id is available on PyPI.
+Use pip to install:
+
+    $ pip install starlette-request-id
+
+## Basic Usage
+
+```py
+import httpx
+import uvicorn
+from starlette.applications import Starlette
+from starlette.responses import PlainTextResponse
+from starlette_request_id import REQUEST_ID_HEADER, RequestIdMiddleware, init_logger, request_id_ctx
+
+LOGGING = {
+    "version": 1,
+    "disable_existing_loggers": 0,
+    "formatters": {
+        "default": {
+            "format": "[%(asctime)s] %(levelname)s [%(request_id)s] %(name)s | %(message)s",
+            "datefmt": "%d/%b/%Y %H:%M:%S",
+        }
+    },
+    "handlers": {
+        "stdout": {
+            "level": "INFO",
+            "class": "logging.StreamHandler",
+            "formatter": "default",
+        },
+    },
+    "loggers": {
+        "": {
+            "handlers": ["stdout"],
+            "propagate": True,
+            "level": "INFO",
+        },
+    },
+}
+
+
+def init_app():
+    init_logger(LOGGING)
+
+    app_ = Starlette()
+    app_.add_middleware(RequestIdMiddleware)
+
+    @app_.route("/")
+    def success(request):
+        httpx.post("https://www.example.org/", headers={REQUEST_ID_HEADER: request_id_ctx.get()})
+        return PlainTextResponse("OK", status_code=200)
+
+    return app_
+
+
+app = init_app()
+
+if __name__ == "__main__":
+    uvicorn.run(
+        app=app,
+        log_config=LOGGING,
+    )
+
+```
+
+curl 127.0.0.1:8000
+
+```bash
+    [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Started server process [576540]
+    [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Waiting for application startup.
+    [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Application startup complete.
+    [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
+    [17/Jan/2021 18:31:22] INFO [22395fa2-e296-420e-93a1-5537e1ba0a62] uvicorn.access | 127.0.0.1:50372 - "GET / HTTP/1.1" 200
+    [17/Jan/2021 18:31:25] INFO [9ac6fa25-5048-4222-ac54-dd2c70e3e042] uvicorn.access | 127.0.0.1:50374 - "GET / HTTP/1.1" 200
+```
+## License
+
+starlette-request-id is developed and distributed under the Apache 2.0 license.
+
+## Reporting a Security Vulnerability
+
+See our [security policy](https://github.com/bigbag/starlette-request-id/security/policy).
```

### Comparing `starlette-request-id-0.6.0/README.md` & `starlette-request-id-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `starlette-request-id-0.6.0/setup.py` & `starlette-request-id-0.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: POSIX",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Environment :: Console",
     "Intended Audience :: Developers",
 ]
```

### Comparing `starlette-request-id-0.6.0/starlette_request_id/context.py` & `starlette-request-id-0.7.0/starlette_request_id/context.py`

 * *Files identical despite different names*

### Comparing `starlette-request-id-0.6.0/starlette_request_id/middleware.py` & `starlette-request-id-0.7.0/starlette_request_id/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette-request-id-0.6.0/starlette_request_id.egg-info/PKG-INFO` & `starlette-request-id-0.7.0/starlette_request_id.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,120 +1,123 @@
 Metadata-Version: 2.1
 Name: starlette-request-id
-Version: 0.6.0
+Version: 0.7.0
 Summary: Helper for starlette to add request id in logger
 Home-page: https://github.com/bigbag/starlette-request-id
+Download-URL: https://pypi.python.org/pypi/starlette-request-id
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/starlette-request-id
-Description: # starlette-request-id
-        
-        [![CI](https://github.com/bigbag/starlette-request-id/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-request-id/actions?query=workflow%3ACI)
-        [![codecov](https://codecov.io/gh/bigbag/starlette-request-id/branch/main/graph/badge.svg?token=ZRUN7SUKB2)](https://codecov.io/gh/bigbag/starlette-request-id)
-        [![pypi](https://img.shields.io/pypi/v/starlette-request-id.svg)](https://pypi.python.org/pypi/starlette-request-id)
-        [![downloads](https://img.shields.io/pypi/dm/starlette-request-id.svg)](https://pypistats.org/packages/starlette-request-id)
-        [![versions](https://img.shields.io/pypi/pyversions/starlette-request-id.svg)](https://github.com/bigbag/starlette-request-id)
-        [![license](https://img.shields.io/github/license/bigbag/starlette-request-id.svg)](https://github.com/bigbag/starlette-request-id/blob/master/LICENSE)
-        
-        
-        **starlette-request-id** is a helper for starlette to add request id in logger.
-        
-        ## Installation
-        
-        starlette-request-id is available on PyPI.
-        Use pip to install:
-        
-            $ pip install starlette-request-id
-        
-        ## Basic Usage
-        
-        ```py
-        import httpx
-        import uvicorn
-        from starlette.applications import Starlette
-        from starlette.responses import PlainTextResponse
-        from starlette_request_id import REQUEST_ID_HEADER, RequestIdMiddleware, init_logger, request_id_ctx
-        
-        LOGGING = {
-            "version": 1,
-            "disable_existing_loggers": 0,
-            "formatters": {
-                "default": {
-                    "format": "[%(asctime)s] %(levelname)s [%(request_id)s] %(name)s | %(message)s",
-                    "datefmt": "%d/%b/%Y %H:%M:%S",
-                }
-            },
-            "handlers": {
-                "stdout": {
-                    "level": "INFO",
-                    "class": "logging.StreamHandler",
-                    "formatter": "default",
-                },
-            },
-            "loggers": {
-                "": {
-                    "handlers": ["stdout"],
-                    "propagate": True,
-                    "level": "INFO",
-                },
-            },
-        }
-        
-        
-        def init_app():
-            init_logger(LOGGING)
-        
-            app_ = Starlette()
-            app_.add_middleware(RequestIdMiddleware)
-        
-            @app_.route("/")
-            def success(request):
-                httpx.post("https://www.example.org/", headers={REQUEST_ID_HEADER: request_id_ctx.get()})
-                return PlainTextResponse("OK", status_code=200)
-        
-            return app_
-        
-        
-        app = init_app()
-        
-        if __name__ == "__main__":
-            uvicorn.run(
-                app=app,
-                log_config=LOGGING,
-            )
-        
-        ```
-        
-        curl 127.0.0.1:8000
-        
-        ```bash
-            [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Started server process [576540]
-            [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Waiting for application startup.
-            [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Application startup complete.
-            [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
-            [17/Jan/2021 18:31:22] INFO [22395fa2-e296-420e-93a1-5537e1ba0a62] uvicorn.access | 127.0.0.1:50372 - "GET / HTTP/1.1" 200
-            [17/Jan/2021 18:31:25] INFO [9ac6fa25-5048-4222-ac54-dd2c70e3e042] uvicorn.access | 127.0.0.1:50374 - "GET / HTTP/1.1" 200
-        ```
-        ## License
-        
-        starlette-request-id is developed and distributed under the Apache 2.0 license.
-        
-        ## Reporting a Security Vulnerability
-        
-        See our [security policy](https://github.com/bigbag/starlette-request-id/security/policy).
-        
 Platform: POSIX
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# starlette-request-id
+
+[![CI](https://github.com/bigbag/starlette-request-id/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-request-id/actions?query=workflow%3ACI)
+[![codecov](https://codecov.io/gh/bigbag/starlette-request-id/branch/main/graph/badge.svg?token=ZRUN7SUKB2)](https://codecov.io/gh/bigbag/starlette-request-id)
+[![pypi](https://img.shields.io/pypi/v/starlette-request-id.svg)](https://pypi.python.org/pypi/starlette-request-id)
+[![downloads](https://img.shields.io/pypi/dm/starlette-request-id.svg)](https://pypistats.org/packages/starlette-request-id)
+[![versions](https://img.shields.io/pypi/pyversions/starlette-request-id.svg)](https://github.com/bigbag/starlette-request-id)
+[![license](https://img.shields.io/github/license/bigbag/starlette-request-id.svg)](https://github.com/bigbag/starlette-request-id/blob/master/LICENSE)
+
+
+**starlette-request-id** is a helper for starlette to add request id in logger.
+
+## Installation
+
+starlette-request-id is available on PyPI.
+Use pip to install:
+
+    $ pip install starlette-request-id
+
+## Basic Usage
+
+```py
+import httpx
+import uvicorn
+from starlette.applications import Starlette
+from starlette.responses import PlainTextResponse
+from starlette_request_id import REQUEST_ID_HEADER, RequestIdMiddleware, init_logger, request_id_ctx
+
+LOGGING = {
+    "version": 1,
+    "disable_existing_loggers": 0,
+    "formatters": {
+        "default": {
+            "format": "[%(asctime)s] %(levelname)s [%(request_id)s] %(name)s | %(message)s",
+            "datefmt": "%d/%b/%Y %H:%M:%S",
+        }
+    },
+    "handlers": {
+        "stdout": {
+            "level": "INFO",
+            "class": "logging.StreamHandler",
+            "formatter": "default",
+        },
+    },
+    "loggers": {
+        "": {
+            "handlers": ["stdout"],
+            "propagate": True,
+            "level": "INFO",
+        },
+    },
+}
+
+
+def init_app():
+    init_logger(LOGGING)
+
+    app_ = Starlette()
+    app_.add_middleware(RequestIdMiddleware)
+
+    @app_.route("/")
+    def success(request):
+        httpx.post("https://www.example.org/", headers={REQUEST_ID_HEADER: request_id_ctx.get()})
+        return PlainTextResponse("OK", status_code=200)
+
+    return app_
+
+
+app = init_app()
+
+if __name__ == "__main__":
+    uvicorn.run(
+        app=app,
+        log_config=LOGGING,
+    )
+
+```
+
+curl 127.0.0.1:8000
+
+```bash
+    [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Started server process [576540]
+    [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Waiting for application startup.
+    [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Application startup complete.
+    [17/Jan/2021 18:31:19] INFO [N/A] uvicorn.error | Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
+    [17/Jan/2021 18:31:22] INFO [22395fa2-e296-420e-93a1-5537e1ba0a62] uvicorn.access | 127.0.0.1:50372 - "GET / HTTP/1.1" 200
+    [17/Jan/2021 18:31:25] INFO [9ac6fa25-5048-4222-ac54-dd2c70e3e042] uvicorn.access | 127.0.0.1:50374 - "GET / HTTP/1.1" 200
+```
+## License
+
+starlette-request-id is developed and distributed under the Apache 2.0 license.
+
+## Reporting a Security Vulnerability
+
+See our [security policy](https://github.com/bigbag/starlette-request-id/security/policy).
```

### Comparing `starlette-request-id-0.6.0/starlette_request_id.egg-info/SOURCES.txt` & `starlette-request-id-0.7.0/starlette_request_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

