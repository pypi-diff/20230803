# Comparing `tmp/easycloudapi-0.0.1.tar.gz` & `tmp/easycloudapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycloudapi-0.0.1.tar", last modified: Thu Aug  3 20:44:40 2023, max compression
+gzip compressed data, was "easycloudapi-0.0.2.tar", last modified: Thu Aug  3 20:59:58 2023, max compression
```

## Comparing `easycloudapi-0.0.1.tar` & `easycloudapi-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 20:44:40.688691 easycloudapi-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-08-03 14:52:52.000000 easycloudapi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3848 2023-08-03 20:44:40.689700 easycloudapi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2087 2023-08-03 19:35:40.000000 easycloudapi-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-08-03 17:30:54.000000 easycloudapi-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       30 2023-08-03 15:40:15.000000 easycloudapi-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      883 2023-08-03 20:44:40.694255 easycloudapi-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-03 20:44:40.579563 easycloudapi-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 20:44:40.611725 easycloudapi-0.0.1/src/easycloudapi/
--rw-rw-rw-   0        0        0        0 2023-08-03 17:04:26.000000 easycloudapi-0.0.1/src/easycloudapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:44:40.665605 easycloudapi-0.0.1/src/easycloudapi/gcp/
--rw-rw-rw-   0        0        0        0 2023-08-03 17:04:12.000000 easycloudapi-0.0.1/src/easycloudapi/gcp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:44:40.668555 easycloudapi-0.0.1/src/easycloudapi/generic/
--rw-rw-rw-   0        0        0        0 2023-08-03 17:04:26.000000 easycloudapi-0.0.1/src/easycloudapi/generic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:44:40.655641 easycloudapi-0.0.1/src/easycloudapi.egg-info/
--rw-rw-rw-   0        0        0     3848 2023-08-03 20:44:40.000000 easycloudapi-0.0.1/src/easycloudapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-08-03 20:44:40.000000 easycloudapi-0.0.1/src/easycloudapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 20:44:40.000000 easycloudapi-0.0.1/src/easycloudapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-08-03 20:44:40.000000 easycloudapi-0.0.1/src/easycloudapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-03 20:44:40.000000 easycloudapi-0.0.1/src/easycloudapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 20:44:40.683399 easycloudapi-0.0.1/tests/
--rw-rw-rw-   0        0        0      432 2023-08-03 20:41:39.000000 easycloudapi-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:59:58.378729 easycloudapi-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-08-03 14:52:52.000000 easycloudapi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3904 2023-08-03 20:59:58.379887 easycloudapi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2143 2023-08-03 20:48:31.000000 easycloudapi-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-08-03 17:30:54.000000 easycloudapi-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       30 2023-08-03 15:40:15.000000 easycloudapi-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0      883 2023-08-03 20:59:58.385552 easycloudapi-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 20:59:58.293049 easycloudapi-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 20:59:58.323641 easycloudapi-0.0.2/src/easycloudapi/
+-rw-rw-rw-   0        0        0        0 2023-08-03 17:04:26.000000 easycloudapi-0.0.2/src/easycloudapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:59:58.368187 easycloudapi-0.0.2/src/easycloudapi/gcp/
+-rw-rw-rw-   0        0        0        0 2023-08-03 17:04:12.000000 easycloudapi-0.0.2/src/easycloudapi/gcp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:59:58.372425 easycloudapi-0.0.2/src/easycloudapi/generic/
+-rw-rw-rw-   0        0        0        0 2023-08-03 17:04:26.000000 easycloudapi-0.0.2/src/easycloudapi/generic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:59:58.363684 easycloudapi-0.0.2/src/easycloudapi.egg-info/
+-rw-rw-rw-   0        0        0     3904 2023-08-03 20:59:58.000000 easycloudapi-0.0.2/src/easycloudapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-08-03 20:59:58.000000 easycloudapi-0.0.2/src/easycloudapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 20:59:58.000000 easycloudapi-0.0.2/src/easycloudapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-08-03 20:59:58.000000 easycloudapi-0.0.2/src/easycloudapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-03 20:59:58.000000 easycloudapi-0.0.2/src/easycloudapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 20:59:58.375902 easycloudapi-0.0.2/tests/
+-rw-rw-rw-   0        0        0      430 2023-08-03 20:46:27.000000 easycloudapi-0.0.2/tests/test.py
```

### Comparing `easycloudapi-0.0.1/LICENSE` & `easycloudapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easycloudapi-0.0.1/PKG-INFO` & `easycloudapi-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: easycloudapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Providing utility functions to help other python developers
 Home-page: https://github.com/easycloudapi/python_utility
 Author: Indranil Pal
 Author-email: info.easycloudapi@gmail.com
 Project-URL: Bug Tracker, https://github.com/easycloudapi/python_utility/issues
 Project-URL: repository, https://github.com/easycloudapi/python_utility
 Keywords: utility,gcp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `python_utility`
-The `python_utility` is a simple uitility to provide ease of developing experience for any Python Applications.
+# easycloudapi
+The `easycloudapi` is a simple uitility to provide ease of developing experience for any Python Applications.
 
 
-## Info:
-1. Version: 1.0.0
+## Functionality Availaible:
+1. Generate Date Dimension
+2. Generate Bigquery Schema from Json
 
 ## Code Samples:
 
 ### Generate Bigquery Schema-
 1. You can directly pass json/dict object to the `generate_bq_schema` method
     ```python
-    from python_utility.gcp.bigquery.bigquery_schema import BigquerySchema
+    from easycloudapi.gcp.bigquery.bigquery_schema import BigquerySchema
 
     sample_json = {
         "name": "Danilo",
         "age": 32,
         "date_joined": "2020-11-05",
         "location": {"country": "United Kingdom", "city": "London"},
         "years_active": [2020, 2021, 2022],
@@ -47,29 +48,29 @@
 
     print(f"out_generate_bq_schema:\n{out_generate_bq_schema}")
     ```
 
 2. You can also convert the json file into json/dict object and pass to the `generate_bq_schema` method
     ```python
     import json
-    from python_utility.gcp.bigquery.bigquery_schema import BigquerySchema
+    from easycloudapi.gcp.bigquery.bigquery_schema import BigquerySchema
 
 
     bq_schema_obj = BigquerySchema()
     with open("tests//test_data//sample_json_01.json") as json_file:
         sample_dict = json.load(json_file)
 
     out_generate_bq_schema = bq_schema_obj.generate_bq_schema(data=sample_dict)
     print(out_generate_bq_schema)
     ```
 
 ### Date Functionality-
 1. Generate Date Dimension
     ```python
-    from python_utility.generic.datetime.generate_date_dimention import generate_date_dimension
+    from easycloudapi.generic.datetime.generate_date_dimention import generate_date_dimension
 
     out1 = generate_date_dimension(start_date="2023\\08\\01", end_date="2023\\08\\03")
     print(f"out1: {out1}")
     out2 = generate_date_dimension(start_date="2023/08/01", end_date="2023/08/03")
     print(f"out2: {out2}")
     out3 = generate_date_dimension(start_date="2023-08-01", end_date="2023-08-03")
     print(f"out3: {out3}")
```

### Comparing `easycloudapi-0.0.1/README.md` & `easycloudapi-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# `python_utility`
-The `python_utility` is a simple uitility to provide ease of developing experience for any Python Applications.
+# easycloudapi
+The `easycloudapi` is a simple uitility to provide ease of developing experience for any Python Applications.
 
 
-## Info:
-1. Version: 1.0.0
+## Functionality Availaible:
+1. Generate Date Dimension
+2. Generate Bigquery Schema from Json
 
 ## Code Samples:
 
 ### Generate Bigquery Schema-
 1. You can directly pass json/dict object to the `generate_bq_schema` method
     ```python
-    from python_utility.gcp.bigquery.bigquery_schema import BigquerySchema
+    from easycloudapi.gcp.bigquery.bigquery_schema import BigquerySchema
 
     sample_json = {
         "name": "Danilo",
         "age": 32,
         "date_joined": "2020-11-05",
         "location": {"country": "United Kingdom", "city": "London"},
         "years_active": [2020, 2021, 2022],
@@ -30,29 +31,29 @@
 
     print(f"out_generate_bq_schema:\n{out_generate_bq_schema}")
     ```
 
 2. You can also convert the json file into json/dict object and pass to the `generate_bq_schema` method
     ```python
     import json
-    from python_utility.gcp.bigquery.bigquery_schema import BigquerySchema
+    from easycloudapi.gcp.bigquery.bigquery_schema import BigquerySchema
 
 
     bq_schema_obj = BigquerySchema()
     with open("tests//test_data//sample_json_01.json") as json_file:
         sample_dict = json.load(json_file)
 
     out_generate_bq_schema = bq_schema_obj.generate_bq_schema(data=sample_dict)
     print(out_generate_bq_schema)
     ```
 
 ### Date Functionality-
 1. Generate Date Dimension
     ```python
-    from python_utility.generic.datetime.generate_date_dimention import generate_date_dimension
+    from easycloudapi.generic.datetime.generate_date_dimention import generate_date_dimension
 
     out1 = generate_date_dimension(start_date="2023\\08\\01", end_date="2023\\08\\03")
     print(f"out1: {out1}")
     out2 = generate_date_dimension(start_date="2023/08/01", end_date="2023/08/03")
     print(f"out2: {out2}")
     out3 = generate_date_dimension(start_date="2023-08-01", end_date="2023-08-03")
     print(f"out3: {out3}")
```

### Comparing `easycloudapi-0.0.1/setup.cfg` & `easycloudapi-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 6173 7963 6c6f 7564 6170 690d   = easycloudapi.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e31  .version = 0.0.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
 00000030: 0d0a 6175 7468 6f72 203d 2049 6e64 7261  ..author = Indra
 00000040: 6e69 6c20 5061 6c0d 0a61 7574 686f 725f  nil Pal..author_
 00000050: 656d 6169 6c20 3d20 696e 666f 2e65 6173  email = info.eas
 00000060: 7963 6c6f 7564 6170 6940 676d 6169 6c2e  ycloudapi@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2050 726f 7669 6469 6e67 2075 7469   = Providing uti
 00000090: 6c69 7479 2066 756e 6374 696f 6e73 2074  lity functions t
```

### Comparing `easycloudapi-0.0.1/src/easycloudapi.egg-info/PKG-INFO` & `easycloudapi-0.0.2/src/easycloudapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: easycloudapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Providing utility functions to help other python developers
 Home-page: https://github.com/easycloudapi/python_utility
 Author: Indranil Pal
 Author-email: info.easycloudapi@gmail.com
 Project-URL: Bug Tracker, https://github.com/easycloudapi/python_utility/issues
 Project-URL: repository, https://github.com/easycloudapi/python_utility
 Keywords: utility,gcp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# `python_utility`
-The `python_utility` is a simple uitility to provide ease of developing experience for any Python Applications.
+# easycloudapi
+The `easycloudapi` is a simple uitility to provide ease of developing experience for any Python Applications.
 
 
-## Info:
-1. Version: 1.0.0
+## Functionality Availaible:
+1. Generate Date Dimension
+2. Generate Bigquery Schema from Json
 
 ## Code Samples:
 
 ### Generate Bigquery Schema-
 1. You can directly pass json/dict object to the `generate_bq_schema` method
     ```python
-    from python_utility.gcp.bigquery.bigquery_schema import BigquerySchema
+    from easycloudapi.gcp.bigquery.bigquery_schema import BigquerySchema
 
     sample_json = {
         "name": "Danilo",
         "age": 32,
         "date_joined": "2020-11-05",
         "location": {"country": "United Kingdom", "city": "London"},
         "years_active": [2020, 2021, 2022],
@@ -47,29 +48,29 @@
 
     print(f"out_generate_bq_schema:\n{out_generate_bq_schema}")
     ```
 
 2. You can also convert the json file into json/dict object and pass to the `generate_bq_schema` method
     ```python
     import json
-    from python_utility.gcp.bigquery.bigquery_schema import BigquerySchema
+    from easycloudapi.gcp.bigquery.bigquery_schema import BigquerySchema
 
 
     bq_schema_obj = BigquerySchema()
     with open("tests//test_data//sample_json_01.json") as json_file:
         sample_dict = json.load(json_file)
 
     out_generate_bq_schema = bq_schema_obj.generate_bq_schema(data=sample_dict)
     print(out_generate_bq_schema)
     ```
 
 ### Date Functionality-
 1. Generate Date Dimension
     ```python
-    from python_utility.generic.datetime.generate_date_dimention import generate_date_dimension
+    from easycloudapi.generic.datetime.generate_date_dimention import generate_date_dimension
 
     out1 = generate_date_dimension(start_date="2023\\08\\01", end_date="2023\\08\\03")
     print(f"out1: {out1}")
     out2 = generate_date_dimension(start_date="2023/08/01", end_date="2023/08/03")
     print(f"out2: {out2}")
     out3 = generate_date_dimension(start_date="2023-08-01", end_date="2023-08-03")
     print(f"out3: {out3}")
```

