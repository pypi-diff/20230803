# Comparing `tmp/parsagon-0.9.1.tar.gz` & `tmp/parsagon-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.9.1.tar", last modified: Wed Aug  2 17:54:10 2023, max compression
+gzip compressed data, was "parsagon-0.9.2.tar", last modified: Wed Aug  2 18:41:38 2023, max compression
```

## Comparing `parsagon-0.9.1.tar` & `parsagon-0.9.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 17:54:10.662508 parsagon-0.9.1/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-02 17:54:10.662121 parsagon-0.9.1/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.9.1/README.md
--rw-r--r--   0 amsuh    (10002)    18010     1048 2023-08-02 09:54:56.000000 parsagon-0.9.1/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-08-02 17:54:10.662627 parsagon-0.9.1/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 17:54:10.642804 parsagon-0.9.1/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.1/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 17:54:10.650359 parsagon-0.9.1/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     5590 2023-08-02 06:48:17.000000 parsagon-0.9.1/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.9.1/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/exceptions.py
--rw-r--r--   0 amsuh    (10002)    18010    15535 2023-08-02 10:33:44.000000 parsagon-0.9.1/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     9218 2023-08-02 10:12:43.000000 parsagon-0.9.1/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.9.1/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 17:54:10.661292 parsagon-0.9.1/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.1/src/parsagon/tests/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/tests/api_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/tests/cli_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/tests/conftest.py
--rw-r--r--   0 amsuh    (10002)    18010      645 2023-07-30 02:55:30.000000 parsagon-0.9.1/src/parsagon/tests/test_executor.py
--rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/tests/test_invalid_args.py
--rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.9.1/src/parsagon/tests/test_pipeline_operations.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 17:54:10.656357 parsagon-0.9.1/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      682 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      263 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-08-02 17:54:10.000000 parsagon-0.9.1/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 18:41:38.234100 parsagon-0.9.2/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-02 18:41:38.233772 parsagon-0.9.2/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.9.2/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1158 2023-08-02 18:41:22.000000 parsagon-0.9.2/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-08-02 18:41:38.234214 parsagon-0.9.2/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 18:41:38.217708 parsagon-0.9.2/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.2/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 18:41:38.225687 parsagon-0.9.2/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.9.2/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     5590 2023-08-02 06:48:17.000000 parsagon-0.9.2/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.9.2/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.9.2/src/parsagon/exceptions.py
+-rw-r--r--   0 amsuh    (10002)    18010    15535 2023-08-02 10:33:44.000000 parsagon-0.9.2/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010    14448 2023-08-02 10:31:32.000000 parsagon-0.9.2/src/parsagon/highlights.js
+-rw-r--r--   0 amsuh    (10002)    18010     9218 2023-08-02 10:12:43.000000 parsagon-0.9.2/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.9.2/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 18:41:38.233120 parsagon-0.9.2/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.2/src/parsagon/tests/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.9.2/src/parsagon/tests/api_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.9.2/src/parsagon/tests/cli_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.9.2/src/parsagon/tests/conftest.py
+-rw-r--r--   0 amsuh    (10002)    18010      645 2023-07-30 02:55:30.000000 parsagon-0.9.2/src/parsagon/tests/test_executor.py
+-rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.9.2/src/parsagon/tests/test_invalid_args.py
+-rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.9.2/src/parsagon/tests/test_pipeline_operations.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-02 18:41:38.228729 parsagon-0.9.2/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-02 18:41:38.000000 parsagon-0.9.2/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      709 2023-08-02 18:41:38.000000 parsagon-0.9.2/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-08-02 18:41:38.000000 parsagon-0.9.2/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-08-02 18:41:38.000000 parsagon-0.9.2/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      263 2023-08-02 18:41:38.000000 parsagon-0.9.2/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010        9 2023-08-02 18:41:38.000000 parsagon-0.9.2/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.9.1/PKG-INFO` & `parsagon-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.9.1
+Version: 0.9.2
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.9.1/README.md` & `parsagon-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/pyproject.toml` & `parsagon-0.9.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+parsagon = ["highlights.js"]
+
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.9.1"
+version = "0.9.2"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
```

### Comparing `parsagon-0.9.1/src/parsagon/api.py` & `parsagon-0.9.2/src/parsagon/api.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/src/parsagon/custom_function.py` & `parsagon-0.9.2/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/src/parsagon/exceptions.py` & `parsagon-0.9.2/src/parsagon/exceptions.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/src/parsagon/executor.py` & `parsagon-0.9.2/src/parsagon/executor.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/src/parsagon/main.py` & `parsagon-0.9.2/src/parsagon/main.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/src/parsagon/settings.py` & `parsagon-0.9.2/src/parsagon/settings.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/src/parsagon/tests/api_mocks.py` & `parsagon-0.9.2/src/parsagon/tests/api_mocks.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/src/parsagon/tests/test_executor.py` & `parsagon-0.9.2/src/parsagon/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/src/parsagon/tests/test_invalid_args.py` & `parsagon-0.9.2/src/parsagon/tests/test_invalid_args.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/src/parsagon/tests/test_pipeline_operations.py` & `parsagon-0.9.2/src/parsagon/tests/test_pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.1/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.9.2/src/parsagon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.9.1
+Version: 0.9.2
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.9.1/src/parsagon.egg-info/SOURCES.txt` & `parsagon-0.9.2/src/parsagon.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 src/__init__.py
 src/parsagon/__init__.py
 src/parsagon/api.py
 src/parsagon/custom_function.py
 src/parsagon/exceptions.py
 src/parsagon/executor.py
+src/parsagon/highlights.js
 src/parsagon/main.py
 src/parsagon/settings.py
 src/parsagon.egg-info/PKG-INFO
 src/parsagon.egg-info/SOURCES.txt
 src/parsagon.egg-info/dependency_links.txt
 src/parsagon.egg-info/entry_points.txt
 src/parsagon.egg-info/requires.txt
```

