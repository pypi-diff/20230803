# Comparing `tmp/grai_source_looker-0.0.1a2.tar.gz` & `tmp/grai_source_looker-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_looker-0.0.1a2.tar", max compression
+gzip compressed data, was "grai_source_looker-0.0.1a3.tar", max compression
```

## Comparing `grai_source_looker-0.0.1a2.tar` & `grai_source_looker-0.0.1a3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      133 2023-08-03 09:33:45.520341 grai_source_looker-0.0.1a2/README.md
--rw-r--r--   0        0        0     1123 2023-08-03 13:09:41.436413 grai_source_looker-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0       97 2023-08-03 13:09:56.434396 grai_source_looker-0.0.1a2/src/grai_source_looker/__init__.py
--rw-r--r--   0        0        0     7947 2023-08-03 13:03:53.516927 grai_source_looker-0.0.1a2/src/grai_source_looker/adapters.py
--rw-r--r--   0        0        0       48 2023-08-03 09:59:32.956516 grai_source_looker-0.0.1a2/src/grai_source_looker/api/__init__.py
--rw-r--r--   0        0        0   642045 2023-08-03 09:33:45.526480 grai_source_looker-0.0.1a2/src/grai_source_looker/api/api_models.py
--rw-r--r--   0        0        0     2215 2023-08-03 13:03:53.418465 grai_source_looker-0.0.1a2/src/grai_source_looker/base.py
--rw-r--r--   0        0        0     3063 2023-08-03 13:03:53.483356 grai_source_looker-0.0.1a2/src/grai_source_looker/loader.py
--rw-r--r--   0        0        0     3379 2023-08-03 13:09:22.303519 grai_source_looker-0.0.1a2/src/grai_source_looker/models.py
--rw-r--r--   0        0        0      195 2023-08-03 09:33:45.526746 grai_source_looker-0.0.1a2/src/grai_source_looker/package_definitions.py
--rw-r--r--   0        0        0        0 2023-08-03 09:33:45.526767 grai_source_looker-0.0.1a2/src/grai_source_looker/py.typed
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 grai_source_looker-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0      133 2023-08-03 09:33:45.520341 grai_source_looker-0.0.1a3/README.md
+-rw-r--r--   0        0        0     1123 2023-08-03 13:29:53.571827 grai_source_looker-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-08-03 13:29:56.894502 grai_source_looker-0.0.1a3/src/grai_source_looker/__init__.py
+-rw-r--r--   0        0        0     7947 2023-08-03 13:03:53.516927 grai_source_looker-0.0.1a3/src/grai_source_looker/adapters.py
+-rw-r--r--   0        0        0       48 2023-08-03 09:59:32.956516 grai_source_looker-0.0.1a3/src/grai_source_looker/api/__init__.py
+-rw-r--r--   0        0        0   642045 2023-08-03 09:33:45.526480 grai_source_looker-0.0.1a3/src/grai_source_looker/api/api_models.py
+-rw-r--r--   0        0        0     2215 2023-08-03 13:03:53.418465 grai_source_looker-0.0.1a3/src/grai_source_looker/base.py
+-rw-r--r--   0        0        0     3015 2023-08-03 13:17:33.954769 grai_source_looker-0.0.1a3/src/grai_source_looker/loader.py
+-rw-r--r--   0        0        0     3454 2023-08-03 13:15:52.413917 grai_source_looker-0.0.1a3/src/grai_source_looker/models.py
+-rw-r--r--   0        0        0      195 2023-08-03 09:33:45.526746 grai_source_looker-0.0.1a3/src/grai_source_looker/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-08-03 09:33:45.526767 grai_source_looker-0.0.1a3/src/grai_source_looker/py.typed
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 grai_source_looker-0.0.1a3/PKG-INFO
```

### Comparing `grai_source_looker-0.0.1a2/pyproject.toml` & `grai_source_looker-0.0.1a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_looker"
-version = "0.0.1a2"
+version = "0.0.1a3"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_looker", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_looker-0.0.1a2/src/grai_source_looker/adapters.py` & `grai_source_looker-0.0.1a3/src/grai_source_looker/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_looker-0.0.1a2/src/grai_source_looker/api/api_models.py` & `grai_source_looker-0.0.1a3/src/grai_source_looker/api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_looker-0.0.1a2/src/grai_source_looker/base.py` & `grai_source_looker-0.0.1a3/src/grai_source_looker/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_looker-0.0.1a2/src/grai_source_looker/loader.py` & `grai_source_looker-0.0.1a3/src/grai_source_looker/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,17 @@
     ):
         passthrough_kwargs = {
             "base_url": base_url,
             "client_id": client_id,
             "client_secret": client_secret,
             "verify_ssl": verify_ssl,
         }
-        self.config = LookerConfig(**{k: v for k, v in passthrough_kwargs.items() if v is not None})
+        self.config = LookerConfig(
+            **{k: v for k, v in passthrough_kwargs.items() if v is not None}
+        )
 
         settings = LookerSettings(self.config)
 
         self.sdk = looker_sdk.init40(config_settings=settings)
 
     def get_dashboards(self):
         result = self.sdk.all_dashboards()
@@ -116,12 +118,8 @@
 
         for dashboard in dashboards:
             fields.extend(dashboard.get_fields())
             edges.extend(dashboard.get_edges())
 
         dashboards.extend(fields)
 
-        print(dashboards)
-        print(fields)
-        print(edges)
-
         return dashboards, edges
```

### Comparing `grai_source_looker-0.0.1a2/src/grai_source_looker/models.py` & `grai_source_looker-0.0.1a3/src/grai_source_looker/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,16 +76,21 @@
     name: str
 
 
 class Query(LookerNode):
     fields: List[str]
 
 
+class ResultMaker(LookerNode):
+    query: Optional[Query]
+
+
 class DashboardElement(LookerNode):
     query: Optional[Query]
+    result_maker: Optional[ResultMaker]
 
 
 class Constraint(str, Enum):
     """ """
 
     foreign_key = "f"
     primary_key = "p"
@@ -103,23 +108,21 @@
 
 
 class Dashboard(LookerNode):
     """ """
 
     name: str = Field(alias="id")
     display_name: str = Field(alias="title")
-    dashboard_elements: Optional[List[DashboardElement]] = Field(
-        alias="dashboard_elements"
-    )
+    dashboard_elements: Optional[List[DashboardElement]]
 
     def get_query(self, element):
         if element.query:
             return element.query
 
-        if element.result_maker.query:
+        if element.result_maker and element.result_maker.query:
             return element.result_maker.query
 
     def get_fields(self):
         """ """
 
         fields = []
```

### Comparing `grai_source_looker-0.0.1a2/PKG-INFO` & `grai_source_looker-0.0.1a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-looker
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
```

