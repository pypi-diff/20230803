# Comparing `tmp/neoclient-0.1.19.tar.gz` & `tmp/neoclient-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neoclient-0.1.19.tar", max compression
+gzip compressed data, was "neoclient-0.1.29.tar", max compression
```

## Comparing `neoclient-0.1.19.tar` & `neoclient-0.1.29.tar`

### file list

```diff
@@ -1,31 +1,39 @@
--rw-r--r--   0        0        0     1067 2023-02-10 21:07:01.444198 neoclient-0.1.19/LICENSE
--rw-r--r--   0        0        0      545 2023-03-01 23:02:53.097704 neoclient-0.1.19/README.md
--rw-r--r--   0        0        0     1010 2023-03-01 23:02:53.097704 neoclient-0.1.19/neoclient/__init__.py
--rw-r--r--   0        0        0     1134 2023-02-10 21:07:01.448198 neoclient-0.1.19/neoclient/api.py
--rw-r--r--   0        0        0     7871 2023-03-01 23:02:53.097704 neoclient-0.1.19/neoclient/client.py
--rw-r--r--   0        0        0     4393 2023-03-01 22:35:23.690076 neoclient-0.1.19/neoclient/composition.py
--rw-r--r--   0        0        0     6617 2023-03-01 23:02:53.097704 neoclient-0.1.19/neoclient/consumers.py
--rw-r--r--   0        0        0     3023 2023-03-01 22:35:23.750076 neoclient-0.1.19/neoclient/converters.py
--rw-r--r--   0        0        0     4544 2023-03-01 23:02:53.097704 neoclient-0.1.19/neoclient/decorators.py
--rw-r--r--   0        0        0     1001 2023-03-01 22:35:23.598076 neoclient-0.1.19/neoclient/defaults.py
--rw-r--r--   0        0        0     5720 2023-03-01 22:35:23.730076 neoclient-0.1.19/neoclient/dependencies.py
--rw-r--r--   0        0        0     1154 2023-03-01 23:02:53.097704 neoclient-0.1.19/neoclient/enums.py
--rw-r--r--   0        0        0     1474 2023-02-26 21:29:40.180359 neoclient-0.1.19/neoclient/errors.py
--rw-r--r--   0        0        0     1621 2023-02-10 21:07:01.448198 neoclient-0.1.19/neoclient/methods.py
--rw-r--r--   0        0        0     2422 2023-02-26 21:29:40.180359 neoclient-0.1.19/neoclient/middleware.py
--rw-r--r--   0        0        0    14789 2023-03-01 23:02:53.097704 neoclient-0.1.19/neoclient/models.py
--rw-r--r--   0        0        0     3808 2023-02-26 21:29:40.180359 neoclient-0.1.19/neoclient/operation.py
--rw-r--r--   0        0        0     7628 2023-03-01 22:35:23.834077 neoclient-0.1.19/neoclient/param_functions.py
--rw-r--r--   0        0        0     9532 2023-02-26 21:29:40.180359 neoclient-0.1.19/neoclient/param_functions.pyi
--rw-r--r--   0        0        0    10943 2023-03-01 23:02:53.097704 neoclient-0.1.19/neoclient/params.py
--rw-r--r--   0        0        0        0 2023-02-10 21:07:01.448198 neoclient-0.1.19/neoclient/py.typed
--rw-r--r--   0        0        0      283 2023-02-26 21:29:40.180359 neoclient-0.1.19/neoclient/resolution.py
--rw-r--r--   0        0        0     1737 2023-02-26 21:29:40.180359 neoclient-0.1.19/neoclient/resolvers.py
--rw-r--r--   0        0        0     1314 2023-03-01 23:02:53.097704 neoclient-0.1.19/neoclient/service.py
--rw-r--r--   0        0        0     2181 2023-03-01 22:35:23.658076 neoclient-0.1.19/neoclient/types.py
--rw-r--r--   0        0        0      980 2023-03-01 23:02:53.097704 neoclient-0.1.19/neoclient/typing.py
--rw-r--r--   0        0        0     3394 2023-03-01 23:02:53.097704 neoclient-0.1.19/neoclient/utils.py
--rw-r--r--   0        0        0     5760 2023-03-01 22:35:23.870077 neoclient-0.1.19/neoclient/validation.py
--rw-r--r--   0        0        0     1090 2023-03-01 23:02:53.097704 neoclient-0.1.19/pyproject.toml
--rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 neoclient-0.1.19/setup.py
--rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 neoclient-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-10 21:07:01.444198 neoclient-0.1.29/LICENSE
+-rw-r--r--   0        0        0      545 2023-03-01 23:02:53.097704 neoclient-0.1.29/README.md
+-rw-r--r--   0        0        0     1062 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/__init__.py
+-rw-r--r--   0        0        0      374 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/annotations.py
+-rw-r--r--   0        0        0     1134 2023-02-10 21:07:01.448198 neoclient-0.1.29/neoclient/api.py
+-rw-r--r--   0        0        0    11794 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/client.py
+-rw-r--r--   0        0        0     4658 2023-03-17 18:35:11.970481 neoclient-0.1.29/neoclient/composition.py
+-rw-r--r--   0        0        0      195 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/constants.py
+-rw-r--r--   0        0        0     7467 2023-03-21 22:00:03.330086 neoclient-0.1.29/neoclient/consumers.py
+-rw-r--r--   0        0        0     3249 2023-03-21 21:42:26.718782 neoclient-0.1.29/neoclient/converters.py
+-rw-r--r--   0        0        0      346 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/decorators/__init__.py
+-rw-r--r--   0        0        0     1651 2023-03-17 20:55:59.246251 neoclient-0.1.29/neoclient/decorators/api.py
+-rw-r--r--   0        0        0      430 2023-03-17 20:55:59.246251 neoclient-0.1.29/neoclient/decorators/client.py
+-rw-r--r--   0        0        0     4648 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/decorators/common.py
+-rw-r--r--   0        0        0     1390 2023-03-31 20:49:07.198408 neoclient-0.1.29/neoclient/decorators/operation.py
+-rw-r--r--   0        0        0     2203 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/decorators/service.py
+-rw-r--r--   0        0        0     1114 2023-03-17 18:35:11.970481 neoclient-0.1.29/neoclient/defaults.py
+-rw-r--r--   0        0        0     8711 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/dependence.py
+-rw-r--r--   0        0        0     3564 2023-03-31 20:30:07.773726 neoclient-0.1.29/neoclient/dependencies.py
+-rw-r--r--   0        0        0     1321 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/enums.py
+-rw-r--r--   0        0        0     1587 2023-03-18 12:43:34.234376 neoclient-0.1.29/neoclient/errors.py
+-rw-r--r--   0        0        0     1615 2023-03-17 20:55:59.246251 neoclient-0.1.29/neoclient/methods.py
+-rw-r--r--   0        0        0     2421 2023-03-31 20:30:07.773726 neoclient-0.1.29/neoclient/middleware.py
+-rw-r--r--   0        0        0    15060 2023-03-21 21:42:26.718782 neoclient-0.1.29/neoclient/models.py
+-rw-r--r--   0        0        0     4118 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/operation.py
+-rw-r--r--   0        0        0     7626 2023-03-31 20:30:07.773726 neoclient-0.1.29/neoclient/param_functions.py
+-rw-r--r--   0        0        0     9532 2023-02-26 21:29:40.180359 neoclient-0.1.29/neoclient/param_functions.pyi
+-rw-r--r--   0        0        0    13351 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/params.py
+-rw-r--r--   0        0        0        0 2023-02-10 21:07:01.448198 neoclient-0.1.29/neoclient/py.typed
+-rw-r--r--   0        0        0      501 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/resolution.py
+-rw-r--r--   0        0        0     3054 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/resolvers.py
+-rw-r--r--   0        0        0     3302 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/service.py
+-rw-r--r--   0        0        0      543 2023-08-02 22:05:55.193607 neoclient-0.1.29/neoclient/specification.py
+-rw-r--r--   0        0        0     2215 2023-03-21 21:42:26.718782 neoclient-0.1.29/neoclient/types.py
+-rw-r--r--   0        0        0     1646 2023-08-02 22:05:55.197607 neoclient-0.1.29/neoclient/typing.py
+-rw-r--r--   0        0        0     3492 2023-03-21 21:42:26.718782 neoclient-0.1.29/neoclient/utils.py
+-rw-r--r--   0        0        0     5747 2023-03-09 22:05:09.312835 neoclient-0.1.29/neoclient/validation.py
+-rw-r--r--   0        0        0     1600 2023-08-02 22:05:55.197607 neoclient-0.1.29/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 neoclient-0.1.29/PKG-INFO
```

### Comparing `neoclient-0.1.19/LICENSE` & `neoclient-0.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `neoclient-0.1.19/README.md` & `neoclient-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `neoclient-0.1.19/neoclient/__init__.py` & `neoclient-0.1.29/neoclient/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,37 +8,41 @@
 
        Fast API Clients for Python
        ~~~~~~~~~~~~~~~~~~~~~~~~~~~
                @tombulled
 ```
 """
 
-__version__: str = "0.1.19"
+__version__: str = "0.1.27"
 
 from .client import NeoClient
 from .decorators import (
     accept,
     base_url,
     content,
     cookie,
     cookies,
     data,
+    depends,
     files,
     header,
     headers,
     json,
     middleware,
     mount,
     path,
     path_params,
     query,
     query_params,
     referer,
+    response,
+    service,
     timeout,
     user_agent,
+    verify,
 )
 from .methods import delete, get, head, options, patch, post, put, request
 from .models import Request, Response
 from .param_functions import (
     URL,
     Body,
     Cookie,
```

### Comparing `neoclient-0.1.19/neoclient/api.py` & `neoclient-0.1.29/neoclient/api.py`

 * *Files identical despite different names*

### Comparing `neoclient-0.1.19/neoclient/composition.py` & `neoclient-0.1.29/neoclient/composition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import collections.abc
 import dataclasses
+import typing
 import urllib.parse
 from collections import Counter
 from typing import (
     Any,
     Callable,
     Mapping,
     MutableMapping,
@@ -49,17 +51,25 @@
         # Parameter Inference
         if not isinstance(field_info, Parameter):
             if field_name in path_params:
                 parameter = PathParameter(
                     alias=field_name,
                     default=utils.get_default(field_info),
                 )
-            elif isinstance(model_field.annotation, type) and (
-                issubclass(model_field.annotation, (BaseModel, dict))
+            elif (
+                (
+                    isinstance(model_field.annotation, type)
+                    and issubclass(model_field.annotation, (BaseModel, dict))
+                )
                 or dataclasses.is_dataclass(model_field.annotation)
+                or (
+                    utils.is_generic_alias(model_field.annotation)
+                    and typing.get_origin(model_field.annotation)
+                    in (collections.abc.Mapping,)
+                )
             ):
                 parameter = BodyParameter(
                     alias=field_name,
                     default=utils.get_default(field_info),
                 )
             else:
                 parameter = QueryParameter(
@@ -124,15 +134,15 @@
     fields: Mapping[str, Tuple[Any, Parameter]] = get_fields(request, func)
 
     # Validate that the fields are acceptable
     validate_fields(fields)
 
     model: BaseModel = api.create_model(func, fields, arguments)
 
-    # By this stage the arguments have been validated (coerced, defaults used, exception thrown if missing)
+    # By this stage the arguments have been validated
     validated_arguments: Mapping[str, Any] = model.dict()
 
     field_name: str
     parameter: Parameter
     for field_name, (_, parameter) in fields.items():
         argument: Any = validated_arguments[field_name]
```

### Comparing `neoclient-0.1.19/neoclient/consumers.py` & `neoclient-0.1.29/neoclient/consumers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from dataclasses import dataclass
-from typing import Any, Mapping, Sequence, Union
+from typing import Any, Mapping, Sequence, Tuple
 
 from httpx import URL, Cookies, Headers, QueryParams, Timeout
 
 from . import converters
-from .errors import CompositionError
 from .models import ClientOptions, PreRequest
 from .types import (
+    CookiesTypes,
     CookieTypes,
+    HeadersTypes,
     HeaderTypes,
     JsonTypes,
     PathsTypes,
     PathTypes,
     QueriesTypes,
     QueryTypes,
     RequestContent,
     RequestData,
     RequestFiles,
     TimeoutTypes,
+    VerifyTypes,
 )
+from .typing import SupportsClientConsumer, SupportsRequestConsumer
 
 __all__: Sequence[str] = (
     "QueryConsumer",
     "HeaderConsumer",
     "CookieConsumer",
     "PathConsumer",
     "QueriesConsumer",
@@ -32,73 +35,80 @@
     "ContentConsumer",
     "DataConsumer",
     "FilesConsumer",
     "JsonConsumer",
     "TimeoutConsumer",
     "MountConsumer",
     "BaseURLConsumer",
+    "VerifyConsumer",
 )
 
 
-class Consumer:
-    def consume(self, target: Union[PreRequest, ClientOptions], /) -> None:
-        if isinstance(target, PreRequest):
-            self.consume_request(target)
-        elif isinstance(target, ClientOptions):
-            self.consume_client(target)
-        else:
-            raise CompositionError(
-                f"Consumer {type(self).__name__!r} does not support consumption of type {type(target)}"
-            )
-
-    def consume_request(self, _: PreRequest, /) -> None:
-        raise CompositionError(
-            f"Consumer {type(self).__name__!r} does not support consumption of type {PreRequest}"
-        )
-
-    def consume_client(self, _: ClientOptions, /) -> None:
-        raise CompositionError(
-            f"Consumer {type(self).__name__!r} does not support consumption of type {ClientOptions}"
-        )
-
-
 @dataclass(init=False)
-class QueryConsumer(Consumer):
+class QueryConsumer(SupportsClientConsumer, SupportsRequestConsumer):
     key: str
-    value: str
+    values: Sequence[str]
 
     def __init__(self, key: str, value: QueryTypes) -> None:
         self.key = key
-        self.value = converters.convert_query_param(value)
+        self.values = converters.convert_query_param(value)
 
     def consume_request(self, request: PreRequest, /) -> None:
-        request.params = request.params.set(self.key, self.value)
+        request.params = self._apply(request.params)
 
     def consume_client(self, client: ClientOptions, /) -> None:
-        client.params = client.params.set(self.key, self.value)
+        client.params = self._apply(client.params)
+
+    def _apply(self, params: QueryParams, /) -> QueryParams:
+        # If there's only one value, set the query param and overwrite any
+        # existing entries for this key
+        if len(self.values) == 1:
+            return params.set(self.key, self.values[0])
+
+        # Otherwise, update the query params and maintain any existing entries for
+        # this key
+        value: str
+        for value in self.values:
+            params = params.add(self.key, value)
+
+        return params
 
 
 @dataclass(init=False)
-class HeaderConsumer(Consumer):
+class HeaderConsumer(SupportsRequestConsumer, SupportsClientConsumer):
     key: str
-    value: str
+    values: Sequence[str]
 
     def __init__(self, key: str, value: HeaderTypes) -> None:
         self.key = key
-        self.value = converters.convert_header(value)
+        self.values = converters.convert_header(value)
 
     def consume_request(self, request: PreRequest, /) -> None:
-        request.headers[self.key] = self.value
+        self._apply(request.headers)
 
     def consume_client(self, client: ClientOptions, /) -> None:
-        client.headers[self.key] = self.value
+        self._apply(client.headers)
+
+    def _apply(self, headers: Headers, /) -> None:
+        # If there's only one value, set the header and overwrite any existing
+        # entries for this key
+        if len(self.values) == 1:
+            headers[self.key] = self.values[0]
+        # Otherwise, update the headers and maintain any existing entries for this
+        # key
+        else:
+            values: Sequence[Tuple[str, str]] = [
+                (self.key, value) for value in self.values
+            ]
+
+            headers.update(values)
 
 
 @dataclass(init=False)
-class CookieConsumer(Consumer):
+class CookieConsumer(SupportsRequestConsumer, SupportsClientConsumer):
     key: str
     value: str
 
     def __init__(self, key: str, value: CookieTypes) -> None:
         self.key = key
         self.value = converters.convert_cookie(value)
 
@@ -106,141 +116,149 @@
         request.cookies[self.key] = self.value
 
     def consume_client(self, client: ClientOptions, /) -> None:
         client.cookies[self.key] = self.value
 
 
 @dataclass(init=False)
-class PathConsumer(Consumer):
+class PathConsumer(SupportsRequestConsumer):
     key: str
     value: str
 
     def __init__(self, key: str, value: PathTypes) -> None:
         self.key = key
         self.value = converters.convert_path_param(value)
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.path_params[self.key] = self.value
 
 
 @dataclass(init=False)
-class QueriesConsumer(Consumer):
+class QueriesConsumer(SupportsRequestConsumer, SupportsClientConsumer):
     params: QueryParams
 
     def __init__(self, params: QueriesTypes, /) -> None:
         self.params = converters.convert_query_params(params)
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.params = request.params.merge(self.params)
 
     def consume_client(self, client: ClientOptions, /) -> None:
         client.params = client.params.merge(self.params)
 
 
 @dataclass(init=False)
-class HeadersConsumer(Consumer):
+class HeadersConsumer(SupportsRequestConsumer, SupportsClientConsumer):
     headers: Headers
 
-    def __init__(self, headers: HeaderTypes, /) -> None:
+    def __init__(self, headers: HeadersTypes, /) -> None:
         self.headers = converters.convert_headers(headers)
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.headers.update(self.headers)
 
     def consume_client(self, client: ClientOptions, /) -> None:
         client.headers.update(self.headers)
 
 
 @dataclass(init=False)
-class CookiesConsumer(Consumer):
+class CookiesConsumer(SupportsRequestConsumer, SupportsClientConsumer):
     cookies: Cookies
 
-    def __init__(self, cookies: CookieTypes, /) -> None:
+    def __init__(self, cookies: CookiesTypes, /) -> None:
         self.cookies = converters.convert_cookies(cookies)
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.cookies.update(self.cookies)
 
     def consume_client(self, client: ClientOptions, /) -> None:
         client.cookies.update(self.cookies)
 
 
 @dataclass(init=False)
-class PathsConsumer(Consumer):
+class PathsConsumer(SupportsRequestConsumer):
     path_params: Mapping[str, str]
 
     def __init__(self, path_params: PathsTypes, /) -> None:
         self.path_params = converters.convert_path_params(path_params)
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.path_params.update(self.path_params)
 
 
 @dataclass
-class ContentConsumer(Consumer):
+class ContentConsumer(SupportsRequestConsumer):
     content: RequestContent
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.content = self.content
 
 
 @dataclass
-class DataConsumer(Consumer):
+class DataConsumer(SupportsRequestConsumer):
     data: RequestData
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.data = self.data
 
 
 @dataclass
-class FilesConsumer(Consumer):
+class FilesConsumer(SupportsRequestConsumer):
     files: RequestFiles
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.files = self.files
 
 
 @dataclass
-class JsonConsumer(Consumer):
+class JsonConsumer(SupportsRequestConsumer):
     json: JsonTypes
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.json = self.json
 
 
 @dataclass(init=False)
-class TimeoutConsumer(Consumer):
+class TimeoutConsumer(SupportsRequestConsumer, SupportsClientConsumer):
     timeout: Timeout
 
     def __init__(self, timeout: TimeoutTypes, /) -> None:
         self.timeout = converters.convert_timeout(timeout)
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.timeout = self.timeout
 
     def consume_client(self, client: ClientOptions, /) -> None:
         client.timeout = self.timeout
 
 
 @dataclass
-class StateConsumer(Consumer):
+class StateConsumer(SupportsRequestConsumer):
     key: str
     value: Any
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.state[self.key] = self.value
 
 
 @dataclass
-class MountConsumer(Consumer):
+class MountConsumer(SupportsRequestConsumer):
     path: str
 
     def consume_request(self, request: PreRequest, /) -> None:
         request.url = request.url.copy_with(path=self.path + request.url.path)
 
 
 @dataclass
-class BaseURLConsumer(Consumer):
+class BaseURLConsumer(SupportsClientConsumer):
     base_url: str
 
     def consume_client(self, client: ClientOptions, /) -> None:
         client.base_url = URL(self.base_url)
+
+
+@dataclass
+class VerifyConsumer(SupportsClientConsumer):
+    verify: VerifyTypes
+
+    def consume_client(self, client: ClientOptions, /) -> None:
+        client.verify = self.verify
```

### Comparing `neoclient-0.1.19/neoclient/converters.py` & `neoclient-0.1.29/neoclient/converters.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from http.cookiejar import CookieJar
-from typing import Any, List, Mapping, MutableMapping, MutableSequence, Sequence, Tuple
+from typing import Mapping, MutableMapping, MutableSequence, Sequence
 
 from httpx import Cookies, Headers, QueryParams, Timeout
 from httpx._utils import primitive_value_to_str
 
 from .errors import ConversionError
 from .types import (
     CookiesTypes,
@@ -28,84 +28,95 @@
     "convert_headers",
     "convert_cookies",
     "convert_path_params",
     "convert_timeout",
 )
 
 
-def convert_query_param(value: QueryTypes, /) -> str:
-    if is_primitive(value):
-        return primitive_value_to_str(value)
-    else:
-        return str(value)
+def convert_query_param(value: QueryTypes, /) -> Sequence[str]:
+    if isinstance(value, (str, int, float, bool)) or value is None:
+        return [primitive_value_to_str(value)]
 
+    if isinstance(value, Sequence):
+        return [primitive_value_to_str(item) for item in value]
 
-def convert_header(value: HeaderTypes, /) -> str:
-    if is_primitive(value):
-        return primitive_value_to_str(value)
-    else:
-        return str(value)
+    raise ConversionError("query param", value)
+
+
+def convert_header(value: HeaderTypes, /) -> Sequence[str]:
+    if isinstance(value, (str, int, float, bool)) or value is None:
+        return [primitive_value_to_str(value)]
+
+    if isinstance(value, Sequence):
+        return [primitive_value_to_str(item) for item in value]
+
+    raise ConversionError("header", value)
 
 
 def convert_cookie(value: CookieTypes, /) -> str:
     if is_primitive(value):
         return primitive_value_to_str(value)
-    else:
-        return str(value)
+
+    return str(value)
 
 
 def convert_path_param(value: PathTypes, /) -> str:
     if isinstance(value, (str, int, float, bool)) or value is None:
         return primitive_value_to_str(value)
-    elif isinstance(value, Sequence):
+
+    if isinstance(value, Sequence):
         segments: MutableSequence = []
 
         segment: Primitive
         for segment in value:
             converted_segment: str = primitive_value_to_str(segment)
 
             if converted_segment:
                 segments.append(converted_segment)
 
         return "/".join(segments)
-    else:
-        raise ConversionError("path param", value)
+
+    raise ConversionError("path param", value)
 
 
 def convert_query_params(value: QueriesTypes, /) -> QueryParams:
     if isinstance(value, QueryParams):
         return value
-    elif isinstance(value, (Mapping, list, tuple)):
+
+    if isinstance(value, (Mapping, list, tuple)):
         return QueryParams(value)
-    else:
-        raise ConversionError("query params", value)
+
+    raise ConversionError("query params", value)
 
 
 def convert_headers(value: HeadersTypes, /) -> Headers:
     if isinstance(value, Headers):
         return value
-    elif isinstance(value, (Mapping, Sequence)):
+
+    if isinstance(value, (Mapping, Sequence)):
         return Headers(dict(value))
-    else:
-        raise ConversionError("headers", value)
+
+    raise ConversionError("headers", value)
 
 
 def convert_cookies(value: CookiesTypes, /) -> Cookies:
     if isinstance(value, Cookies):
         return value
-    elif isinstance(value, CookieJar):
+
+    if isinstance(value, CookieJar):
         return Cookies(value)
-    elif isinstance(value, (Mapping, Sequence)):
+
+    if isinstance(value, (Mapping, Sequence)):
         return Cookies(dict(value))
-    else:
-        raise ConversionError("cookies", value)
+
+    raise ConversionError("cookies", value)
 
 
 def convert_path_params(path_params: PathsTypes, /) -> MutableMapping[str, str]:
     if isinstance(path_params, Mapping):
         return {key: convert_path_param(value) for key, value in path_params.items()}
-    else:
-        return {key: convert_path_param(value) for key, value in path_params}
+
+    return {key: convert_path_param(value) for key, value in path_params}
 
 
 def convert_timeout(value: TimeoutTypes, /) -> Timeout:
     return Timeout(value)
```

### Comparing `neoclient-0.1.19/neoclient/decorators.py` & `neoclient-0.1.29/neoclient/decorators/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,178 +1,172 @@
-from dataclasses import dataclass
-from typing import Callable, Protocol, Sequence, Type, TypeVar
+from typing import Any, Callable, Sequence, Type, Union
 
 from mediate.protocols import MiddlewareCallable
+from typing_extensions import TypeAlias
 
-from .consumers import (
-    BaseURLConsumer,
-    Consumer,
-    ContentConsumer,
+from ..consumers import (
     CookieConsumer,
     CookiesConsumer,
-    DataConsumer,
-    FilesConsumer,
     HeaderConsumer,
     HeadersConsumer,
-    JsonConsumer,
-    MountConsumer,
-    PathConsumer,
-    PathsConsumer,
     QueriesConsumer,
     QueryConsumer,
     TimeoutConsumer,
+    VerifyConsumer,
 )
-from .enums import HeaderName
-from .errors import CompositionError
-from .models import ClientOptions, PreRequest, Request, Response
-from .operation import OperationSpecification, get_operation
-from .service import Service
-from .types import (
+from ..enums import HTTPHeader
+from ..errors import CompositionError
+from ..models import Request, Response
+from ..operation import Operation, get_operation
+from ..service import ClientSpecification, Service
+from ..types import (
     CookiesTypes,
     CookieTypes,
     HeadersTypes,
     HeaderTypes,
-    JsonTypes,
-    PathsTypes,
-    PathTypes,
     QueriesTypes,
     QueryTypes,
-    RequestContent,
-    RequestData,
-    RequestFiles,
     TimeoutTypes,
+    VerifyTypes,
 )
+from .api import ConsumerDecorator, Decorator, T
 
 __all__: Sequence[str] = (
-    "query",
-    "header",
+    "accept",
     "cookie",
-    "path",
-    "query_params",
-    "headers",
     "cookies",
-    "path_params",
-    "content",
-    "data",
-    "files",
-    "json",
+    "depends",
+    "header",
+    "headers",
+    "middleware",
+    "query",
+    "query_params",
+    "referer",
+    "response",
     "timeout",
+    "user_agent",
+    "verify",
 )
 
-T = TypeVar("T", Callable, Type[Service])
-
+CommonDecorator: TypeAlias = Decorator[Union[Callable, Type[Service]]]
 
-class Decorator(Protocol):
-    def __call__(self, target: T, /) -> T:
-        ...
 
+def accept(*content_types: str) -> CommonDecorator:
+    return ConsumerDecorator(
+        HeaderConsumer(
+            HTTPHeader.ACCEPT,
+            ",".join(content_types),
+        )
+    )
 
-@dataclass
-class CompositionDecorator(Decorator):
-    consumer: Consumer
 
-    def __call__(self, target: T, /) -> T:
+def depends(*dependencies: Callable[..., Any]) -> CommonDecorator:
+    def decorate(target: T, /) -> T:
         if isinstance(target, type):
             if not issubclass(target, Service):
                 raise CompositionError(f"Target class is not a subclass of {Service}")
 
-            client: ClientOptions = target._opts
+            client_specification: ClientSpecification = target._spec
 
-            self.consumer.consume_client(client)
+            client_specification.dependencies.extend(dependencies)
         elif callable(target):
-            request: PreRequest = get_operation(target).specification.request
+            operation: Operation = get_operation(target)
 
-            self.consumer.consume_request(request)
+            operation.dependencies.extend(dependencies)
         else:
             raise CompositionError(f"Target of unsupported type {type(target)}")
 
         return target
 
-
-def query(key: str, value: QueryTypes) -> Decorator:
-    return CompositionDecorator(QueryConsumer(key, value))
-
-
-def header(key: str, value: HeaderTypes) -> Decorator:
-    return CompositionDecorator(HeaderConsumer(key, value))
-
-
-def cookie(key: str, value: CookieTypes) -> Decorator:
-    return CompositionDecorator(CookieConsumer(key, value))
+    return decorate
 
 
-def path(key: str, value: PathTypes) -> Decorator:
-    return CompositionDecorator(PathConsumer(key, value))
+def cookie(key: str, value: CookieTypes) -> CommonDecorator:
+    return ConsumerDecorator(CookieConsumer(key, value))
 
 
-def query_params(params: QueriesTypes, /) -> Decorator:
-    return CompositionDecorator(QueriesConsumer(params))
+def cookies(cookies: CookiesTypes, /) -> CommonDecorator:
+    return ConsumerDecorator(CookiesConsumer(cookies))
 
 
-def headers(headers: HeadersTypes, /) -> Decorator:
-    return CompositionDecorator(HeadersConsumer(headers))
+def header(key: str, value: HeaderTypes) -> CommonDecorator:
+    return ConsumerDecorator(HeaderConsumer(key, value))
 
 
-def cookies(cookies: CookiesTypes, /) -> Decorator:
-    return CompositionDecorator(CookiesConsumer(cookies))
+def headers(headers: HeadersTypes, /) -> CommonDecorator:
+    return ConsumerDecorator(HeadersConsumer(headers))
 
 
-def path_params(path_params: PathsTypes, /) -> Decorator:
-    return CompositionDecorator(PathsConsumer(path_params))
+def middleware(*middleware: MiddlewareCallable[Request, Response]) -> CommonDecorator:
+    def decorate(target: T, /) -> T:
+        if isinstance(target, type):
+            if not issubclass(target, Service):
+                raise CompositionError(f"Target class is not a subclass of {Service}")
 
+            client_specification: ClientSpecification = target._spec
 
-def content(content: RequestContent, /) -> Decorator:
-    return CompositionDecorator(ContentConsumer(content))
+            client_specification.middleware.add_all(middleware)
+        elif callable(target):
+            operation: Operation = get_operation(target)
 
+            operation.middleware.add_all(middleware)
+        else:
+            raise CompositionError(f"Target of unsupported type {type(target)}")
 
-def data(data: RequestData, /) -> Decorator:
-    return CompositionDecorator(DataConsumer(data))
+        return target
 
+    return decorate
 
-def files(files: RequestFiles, /) -> Decorator:
-    return CompositionDecorator(FilesConsumer(files))
 
+def query(key: str, value: QueryTypes) -> CommonDecorator:
+    return ConsumerDecorator(QueryConsumer(key, value))
 
-def json(json: JsonTypes, /) -> Decorator:
-    return CompositionDecorator(JsonConsumer(json))
 
+def query_params(params: QueriesTypes, /) -> CommonDecorator:
+    return ConsumerDecorator(QueriesConsumer(params))
 
-def timeout(timeout: TimeoutTypes, /) -> Decorator:
-    return CompositionDecorator(TimeoutConsumer(timeout))
 
+def referer(referer: str, /) -> CommonDecorator:
+    return ConsumerDecorator(
+        HeaderConsumer(
+            HTTPHeader.REFERER,
+            referer,
+        )
+    )
 
-def mount(path: str, /) -> Decorator:
-    return CompositionDecorator(MountConsumer(path))
 
+def response(response: Callable[..., Any]) -> CommonDecorator:
+    def decorate(target: T, /) -> T:
+        if isinstance(target, type):
+            if not issubclass(target, Service):
+                raise CompositionError(f"Target class is not a subclass of {Service}")
 
-def base_url(base_url: str, /) -> Decorator:
-    return CompositionDecorator(BaseURLConsumer(base_url))
+            client_specification: ClientSpecification = target._spec
 
+            client_specification.default_response = response
+        elif callable(target):
+            operation: Operation = get_operation(target)
 
-def middleware(*middleware: MiddlewareCallable[Request, Response]) -> Decorator:
-    def decorate(target: T, /) -> T:
-        if isinstance(target, type) and issubclass(target, Service):
-            raise CompositionError(
-                "Middleware decorator currently unsupported for service classes"
-            )
-
-        specification: OperationSpecification = get_operation(target).specification
-
-        middleware_callable: MiddlewareCallable[Request, Response]
-        for middleware_callable in middleware:
-            specification.middleware.add(middleware_callable)
+            operation.response = response
+        else:
+            raise CompositionError(f"Target of unsupported type {type(target)}")
 
         return target
 
     return decorate
 
 
-def user_agent(user_agent: str, /) -> Decorator:
-    return header(HeaderName.USER_AGENT, user_agent)
+def timeout(timeout: TimeoutTypes, /) -> CommonDecorator:
+    return ConsumerDecorator(TimeoutConsumer(timeout))
 
 
-def accept(*content_types: str) -> Decorator:
-    return header(HeaderName.ACCEPT, ",".join(content_types))
+def user_agent(user_agent: str, /) -> CommonDecorator:
+    return ConsumerDecorator(
+        HeaderConsumer(
+            HTTPHeader.USER_AGENT,
+            user_agent,
+        )
+    )
 
 
-def referer(referer: str, /) -> Decorator:
-    return header(HeaderName.REFERER, referer)
+def verify(verify: VerifyTypes, /) -> CommonDecorator:
+    return ConsumerDecorator(VerifyConsumer(verify))
```

### Comparing `neoclient-0.1.19/neoclient/defaults.py` & `neoclient-0.1.29/neoclient/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Sequence
 
-from httpx import URL, Timeout
+from httpx import URL, Limits, Timeout
 
 from .types import (
     AuthTypes,
     CookiesTypes,
     DefaultEncodingTypes,
     EventHooks,
     HeadersTypes,
@@ -21,20 +21,22 @@
     "DEFAULT_COOKIES",
     "DEFAULT_TIMEOUT",
     "DEFAULT_FOLLOW_REDIRECTS",
     "DEFAULT_MAX_REDIRECTS",
     "DEFAULT_EVENT_HOOKS",
     "DEFAULT_TRUST_ENV",
     "DEFAULT_ENCODING",
+    "DEFAULT_LIMITS",
 )
 
 DEFAULT_BASE_URL: URLTypes = URL()
 DEFAULT_AUTH: Optional[AuthTypes] = None
 DEFAULT_PARAMS: Optional[QueriesTypes] = None
 DEFAULT_HEADERS: Optional[HeadersTypes] = None
 DEFAULT_COOKIES: Optional[CookiesTypes] = None
-DEFAULT_TIMEOUT: TimeoutTypes = Timeout(5.0)
+DEFAULT_TIMEOUT: TimeoutTypes = Timeout(timeout=5.0)
 DEFAULT_FOLLOW_REDIRECTS: bool = False
 DEFAULT_MAX_REDIRECTS: int = 20
-DEFAULT_EVENT_HOOKS: Optional[EventHooks] = None
 DEFAULT_TRUST_ENV: bool = True
 DEFAULT_ENCODING: DefaultEncodingTypes = "utf-8"
+DEFAULT_LIMITS = Limits(max_connections=100, max_keepalive_connections=20)
+DEFAULT_EVENT_HOOKS: Optional[EventHooks] = None
```

### Comparing `neoclient-0.1.19/neoclient/dependencies.py` & `neoclient-0.1.29/neoclient/dependence.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,58 @@
+import collections.abc
 import dataclasses
+import typing
 from dataclasses import dataclass
 from typing import (
     Any,
     Callable,
+    Generic,
     Mapping,
     MutableMapping,
     Optional,
+    Sequence,
     Tuple,
     Type,
     TypeVar,
+    Union,
 )
 
 import httpx
 from httpx import URL, Cookies, Headers, QueryParams
 from pydantic import BaseModel
 from pydantic.fields import FieldInfo, ModelField
 
 from . import api, utils
 from .errors import PreparationError, ResolutionError
-from .models import Request, Response
+from .models import PreRequest, Request, Response
 from .params import (
     BodyParameter,
     CookiesParameter,
+    HeaderParameter,
     HeadersParameter,
     Parameter,
     QueriesParameter,
     QueryParameter,
     RequestParameter,
     ResponseParameter,
     URLParameter,
 )
-from .typing import Resolver
+from .typing import ResponseResolver
 from .validation import ValidatedFunction
 
 T = TypeVar("T")
 
 
 def get_fields(func: Callable, /) -> Mapping[str, Tuple[Any, Parameter]]:
     class Config:
         allow_population_by_field_name: bool = True
         arbitrary_types_allowed: bool = True
 
     httpx_lookup: Mapping[Type[Any], Type[Parameter]] = {
+        PreRequest: RequestParameter,
         Request: RequestParameter,
         Response: ResponseParameter,
         httpx.Request: RequestParameter,
         httpx.Response: ResponseParameter,
         URL: URLParameter,
         QueryParams: QueriesParameter,
         Headers: HeadersParameter,
@@ -62,17 +69,24 @@
         field_info: FieldInfo = model_field.field_info
         parameter: Parameter
 
         if not isinstance(field_info, Parameter):
             if model_field.annotation in httpx_lookup:
                 parameter = httpx_lookup[model_field.annotation]()
             elif (
-                isinstance(model_field.annotation, type)
-                and issubclass(model_field.annotation, (BaseModel, dict))
+                (
+                    isinstance(model_field.annotation, type)
+                    and issubclass(model_field.annotation, (BaseModel, dict))
+                )
                 or dataclasses.is_dataclass(model_field.annotation)
+                or (
+                    utils.is_generic_alias(model_field.annotation)
+                    and typing.get_origin(model_field.annotation)
+                    in (collections.abc.Mapping,)
+                )
             ):
                 parameter = BodyParameter(
                     default=utils.get_default(field_info),
                 )
             else:
                 parameter = QueryParameter(
                     default=utils.get_default(field_info),
@@ -87,52 +101,101 @@
 
         fields[field_name] = (model_field.annotation, parameter_clone)
 
     return fields
 
 
 @dataclass
-class DependencyResolver(Resolver[T]):
+class DependencyResolver(Generic[T]):
     dependency: Callable[..., T]
 
-    def __call__(
+    def resolve_request(
+        self,
+        request: PreRequest,
+        /,
+        *,
+        cache: Optional[MutableMapping[Parameter, Any]] = None,
+    ) -> T:
+        return self.resolve(request, cache=cache)
+
+    def resolve_response(
         self,
         response: Response,
         /,
         *,
         cache: Optional[MutableMapping[Parameter, Any]] = None,
     ) -> T:
+        return self.resolve(response, cache=cache)
+
+    def resolve(
+        self,
+        request_or_response: Union[PreRequest, Response],
+        /,
+        *,
+        cache: Optional[MutableMapping[Parameter, Any]] = None,
+    ) -> T:
         if cache is None:
             cache = {}
 
         fields: Mapping[str, Tuple[Any, Parameter]] = get_fields(self.dependency)
 
         model_cls: Type[BaseModel] = api.create_model_cls(self.dependency, fields)
 
         arguments: MutableMapping[str, Any] = {}
 
         field_name: str
+        field_annotation: Any
         parameter: Parameter
-        for field_name, (_, parameter) in fields.items():
+        for field_name, (field_annotation, parameter) in fields.items():
             resolution: Any
 
             if parameter in cache:
                 resolution = cache[parameter]
             else:
                 cache_parameter: bool = True
 
                 if isinstance(parameter, DependencyParameter):
-                    resolution = parameter.resolve(
-                        response,
-                        cache=cache,
-                    )
+                    if isinstance(request_or_response, PreRequest):
+                        resolution = parameter.resolve_request(
+                            request_or_response,
+                            cache=cache,
+                        )
+                    else:
+                        resolution = parameter.resolve_response(
+                            request_or_response,
+                            cache=cache,
+                        )
 
                     cache_parameter = parameter.use_cache
                 else:
-                    resolution = parameter.resolve(response)
+                    if isinstance(request_or_response, PreRequest):
+                        resolution = parameter.resolve_request(request_or_response)
+                    else:
+                        resolution = parameter.resolve_response(request_or_response)
+
+                # If the parameter has a resolution function that is backed to
+                # a multi-value mapping (and will yield a sequence of values),
+                # inspect the field's annotation to decide whether to use the
+                # entire sequence, or only the first value within in.
+                if isinstance(parameter, (QueryParameter, HeaderParameter)):
+                    field_annotation_origin: Optional[Any] = typing.get_origin(
+                        field_annotation
+                    )
+
+                    if (
+                        field_annotation is Any
+                        or field_annotation not in (list, tuple)
+                        and (
+                            not utils.is_generic_alias(field_annotation)
+                            or field_annotation_origin
+                            not in (list, tuple, collections.abc.Sequence)
+                        )
+                    ):
+                        if isinstance(resolution, Sequence) and resolution:
+                            resolution = resolution[0]
 
                 if cache_parameter:
                     cache[parameter] = resolution
 
             # If there is no resolution (e.g. missing header/query param etc.)
             # and the parameter has a default, then we can omit the value from
             # the arguments.
@@ -155,27 +218,43 @@
 
 
 @dataclass(unsafe_hash=True)
 class DependencyParameter(Parameter):
     dependency: Optional[Callable] = None
     use_cache: bool = True
 
-    def resolve(
+    def resolve_request(
+        self,
+        request: PreRequest,
+        /,
+        *,
+        cache: Optional[MutableMapping[Parameter, Any]] = None,
+    ) -> Any:
+        if self.dependency is None:
+            raise ResolutionError(
+                f"Cannot resolve parameter {type(self)!r} without a dependency"
+            )
+
+        return DependencyResolver(self.dependency).resolve_request(request, cache=cache)
+
+    def resolve_response(
         self,
         response: Response,
         /,
         *,
         cache: Optional[MutableMapping[Parameter, Any]] = None,
     ) -> Any:
         if self.dependency is None:
             raise ResolutionError(
                 f"Cannot resolve parameter {type(self)!r} without a dependency"
             )
 
-        return DependencyResolver(self.dependency)(response, cache=cache)
+        return DependencyResolver(self.dependency).resolve_response(
+            response, cache=cache
+        )
 
     def prepare(self, field: ModelField, /) -> None:
         if self.dependency is not None:
             return
 
         # NOTE: The annotation will nearly always be callable (e.g. `int`)
         # This check needs to be changed to check for non primitive callables,
```

### Comparing `neoclient-0.1.19/neoclient/enums.py` & `neoclient-0.1.29/neoclient/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-from enum import Enum
+from enum import Enum, auto
 from typing import Sequence
 
 __all__: Sequence[str] = (
-    "HttpMethod",
-    "HeaderName",
+    "Entity",
+    "HTTPMethod",
+    "HTTPHeader",
 )
 
 
 class HiddenValueEnum(Enum):
     def __repr__(self) -> str:
         return f"<{type(self).__name__}.{self.name}>"
 
 
 class StrEnum(str, Enum):
     def __str__(self) -> str:
         return self.value
 
 
-class HttpMethod(HiddenValueEnum, StrEnum):
-    PUT = "PUT"
+class Entity(HiddenValueEnum):
+    MIDDLEWARE = auto()
+    RESPONSE = auto()
+    DEPENDENCY = auto()
+
+
+class HTTPMethod(HiddenValueEnum, StrEnum):
+    CONNECT = "CONNECT"
+    DELETE = "DELETE"
     GET = "GET"
-    POST = "POST"
     HEAD = "HEAD"
-    PATCH = "PATCH"
-    DELETE = "DELETE"
     OPTIONS = "OPTIONS"
+    PATCH = "PATCH"
+    POST = "POST"
+    PUT = "PUT"
+    TRACE = "TRACE"
 
 
-class HeaderName(HiddenValueEnum, StrEnum):
+class HTTPHeader(HiddenValueEnum, StrEnum):
     ACCEPT = "Accept"
     ACCEPT_ENCODING = "Accept-Encoding"
     ACCEPT_LANGUAGE = "Accept-Language"
     CACHE_CONTROL = "Cache-Control"
     CONNECTION = "Connection"
     CONTENT_TYPE = "Content-Type"
     COOKIE = "Cookie"
```

### Comparing `neoclient-0.1.19/neoclient/errors.py` & `neoclient-0.1.29/neoclient/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "CompositionError",
     "ResolutionError",
     "ConversionError",
     "NotAnOperationError",
     "ExpectedStatusCodeError",
     "ExpectedHeaderError",
     "MissingStateError",
+    "ServiceInitialisationError",
 )
 
 
 class DuplicateParameters(Exception):
     pass
 
 
@@ -57,17 +58,24 @@
     name: str
     value: Optional[str] = None
     expected_value: Optional[str] = None
 
     def __str__(self) -> str:
         if self.value is None:
             return f"Response missing expected header {str(self.name)!r}"
-        else:
-            return f"Response header {str(self.name)!r} has incorrect value. Expected {self.expected_value!r}, got {self.value!r}"
+
+        return (
+            f"Response header {str(self.name)!r} has incorrect value."
+            f" Expected {self.expected_value!r}, got {self.value!r}"
+        )
 
 
 @dataclass
 class MissingStateError(Exception):
     key: str
 
     def __str__(self) -> str:
         return f"State entry missing for key {self.key!r}"
+
+
+class ServiceInitialisationError(Exception):
+    pass
```

### Comparing `neoclient-0.1.19/neoclient/methods.py` & `neoclient-0.1.29/neoclient/methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Any, Callable, Optional, Protocol, Sequence, TypeVar
 
 from typing_extensions import ParamSpec
 
-from .client import NeoClient
-from .enums import HttpMethod
+from .client import Client
+from .enums import HTTPMethod
 
 __all__: Sequence[str] = (
     "request",
     "put",
     "get",
     "post",
     "head",
@@ -31,23 +31,23 @@
 @dataclass
 class MethodOperationDecorator(OperationDecorator):
     method: str
 
     def __call__(
         self, endpoint: str, /, *, response: Optional[Callable[..., Any]] = None
     ) -> Callable[[Callable[PS, RT]], Callable[PS, RT]]:
-        return NeoClient().request(self.method, endpoint, response=response)
+        return Client().request(self.method, endpoint, response=response)
 
 
 def request(
     method: str, endpoint: str, /, *, response: Optional[Callable[..., Any]] = None
 ) -> Callable[[Callable[PS, RT]], Callable[PS, RT]]:
     return MethodOperationDecorator(method)(endpoint, response=response)
 
 
-put: OperationDecorator = MethodOperationDecorator(HttpMethod.PUT)
-get: OperationDecorator = MethodOperationDecorator(HttpMethod.GET)
-post: OperationDecorator = MethodOperationDecorator(HttpMethod.POST)
-head: OperationDecorator = MethodOperationDecorator(HttpMethod.HEAD)
-patch: OperationDecorator = MethodOperationDecorator(HttpMethod.PATCH)
-delete: OperationDecorator = MethodOperationDecorator(HttpMethod.DELETE)
-options: OperationDecorator = MethodOperationDecorator(HttpMethod.OPTIONS)
+put: OperationDecorator = MethodOperationDecorator(HTTPMethod.PUT)
+get: OperationDecorator = MethodOperationDecorator(HTTPMethod.GET)
+post: OperationDecorator = MethodOperationDecorator(HTTPMethod.POST)
+head: OperationDecorator = MethodOperationDecorator(HTTPMethod.HEAD)
+patch: OperationDecorator = MethodOperationDecorator(HTTPMethod.PATCH)
+delete: OperationDecorator = MethodOperationDecorator(HTTPMethod.DELETE)
+options: OperationDecorator = MethodOperationDecorator(HTTPMethod.OPTIONS)
```

### Comparing `neoclient-0.1.19/neoclient/middleware.py` & `neoclient-0.1.29/neoclient/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass, field
 from typing import Optional, Protocol, Sequence
 
 import mediate
 
-from .enums import HeaderName
+from .enums import HTTPHeader
 from .errors import ExpectedHeaderError, ExpectedStatusCodeError
 from .models import Request, Response
 
 __all__: Sequence[str] = (
     "Middleware",
     "RequestMiddleware",
     "ExpectedStatusCodeMiddleware",
@@ -50,15 +50,16 @@
     def __call__(self, call_next: RequestMiddleware, request: Request, /) -> Response:
         response: Response = call_next(request)
 
         header_value: str = response.headers[self.name]
 
         if self.name not in response.headers:
             raise ExpectedHeaderError(name=self.name)
-        elif self.value is not None and header_value != self.value:
+
+        if self.value is not None and header_value != self.value:
             raise ExpectedHeaderError(
                 name=self.name, value=header_value, expected_value=self.value
             )
 
         return response
 
 
@@ -67,15 +68,15 @@
     content_type: str
 
     def __call__(self, call_next: RequestMiddleware, request: Request, /) -> Response:
         # NOTE: In the future this should parse the content type to support
         # lenient checking.
         # For example, 'application/json+foo' should likely be an acceptable
         # value when expecting a lenient form of 'application/json'
-        return ExpectedHeaderMiddleware(HeaderName.CONTENT_TYPE, self.content_type)(
+        return ExpectedHeaderMiddleware(HTTPHeader.CONTENT_TYPE, self.content_type)(
             call_next, request
         )
 
 
 def raise_for_status(call_next: RequestMiddleware, request: Request, /) -> Response:
     response: Response = call_next(request)
```

### Comparing `neoclient-0.1.19/neoclient/models.py` & `neoclient-0.1.29/neoclient/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,66 @@
 import urllib.parse
 from dataclasses import dataclass
 from typing import (
     Any,
     Callable,
     Dict,
     List,
+    Mapping,
     MutableMapping,
     Optional,
     Sequence,
     Set,
     Union,
 )
 
 import httpx
-from httpx import URL, Cookies, Headers, QueryParams, Timeout
-from httpx._auth import Auth
+from httpx import URL, BaseTransport, Cookies, Headers, Limits, QueryParams, Timeout
 from httpx._config import DEFAULT_MAX_REDIRECTS, DEFAULT_TIMEOUT_CONFIG
 
 from . import converters, utils
+from .defaults import (
+    DEFAULT_BASE_URL,
+    DEFAULT_ENCODING,
+    DEFAULT_FOLLOW_REDIRECTS,
+    DEFAULT_LIMITS,
+    DEFAULT_TRUST_ENV,
+)
 from .errors import IncompatiblePathParameters, MissingStateError
 from .types import (
     AsyncByteStream,
     AuthTypes,
+    CertTypes,
     CookiesTypes,
-    CookieTypes,
     DefaultEncodingTypes,
     EventHooks,
     HeadersTypes,
-    HeaderTypes,
     JsonTypes,
     MethodTypes,
     PathsTypes,
+    ProxiesTypes,
     QueriesTypes,
     RequestContent,
     RequestData,
     RequestExtensions,
     RequestFiles,
     ResponseContent,
     ResponseExtensions,
     SyncByteStream,
     TimeoutTypes,
     URLTypes,
+    VerifyTypes,
 )
 
 __all__: Sequence[str] = (
-    "Client",
+    "State",
+    "ClientOptions",
     "Request",
     "Response",
     "PreRequest",
-    "OperationSpecification",
 )
 
 
 class State:
     _state: MutableMapping[str, Any]
 
     def __init__(self, state: Optional[MutableMapping[str, Any]] = None):
@@ -66,25 +74,25 @@
             f"{key}={value!r}" for key, value in self._state.items()
         )
         return f"{type(self).__name__}({context})"
 
     def __eq__(self, value: object) -> bool:
         if isinstance(value, type(self)):
             return self._state == value._state
-        else:
-            return False
+
+        return False
 
     def _set(self, key: str, value: Any) -> None:
         self._state[key] = value
 
     def _get(self, key: str) -> Any:
         if key in self._state:
             return self._state[key]
-        else:
-            raise MissingStateError(key=key)
+
+        raise MissingStateError(key=key)
 
     def _del(self, key: str) -> None:
         del self._state[key]
 
     def __setitem__(self, key: str, value: Any) -> None:
         self._set(key, value)
 
@@ -120,71 +128,77 @@
 
     def __init__(
         self,
         method: MethodTypes,
         url: URLTypes,
         *,
         params: Optional[QueriesTypes] = None,
-        headers: Optional[HeaderTypes] = None,
-        cookies: Optional[CookieTypes] = None,
+        headers: Optional[HeadersTypes] = None,
+        cookies: Optional[CookiesTypes] = None,
         content: Optional[RequestContent] = None,
         data: Optional[RequestData] = None,
         files: Optional[RequestFiles] = None,
         json: Optional[Any] = None,
         stream: Union[SyncByteStream, AsyncByteStream, None] = None,
         extensions: Optional[RequestExtensions] = None,
         state: Optional[State] = None,
     ):
         super().__init__(
             method=method,
             url=url,
             params=params,
             headers=headers,
-            cookies=cookies,
+            cookies=(
+                converters.convert_cookies(cookies) if cookies is not None else None
+            ),
             content=content,
             data=data,
             files=files,
             json=json,
             stream=stream,
             extensions=extensions,
         )
 
         if state is not None:
             self.state = state
         else:
             self.state = State()
 
     @classmethod
-    def from_httpx_request(cls, request: httpx.Request, /) -> "Request":
-        if hasattr(request, "_content"):
-            return cls(
-                method=request.method,
-                url=request.url,
-                headers=request.headers,
-                extensions=request.extensions,
-                content=request.content,
-            )
-        else:
-            return cls(
-                method=request.method,
-                url=request.url,
-                headers=request.headers,
-                extensions=request.extensions,
-                stream=request.stream,
+    def from_httpx_request(cls, httpx_request: httpx.Request, /) -> "Request":
+        if hasattr(httpx_request, "_content"):
+            request: Request = cls(
+                method=httpx_request.method,
+                url=httpx_request.url,
+                headers=httpx_request.headers,
+                extensions=httpx_request.extensions,
+                stream=httpx_request.stream,
             )
 
+            request._content = httpx_request.content
+
+            return request
+
+        return cls(
+            method=httpx_request.method,
+            url=httpx_request.url,
+            headers=httpx_request.headers,
+            extensions=httpx_request.extensions,
+            stream=httpx_request.stream,
+        )
+
 
 class Response(httpx.Response):
     state: State
 
     def __init__(
         self,
         status_code: int,
         *,
-        headers: Optional[HeaderTypes] = None,
+        headers: Optional[HeadersTypes] = None,
         content: Optional[ResponseContent] = None,
         text: Optional[str] = None,
         html: Optional[str] = None,
         json: Any = None,
         stream: Union[SyncByteStream, AsyncByteStream, None] = None,
         request: Optional[httpx.Request] = None,
         extensions: Optional[ResponseExtensions] = None,
@@ -208,63 +222,78 @@
 
         if state is not None:
             self.state = state
         else:
             self.state = State()
 
     @classmethod
-    def from_httpx_response(cls, response: httpx.Response, /) -> "Response":
-        if hasattr(response, "_content"):
-            return cls(
-                status_code=response.status_code,
-                headers=response.headers,
-                request=response.request,
-                content=response.content,
-            )
-        else:
-            return cls(
-                status_code=response.status_code,
-                headers=response.headers,
-                request=response.request,
-                stream=response.stream,
+    def from_httpx_response(cls, httpx_response: httpx.Response, /) -> "Response":
+        if hasattr(httpx_response, "_content"):
+            response: Response = cls(
+                status_code=httpx_response.status_code,
+                headers=httpx_response.headers,
+                request=httpx_response.request,
+                stream=httpx_response.stream,
             )
 
+            response._content = httpx_response.content
 
-DEFAULT_TRUST_ENV: bool = True
-DEFAULT_ENCODING: str = "utf-8"
-DEFAULT_FOLLOW_REDIRECTS: bool = False
-DEFAULT_BASE_URL: URLTypes = ""
-DEFAULT_EVENT_HOOKS: EventHooks = {"request": [], "response": []}
+            return response
+
+        return cls(
+            status_code=httpx_response.status_code,
+            headers=httpx_response.headers,
+            request=httpx_response.request,
+            stream=httpx_response.stream,
+        )
 
 
 @dataclass(init=False)
 class ClientOptions:
     auth: Optional[AuthTypes]
     params: QueryParams
     headers: Headers
     cookies: Cookies
+    verify: VerifyTypes
+    cert: Optional[CertTypes]
+    http1: bool
+    http2: bool
+    proxies: Optional[ProxiesTypes]
+    mounts: Mapping[str, BaseTransport]
     timeout: Timeout
     follow_redirects: bool
+    limits: Limits
     max_redirects: int
     event_hooks: EventHooks
     base_url: URL
+    transport: Optional[BaseTransport]
+    app: Optional[Callable[..., Any]]
     trust_env: bool
     default_encoding: DefaultEncodingTypes
 
     def __init__(
         self,
         auth: Optional[AuthTypes] = None,
         params: Optional[QueriesTypes] = None,
         headers: Optional[HeadersTypes] = None,
         cookies: Optional[CookiesTypes] = None,
+        verify: VerifyTypes = True,
+        cert: Optional[CertTypes] = None,
+        http1: bool = True,
+        http2: bool = False,
+        proxies: Optional[ProxiesTypes] = None,
+        mounts: Optional[Mapping[str, BaseTransport]] = None,
         timeout: TimeoutTypes = DEFAULT_TIMEOUT_CONFIG,
         follow_redirects: bool = DEFAULT_FOLLOW_REDIRECTS,
+        limits: Limits = DEFAULT_LIMITS,
         max_redirects: int = DEFAULT_MAX_REDIRECTS,
         event_hooks: Optional[EventHooks] = None,
         base_url: URLTypes = DEFAULT_BASE_URL,
+        transport: Optional[BaseTransport] = None,
+        app: Optional[Callable[..., Any]] = None,
         trust_env: bool = DEFAULT_TRUST_ENV,
         default_encoding: DefaultEncodingTypes = DEFAULT_ENCODING,
     ) -> None:
         self.auth = auth
         self.params = (
             converters.convert_query_params(params)
             if params is not None
@@ -272,74 +301,59 @@
         )
         self.headers = (
             converters.convert_headers(headers) if headers is not None else Headers()
         )
         self.cookies = (
             converters.convert_cookies(cookies) if cookies is not None else Cookies()
         )
+        self.verify = verify
+        self.cert = cert
+        self.http1 = http1
+        self.http2 = http2
+        self.proxies = proxies
+        self.mounts = mounts if mounts is not None else {}
         self.timeout = (
             converters.convert_timeout(timeout) if timeout is not None else Timeout()
         )
         self.follow_redirects = follow_redirects
+        self.limits = limits
         self.max_redirects = max_redirects
         self.event_hooks = (
-            event_hooks if event_hooks is not None else DEFAULT_EVENT_HOOKS
+            event_hooks if event_hooks is not None else {"request": [], "response": []}
         )
         self.base_url = URL(base_url)
+        self.transport = transport
+        self.app = app
         self.trust_env = trust_env
         self.default_encoding = default_encoding
 
     def build(self) -> httpx.Client:
         return httpx.Client(
             auth=self.auth,
             params=self.params,
             headers=self.headers,
             cookies=self.cookies,
+            verify=self.verify,
+            cert=self.cert,
+            http1=self.http1,
+            http2=self.http2,
+            proxies=self.proxies,
+            mounts=self.mounts,
             timeout=self.timeout,
             follow_redirects=self.follow_redirects,
+            limits=self.limits,
             max_redirects=self.max_redirects,
             event_hooks=self.event_hooks,
             base_url=self.base_url,
+            transport=self.transport,
+            app=self.app,
             trust_env=self.trust_env,
             default_encoding=self.default_encoding,
         )
 
-    def is_default(self) -> bool:
-        return all(
-            (
-                self.auth == None,
-                self.params == QueryParams(),
-                self.headers == Headers(),
-                self.cookies == Cookies(),
-                self.timeout == DEFAULT_TIMEOUT_CONFIG,
-                self.follow_redirects == DEFAULT_FOLLOW_REDIRECTS,
-                self.max_redirects == DEFAULT_MAX_REDIRECTS,
-                self.event_hooks == DEFAULT_EVENT_HOOKS,
-                self.base_url == DEFAULT_BASE_URL,
-                self.trust_env == DEFAULT_TRUST_ENV,
-                self.default_encoding == DEFAULT_ENCODING,
-            )
-        )
-
-    @classmethod
-    def from_client(cls, client: httpx.Client, /) -> "ClientOptions":
-        return cls(
-            auth=client.auth,
-            params=client.params,
-            headers=client.headers,
-            cookies=client.cookies,
-            timeout=client.timeout,
-            follow_redirects=client.follow_redirects,
-            max_redirects=client.max_redirects,
-            event_hooks=client.event_hooks,
-            base_url=client.base_url,
-            trust_env=client.trust_env,
-            default_encoding=client._default_encoding,
-        )
-
 
 @dataclass(init=False)
 class PreRequest:
     method: str
     url: URL
     params: QueryParams
     headers: Headers
@@ -364,15 +378,14 @@
         data: Optional[RequestData] = None,
         files: Optional[RequestFiles] = None,
         json: Optional[JsonTypes] = None,
         timeout: Optional[TimeoutTypes] = None,
         path_params: Optional[PathsTypes] = None,
         state: Optional[State] = None,
     ) -> None:
-        ...
         self.method = method if isinstance(method, str) else method.decode()
         self.url = URL(url)
         self.params = (
             converters.convert_query_params(params)
             if params is not None
             else QueryParams()
         )
@@ -414,34 +427,34 @@
                 content=self.content,
                 data=self.data,
                 files=self.files,
                 json=self.json,
                 extensions=extensions,
                 state=self.state,
             )
-        else:
-            httpx_request: httpx.Request = client.build_request(
-                self.method,
-                url,
-                params=self.params,
-                headers=self.headers,
-                cookies=self.cookies,
-                content=self.content,
-                data=self.data,
-                files=self.files,
-                json=self.json,
-                timeout=self.timeout,
-                extensions=extensions,
-            )
 
-            request: Request = Request.from_httpx_request(httpx_request)
+        httpx_request: httpx.Request = client.build_request(
+            self.method,
+            url,
+            params=self.params,
+            headers=self.headers,
+            cookies=self.cookies,
+            content=self.content,
+            data=self.data,
+            files=self.files,
+            json=self.json,
+            timeout=self.timeout,
+            extensions=extensions,
+        )
+
+        request: Request = Request.from_httpx_request(httpx_request)
 
-            request.state = self.state
+        request.state = self.state
 
-            return request
+        return request
 
     def merge(self, pre_request: "PreRequest", /) -> "PreRequest":
         return self.__class__(
             method=pre_request.method,
             url=pre_request.url,
             params=self.params.merge(pre_request.params),
             headers=httpx.Headers({**self.headers, **pre_request.headers}),
@@ -457,14 +470,17 @@
             ),
             path_params={
                 **self.path_params,
                 **pre_request.path_params,
             },
         )
 
+    def clone(self) -> "PreRequest":
+        return self.merge(PreRequest(method=self.method, url=self.url))
+
     def _get_formatted_url(self) -> str:
         return urllib.parse.unquote(str(self.url)).format(**self.path_params)
 
     def validate(self):
         url: str = urllib.parse.unquote(str(self.url))
 
         expected_path_params: Set[str] = utils.parse_format_string(url)
```

### Comparing `neoclient-0.1.19/neoclient/operation.py` & `neoclient-0.1.29/neoclient/operation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import functools
 import inspect
 from dataclasses import dataclass, field
 from json import JSONDecodeError
-from typing import Any, Callable, Generic, Optional, Sequence, TypeVar
+from typing import Any, Callable, Generic, MutableSequence, Optional, Sequence, TypeVar
 
 import httpx
 import pydantic
 from httpx import Client
 from pydantic import BaseModel
 from typing_extensions import ParamSpec
 
 from .composition import compose
 from .errors import NotAnOperationError
 from .middleware import Middleware
-from .models import PreRequest, Request, Response
-from .resolution import resolve
+from .models import ClientOptions, PreRequest, Request, Response
+from .resolution import resolve_request, resolve_response
 
 __all__: Sequence[str] = (
     "set_operation",
     "has_operation",
     "get_operation",
     "Operation",
 )
 
 PS = ParamSpec("PS")
-RT = TypeVar("RT", covariant=True)
+RT_co = TypeVar("RT_co", covariant=True)
 
 ATTRIBUTE_OPERATION: str = "operation"
 
 
 def set_operation(func: Callable, operation: "Operation", /) -> None:
     setattr(func, ATTRIBUTE_OPERATION, operation)
 
@@ -43,63 +43,64 @@
     if operation is None:
         raise NotAnOperationError(f"{func!r} is not an operation")
 
     return operation
 
 
 @dataclass
-class OperationSpecification:
-    request: PreRequest
+class Operation(Generic[PS, RT_co]):
+    func: Callable[PS, RT_co]
+    client_options: ClientOptions
+    request_options: PreRequest
+    client: Optional[Client] = None
     response: Optional[Callable[..., Any]] = None
     middleware: Middleware = field(default_factory=Middleware)
-
-
-@dataclass
-class Operation(Generic[PS, RT]):
-    func: Callable[PS, RT]
-    specification: OperationSpecification
-    client: Optional[Client]
-    middleware: Middleware = field(default_factory=Middleware)
+    dependencies: MutableSequence[Callable[..., Any]] = field(default_factory=list)
 
     def __call__(self, *args: PS.args, **kwargs: PS.kwargs) -> Any:
-        pre_request: PreRequest = self.specification.request.merge(
-            PreRequest(
-                method=self.specification.request.method,
-                url=self.specification.request.url,
-            )
-        )
+        client: Client
+
+        if self.client is not None:
+            client = self.client
+        else:
+            # Build a disposable client using the available client options
+            client = self.client_options.build()
+
+        # Create a clone of the request options, so that mutations don't
+        # affect the original copy.
+        # Mutations to the request options will occur during composition.
+        pre_request: PreRequest = self.request_options.clone()
 
+        # Compose the request using the provided arguments
         compose(self.func, pre_request, args, kwargs)
 
-        request: Request = pre_request.build_request(self.client)
+        # Compose the request using each of the composition dependencies
+        dependency: Callable[..., None]
+        for dependency in self.dependencies:
+            resolve_request(dependency, pre_request)
+
+        request: Request = pre_request.build_request(client)
 
         return_annotation: Any = inspect.signature(self.func).return_annotation
 
         if return_annotation is PreRequest:
             return pre_request
         if return_annotation is Request:
             return request
 
-        client: Client = self.client if self.client is not None else Client()
-
-        middleware: Middleware = Middleware()
-
-        middleware.record.extend(self.specification.middleware.record)
-        middleware.record.extend(self.middleware.record)
-
-        @middleware.compose
+        @self.middleware.compose
         def send_request(request: Request, /) -> Response:
             httpx_response: httpx.Response = client.send(request)
 
             return Response.from_httpx_response(httpx_response)
 
         response: Response = send_request(request)
 
-        if self.specification.response is not None:
-            return resolve(self.specification.response, response)
+        if self.response is not None:
+            return resolve_response(self.response, response)
 
         if return_annotation is inspect.Parameter.empty:
             try:
                 return response.json()
             except JSONDecodeError:
                 return response.text
         if return_annotation is None:
@@ -110,17 +111,17 @@
             return_annotation, BaseModel
         ):
             return return_annotation.parse_obj(response.json())
 
         return pydantic.parse_raw_as(return_annotation, response.text)
 
     @property
-    def wrapper(self) -> Callable[PS, RT]:
+    def wrapper(self) -> Callable[PS, RT_co]:
         @functools.wraps(self.func)
-        def wrapper(*args: PS.args, **kwargs: PS.kwargs) -> RT:
+        def wrapper(*args: PS.args, **kwargs: PS.kwargs) -> RT_co:
             if inspect.ismethod(self.func):
                 # Read off `self` or `cls`
                 _, *args = args  # type: ignore
 
             return self(*args, **kwargs)
 
         set_operation(wrapper, self)
```

### Comparing `neoclient-0.1.19/neoclient/param_functions.py` & `neoclient-0.1.29/neoclient/param_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Callable, Optional, Sequence
 
 from pydantic import Required
 
-from .dependencies import DependencyParameter
+from .dependence import DependencyParameter
 from .params import (
     BodyParameter,
     CookieParameter,
     CookiesParameter,
     HeaderParameter,
     HeadersParameter,
     PathParameter,
```

### Comparing `neoclient-0.1.19/neoclient/param_functions.pyi` & `neoclient-0.1.29/neoclient/param_functions.pyi`

 * *Files identical despite different names*

### Comparing `neoclient-0.1.19/neoclient/params.py` & `neoclient-0.1.29/neoclient/params.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 from .converters import (
     convert_cookie,
     convert_header,
     convert_path_param,
     convert_query_param,
 )
 from .errors import CompositionError, ResolutionError
-from .models import PreRequest, Response
+from .models import PreRequest, Request, Response
 from .resolvers import (
     BodyResolver,
     CookieResolver,
     CookiesResolver,
     HeaderResolver,
     HeadersResolver,
     QueriesResolver,
     QueryResolver,
     StateResolver,
 )
 from .types import CookiesTypes, HeadersTypes, PathsTypes, QueriesTypes
-from .typing import RequestConsumer, Resolver, Supplier
+from .typing import RequestConsumer, RequestResolver, ResponseResolver, Supplier
 from .utils import parse_obj_as
 
 __all__: Sequence[str] = (
     "QueryParameter",
     "HeaderParameter",
     "CookieParameter",
     "PathParameter",
@@ -103,16 +103,23 @@
         # To mitigate this, the alias is explicity converted to a string here.
         if self.alias is not None:
             self.alias = str(self.alias)
 
     def compose(self, request: PreRequest, argument: Any, /) -> None:
         raise CompositionError(f"Parameter {type(self)!r} is not composable")
 
-    def resolve(self, response: Response, /) -> Any:
-        raise ResolutionError(f"Parameter {type(self)!r} is not resolvable")
+    def resolve_response(self, response: Response, /) -> Any:
+        raise ResolutionError(
+            f"Parameter {type(self)!r} is not resolvable for type {Response!r}"
+        )
+
+    def resolve_request(self, request: PreRequest, /) -> Any:
+        raise ResolutionError(
+            f"Parameter {type(self)!r} is not resolvable for type {PreRequest!r}"
+        )
 
     def prepare(self, model_field: ModelField, /) -> None:
         if self.alias is None:
             self.alias = model_field.name
 
 
 class ComposableSingletonParameter(ABC, Parameter, Generic[K, V]):
@@ -142,32 +149,48 @@
 
     @abstractmethod
     def build_consumer(self, key: K, value: V) -> RequestConsumer:
         ...
 
 
 class ResolvableSingletonParameter(ABC, Parameter, Generic[K, V]):
-    def resolve(self, response: Response, /) -> V:
+    def resolve_request(self, request: PreRequest, /) -> V:
         if self.alias is None:
             raise ResolutionError(
                 f"Cannot resolve parameter {type(self)!r} without an alias"
             )
 
-        resolver: Resolver[V] = self.build_resolver(
+        resolver: RequestResolver[V] = self.build_request_resolver(
+            self.parse_key(self.alias),
+        )
+
+        return resolver(request)
+
+    def resolve_response(self, response: Response, /) -> V:
+        if self.alias is None:
+            raise ResolutionError(
+                f"Cannot resolve parameter {type(self)!r} without an alias"
+            )
+
+        resolver: ResponseResolver[V] = self.build_response_resolver(
             self.parse_key(self.alias),
         )
 
         return resolver(response)
 
     @abstractmethod
     def parse_key(self, key: str, /) -> K:
         ...
 
     @abstractmethod
-    def build_resolver(self, key: K) -> Resolver[V]:
+    def build_request_resolver(self, key: K) -> RequestResolver[V]:
+        ...
+
+    @abstractmethod
+    def build_response_resolver(self, key: K) -> ResponseResolver[V]:
         ...
 
 
 class ComposableSingletonStringParameter(ComposableSingletonParameter[str, str]):
     def parse_key(self, key: str, /) -> str:
         return key
 
@@ -176,59 +199,81 @@
     ResolvableSingletonParameter[str, Optional[str]]
 ):
     def parse_key(self, key: str, /) -> str:
         return key
 
 
 class QueryParameter(
-    ComposableSingletonStringParameter, ResolvableSingletonStringParameter
+    ComposableSingletonParameter[str, Sequence[str]],
+    ResolvableSingletonParameter[str, Optional[Sequence[str]]],
 ):
-    def parse_value(self, value: Any, /) -> str:
+    def parse_key(self, key: str, /) -> str:
+        return key
+
+    def parse_value(self, value: Any, /) -> Sequence[str]:
         return convert_query_param(value)
 
-    def build_consumer(self, key: str, value: str) -> RequestConsumer:
+    def build_consumer(self, key: str, value: Sequence[str]) -> RequestConsumer:
         return QueryConsumer(key, value).consume_request
 
-    def build_resolver(self, key: str) -> Resolver[Optional[str]]:
-        return QueryResolver(key)
+    def build_request_resolver(
+        self, key: str
+    ) -> RequestResolver[Optional[Sequence[str]]]:
+        return QueryResolver(key).resolve_request
+
+    def build_response_resolver(
+        self, key: str
+    ) -> ResponseResolver[Optional[Sequence[str]]]:
+        return QueryResolver(key).resolve_response
 
 
 @dataclass(unsafe_hash=True)
 class HeaderParameter(
-    ComposableSingletonStringParameter, ResolvableSingletonStringParameter
+    ComposableSingletonParameter[str, Sequence[str]],
+    ResolvableSingletonParameter[str, Optional[Sequence[str]]],
 ):
     convert_underscores: bool = True
 
     def parse_key(self, key: str, /) -> str:
         if self.convert_underscores:
             return key.replace("_", "-")
-        else:
-            return key
 
-    def parse_value(self, value: Any, /) -> str:
+        return key
+
+    def parse_value(self, value: Any, /) -> Sequence[str]:
         return convert_header(value)
 
-    def build_consumer(self, key: str, value: str) -> RequestConsumer:
+    def build_consumer(self, key: str, value: Sequence[str]) -> RequestConsumer:
         return HeaderConsumer(key, value).consume_request
 
-    def build_resolver(self, key: str) -> Resolver[Optional[str]]:
-        return HeaderResolver(key)
+    def build_request_resolver(
+        self, key: str
+    ) -> RequestResolver[Optional[Sequence[str]]]:
+        return HeaderResolver(key).resolve_request
+
+    def build_response_resolver(
+        self, key: str
+    ) -> ResponseResolver[Optional[Sequence[str]]]:
+        return HeaderResolver(key).resolve_response
 
 
 class CookieParameter(
     ComposableSingletonStringParameter, ResolvableSingletonStringParameter
 ):
     def parse_value(self, value: Any, /) -> str:
         return convert_cookie(value)
 
     def build_consumer(self, key: str, value: str) -> RequestConsumer:
         return CookieConsumer(key, value).consume_request
 
-    def build_resolver(self, key: str) -> Resolver[Optional[str]]:
-        return CookieResolver(key)
+    def build_request_resolver(self, key: str) -> RequestResolver[Optional[str]]:
+        return CookieResolver(key).resolve_request
+
+    def build_response_resolver(self, key: str) -> ResponseResolver[Optional[str]]:
+        return CookieResolver(key).resolve_response
 
 
 class PathParameter(ComposableSingletonStringParameter):
     def parse_value(self, value: Any, /) -> str:
         return convert_path_param(value)
 
     def build_consumer(self, key: str, value: str) -> RequestConsumer:
@@ -237,36 +282,45 @@
 
 class QueriesParameter(Parameter):
     def compose(self, request: PreRequest, argument: Any, /) -> None:
         params: QueriesTypes = parse_obj_as(QueriesTypes, argument)  # type: ignore
 
         QueriesConsumer(params).consume_request(request)
 
-    def resolve(self, response: Response, /) -> QueryParams:
-        return QueriesResolver()(response)
+    def resolve_request(self, request: PreRequest, /) -> QueryParams:
+        return QueriesResolver().resolve_request(request)
+
+    def resolve_response(self, response: Response, /) -> QueryParams:
+        return QueriesResolver().resolve_response(response)
 
 
 class HeadersParameter(Parameter):
     def compose(self, request: PreRequest, argument: Any, /) -> None:
         headers: HeadersTypes = parse_obj_as(HeadersTypes, argument)  # type: ignore
 
         HeadersConsumer(headers).consume_request(request)
 
-    def resolve(self, response: Response, /) -> Headers:
-        return HeadersResolver()(response)
+    def resolve_request(self, request: PreRequest, /) -> Headers:
+        return HeadersResolver().resolve_request(request)
+
+    def resolve_response(self, response: Response, /) -> Headers:
+        return HeadersResolver().resolve_response(response)
 
 
 class CookiesParameter(Parameter):
     def compose(self, request: PreRequest, argument: Any, /) -> None:
         cookies: CookiesTypes = parse_obj_as(CookiesTypes, argument)  # type: ignore
 
         CookiesConsumer(cookies).consume_request(request)
 
-    def resolve(self, response: Response, /) -> Cookies:
-        return CookiesResolver()(response)
+    def resolve_request(self, request: PreRequest, /) -> Cookies:
+        return CookiesResolver().resolve_request(request)
+
+    def resolve_response(self, response: Response, /) -> Cookies:
+        return CookiesResolver().resolve_response(response)
 
 
 class PathsParameter(Parameter):
     def compose(self, request: PreRequest, argument: Any, /) -> None:
         path_params: PathsTypes = parse_obj_as(PathsTypes, argument)  # type: ignore
 
         PathsConsumer(path_params).consume_request(request)
@@ -297,35 +351,41 @@
             request.json = json_value
         else:
             if request.json is None:
                 request.json = json_value
             else:
                 request.json.update(json_value)
 
-    def resolve(self, response: Response, /) -> Any:
+    def resolve_response(self, response: Response, /) -> Any:
         return BodyResolver()(response)
 
 
 class URLParameter(Parameter):
-    def resolve(self, response: Response, /) -> httpx.URL:
+    def resolve_request(self, request: PreRequest, /) -> httpx.URL:
+        return request.url
+
+    def resolve_response(self, response: Response, /) -> httpx.URL:
         return response.request.url
 
 
 class ResponseParameter(Parameter):
-    def resolve(self, response: Response, /) -> Response:
+    def resolve_response(self, response: Response, /) -> Response:
         return response
 
 
 class RequestParameter(Parameter):
-    def resolve(self, response: Response, /) -> httpx.Request:
+    def resolve_response(self, response: Response, /) -> httpx.Request:
         return response.request
 
+    def resolve_request(self, request: PreRequest, /) -> PreRequest:
+        return request
+
 
 class StatusCodeParameter(Parameter):
-    def resolve(self, response: Response, /) -> int:
+    def resolve_response(self, response: Response, /) -> int:
         return response.status_code
 
 
 class StateParameter(
     ComposableSingletonParameter[str, Any], ResolvableSingletonParameter[str, Any]
 ):
     def parse_key(self, key: str, /) -> str:
@@ -333,9 +393,12 @@
 
     def parse_value(self, value: Any, /) -> Any:
         return value
 
     def build_consumer(self, key: str, value: Any) -> RequestConsumer:
         return StateConsumer(key, value).consume_request
 
-    def build_resolver(self, key: str) -> Resolver[Any]:
-        return StateResolver(key)
+    def build_request_resolver(self, key: str) -> RequestResolver[Any]:
+        return StateResolver(key).resolve_request
+
+    def build_response_resolver(self, key: str) -> ResponseResolver[Any]:
+        return StateResolver(key).resolve_response
```

### Comparing `neoclient-0.1.19/neoclient/resolvers.py` & `neoclient-0.1.29/neoclient/resolvers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Any, Optional, Sequence, TypeVar
 
 from httpx import Cookies, Headers, QueryParams
 
-from .models import Response
-from .typing import Resolver
+from .models import PreRequest, Response, State
+from .typing import ResponseResolver
 
 __all__: Sequence[str] = (
     "BodyResolver",
     "CookieResolver",
     "CookiesResolver",
     "HeaderResolver",
     "HeadersResolver",
@@ -17,60 +17,102 @@
     "StateResolver",
 )
 
 T = TypeVar("T")
 
 
 @dataclass
-class QueryResolver(Resolver[Optional[str]]):
+class QueryResolver:
     name: str
 
-    def __call__(self, response: Response, /) -> Optional[str]:
-        return response.request.url.params.get(self.name)
+    def resolve_request(self, request: PreRequest, /) -> Optional[Sequence[str]]:
+        return self.resolve(request.params)
+
+    def resolve_response(self, response: Response, /) -> Optional[Sequence[str]]:
+        return self.resolve(response.request.url.params)
+
+    def resolve(self, query_params: QueryParams, /) -> Optional[Sequence[str]]:
+        if self.name in query_params:
+            return query_params.get_list(self.name)
+
+        return None
 
 
 @dataclass
-class HeaderResolver(Resolver[Optional[str]]):
+class HeaderResolver:
     name: str
 
-    def __call__(self, response: Response, /) -> Optional[str]:
-        return response.headers.get(self.name)
+    def resolve_request(self, request: PreRequest, /) -> Optional[Sequence[str]]:
+        return self.resolve(request.headers)
+
+    def resolve_response(self, response: Response, /) -> Optional[Sequence[str]]:
+        return self.resolve(response.headers)
+
+    def resolve(self, headers: Headers, /) -> Optional[Sequence[str]]:
+        if self.name in headers:
+            return headers.get_list(self.name)
+
+        return None
 
 
 @dataclass
-class CookieResolver(Resolver[Optional[str]]):
+class CookieResolver:
     name: str
 
-    def __call__(self, response: Response, /) -> Optional[str]:
-        return response.cookies.get(self.name)
+    def resolve_request(self, request: PreRequest, /) -> Optional[str]:
+        return self.resolve(request.cookies)
+
+    def resolve_response(self, response: Response, /) -> Optional[str]:
+        return self.resolve(response.cookies)
+
+    def resolve(self, cookies: Cookies, /) -> Optional[str]:
+        return cookies.get(self.name)
 
 
-class QueriesResolver(Resolver[QueryParams]):
+class QueriesResolver:
     @staticmethod
-    def __call__(response: Response, /) -> QueryParams:
+    def resolve_request(request: PreRequest, /) -> QueryParams:
+        return request.params
+
+    @staticmethod
+    def resolve_response(response: Response, /) -> QueryParams:
         return response.request.url.params
 
 
-class HeadersResolver(Resolver[Headers]):
+class HeadersResolver:
+    @staticmethod
+    def resolve_request(request: PreRequest, /) -> Headers:
+        return request.headers
+
     @staticmethod
-    def __call__(response: Response, /) -> Headers:
+    def resolve_response(response: Response, /) -> Headers:
         return response.headers
 
 
-class CookiesResolver(Resolver[Cookies]):
+class CookiesResolver:
     @staticmethod
-    def __call__(response: Response, /) -> Cookies:
+    def resolve_request(request: PreRequest, /) -> Cookies:
+        return request.cookies
+
+    @staticmethod
+    def resolve_response(response: Response, /) -> Cookies:
         return response.cookies
 
 
-class BodyResolver(Resolver[Any]):
+class BodyResolver(ResponseResolver[Any]):
     @staticmethod
     def __call__(response: Response, /) -> Any:
         return response.json()
 
 
 @dataclass
-class StateResolver(Resolver[Any]):
+class StateResolver:
     key: str
 
-    def __call__(self, response: Response, /) -> Any:
-        return response.state.get(self.key)
+    def resolve_request(self, request: PreRequest, /) -> Any:
+        return self.resolve(request.state)
+
+    def resolve_response(self, response: Response, /) -> Any:
+        return self.resolve(response.state)
+
+    def resolve(self, state: State, /) -> Any:
+        return state.get(self.key)
```

### Comparing `neoclient-0.1.19/neoclient/types.py` & `neoclient-0.1.29/neoclient/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     str,
     int,
     float,
     bool,
     None,
 ]
 QueryTypes: TypeAlias = Any
-HeaderTypes: TypeAlias = Any
+HeaderTypes: TypeAlias = Union[Primitive, Sequence[Primitive]]
 CookieTypes: TypeAlias = Any
 PathTypes: TypeAlias = Union[Primitive, Sequence[Primitive]]
 QueriesTypes: TypeAlias = Union[
     QueryParams,
     Mapping[str, Union[Primitive, Sequence[Primitive]]],
     List[Tuple[str, Primitive]],
     Tuple[Tuple[str, Primitive], ...],
```

### Comparing `neoclient-0.1.19/neoclient/utils.py` & `neoclient-0.1.29/neoclient/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import string
+import typing
 from typing import (
     Any,
     Callable,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
@@ -21,16 +22,16 @@
 __all__: Sequence[str] = (
     "parse_format_string",
     "bind_arguments",
     "is_primitive",
     "unpack_arguments",
     "get_default",
     "has_default",
-    "get_method_kind",
     "parse_obj_as",
+    "is_generic_alias",
 )
 
 T = TypeVar("T")
 
 
 def parse_format_string(format_string: str, /) -> Set[str]:
     """
@@ -103,16 +104,16 @@
 
     return (tuple(args), kwargs)
 
 
 def get_default(field_info: FieldInfo, /) -> Any:
     if field_info.default_factory is not None:
         return field_info.default_factory()
-    else:
-        return field_info.default
+
+    return field_info.default
 
 
 def has_default(field_info: FieldInfo, /) -> bool:
     return field_info.default is not Undefined or field_info.default_factory is not None
 
 
 def parse_obj_as(type_: Type[T], obj: Any) -> T:
@@ -126,7 +127,11 @@
         __config__=Config,
         __root__=(type_, ...),
     )
 
     model: BaseModel = model_cls(__root__=obj)
 
     return getattr(model, "__root__")
+
+
+def is_generic_alias(type_: Type, /) -> bool:
+    return typing.get_origin(type_) is not None
```

### Comparing `neoclient-0.1.19/neoclient/validation.py` & `neoclient-0.1.29/neoclient/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
         setattr(wrapper, "validator", validated_func)
 
         return wrapper
 
     if func:
         return decorate(func)
-    else:
-        return decorate
+
+    return decorate
 
 
 def create_func_model(
     function: Callable,
     fields: Mapping[str, Any],
     *,
     config: Optional[ConfigType] = None,
```

### Comparing `neoclient-0.1.19/PKG-INFO` & `neoclient-0.1.29/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: neoclient
-Version: 0.1.19
+Version: 0.1.29
 Summary: Fast API Clients for Python
 Home-page: https://github.com/tombulled/neoclient
 License: MIT
 Keywords: python,api,http,client,json,framework,web,rest
 Author: Tom Bulled
 Author-email: 26026015+tombulled@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: mediate (>=0.1.7,<0.2.0)
+Requires-Dist: mediate (>=0.1.8,<0.2.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: tombulled-annotate (>=0.1.15,<0.2.0)
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
 Project-URL: Repository, https://github.com/tombulled/neoclient
 Description-Content-Type: text/markdown
 
 # neoclient
 🚀 Fast API Clients for Python
```

