# Comparing `tmp/django_api_decorator-0.2.0a2.tar.gz` & `tmp/django_api_decorator-0.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_api_decorator-0.2.0a2.tar", max compression
+gzip compressed data, was "django_api_decorator-0.2.0a3.tar", max compression
```

## Comparing `django_api_decorator-0.2.0a2.tar` & `django_api_decorator-0.2.0a3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/LICENSE
--rw-r--r--   0        0        0      373 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/README.md
--rw-r--r--   0        0        0        0 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/__init__.py
--rw-r--r--   0        0        0      390 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/apps.py
--rw-r--r--   0        0        0    12218 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/decorators.py
--rw-r--r--   0        0        0        0 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/management/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/management/commands/generate_api_schemas.py
--rw-r--r--   0        0        0     9000 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/openapi.py
--rw-r--r--   0        0        0        0 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/py.typed
--rw-r--r--   0        0        0     1552 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/schema_file.py
--rw-r--r--   0        0        0     1037 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/types.py
--rw-r--r--   0        0        0     1993 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/utils.py
--rw-r--r--   0        0        0     1074 2023-07-26 11:02:11.524817 django_api_decorator-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 django_api_decorator-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/LICENSE
+-rw-r--r--   0        0        0     2697 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/__init__.py
+-rw-r--r--   0        0        0      390 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/apps.py
+-rw-r--r--   0        0        0    12466 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/decorators.py
+-rw-r--r--   0        0        0        0 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/management/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/management/commands/generate_api_schemas.py
+-rw-r--r--   0        0        0     9000 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/openapi.py
+-rw-r--r--   0        0        0        0 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/py.typed
+-rw-r--r--   0        0        0     1552 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/schema_file.py
+-rw-r--r--   0        0        0     1037 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/types.py
+-rw-r--r--   0        0        0     1993 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/django_api_decorator/utils.py
+-rw-r--r--   0        0        0     1074 2023-08-03 13:50:16.820040 django_api_decorator-0.2.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 django_api_decorator-0.2.0a3/PKG-INFO
```

### Comparing `django_api_decorator-0.2.0a2/LICENSE` & `django_api_decorator-0.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a2/django_api_decorator/decorators.py` & `django_api_decorator-0.2.0a3/django_api_decorator/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     *,
     method: str,
     query_params: list[str] | None = None,
     login_required: bool | None = None,
     response_status: int = 200,
     atomic: bool | None = None,
     auth_check: Callable[[HttpRequest], bool] | None = None,
+    serialize_by_alias: bool = False,
 ) -> Callable[[Callable[P, T]], Callable[P, HttpResponse]]:
     """
     Defines an API view. This handles validation of query parameters, parsing of
     the request body, access control, and serialization of the response payload.
 
     * query_params:
         This is a list of the function parameters that should be
@@ -45,14 +46,18 @@
         Indicates that this endpoint is only available to authenticated
         users. Non-authenticated users will get a 401 response.
 
     * response_status:
         HTTP status code to use if the view _does not_ return an
         Response object, but rather just the data we should return.
 
+    * serialize_by_alias:
+        Is passed as the by_alias argument to TypeAdapter.dump_json(), making
+        the model use the aliases defined in model_config when serializing.
+
     The request body parsing is done by inspecting the view parameter types. If
     the view has a body parameter, we will try to decode the payload to that
     type. Currently Django Rest Framework serializers and pydantic models are are
      supported.
 
     Similarly the response body is encoded based on the type annotation for the
     return type. If the view is type annotated to return an HttpResponse object
@@ -178,15 +183,15 @@
             if not response_adapter:
                 raise TypeError(
                     f"{func} is annotated to return an http response, but returned "
                     f"{type(response)}"
                 )
 
             # Encode the response from the view to json and create a response object.
-            payload = response_adapter.dump_json(response)
+            payload = response_adapter.dump_json(response, by_alias=serialize_by_alias)
             return HttpResponse(
                 payload, status=response_status, content_type="application/json"
             )
 
         inner._api_meta = ApiMeta(  # type: ignore[attr-defined]
             method=method,
             query_params=query_params or [],
```

### Comparing `django_api_decorator-0.2.0a2/django_api_decorator/management/commands/generate_api_schemas.py` & `django_api_decorator-0.2.0a3/django_api_decorator/management/commands/generate_api_schemas.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a2/django_api_decorator/openapi.py` & `django_api_decorator-0.2.0a3/django_api_decorator/openapi.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a2/django_api_decorator/schema_file.py` & `django_api_decorator-0.2.0a3/django_api_decorator/schema_file.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a2/django_api_decorator/types.py` & `django_api_decorator-0.2.0a3/django_api_decorator/types.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a2/django_api_decorator/utils.py` & `django_api_decorator-0.2.0a3/django_api_decorator/utils.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a2/pyproject.toml` & `django_api_decorator-0.2.0a3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-api-decorator"
-version = "0.2.0a2"
+version = "0.2.0a3"
 description = "A collection of tools to build function based Django APIs"
 authors = ["Oda <tech@oda.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/django-api-decorator"
 repository = "https://github.com/kolonialno/django-api-decorator"
 packages = [{include = "django_api_decorator"}]
```

