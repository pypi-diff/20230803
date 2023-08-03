# Comparing `tmp/milkstraw-client-0.1.0.tar.gz` & `tmp/milkstraw-client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milkstraw-client-0.1.0.tar", last modified: Tue Aug  1 13:15:22 2023, max compression
+gzip compressed data, was "milkstraw-client-1.0.0.tar", last modified: Thu Aug  3 13:29:52 2023, max compression
```

## Comparing `milkstraw-client-0.1.0.tar` & `milkstraw-client-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)    11357 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/LICENSE
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)    17804 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/PKG-INFO
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     4075 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/README.md
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)      889 2023-08-01 13:10:57.000000 milkstraw-client-0.1.0/pyproject.toml
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)       38 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/setup.cfg
-drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/src/
-drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/src/milkstraw_client/
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)      474 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/src/milkstraw_client/__init__.py
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1969 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/src/milkstraw_client/api_client.py
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1802 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/src/milkstraw_client/generated_data.py
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1709 2023-08-01 12:46:35.000000 milkstraw-client-0.1.0/src/milkstraw_client/model.py
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)     1796 2023-08-01 13:10:57.000000 milkstraw-client-0.1.0/src/milkstraw_client/source_data.py
-drwxrwxr-x   0 ibraheem  (1000) ibraheem  (1000)        0 2023-08-01 13:15:22.403707 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)    17804 2023-08-01 13:15:22.000000 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/PKG-INFO
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)      424 2023-08-01 13:15:22.000000 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)        1 2023-08-01 13:15:22.000000 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)       17 2023-08-01 13:15:22.000000 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/requires.txt
--rw-rw-r--   0 ibraheem  (1000) ibraheem  (1000)       17 2023-08-01 13:15:22.000000 milkstraw-client-0.1.0/src/milkstraw_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:29:52.555563 milkstraw-client-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 13:29:32.000000 milkstraw-client-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-08-03 13:29:52.555563 milkstraw-client-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-08-03 13:29:32.000000 milkstraw-client-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-03 13:29:32.000000 milkstraw-client-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 13:29:52.555563 milkstraw-client-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:29:52.555563 milkstraw-client-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:29:52.555563 milkstraw-client-1.0.0/src/milkstraw_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-03 13:29:32.000000 milkstraw-client-1.0.0/src/milkstraw_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-03 13:29:32.000000 milkstraw-client-1.0.0/src/milkstraw_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-03 13:29:32.000000 milkstraw-client-1.0.0/src/milkstraw_client/generated_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-03 13:29:32.000000 milkstraw-client-1.0.0/src/milkstraw_client/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-03 13:29:32.000000 milkstraw-client-1.0.0/src/milkstraw_client/source_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:29:52.555563 milkstraw-client-1.0.0/src/milkstraw_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-08-03 13:29:52.000000 milkstraw-client-1.0.0/src/milkstraw_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-03 13:29:52.000000 milkstraw-client-1.0.0/src/milkstraw_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 13:29:52.000000 milkstraw-client-1.0.0/src/milkstraw_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 13:29:52.000000 milkstraw-client-1.0.0/src/milkstraw_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 13:29:52.000000 milkstraw-client-1.0.0/src/milkstraw_client.egg-info/top_level.txt
```

### Comparing `milkstraw-client-0.1.0/LICENSE` & `milkstraw-client-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `milkstraw-client-0.1.0/PKG-INFO` & `milkstraw-client-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milkstraw-client
-Version: 0.1.0
+Version: 1.0.0
 Summary: Generate synthetic data with a simple python client for milkstraw.ai
 Author-email: "Milkstraw AI, Inc." <admin@milkstraw.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `milkstraw-client-0.1.0/README.md` & `milkstraw-client-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `milkstraw-client-0.1.0/pyproject.toml` & `milkstraw-client-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "milkstraw-client"
-version = "0.1.0"
+version = "1.0.0"
 description = "Generate synthetic data with a simple python client for milkstraw.ai"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `milkstraw-client-0.1.0/src/milkstraw_client/api_client.py` & `milkstraw-client-1.0.0/src/milkstraw_client/api_client.py`

 * *Files identical despite different names*

### Comparing `milkstraw-client-0.1.0/src/milkstraw_client/generated_data.py` & `milkstraw-client-1.0.0/src/milkstraw_client/generated_data.py`

 * *Files identical despite different names*

### Comparing `milkstraw-client-0.1.0/src/milkstraw_client/model.py` & `milkstraw-client-1.0.0/src/milkstraw_client/source_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,48 +2,51 @@
 
 from typing import Optional
 
 import milkstraw_client
 from milkstraw_client import APIClient
 
 
-class Model:
-    def __init__(self, id: str, name: str, status: str, source_data: str):
+class SourceData:
+    def __init__(self, id: str, name: str, status: str):
         self.id = id
         self.name = name
         self.status = status
-        self.source_data = source_data
 
     def __repr__(self) -> str:
         attributes = ", ".join(f"{key}='{value}'" for key, value in vars(self).items())
         return f"{self.__class__.__name__}({attributes})"
 
     @staticmethod
-    def create(name: str, source_data: str, anonymize_personal_info: Optional[bool] = None) -> Model:
-        url = f"{milkstraw_client.edge_service_url}/models/"
-        json = {"name": name, "sourceDataId": source_data}
-        if anonymize_personal_info is not None:
-            json["anonymizePersonalInfo"] = anonymize_personal_info
-        response = APIClient.request("post", url, json=json)
-        return Model.__parse_dict(response)
+    def upload(
+        name: str,
+        file_path: str,
+        auto_primary_key: Optional[bool] = None,
+        primary_key_column: Optional[str] = None,
+    ) -> SourceData:
+        url = f"{milkstraw_client.edge_service_url}/source-data/"
+        params = {"name": name}
+        if auto_primary_key is not None:
+            params["auto_primary_key"] = auto_primary_key
+        if primary_key_column is not None:
+            params["primary_key_column"] = primary_key_column
+        file_paths = {"file": file_path}
+        response = APIClient.request("post", url, params=params, file_paths=file_paths)
+        return SourceData(**response)
 
     @staticmethod
-    def get(id: str) -> Model:
-        url = f"{milkstraw_client.edge_service_url}/models/{id}"
+    def get(id: str) -> SourceData:
+        url = f"{milkstraw_client.edge_service_url}/source-data/{id}"
         response = APIClient.request("get", url)
-        return Model.__parse_dict(response)
+        return SourceData(**response)
 
     @staticmethod
-    def list() -> list[Model]:
-        url = f"{milkstraw_client.edge_service_url}/models"
+    def list() -> list[SourceData]:
+        url = f"{milkstraw_client.edge_service_url}/source-data"
         response = APIClient.request("get", url)
-        models = [Model.__parse_dict(model_dict) for model_dict in response]
-        return models
+        data = [SourceData(**data_dict) for data_dict in response]
+        return data
 
     @staticmethod
-    def __parse_dict(model_dict: dict[str, str]) -> Model:
-        return Model(
-            id=model_dict["id"],
-            name=model_dict["name"],
-            status=model_dict["status"],
-            source_data=model_dict["sourceData"],
-        )
+    def download(id: str, file_path: str) -> str:
+        url = f"{milkstraw_client.edge_service_url}/source-data/download/{id}"
+        return APIClient.download_file(file_path, url)
```

### Comparing `milkstraw-client-0.1.0/src/milkstraw_client.egg-info/PKG-INFO` & `milkstraw-client-1.0.0/src/milkstraw_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milkstraw-client
-Version: 0.1.0
+Version: 1.0.0
 Summary: Generate synthetic data with a simple python client for milkstraw.ai
 Author-email: "Milkstraw AI, Inc." <admin@milkstraw.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

