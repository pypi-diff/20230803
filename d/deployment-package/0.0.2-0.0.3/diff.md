# Comparing `tmp/deployment_package-0.0.2.tar.gz` & `tmp/deployment_package-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deployment_package-0.0.2.tar", last modified: Thu Aug  3 19:06:31 2023, max compression
+gzip compressed data, was "deployment_package-0.0.3.tar", last modified: Thu Aug  3 19:24:18 2023, max compression
```

## Comparing `deployment_package-0.0.2.tar` & `deployment_package-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.456105 deployment_package-0.0.2/
--rw-rw-rw-   0        0        0      435 2023-08-03 19:06:31.454932 deployment_package-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.441043 deployment_package-0.0.2/app/
--rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/README.md
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.446071 deployment_package-0.0.2/app/deployment_package.egg-info/
--rw-rw-rw-   0        0        0      435 2023-08-03 19:06:31.000000 deployment_package-0.0.2/app/deployment_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-08-03 19:06:31.000000 deployment_package-0.0.2/app/deployment_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 19:06:31.000000 deployment_package-0.0.2/app/deployment_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-03 19:06:31.000000 deployment_package-0.0.2/app/deployment_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-03 19:06:31.000000 deployment_package-0.0.2/app/deployment_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.446071 deployment_package-0.0.2/app/deployment_utils/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.2/app/deployment_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.449392 deployment_package-0.0.2/app/deployment_utils/src/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.450401 deployment_package-0.0.2/app/deployment_utils/src/__pycache__/
--rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
--rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.2/app/deployment_utils/src/preprocessing.py
--rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/src/schemas.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.453920 deployment_package-0.0.2/app/deployment_utils/test/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/test/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/test/test.pkl
--rw-rw-rw-   0        0        0     1593 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/test/testing.py
--rw-rw-rw-   0        0        0       42 2023-08-03 19:06:31.456105 deployment_package-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-08-03 19:03:59.000000 deployment_package-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.294216 deployment_package-0.0.3/
+-rw-rw-rw-   0        0        0      435 2023-08-03 19:24:18.294216 deployment_package-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.281668 deployment_package-0.0.3/app/
+-rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/README.md
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.285723 deployment_package-0.0.3/app/deployment_package.egg-info/
+-rw-rw-rw-   0        0        0      435 2023-08-03 19:24:18.000000 deployment_package-0.0.3/app/deployment_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-08-03 19:24:18.000000 deployment_package-0.0.3/app/deployment_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 19:24:18.000000 deployment_package-0.0.3/app/deployment_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-03 19:24:18.000000 deployment_package-0.0.3/app/deployment_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 19:24:18.000000 deployment_package-0.0.3/app/deployment_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.286621 deployment_package-0.0.3/app/deployment_utils/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.3/app/deployment_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.288635 deployment_package-0.0.3/app/deployment_utils/src/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.290926 deployment_package-0.0.3/app/deployment_utils/src/__pycache__/
+-rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.3/app/deployment_utils/src/preprocessing.py
+-rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/src/schemas.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.292929 deployment_package-0.0.3/app/deployment_utils/test/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/test/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/test/test.pkl
+-rw-rw-rw-   0        0        0     1610 2023-08-03 19:23:46.000000 deployment_package-0.0.3/app/deployment_utils/test/testing.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 19:24:18.294216 deployment_package-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-08-03 19:24:09.000000 deployment_package-0.0.3/setup.py
```

### Comparing `deployment_package-0.0.2/app/deployment_package.egg-info/SOURCES.txt` & `deployment_package-0.0.3/app/deployment_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.2/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc` & `deployment_package-0.0.3/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.2/app/deployment_utils/src/preprocessing.py` & `deployment_package-0.0.3/app/deployment_utils/src/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.2/app/deployment_utils/src/schemas.py` & `deployment_package-0.0.3/app/deployment_utils/src/schemas.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.2/app/deployment_utils/test/test.pkl` & `deployment_package-0.0.3/app/deployment_utils/test/test.pkl`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.2/app/deployment_utils/test/testing.py` & `deployment_package-0.0.3/app/deployment_utils/test/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from unittest import TestCase, mock 
-import src.preprocessing as prep
+import deployment_utils.src.preprocessing as prep
 import pandas as pd
 
 class DataPreprocessTest(TestCase):
     def test_drop_columns_function(self):
         instance = prep.DataPreprocess("","","")
         data = pd.DataFrame(columns=["age","sex","on_thyroxine","query_on_thyroxine","on_antithyroid_medication","sick","pregnant","thyroid_surgery","I131_treatment",
                                             "query_hypothyroid","query_hyperthyroid","lithium","goitre","tumor","hypopituitary","psych","TSH_measured","TSH","T3_measured","T3",
```

### Comparing `deployment_package-0.0.2/setup.py` & `deployment_package-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="deployment_package",
-    version="0.0.2",
+    version="0.0.3",
     description="Package for preprocessing functions used during Model Deployment module",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/davidbognar201/Model_deployment_package",
     author="David Bognar",
```

