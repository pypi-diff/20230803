# Comparing `tmp/sanic-rest-1.7.1.tar.gz` & `tmp/sanic_rest-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic-rest-1.7.1.tar", max compression
+gzip compressed data, was "sanic_rest-1.8.0.tar", max compression
```

## Comparing `sanic-rest-1.7.1.tar` & `sanic_rest-1.8.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    11358 2022-04-27 19:04:31.441289 sanic-rest-1.7.1/LICENSE.md
--rw-r--r--   0        0        0      553 2022-04-27 19:04:31.441289 sanic-rest-1.7.1/README.md
--rw-r--r--   0        0        0     1342 2022-04-27 19:04:31.441289 sanic-rest-1.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-27 19:04:31.441289 sanic-rest-1.7.1/sanic_rest/__init__.py
--rw-r--r--   0        0        0      875 2022-04-27 19:04:31.441289 sanic-rest-1.7.1/sanic_rest/exceptions.py
--rw-r--r--   0        0        0      489 2022-04-27 19:04:31.441289 sanic-rest-1.7.1/sanic_rest/protected_views.py
--rw-r--r--   0        0        0    15445 2022-04-27 19:04:31.441289 sanic-rest-1.7.1/sanic_rest/views.py
--rw-r--r--   0        0        0     1374 2022-04-27 19:04:43.723458 sanic-rest-1.7.1/setup.py
--rw-r--r--   0        0        0     1380 2022-04-27 19:04:43.723751 sanic-rest-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-08-02 22:12:56.186423 sanic_rest-1.8.0/LICENSE.md
+-rw-r--r--   0        0        0      553 2023-08-02 22:12:56.187161 sanic_rest-1.8.0/README.md
+-rw-r--r--   0        0        0     1529 2023-08-02 22:16:08.506760 sanic_rest-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 22:12:56.186842 sanic_rest-1.8.0/sanic_rest/__init__.py
+-rw-r--r--   0        0        0      875 2023-08-02 22:12:56.187466 sanic_rest-1.8.0/sanic_rest/exceptions.py
+-rw-r--r--   0        0        0      489 2023-08-02 22:17:15.668519 sanic_rest-1.8.0/sanic_rest/protected_views.py
+-rw-r--r--   0        0        0    15419 2023-08-02 22:19:08.087003 sanic_rest-1.8.0/sanic_rest/views.py
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 sanic_rest-1.8.0/PKG-INFO
```

### Comparing `sanic-rest-1.7.1/LICENSE.md` & `sanic_rest-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sanic-rest-1.7.1/README.md` & `sanic_rest-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `sanic-rest-1.7.1/sanic_rest/exceptions.py` & `sanic_rest-1.8.0/sanic_rest/exceptions.py`

 * *Files identical despite different names*

### Comparing `sanic-rest-1.7.1/sanic_rest/views.py` & `sanic_rest-1.8.0/sanic_rest/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,54 +2,54 @@
 import inspect
 import json
 import math
 import os
 import uuid
 from collections import defaultdict
 from pathlib import Path
-from typing import Tuple, Dict, Any, List, Type, Optional
+from typing import Any
 
 import aiofiles
 import pydantic
+import sanic.request
+import sanic.views
 from gcp_pilot.datastore import (
+    DEFAULT_PK_FIELD_NAME,
+    DEFAULT_PK_FIELD_TYPE,
     Document,
     DoesNotExist,
-    DEFAULT_PK_FIELD_TYPE,
-    DEFAULT_PK_FIELD_NAME,
     EmbeddedDocument,
 )
 from gcp_pilot.exceptions import ValidationError
-import sanic.views
-import sanic.request
 
 from sanic_rest import exceptions
 
-PayloadType = Dict[str, Any]
-ResponseType = Tuple[PayloadType, int]
+PayloadType = dict[str, Any]
+ResponseType = tuple[PayloadType, int]
 
 STAGE_DIR = os.environ.get("SANIC_FILE_DIR", default=Path(__file__).parent)
 
 
-def get_model_or_404(model_klass: Type[Document], pk: Any, query_filters: Dict = None) -> Document:
+def get_model_or_404(model_klass: type[Document], pk: Any, query_filters: dict | None = None) -> Document:
     query_filters = query_filters or {}
     try:
         return model_klass.documents.get(id=pk, **query_filters)
     except DoesNotExist as exc:
         raise exceptions.NotFoundError() from exc
 
 
 class FileProcessingMixin:
     async def store_file(self, field_name: str, file: sanic.request.File) -> str:
         identifier = uuid.uuid4().hex
         filepath = Path("media") / identifier / field_name / file.name
         output = await self.write_file(file=file, filepath=filepath)
         return str(output)
 
-    async def process_files(self, files: Dict[str, sanic.request.File]) -> Dict[str, Any]:
-        file_updates: Dict[str, Any] = defaultdict(list)
+    async def process_files(self, files: dict[str, sanic.request.File]) -> dict[str, Any]:
+        file_updates: dict[str, Any] = defaultdict(list)
         for key, key_files in files.items():
             for file in key_files:
                 filepath = await self.store_file(
                     field_name=key,
                     file=file,
                 )
                 file_updates[key].append(filepath)
@@ -62,15 +62,15 @@
         async with aiofiles.open(filepath, "wb") as file:
             await file.write(file.body)
         await file.close()
         return str(filepath)
 
 
 class ValidationMixin:
-    def validate(self, data, model_klass: Optional[Type[Document]] = None, current_obj: Optional[Document] = None):
+    def validate(self, data, model_klass: type[Document] | None = None, current_obj: Document | None = None):
         model_klass = model_klass or self.model
 
         model_data = (current_obj.dict() if current_obj else {}) | data
         try:
             model_klass(**model_data)
         except pydantic.ValidationError as exc:
             field_errors = {}
@@ -78,21 +78,21 @@
                 for field in err["loc"]:
                     field_errors[field] = err["msg"]
             raise exceptions.ValidationError(message=field_errors) from exc
         return data
 
 
 class ViewBase(FileProcessingMixin, ValidationMixin, sanic.views.HTTPMethodView):
-    model: Type[Document]
+    model: type[Document]
 
-    def _parse_body(self, request: sanic.request.Request) -> Tuple[Dict[str, Any], Dict[str, sanic.request.File]]:
+    def _parse_body(self, request: sanic.request.Request) -> tuple[dict[str, Any], dict[str, sanic.request.File]]:
         if "form" in request.content_type:
             data = {}
-            for key, value in dict(request.form).items():
-                value = [json.loads(item) for item in value]
+            for key, form_value in dict(request.form).items():
+                value = [json.loads(item) for item in form_value]
                 if len(value) == 1:
                     value = value[0]
                 data[key] = value
         else:
             data = request.json
 
         return data, dict(request.files)
@@ -124,19 +124,18 @@
         response_body = {
             "results": [obj.to_dict() for obj in items_in_page],
             "count": len(items),
             "num_pages": int(math.ceil(len(items) / page_size)),
         }
         return sanic.response.json(response_body, 200 if any(items_in_page) else 404, default=str)
 
-    def _parse_query_args(self, request: sanic.request.Request) -> Tuple[Dict[str, Any], int, int]:
+    def _parse_query_args(self, request: sanic.request.Request) -> tuple[dict[str, Any], int, int]:
         query_args = {}
-        for key, value in request.query_args:
-            if key == "q":
-                key = f"{self.search_field}__startswith"
+        for q_key, value in request.query_args:
+            key = f"{self.search_field}__startswith" if q_key == "q" else q_key
 
             if key not in query_args:
                 query_args[key] = value
             elif isinstance(query_args[key], list):
                 query_args[key].append(value)
             else:
                 query_args[key] = [query_args[key], value]
@@ -150,41 +149,41 @@
         if page < 1:
             raise exceptions.ValidationError("page starts at 1")
         if page_size < 1:
             raise exceptions.ValidationError("page_size must be at least at 1")
 
         return query_args, page, page_size
 
-    def _paginate(self, items: List[Document], page: int, page_size: int) -> List[Document]:
+    def _paginate(self, items: list[Document], page: int, page_size: int) -> list[Document]:
         # TODO Add proper pagination with cursors
         start_idx = (page - 1) * page_size
         start_idx = min(start_idx, len(items))
 
         end_idx = start_idx + page_size
         end_idx = min(end_idx, len(items))
 
         items_in_page = items[start_idx:end_idx]
         return items_in_page
 
-    async def perform_get(self, query_filters) -> List[Document]:
+    async def perform_get(self, query_filters) -> list[Document]:
         return list(self.model.documents.filter(**query_filters))
 
     async def post(self, request: sanic.request.Request) -> sanic.response.HTTPResponse:
         data, files = self._parse_body(request=request)
         validated_data = self.validate(data=data)
 
         try:
             obj = await self.perform_create(data=validated_data, files=files)
         except ValidationError as exc:
             raise exceptions.ValidationError(message=str(exc)) from exc
 
         response_body = obj.to_dict()
         return sanic.response.json(response_body, 201, default=str)
 
-    async def perform_create(self, data: PayloadType, files: Dict[str, sanic.request.File]) -> Document:
+    async def perform_create(self, data: PayloadType, files: dict[str, sanic.request.File]) -> Document:
         file_updates = await self.process_files(files=files)
 
         obj = self.model.from_dict(**data, **file_updates)
         return obj.save()
 
     async def options(self, request: sanic.request.Request) -> sanic.response.HTTPResponse:
         data = await self.perform_options()
@@ -234,15 +233,15 @@
             obj = await self.perform_create(obj=current_obj, data=validated_data, files=files)
         except ValidationError as exc:
             raise exceptions.ValidationError(message=str(exc)) from exc
 
         response_body = obj.to_dict()
         return sanic.response.json(response_body, 200, default=str)
 
-    async def perform_create(self, obj: Document, data: PayloadType, files: Dict[str, sanic.request.File]) -> Document:
+    async def perform_create(self, obj: Document, data: PayloadType, files: dict[str, sanic.request.File]) -> Document:
         file_updates = await self.process_files(files=files)
 
         obj = self.model.from_dict(pk=obj.pk, **data, **file_updates)
         return obj.save()
 
     async def patch(self, request: sanic.request.Request, pk: str) -> sanic.response.HTTPResponse:
         current_obj = self.get_model(pk=pk)
@@ -254,15 +253,15 @@
             obj = await self.perform_update(obj=current_obj, data=validated_data, files=files)
         except ValidationError as exc:
             raise exceptions.ValidationError(message=str(exc)) from exc
 
         response_body = obj.to_dict()
         return sanic.response.json(response_body, 200, default=str)
 
-    async def perform_update(self, obj: Document, data: PayloadType, files: Dict[str, sanic.request.File]) -> Document:
+    async def perform_update(self, obj: Document, data: PayloadType, files: dict[str, sanic.request.File]) -> Document:
         file_updates = await self.process_files(files=files)
 
         obj = self.model.documents.update(pk=obj.pk, **data, **file_updates)
 
         return obj
 
     async def delete(self, request: sanic.request.Request, pk: str) -> sanic.response.HTTPResponse:
@@ -270,15 +269,15 @@
         return sanic.response.json({}, 204, default=str)
 
     async def perform_delete(self, pk: str) -> None:
         self.model.documents.delete(pk=pk)
 
 
 class NestViewBase(ViewBase):
-    nest_model: Type[Document]
+    nest_model: type[Document]
 
     def get_nest_model(self, pk: str):
         return get_model_or_404(model_klass=self.nest_model, pk=pk)
 
 
 class NestedListView(NestViewBase):
     async def get(self, request: sanic.request.Request, nest_pk: str) -> sanic.response.HTTPResponse:
```

### Comparing `sanic-rest-1.7.1/PKG-INFO` & `sanic_rest-1.8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: sanic-rest
-Version: 1.7.1
+Version: 1.8.0
 Summary: Sanic Rest Framework with Google Cloud Datastore
 Home-page: https://github.com/flamingo-run/sanic-rest
 Keywords: sanic,restful,datastore
 Author: Joao Daher
 Author-email: joao@daher.dev
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: auth
-Requires-Dist: argon2_cffi; extra == "auth"
-Requires-Dist: gcp-pilot[storage,datastore]
-Requires-Dist: passlib; extra == "auth"
+Requires-Dist: argon2_cffi ; extra == "auth"
+Requires-Dist: gcp-pilot[datastore,storage]
+Requires-Dist: passlib ; extra == "auth"
 Requires-Dist: sanic
-Requires-Dist: sanic-jwt; extra == "auth"
+Requires-Dist: sanic-jwt ; extra == "auth"
 Requires-Dist: sanic-openapi
 Project-URL: Repository, https://github.com/flamingo-run/sanic-rest
 Description-Content-Type: text/markdown
 
 ![Github CI](https://github.com/flamingo-run/sanic-rest/workflows/Github%20CI/badge.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/0d6eb6158bc33aa2af1c/maintainability)](https://codeclimate.com/github/flamingo-run/sanic-rest/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/0d6eb6158bc33aa2af1c/test_coverage)](https://codeclimate.com/github/flamingo-run/sanic-rest/test_coverage)
```

