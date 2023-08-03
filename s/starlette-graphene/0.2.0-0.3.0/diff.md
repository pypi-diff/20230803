# Comparing `tmp/starlette-graphene-0.2.0.tar.gz` & `tmp/starlette-graphene-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette-graphene-0.2.0.tar", last modified: Mon Jul 26 09:36:07 2021, max compression
+gzip compressed data, was "starlette-graphene-0.3.0.tar", last modified: Thu Aug  3 11:46:06 2023, max compression
```

## Comparing `starlette-graphene-0.2.0.tar` & `starlette-graphene-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:36:07.347418 starlette-graphene-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11466 2021-07-26 09:35:53.000000 starlette-graphene-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-07-26 09:35:53.000000 starlette-graphene-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3744 2021-07-26 09:36:07.347418 starlette-graphene-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2142 2021-07-26 09:35:53.000000 starlette-graphene-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      427 2021-07-26 09:35:53.000000 starlette-graphene-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-26 09:36:07.347418 starlette-graphene-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2021-07-26 09:35:53.000000 starlette-graphene-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:36:07.347418 starlette-graphene-0.2.0/starlette_graphene/
--rw-r--r--   0 runner    (1001) docker     (121)     8712 2021-07-26 09:35:53.000000 starlette-graphene-0.2.0/starlette_graphene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-07-26 09:35:53.000000 starlette-graphene-0.2.0/starlette_graphene/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-26 09:36:07.347418 starlette-graphene-0.2.0/starlette_graphene.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3744 2021-07-26 09:36:07.000000 starlette-graphene-0.2.0/starlette_graphene.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      364 2021-07-26 09:36:07.000000 starlette-graphene-0.2.0/starlette_graphene.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 09:36:07.000000 starlette-graphene-0.2.0/starlette_graphene.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-26 09:36:07.000000 starlette-graphene-0.2.0/starlette_graphene.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-07-26 09:36:07.000000 starlette-graphene-0.2.0/starlette_graphene.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-07-26 09:36:07.000000 starlette-graphene-0.2.0/starlette_graphene.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:46:06.519577 starlette-graphene-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-08-03 11:45:51.000000 starlette-graphene-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-03 11:45:51.000000 starlette-graphene-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-03 11:46:06.519577 starlette-graphene-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-03 11:45:51.000000 starlette-graphene-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-03 11:45:51.000000 starlette-graphene-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:46:06.519577 starlette-graphene-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-03 11:45:51.000000 starlette-graphene-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:46:06.519577 starlette-graphene-0.3.0/starlette_graphene/
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-08-03 11:45:51.000000 starlette-graphene-0.3.0/starlette_graphene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 11:45:51.000000 starlette-graphene-0.3.0/starlette_graphene/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:46:06.519577 starlette-graphene-0.3.0/starlette_graphene.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-03 11:46:06.000000 starlette-graphene-0.3.0/starlette_graphene.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-03 11:46:06.000000 starlette-graphene-0.3.0/starlette_graphene.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:46:06.000000 starlette-graphene-0.3.0/starlette_graphene.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:46:06.000000 starlette-graphene-0.3.0/starlette_graphene.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 11:46:06.000000 starlette-graphene-0.3.0/starlette_graphene.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 11:46:06.000000 starlette-graphene-0.3.0/starlette_graphene.egg-info/top_level.txt
```

### Comparing `starlette-graphene-0.2.0/LICENSE` & `starlette-graphene-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette-graphene-0.2.0/PKG-INFO` & `starlette-graphene-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,105 @@
 Metadata-Version: 2.1
 Name: starlette-graphene
-Version: 0.2.0
+Version: 0.3.0
 Summary: Helper for add support for graphene in starlette
 Home-page: https://github.com/bigbag/starlette-graphene
+Download-URL: https://pypi.python.org/pypi/starlette-graphene
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/starlette-graphene
-Description: # starlette-graphene
-        
-        [![CI](https://github.com/bigbag/starlette-graphene/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-graphene/actions?query=workflow%3ACI)
-        [![codecov](https://codecov.io/gh/bigbag/starlette-graphene/branch/main/graph/badge.svg?token=FQTY888XG1)](https://codecov.io/gh/bigbag/starlette-graphene)
-        [![pypi](https://img.shields.io/pypi/v/starlette-graphene.svg)](https://pypi.python.org/pypi/starlette-graphene)
-        [![downloads](https://img.shields.io/pypi/dm/starlette-graphene.svg)](https://pypistats.org/packages/starlette-graphene)
-        [![versions](https://img.shields.io/pypi/pyversions/starlette-graphene.svg)](https://github.com/bigbag/starlette-graphene)
-        [![license](https://img.shields.io/github/license/bigbag/starlette-graphene.svg)](https://github.com/bigbag/starlette-graphene/blob/master/LICENSE)
-        
-        
-        **starlette-graphene** is a helper for add support for graphene in starlette.
-        
-        
-        ## Installation
-        
-        starlette-graphene is available on PyPI.
-        Use pip to install:
-        
-            $ pip install starlette-graphene
-        
-        ## Basic Usage
-        
-        ```py
-        import uvicorn
-        from graphene import types as grt
-        from starlette.applications import Starlette
-        
-        from starlette_graphene import GraphQLApp
-        
-        
-        class Account(grt.ObjectType):
-            account = grt.Int(required=True)
-        
-        
-        class AccountFilter(grt.InputObjectType):
-            accounts = grt.List(grt.Int)
-        
-        
-        class Query(grt.ObjectType):
-            course_list = None
-            accounts = grt.Field(
-                grt.List(Account),
-                filters=AccountFilter(),
-            )
-        
-            async def resolve_accounts(
-                self,
-                info,
-                filters: AccountFilter,
-            ):
-        
-                return [Account(account=1212), Account(account=43434)]
-        
-        
-        def get_graphql_app() -> GraphQLApp:
-            return GraphQLApp(schema=grt.Schema(query=Query))
-        
-        
-        def init_app():
-            app_ = Starlette()
-            app_.mount("/graphql/", get_graphql_app())
-            return app_
-        
-        
-        app = init_app()
-        
-        if __name__ == "__main__":
-            uvicorn.run(app=app)
-        ```
-        
-        ## License
-        
-        starlette-graphene is developed and distributed under the Apache 2.0 license.
-        
-        ## Reporting a Security Vulnerability
-        
-        See our [security policy](https://github.com/bigbag/starlette-graphene/security/policy).
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
+# starlette-graphene
+
+[![CI](https://github.com/bigbag/starlette-graphene/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-graphene/actions?query=workflow%3ACI)
+[![codecov](https://codecov.io/gh/bigbag/starlette-graphene/branch/main/graph/badge.svg?token=FQTY888XG1)](https://codecov.io/gh/bigbag/starlette-graphene)
+[![pypi](https://img.shields.io/pypi/v/starlette-graphene.svg)](https://pypi.python.org/pypi/starlette-graphene)
+[![downloads](https://img.shields.io/pypi/dm/starlette-graphene.svg)](https://pypistats.org/packages/starlette-graphene)
+[![versions](https://img.shields.io/pypi/pyversions/starlette-graphene.svg)](https://github.com/bigbag/starlette-graphene)
+[![license](https://img.shields.io/github/license/bigbag/starlette-graphene.svg)](https://github.com/bigbag/starlette-graphene/blob/master/LICENSE)
+
+
+**starlette-graphene** is a helper for add support for graphene in starlette.
+
+
+## Installation
+
+starlette-graphene is available on PyPI.
+Use pip to install:
+
+    $ pip install starlette-graphene
+
+## Basic Usage
+
+```py
+import uvicorn
+from graphene import types as grt
+from starlette.applications import Starlette
+
+from starlette_graphene import GraphQLApp
+
+
+class Account(grt.ObjectType):
+    account = grt.Int(required=True)
+
+
+class AccountFilter(grt.InputObjectType):
+    accounts = grt.List(grt.Int)
+
+
+class Query(grt.ObjectType):
+    course_list = None
+    accounts = grt.Field(
+        grt.List(Account),
+        filters=AccountFilter(),
+    )
+
+    async def resolve_accounts(
+        self,
+        info,
+        filters: AccountFilter,
+    ):
+
+        return [Account(account=1212), Account(account=43434)]
+
+
+def get_graphql_app() -> GraphQLApp:
+    return GraphQLApp(schema=grt.Schema(query=Query))
+
+
+def init_app():
+    app_ = Starlette()
+    app_.mount("/graphql/", get_graphql_app())
+    return app_
+
+
+app = init_app()
+
+if __name__ == "__main__":
+    uvicorn.run(app=app)
+```
+
+## License
+
+starlette-graphene is developed and distributed under the Apache 2.0 license.
+
+## Reporting a Security Vulnerability
+
+See our [security policy](https://github.com/bigbag/starlette-graphene/security/policy).
```

### Comparing `starlette-graphene-0.2.0/README.md` & `starlette-graphene-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `starlette-graphene-0.2.0/setup.py` & `starlette-graphene-0.3.0/setup.py`

 * *Files 4% similar despite different names*

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

### Comparing `starlette-graphene-0.2.0/starlette_graphene/__init__.py` & `starlette-graphene-0.3.0/starlette_graphene/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import json
 import typing as t
 from dataclasses import dataclass
 
 import graphene
-from graphql import ExecutionContext, GraphQLError, Middleware, format_error, graphql
+from graphql import ExecutionContext, GraphQLError, GraphQLFormattedError, Middleware, graphql
 from starlette import status
 from starlette import types as st
 from starlette.background import BackgroundTasks
 from starlette.requests import HTTPConnection, Request
 from starlette.responses import HTMLResponse, JSONResponse, PlainTextResponse, Response
 
 
+def format_error(error: GraphQLError) -> GraphQLFormattedError:
+    if not isinstance(error, GraphQLError):
+        raise TypeError("Expected a GraphQLError.")
+    return error.formatted
+
+
 @dataclass
 class GraphQLApp:
     schema: graphene.Schema
     graphiql: bool = True
     context_value: t.Optional[t.Any] = None
     root_value: t.Optional[t.Any] = None
     middleware: t.Optional[Middleware] = None
-    error_formatter: t.Callable[[GraphQLError], t.Dict[str, t.Any]] = format_error
+    error_formatter: t.Callable[[GraphQLError], GraphQLFormattedError] = format_error
     execution_context_class: t.Optional[t.Type[ExecutionContext]] = None
 
     async def __call__(self, scope: st.Scope, receive: st.Receive, send: st.Send) -> None:
         request = Request(scope, receive=receive)
         response = await self._handle_graphql(request)
         await response(scope, receive, send)
```

### Comparing `starlette-graphene-0.2.0/starlette_graphene.egg-info/PKG-INFO` & `starlette-graphene-0.3.0/starlette_graphene.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,105 @@
 Metadata-Version: 2.1
 Name: starlette-graphene
-Version: 0.2.0
+Version: 0.3.0
 Summary: Helper for add support for graphene in starlette
 Home-page: https://github.com/bigbag/starlette-graphene
+Download-URL: https://pypi.python.org/pypi/starlette-graphene
 Author: Pavel Liashkov
 Author-email: pavel.liashkov@protonmail.com
 Maintainer: Pavel Liashkov
 Maintainer-email: pavel.liashkov@protonmail.com
 License: Apache License, Version 2.0
-Download-URL: https://pypi.python.org/pypi/starlette-graphene
-Description: # starlette-graphene
-        
-        [![CI](https://github.com/bigbag/starlette-graphene/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-graphene/actions?query=workflow%3ACI)
-        [![codecov](https://codecov.io/gh/bigbag/starlette-graphene/branch/main/graph/badge.svg?token=FQTY888XG1)](https://codecov.io/gh/bigbag/starlette-graphene)
-        [![pypi](https://img.shields.io/pypi/v/starlette-graphene.svg)](https://pypi.python.org/pypi/starlette-graphene)
-        [![downloads](https://img.shields.io/pypi/dm/starlette-graphene.svg)](https://pypistats.org/packages/starlette-graphene)
-        [![versions](https://img.shields.io/pypi/pyversions/starlette-graphene.svg)](https://github.com/bigbag/starlette-graphene)
-        [![license](https://img.shields.io/github/license/bigbag/starlette-graphene.svg)](https://github.com/bigbag/starlette-graphene/blob/master/LICENSE)
-        
-        
-        **starlette-graphene** is a helper for add support for graphene in starlette.
-        
-        
-        ## Installation
-        
-        starlette-graphene is available on PyPI.
-        Use pip to install:
-        
-            $ pip install starlette-graphene
-        
-        ## Basic Usage
-        
-        ```py
-        import uvicorn
-        from graphene import types as grt
-        from starlette.applications import Starlette
-        
-        from starlette_graphene import GraphQLApp
-        
-        
-        class Account(grt.ObjectType):
-            account = grt.Int(required=True)
-        
-        
-        class AccountFilter(grt.InputObjectType):
-            accounts = grt.List(grt.Int)
-        
-        
-        class Query(grt.ObjectType):
-            course_list = None
-            accounts = grt.Field(
-                grt.List(Account),
-                filters=AccountFilter(),
-            )
-        
-            async def resolve_accounts(
-                self,
-                info,
-                filters: AccountFilter,
-            ):
-        
-                return [Account(account=1212), Account(account=43434)]
-        
-        
-        def get_graphql_app() -> GraphQLApp:
-            return GraphQLApp(schema=grt.Schema(query=Query))
-        
-        
-        def init_app():
-            app_ = Starlette()
-            app_.mount("/graphql/", get_graphql_app())
-            return app_
-        
-        
-        app = init_app()
-        
-        if __name__ == "__main__":
-            uvicorn.run(app=app)
-        ```
-        
-        ## License
-        
-        starlette-graphene is developed and distributed under the Apache 2.0 license.
-        
-        ## Reporting a Security Vulnerability
-        
-        See our [security policy](https://github.com/bigbag/starlette-graphene/security/policy).
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
+# starlette-graphene
+
+[![CI](https://github.com/bigbag/starlette-graphene/workflows/CI/badge.svg)](https://github.com/bigbag/starlette-graphene/actions?query=workflow%3ACI)
+[![codecov](https://codecov.io/gh/bigbag/starlette-graphene/branch/main/graph/badge.svg?token=FQTY888XG1)](https://codecov.io/gh/bigbag/starlette-graphene)
+[![pypi](https://img.shields.io/pypi/v/starlette-graphene.svg)](https://pypi.python.org/pypi/starlette-graphene)
+[![downloads](https://img.shields.io/pypi/dm/starlette-graphene.svg)](https://pypistats.org/packages/starlette-graphene)
+[![versions](https://img.shields.io/pypi/pyversions/starlette-graphene.svg)](https://github.com/bigbag/starlette-graphene)
+[![license](https://img.shields.io/github/license/bigbag/starlette-graphene.svg)](https://github.com/bigbag/starlette-graphene/blob/master/LICENSE)
+
+
+**starlette-graphene** is a helper for add support for graphene in starlette.
+
+
+## Installation
+
+starlette-graphene is available on PyPI.
+Use pip to install:
+
+    $ pip install starlette-graphene
+
+## Basic Usage
+
+```py
+import uvicorn
+from graphene import types as grt
+from starlette.applications import Starlette
+
+from starlette_graphene import GraphQLApp
+
+
+class Account(grt.ObjectType):
+    account = grt.Int(required=True)
+
+
+class AccountFilter(grt.InputObjectType):
+    accounts = grt.List(grt.Int)
+
+
+class Query(grt.ObjectType):
+    course_list = None
+    accounts = grt.Field(
+        grt.List(Account),
+        filters=AccountFilter(),
+    )
+
+    async def resolve_accounts(
+        self,
+        info,
+        filters: AccountFilter,
+    ):
+
+        return [Account(account=1212), Account(account=43434)]
+
+
+def get_graphql_app() -> GraphQLApp:
+    return GraphQLApp(schema=grt.Schema(query=Query))
+
+
+def init_app():
+    app_ = Starlette()
+    app_.mount("/graphql/", get_graphql_app())
+    return app_
+
+
+app = init_app()
+
+if __name__ == "__main__":
+    uvicorn.run(app=app)
+```
+
+## License
+
+starlette-graphene is developed and distributed under the Apache 2.0 license.
+
+## Reporting a Security Vulnerability
+
+See our [security policy](https://github.com/bigbag/starlette-graphene/security/policy).
```

