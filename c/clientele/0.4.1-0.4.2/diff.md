# Comparing `tmp/clientele-0.4.1.tar.gz` & `tmp/clientele-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clientele-0.4.1.tar", max compression
+gzip compressed data, was "clientele-0.4.2.tar", max compression
```

## Comparing `clientele-0.4.1.tar` & `clientele-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1069 2023-07-25 03:31:07.492783 clientele-0.4.1/LICENSE
--rw-r--r--   0        0        0     1718 2023-08-02 04:28:12.938554 clientele-0.4.1/README.md
--rw-r--r--   0        0        0      905 2023-08-02 21:28:27.197731 clientele-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.4.1/src/__init__.py
--rw-r--r--   0        0        0     2924 2023-08-01 23:27:45.401764 clientele-0.4.1/src/cli.py
--rw-r--r--   0        0        0       50 2023-07-31 02:40:13.111663 clientele-0.4.1/src/client_template/MANIFEST
--rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.4.1/src/client_template/__init__.py
--rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.4.1/src/client_template/client.py
--rw-r--r--   0        0        0      993 2023-08-02 03:52:10.187256 clientele-0.4.1/src/client_template/http.py
--rw-r--r--   0        0        0       76 2023-08-02 03:43:33.184239 clientele-0.4.1/src/client_template/schemas.py
--rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.4.1/src/constants_template.py
--rw-r--r--   0        0        0     2069 2023-08-01 23:23:41.098914 clientele-0.4.1/src/generator.py
--rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.4.1/src/generators/__init__.py
--rw-r--r--   0        0        0     9967 2023-08-02 21:23:33.310164 clientele-0.4.1/src/generators/clients.py
--rw-r--r--   0        0        0     2830 2023-08-02 21:22:03.573057 clientele-0.4.1/src/generators/http.py
--rw-r--r--   0        0        0     6297 2023-08-02 21:11:36.405951 clientele-0.4.1/src/generators/schemas.py
--rw-r--r--   0        0        0      391 2023-08-02 21:28:31.333711 clientele-0.4.1/src/settings.py
--rw-r--r--   0        0        0      464 2023-08-02 04:21:15.956387 clientele-0.4.1/src/templates/async_methods.jinja2
--rw-r--r--   0        0        0       75 2023-08-01 23:33:19.745482 clientele-0.4.1/src/templates/basic_client.jinja2
--rw-r--r--   0        0        0      134 2023-08-01 23:34:59.694567 clientele-0.4.1/src/templates/bearer_client.jinja2
--rw-r--r--   0        0        0       34 2023-08-01 23:32:13.768760 clientele-0.4.1/src/templates/client.jinja2
--rw-r--r--   0        0        0      571 2023-08-02 21:24:19.832994 clientele-0.4.1/src/templates/get_method.jinja2
--rw-r--r--   0        0        0      607 2023-08-02 04:27:04.858109 clientele-0.4.1/src/templates/post_method.jinja2
--rw-r--r--   0        0        0      115 2023-08-02 04:06:42.400353 clientele-0.4.1/src/templates/schema_class.jinja2
--rw-r--r--   0        0        0      428 2023-08-02 04:21:04.265390 clientele-0.4.1/src/templates/sync_methods.jinja2
--rw-r--r--   0        0        0     2884 2023-08-02 21:18:05.831839 clientele-0.4.1/src/utils.py
--rw-r--r--   0        0        0      558 2023-08-02 21:21:10.707203 clientele-0.4.1/src/writer.py
--rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 clientele-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-25 03:31:07.492783 clientele-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1718 2023-08-02 04:28:12.938554 clientele-0.4.2/README.md
+-rw-r--r--   0        0        0      905 2023-08-03 02:41:02.434954 clientele-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.674462 clientele-0.4.2/src/__init__.py
+-rw-r--r--   0        0        0     2924 2023-08-01 23:27:45.401764 clientele-0.4.2/src/cli.py
+-rw-r--r--   0        0        0       50 2023-07-31 02:40:13.111663 clientele-0.4.2/src/client_template/MANIFEST
+-rw-r--r--   0        0        0        0 2023-07-24 01:55:07.678461 clientele-0.4.2/src/client_template/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-24 21:14:06.265426 clientele-0.4.2/src/client_template/client.py
+-rw-r--r--   0        0        0     1033 2023-08-03 02:35:56.531680 clientele-0.4.2/src/client_template/http.py
+-rw-r--r--   0        0        0       99 2023-08-03 02:32:37.858872 clientele-0.4.2/src/client_template/schemas.py
+-rw-r--r--   0        0        0      763 2023-07-25 01:10:08.502988 clientele-0.4.2/src/constants_template.py
+-rw-r--r--   0        0        0     2116 2023-08-03 02:38:38.596407 clientele-0.4.2/src/generator.py
+-rw-r--r--   0        0        0        0 2023-07-24 02:31:15.493615 clientele-0.4.2/src/generators/__init__.py
+-rw-r--r--   0        0        0     9967 2023-08-02 21:23:33.310164 clientele-0.4.2/src/generators/clients.py
+-rw-r--r--   0        0        0     2830 2023-08-02 21:22:03.573057 clientele-0.4.2/src/generators/http.py
+-rw-r--r--   0        0        0     6534 2023-08-03 02:38:22.201082 clientele-0.4.2/src/generators/schemas.py
+-rw-r--r--   0        0        0      391 2023-08-03 02:41:05.134859 clientele-0.4.2/src/settings.py
+-rw-r--r--   0        0        0      464 2023-08-02 04:21:15.956387 clientele-0.4.2/src/templates/async_methods.jinja2
+-rw-r--r--   0        0        0       75 2023-08-01 23:33:19.745482 clientele-0.4.2/src/templates/basic_client.jinja2
+-rw-r--r--   0        0        0      134 2023-08-01 23:34:59.694567 clientele-0.4.2/src/templates/bearer_client.jinja2
+-rw-r--r--   0        0        0       34 2023-08-01 23:32:13.768760 clientele-0.4.2/src/templates/client.jinja2
+-rw-r--r--   0        0        0      571 2023-08-02 21:24:19.832994 clientele-0.4.2/src/templates/get_method.jinja2
+-rw-r--r--   0        0        0      607 2023-08-02 04:27:04.858109 clientele-0.4.2/src/templates/post_method.jinja2
+-rw-r--r--   0        0        0      115 2023-08-02 04:06:42.400353 clientele-0.4.2/src/templates/schema_class.jinja2
+-rw-r--r--   0        0        0      804 2023-08-03 02:40:29.124147 clientele-0.4.2/src/templates/schema_helpers.jinja2
+-rw-r--r--   0        0        0      428 2023-08-02 04:21:04.265390 clientele-0.4.2/src/templates/sync_methods.jinja2
+-rw-r--r--   0        0        0     2884 2023-08-02 21:18:05.831839 clientele-0.4.2/src/utils.py
+-rw-r--r--   0        0        0      558 2023-08-02 21:21:10.707203 clientele-0.4.2/src/writer.py
+-rw-r--r--   0        0        0     2588 1970-01-01 00:00:00.000000 clientele-0.4.2/PKG-INFO
```

### Comparing `clientele-0.4.1/LICENSE` & `clientele-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clientele-0.4.1/README.md` & `clientele-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `clientele-0.4.1/pyproject.toml` & `clientele-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clientele"
-version = "0.4.1"
+version = "0.4.2"
 description = "Typed API Clients from OpenAPI schemas"
 authors = ["Paul Hallett <paulandrewhallett@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "src"}]
 homepage = "https://phalt.github.io/clientele/"
```

### Comparing `clientele-0.4.1/src/cli.py` & `clientele-0.4.2/src/cli.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.1/src/client_template/http.py` & `clientele-0.4.2/src/client_template/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,20 +17,21 @@
     return url_parts.geturl()
 
 
 def handle_response(func, response):
     """
     returns a response that matches the data neatly for a function
     """
-    response.raise_for_status()
     response_data = response.json()
     response_types = typing.get_type_hints(func).get("return")
     if typing.get_origin(response_types) == typing.Union:
         response_types = list(typing.get_args(response_types))
     else:
         response_types = [response_types]
 
     for single_type in response_types:
         try:
             return single_type.model_validate(response_data)
         except ValidationError:
             continue
+    # As a fall back, return the response_data
+    return response_data
```

### Comparing `clientele-0.4.1/src/constants_template.py` & `clientele-0.4.2/src/constants_template.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.1/src/generator.py` & `clientele-0.4.2/src/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,7 +55,8 @@
                 f"{CONSTANTS_ROOT}/constants_template.py",
                 f"{self.output_dir}constants.py",
             )
         self.generate_manifest()
         self.schemas_generator.generate_schema_classes()
         self.clients_generator.generate_paths()
         self.http_generator.generate_http_content()
+        self.schemas_generator.write_helpers()
```

### Comparing `clientele-0.4.1/src/generators/clients.py` & `clientele-0.4.2/src/generators/clients.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.1/src/generators/http.py` & `clientele-0.4.2/src/generators/http.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.1/src/generators/schemas.py` & `clientele-0.4.2/src/generators/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,22 @@
             class_name=schema_key, properties=properties, enum=enum
         )
         write_to_schemas(
             content,
             output_dir=self.output_dir,
         )
 
+    def write_helpers(self) -> None:
+        template = templates.get_template("schema_helpers.jinja2")
+        content = template.render()
+        write_to_schemas(
+            content,
+            output_dir=self.output_dir,
+        )
+
     def generate_schema_classes(self) -> None:
         """
         Generates all Pydantic schema classes.
         """
         for schema_key, schema in self.spec["components"]["schemas"].items():
             self.make_schema_class(schema_key=schema_key, schema=schema)
-
         console.log(f"Generated {len(self.schemas.items())} schemas...")
```

### Comparing `clientele-0.4.1/src/templates/get_method.jinja2` & `clientele-0.4.2/src/templates/get_method.jinja2`

 * *Files identical despite different names*

### Comparing `clientele-0.4.1/src/templates/post_method.jinja2` & `clientele-0.4.2/src/templates/post_method.jinja2`

 * *Files identical despite different names*

### Comparing `clientele-0.4.1/src/utils.py` & `clientele-0.4.2/src/utils.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.1/src/writer.py` & `clientele-0.4.2/src/writer.py`

 * *Files identical despite different names*

### Comparing `clientele-0.4.1/PKG-INFO` & `clientele-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clientele
-Version: 0.4.1
+Version: 0.4.2
 Summary: Typed API Clients from OpenAPI schemas
 Home-page: https://phalt.github.io/clientele/
 License: MIT
 Author: Paul Hallett
 Author-email: paulandrewhallett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clientele Version: 0.4.1 Summary: Typed API Clients
+Metadata-Version: 2.1 Name: clientele Version: 0.4.2 Summary: Typed API Clients
 from OpenAPI schemas Home-page: https://phalt.github.io/clientele/ License: MIT
 Author: Paul Hallett Author-email: paulandrewhallett@gmail.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
```

