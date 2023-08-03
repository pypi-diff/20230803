# Comparing `tmp/pulp-glue-0.20.3.tar.gz` & `tmp/pulp-glue-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-0.20.3.tar", last modified: Fri Jul 28 15:30:58 2023, max compression
+gzip compressed data, was "pulp-glue-0.21.0.tar", last modified: Thu Aug  3 12:58:38 2023, max compression
```

## Comparing `pulp-glue-0.20.3.tar` & `pulp-glue-0.21.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.136000 pulp-glue-0.20.3/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-28 15:30:58.136000 pulp-glue-0.20.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/ansible/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/ansible/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/certguard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/certguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/certguard/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/certguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/common/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38246 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/common/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/common/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/common/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/container/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/container/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/file/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/file/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.136000 pulp-glue-0.20.3/pulp_glue/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/python/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/python/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.136000 pulp-glue-0.20.3/pulp_glue/rpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/rpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/rpm/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pulp_glue/rpm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:30:58.132000 pulp-glue-0.20.3/pulp_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-28 15:30:58.000000 pulp-glue-0.20.3/pulp_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 15:30:58.000000 pulp-glue-0.20.3/pulp_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:30:58.000000 pulp-glue-0.20.3/pulp_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 15:30:58.000000 pulp-glue-0.20.3/pulp_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 15:30:58.000000 pulp-glue-0.20.3/pulp_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:30:58.136000 pulp-glue-0.20.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-28 15:30:48.000000 pulp-glue-0.20.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.427363 pulp-glue-0.21.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-03 12:58:38.427363 pulp-glue-0.21.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.423363 pulp-glue-0.21.0/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.423363 pulp-glue-0.21.0/pulp_glue/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/ansible/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/ansible/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.423363 pulp-glue-0.21.0/pulp_glue/certguard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/certguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/certguard/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/certguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.427363 pulp-glue-0.21.0/pulp_glue/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37710 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/common/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/common/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/common/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.427363 pulp-glue-0.21.0/pulp_glue/container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/container/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/container/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.427363 pulp-glue-0.21.0/pulp_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.427363 pulp-glue-0.21.0/pulp_glue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/file/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/file/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.427363 pulp-glue-0.21.0/pulp_glue/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/python/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.427363 pulp-glue-0.21.0/pulp_glue/rpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/rpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/rpm/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pulp_glue/rpm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:58:38.423363 pulp-glue-0.21.0/pulp_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-03 12:58:38.000000 pulp-glue-0.21.0/pulp_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-03 12:58:38.000000 pulp-glue-0.21.0/pulp_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:58:38.000000 pulp-glue-0.21.0/pulp_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 12:58:38.000000 pulp-glue-0.21.0/pulp_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 12:58:38.000000 pulp-glue-0.21.0/pulp_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:58:38.427363 pulp-glue-0.21.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-03 12:58:27.000000 pulp-glue-0.21.0/setup.py
```

### Comparing `pulp-glue-0.20.3/PKG-INFO` & `pulp-glue-0.21.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.20.3
+Version: 0.21.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-0.20.3/pulp_glue/ansible/context.py` & `pulp-glue-0.21.0/pulp_glue/ansible/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.3/pulp_glue/certguard/context.py` & `pulp-glue-0.21.0/pulp_glue/certguard/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.3/pulp_glue/common/context.py` & `pulp-glue-0.21.0/pulp_glue/common/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import os
 import re
 import sys
 import time
+import typing as t
 from typing import IO, Any, ClassVar, Dict, List, Mapping, Optional, Set, Type, Union, cast
 
 from packaging.specifiers import SpecifierSet
 from requests import HTTPError
 
 from pulp_glue.common.i18n import get_translation
 from pulp_glue.common.openapi import OpenAPI, OpenAPIError
@@ -71,14 +72,19 @@
             self.specifier = SpecifierSet(specifier, prereleases=True)
 
     def __contains__(self, version: Optional[str]) -> bool:
         if version is None:
             return self.inverted
         return (version in self.specifier) != self.inverted
 
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}({self.name}{self.specifier})"
+
+    __repr__ = __str__
+
 
 class PulpException(Exception):
     pass
 
 
 class PulpNoWait(Exception):
     pass
@@ -99,14 +105,86 @@
         return payload
 
     return PreprocessedEntityDefinition(
         {key: _preprocess_value(value) for key, value in payload.items() if value is not None}
     )
 
 
+_REGISTERED_API_QUIRKS: t.List[t.Tuple[PluginRequirement, t.Callable[[OpenAPI], None]]] = []
+
+
+def api_quirk(
+    req: PluginRequirement,
+) -> t.Callable[[t.Callable[[OpenAPI], None]], None]:
+    def _decorator(patch: t.Callable[[OpenAPI], None]) -> None:
+        _REGISTERED_API_QUIRKS.append((req, patch))
+
+    return _decorator
+
+
+@api_quirk(PluginRequirement("core", specifier="<3.20.0"))
+def patch_ordering_filters(api: OpenAPI) -> None:
+    for method, path in api.operations.values():
+        operation = api.api_spec["paths"][path][method]
+        if method == "get" and "parameters" in operation:
+            for parameter in operation["parameters"]:
+                if (
+                    parameter["name"] == "ordering"
+                    and parameter["in"] == "query"
+                    and "schema" in parameter
+                    and parameter["schema"]["type"] == "string"
+                ):
+                    parameter["schema"] = {"type": "array", "items": {"type": "string"}}
+                    parameter["explode"] = False
+                    parameter["style"] = "form"
+
+
+@api_quirk(PluginRequirement("core", specifier="<3.22.0"))
+def patch_field_select_filters(api: OpenAPI) -> None:
+    for method, path in api.operations.values():
+        operation = api.api_spec["paths"][path][method]
+        if method == "get" and "parameters" in operation:
+            for parameter in operation["parameters"]:
+                if (
+                    parameter["name"] in ["fields", "exclude_fields"]
+                    and parameter["in"] == "query"
+                    and "schema" in parameter
+                    and parameter["schema"]["type"] == "string"
+                ):
+                    parameter["schema"] = {"type": "array", "items": {"type": "string"}}
+
+
+@api_quirk(PluginRequirement("core", specifier="<99.99.0"))
+def patch_content_in_query_filters(api: OpenAPI) -> None:
+    # https://github.com/pulp/pulpcore/issues/3634
+    for operation_id, (method, path) in api.operations.items():
+        if (
+            operation_id == "repository_versions_list"
+            or (
+                operation_id.startswith("repositories_") and operation_id.endswith("_versions_list")
+            )
+            or (operation_id.startswith("publications_") and operation_id.endswith("_list"))
+        ):
+            operation = api.api_spec["paths"][path][method]
+            for parameter in operation["parameters"]:
+                if (
+                    parameter["name"] == "content__in"
+                    and parameter["in"] == "query"
+                    and "schema" in parameter
+                    and parameter["schema"]["type"] == "string"
+                ):
+                    parameter["schema"] = {"type": "array", "items": {"type": "string"}}
+
+
+@api_quirk(PluginRequirement("core", specifier=">=3.23,<3.30.0"))
+def patch_upstream_pulp_replicate_request_body(api: OpenAPI) -> None:
+    operation = api.api_spec["paths"]["{upstream_pulp_href}replicate/"]["post"]
+    operation.pop("requestBody", None)
+
+
 class PulpContext:
     """
     Abstract class for the global PulpContext object.
     It is an abstraction layer for api access and output handling.
     """
 
     def echo(self, message: str, nl: bool = True, err: bool = False) -> None:
@@ -116,98 +194,39 @@
         raise NotImplementedError("PulpContext is an abstract class.")
 
     def __init__(
         self,
         api_root: str,
         api_kwargs: Dict[str, Any],
         background_tasks: bool,
-        timeout: int,
+        timeout: Union[int, datetime.timedelta],
         domain: str = "default",
         format: Optional[str] = None,  # Deprecated
     ) -> None:
         self._api: Optional[OpenAPI] = None
         self._api_root: str = api_root
         self._api_kwargs = api_kwargs
         self._needed_plugins: List[PluginRequirement] = [
             PluginRequirement("core", specifier=">=3.11.0")
         ]
         self.isatty: bool = sys.stdout.isatty()
         self.pulp_domain: str = domain
 
         self.background_tasks: bool = background_tasks
-        self.timeout: int = timeout
-        self.start_time: Optional[datetime.datetime] = None
+        if isinstance(timeout, int):
+            timeout = datetime.timedelta(seconds=timeout)
+        self.timeout: datetime.timedelta = timeout
 
     def _patch_api_spec(self) -> None:
         # A place for last minute fixes to the api_spec.
         # WARNING: Operations are already indexed at this point.
-        api_spec = self.api.api_spec
-        if self.has_plugin(PluginRequirement("core", specifier="<3.20.0")):
-            for method, path in self.api.operations.values():
-                operation = api_spec["paths"][path][method]
-                if method == "get" and "parameters" in operation:
-                    for parameter in operation["parameters"]:
-                        if (
-                            parameter["name"] == "ordering"
-                            and parameter["in"] == "query"
-                            and "schema" in parameter
-                            and parameter["schema"]["type"] == "string"
-                        ):
-                            parameter["schema"] = {"type": "array", "items": {"type": "string"}}
-                            parameter["explode"] = False
-                            parameter["style"] = "form"
-        if self.has_plugin(PluginRequirement("core", specifier="<3.22.0")):
-            for method, path in self.api.operations.values():
-                operation = api_spec["paths"][path][method]
-                if method == "get" and "parameters" in operation:
-                    for parameter in operation["parameters"]:
-                        if (
-                            parameter["name"] in ["fields", "exclude_fields"]
-                            and parameter["in"] == "query"
-                            and "schema" in parameter
-                            and parameter["schema"]["type"] == "string"
-                        ):
-                            parameter["schema"] = {"type": "array", "items": {"type": "string"}}
-        if self.has_plugin(PluginRequirement("core", specifier="<99.99.0")):
-            # https://github.com/pulp/pulpcore/issues/3634
-            for operation_id, (method, path) in self.api.operations.items():
-                if (
-                    operation_id == "repository_versions_list"
-                    or (
-                        operation_id.startswith("repositories_")
-                        and operation_id.endswith("_versions_list")
-                    )
-                    or (operation_id.startswith("publications_") and operation_id.endswith("_list"))
-                ):
-                    operation = api_spec["paths"][path][method]
-                    for parameter in operation["parameters"]:
-                        if (
-                            parameter["name"] == "content__in"
-                            and parameter["in"] == "query"
-                            and "schema" in parameter
-                            and parameter["schema"]["type"] == "string"
-                        ):
-                            parameter["schema"] = {"type": "array", "items": {"type": "string"}}
-        if self.has_plugin(PluginRequirement("file", specifier=">=1.10.0,<1.11.0")):
-            operation = api_spec["paths"]["{file_file_alternate_content_source_href}refresh/"][
-                "post"
-            ]
-            operation.pop("requestBody", None)
-        if self.has_plugin(
-            PluginRequirement("python", specifier="<99.99.0.dev")
-        ):  # TODO Add version bounds
-            python_remote_serializer = api_spec["components"]["schemas"]["python.PythonRemote"]
-            patched_python_remote_serializer = api_spec["components"]["schemas"][
-                "Patchedpython.PythonRemote"
-            ]
-            for prop in ("includes", "excludes"):
-                python_remote_serializer["properties"][prop]["type"] = "array"
-                python_remote_serializer["properties"][prop]["items"] = {"type": "string"}
-                patched_python_remote_serializer["properties"][prop]["type"] = "array"
-                patched_python_remote_serializer["properties"][prop]["items"] = {"type": "string"}
+        assert self._api is not None
+        for req, patch in _REGISTERED_API_QUIRKS:
+            if self.has_plugin(req):
+                patch(self._api)
 
     @property
     def domain_enabled(self) -> bool:
         return cast(bool, self.api.api_spec.get("info", {}).get("x-pulp-domain-enabled", False))
 
     @property
     def api_path(self) -> str:
@@ -291,16 +310,16 @@
                 ),
                 err=True,
             )
             if not non_blocking:
                 result = self.wait_for_task_group(result)
         return result
 
-    @classmethod
-    def _check_task_finished(cls, task: EntityDefinition, expect_cancel: bool = False) -> bool:
+    @staticmethod
+    def _task_finished(task: EntityDefinition, expect_cancel: bool = False) -> bool:
         task_href = task["pulp_href"]
 
         if task["state"] == "completed":
             if expect_cancel:
                 raise PulpException(
                     _("The task {task_href} meant to be canceled, completed instead.")
                 )
@@ -317,85 +336,81 @@
                 return True
             raise PulpException(_("Task {task_href} canceled").format(task_href=task_href))
         elif task["state"] in ["waiting", "running", "canceling"]:
             return False
         else:
             raise NotImplementedError(_("Unknown task state: {state}").format(state=task["state"]))
 
-    def _poll_task(self, task: EntityDefinition, expect_cancel: bool = False) -> EntityDefinition:
-        while True:
-            if self._check_task_finished(task, expect_cancel=expect_cancel):
-                self.echo("Done.", err=True)
-                return task
-            else:
-                if self.timeout:
-                    assert isinstance(self.start_time, datetime.datetime)
-                    if (datetime.datetime.now() - self.start_time).seconds > self.timeout:
-                        raise PulpNoWait(
-                            _("Waiting for task {task_href} timed out.").format(
-                                task_href=task["pulp_href"]
-                            )
-                        )
-                time.sleep(1)
-                self.echo(".", nl=False, err=True)
-                task = self.api.call("tasks_read", parameters={"task_href": task["pulp_href"]})
-
     def wait_for_task(self, task: EntityDefinition, expect_cancel: bool = False) -> Any:
         """
         Wait for a task to finish and return the finished task object.
 
         Raise `PulpNoWait` on timeout, background, ctrl-c, if task failed or was canceled.
         """
-        self.start_time = datetime.datetime.now()
+        deadline = datetime.datetime.now() + self.timeout if self.timeout else None
 
         if self.background_tasks:
             raise PulpNoWait(_("Not waiting for task because --background was specified."))
         task_href = task["pulp_href"]
         try:
-            return self._poll_task(task, expect_cancel=expect_cancel)
+            while not self._task_finished(task, expect_cancel=expect_cancel):
+                if deadline and datetime.datetime.now() > deadline:
+                    raise PulpNoWait(
+                        _("Waiting for task {task_href} timed out.").format(
+                            task_href=task["pulp_href"]
+                        )
+                    )
+                time.sleep(1)
+                self.echo(".", nl=False, err=True)
+                task = self.api.call("tasks_read", parameters={"task_href": task["pulp_href"]})
+            self.echo("Done.", err=True)
+            return task
         except KeyboardInterrupt:
             raise PulpNoWait(_("Task {task_href} sent to background.").format(task_href=task_href))
 
+    def _task_group_finished(self, task_group: EntityDefinition) -> bool:
+        if task_group["waiting"] + task_group["running"] + task_group["canceling"] > 0:
+            return False
+        if task_group["failed"] + task_group["canceled"] > 0:
+            errors = []
+            for task in task_group["tasks"]:
+                if task["state"] in ["failed", "canceled"]:
+                    task = self.api.call("tasks_read", parameters={"task_href": task["pulp_href"]})
+                    errors.append(task["error"].get("description") or task["error"].get("reason"))
+            raise PulpException(
+                _("Task group {task_group_href} has failed/canceled tasks: '{errors}'").format(
+                    task_group_href=task_group["pulp_href"],
+                    errors="\n".join(errors),
+                )
+            )
+        return True
+
     def wait_for_task_group(self, task_group: EntityDefinition) -> Any:
         """
         Wait for a task group to finish and return the finished task object.
 
         Raise `PulpNoWait` on timeout, background, ctrl-c, if tasks failed or were canceled.
         """
-        self.start_time = datetime.datetime.now()
+        deadline = datetime.datetime.now() + self.timeout if self.timeout else None
 
         if self.background_tasks:
             raise PulpNoWait("Not waiting for task group because --background was specified.")
         try:
-            while True:
-                if task_group["all_tasks_dispatched"] is True:
-                    for task in task_group["tasks"]:
-                        task = self.api.call(
-                            "tasks_read", parameters={"task_href": task["pulp_href"]}
-                        )
-                        self.echo(
-                            _("Waiting for task {task_href}").format(task_href=task["pulp_href"]),
-                            err=True,
+            while not self._task_group_finished(task_group):
+                if deadline and datetime.datetime.now() > deadline:
+                    raise PulpNoWait(
+                        _("Waiting for task group {task_group_href} timed out.").format(
+                            task_group_href=task_group["pulp_href"]
                         )
-                        self._poll_task(task)
-                    return task_group
-                else:
-                    if self.timeout:
-                        assert isinstance(self.start_time, datetime.datetime)
-                        if (datetime.datetime.now() - self.start_time).seconds > self.timeout:
-                            raise PulpNoWait(
-                                _("Waiting for task group {task_group_href} timed out.").format(
-                                    task_group_href=task_group["pulp_href"]
-                                )
-                            )
-                    time.sleep(1)
-                    self.echo(".", nl=False, err=True)
-                    task_group = self.api.call(
-                        "task_groups_read", parameters={"task_group_href": task_group["pulp_href"]}
                     )
+                time.sleep(1)
+                self.echo(".", nl=False, err=True)
+                task_group = self.api.call(
+                    "task_groups_read", parameters={"task_group_href": task_group["pulp_href"]}
+                )
         except KeyboardInterrupt:
             raise PulpNoWait(
                 _("Task group {task_group_href} sent to background.").format(
                     task_group_href=task_group["pulp_href"]
                 )
             )
```

### Comparing `pulp-glue-0.20.3/pulp_glue/common/i18n.py` & `pulp-glue-0.21.0/pulp_glue/common/i18n.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.3/pulp_glue/common/openapi.py` & `pulp-glue-0.21.0/pulp_glue/common/openapi.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.3/pulp_glue/container/context.py` & `pulp-glue-0.21.0/pulp_glue/container/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.3/pulp_glue/core/context.py` & `pulp-glue-0.21.0/pulp_glue/core/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -527,7 +527,37 @@
 
 class PulpWorkerContext(PulpEntityContext):
     ENTITY = _("worker")
     ENTITIES = _("workers")
     HREF = "worker_href"
     ID_PREFIX = "workers"
     HREF_PATTERN = r"workers/"
+
+
+class PulpUpstreamPulpContext(PulpEntityContext):
+    ENTITY = _("upstream pulp")
+    ENTITIES = _("upstream pulps")
+    HREF = "upstream_pulp_href"
+    ID_PREFIX = "upstream_pulps"
+    HREF_PATTERN = r"upstream-pulps/"
+    NEEDS_PLUGINS = [PluginRequirement("core", specifier=">=3.23.0")]
+
+    def find(self, **kwargs: Any) -> Any:
+        """Workaroud for the missing ability to filter"""
+        # # TODO fix upstream and adjust to guard for the proper version
+        # # https://github.com/pulp/pulpcore/issues/4110
+        # if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.99.dev")):
+        #     # Workaround not needed anymore
+        #     return super().find(**kwargs)
+        search_result = self.list(limit=sys.maxsize, offset=0, parameters={})
+        for key, value in kwargs.items():
+            search_result = [res for res in search_result if res[key] == value]
+        if len(search_result) != 1:
+            raise PulpException(
+                _("Could not find {entity} with {kwargs}.").format(
+                    entity=self.ENTITY, kwargs=kwargs
+                )
+            )
+        return search_result[0]
+
+    def replicate(self) -> Any:
+        return self.call("replicate", parameters={self.HREF: self.pulp_href})
```

### Comparing `pulp-glue-0.20.3/pulp_glue/file/context.py` & `pulp-glue-0.21.0/pulp_glue/file/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-from typing import Any, Mapping, Optional
+import typing as t
 
 from pulp_glue.common.context import (
     EntityDefinition,
     PluginRequirement,
     PulpACSContext,
     PulpContentContext,
     PulpDistributionContext,
     PulpPublicationContext,
     PulpRemoteContext,
     PulpRepositoryContext,
     PulpRepositoryVersionContext,
+    api_quirk,
 )
 from pulp_glue.common.i18n import get_translation
+from pulp_glue.common.openapi import OpenAPI
 from pulp_glue.core.context import PulpArtifactContext
 
 translation = get_translation(__name__)
 _ = translation.gettext
 
 
+@api_quirk(PluginRequirement("file", specifier=">=1.10.0,<1.11.0"))
+def patch_file_acs_refresh_request_body(api: OpenAPI) -> None:
+    operation = api.api_spec["paths"]["{file_file_alternate_content_source_href}refresh/"]["post"]
+    operation.pop("requestBody", None)
+
+
 class PulpFileACSContext(PulpACSContext):
     PLUGIN = "file"
     RESOURCE_TYPE = "file"
     ENTITY = _("file ACS")
     ENTITIES = _("file ACSes")
     HREF = "file_file_alternate_content_source_href"
     ID_PREFIX = "acs_file_file"
@@ -38,17 +46,17 @@
     ID_PREFIX = "content_file_files"
     NEEDS_PLUGINS = [PluginRequirement("file", specifier=">=1.6.0")]
     CAPABILITIES = {"upload": []}
 
     def create(
         self,
         body: EntityDefinition,
-        parameters: Optional[Mapping[str, Any]] = None,
+        parameters: t.Optional[t.Mapping[str, t.Any]] = None,
         non_blocking: bool = False,
-    ) -> Any:
+    ) -> t.Any:
         if "sha256" in body:
             body = body.copy()
             body["artifact"] = PulpArtifactContext(
                 self.pulp_ctx, entity={"sha256": body.pop("sha256")}
             )
         return super().create(body=body, parameters=parameters, non_blocking=non_blocking)
```

### Comparing `pulp-glue-0.20.3/pulp_glue/python/context.py` & `pulp-glue-0.21.0/pulp_glue/python/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,36 @@
     PluginRequirement,
     PulpContentContext,
     PulpDistributionContext,
     PulpPublicationContext,
     PulpRemoteContext,
     PulpRepositoryContext,
     PulpRepositoryVersionContext,
+    api_quirk,
 )
 from pulp_glue.common.i18n import get_translation
+from pulp_glue.common.openapi import OpenAPI
 
 translation = get_translation(__name__)
 _ = translation.gettext
 
 
+@api_quirk(PluginRequirement("python", specifier="<3.9.0"))
+def patch_python_remote_includes_excludes(api: OpenAPI) -> None:
+    python_remote_serializer = api.api_spec["components"]["schemas"]["python.PythonRemote"]
+    patched_python_remote_serializer = api.api_spec["components"]["schemas"][
+        "Patchedpython.PythonRemote"
+    ]
+    for prop in ("includes", "excludes"):
+        python_remote_serializer["properties"][prop]["type"] = "array"
+        python_remote_serializer["properties"][prop]["items"] = {"type": "string"}
+        patched_python_remote_serializer["properties"][prop]["type"] = "array"
+        patched_python_remote_serializer["properties"][prop]["items"] = {"type": "string"}
+
+
 class PulpPythonContentContext(PulpContentContext):
     PLUGIN = "python"
     RESOURCE_TYPE = "package"
     ENTITY = _("python package")
     ENTITIES = _("python packages")
     HREF = "python_python_package_content_href"
     ID_PREFIX = "content_python_packages"
```

### Comparing `pulp-glue-0.20.3/pulp_glue/rpm/context.py` & `pulp-glue-0.21.0/pulp_glue/rpm/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     PLUGIN = "rpm"
     RESOURCE_TYPE = "rpm"
     ENTITY = _("rpm ACS")
     ENTITIES = _("rpm ACSes")
     HREF = "rpm_rpm_alternate_content_source_href"
     ID_PREFIX = "acs_rpm_rpm"
     NEEDS_PLUGINS = [PluginRequirement("rpm", specifier=">=3.18.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("rpm", specifier=">=3.19.0")]}
 
 
 class PulpRpmCompsXmlContext(PulpEntityContext):
     UPLOAD_COMPS_ID: ClassVar[str] = "rpm_comps_upload"
     NEEDS_PLUGINS = [PluginRequirement("rpm", specifier=">=3.17.0")]
 
     def upload_comps(
@@ -50,14 +51,15 @@
     PLUGIN = "rpm"
     RESOURCE_TYPE = "rpm"
     ENTITY = _("rpm distribution")
     ENTITIES = _("rpm distributions")
     HREF = "rpm_rpm_distribution_href"
     ID_PREFIX = "distributions_rpm_rpm"
     NEEDS_PLUGINS = [PluginRequirement("rpm", specifier=">=3.9.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("rpm", specifier=">=3.19.0")]}
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         if self.pulp_ctx.has_plugin(PluginRequirement("core", specifier=">=3.16.0")):
             if "repository" in body and "publication" not in body:
                 body["publication"] = None
             if "repository" not in body and "publication" in body:
@@ -179,14 +181,15 @@
     PLUGIN = "rpm"
     RESOURCE_TYPE = "rpm"
     ENTITY = _("rpm publication")
     ENTITIES = _("rpm publications")
     HREF = "rpm_rpm_publication_href"
     ID_PREFIX = "publications_rpm_rpm"
     NEEDS_PLUGINS = [PluginRequirement("rpm", specifier=">=3.9.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("rpm", specifier=">=3.19.0")]}
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         version = body.pop("version", None)
         if version is not None:
             repository_href = body.pop("repository")
             body["repository_version"] = f"{repository_href}versions/{version}/"
@@ -208,25 +211,27 @@
         "password",
         "proxy_url",
         "proxy_username",
         "proxy_password",
         "sles_auth_token",
     }
     NEEDS_PLUGINS = [PluginRequirement("rpm", specifier=">=3.9.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("rpm", specifier=">=3.19.0")]}
 
 
 class PulpUlnRemoteContext(PulpRemoteContext):
     PLUGIN = "rpm"
     RESOURCE_TYPE = "uln"
     ENTITY = _("uln remote")
     ENTITIES = _("uln remotes")
     HREF = "rpm_uln_remote_href"
     ID_PREFIX = "remotes_rpm_uln"
     NULLABLES = PulpRemoteContext.NULLABLES | {"uln-server-base-url"}
     NEEDS_PLUGINS = [PluginRequirement("rpm", specifier=">=3.12.0")]
+    CAPABILITIES = {"roles": [PluginRequirement("rpm", specifier=">=3.19.0")]}
 
 
 class PulpRpmRepositoryVersionContext(PulpRepositoryVersionContext):
     HREF = "rpm_rpm_repository_version_href"
     ID_PREFIX = "repositories_rpm_rpm_versions"
     NEEDS_PLUGINS = [PluginRequirement("rpm", specifier=">=3.9.0")]
 
@@ -235,15 +240,19 @@
     PLUGIN = "rpm"
     RESOURCE_TYPE = "rpm"
     HREF = "rpm_rpm_repository_href"
     ID_PREFIX = "repositories_rpm_rpm"
     ENTITY = _("rpm repository")
     ENTITIES = _("rpm repositories")
     VERSION_CONTEXT = PulpRpmRepositoryVersionContext
-    CAPABILITIES = {"sync": [], "pulpexport": []}
+    CAPABILITIES = {
+        "sync": [],
+        "pulpexport": [],
+        "roles": [PluginRequirement("rpm", specifier=">=3.19.0")],
+    }
     NEEDS_PLUGINS = [PluginRequirement("rpm", specifier=">=3.9.0")]
 
     def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
         body = super().preprocess_entity(body, partial=partial)
         if "autopublish" in body:
             self.pulp_ctx.needs_plugin(PluginRequirement("rpm", specifier=">=3.12.0"))
         return body
```

### Comparing `pulp-glue-0.20.3/pulp_glue.egg-info/PKG-INFO` & `pulp-glue-0.21.0/pulp_glue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.20.3
+Version: 0.21.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-0.20.3/pulp_glue.egg-info/SOURCES.txt` & `pulp-glue-0.21.0/pulp_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.20.3/setup.py` & `pulp-glue-0.21.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     name="pulp-glue",
     description="Version agnostic glue library to talk to pulpcore's REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Pulp Team",
     author_email="pulp-list@redhat.com",
     url="https://github.com/pulp/pulp-cli",
-    version="0.20.3",
+    version="0.21.0",
     packages=plugin_packages,
     package_data={"": ["py.typed"]},
     python_requires=">=3.6",
     install_requires=[
         "packaging>=20.0,<24",
         "requests>=2.24.0,<2.32",
     ],
```

