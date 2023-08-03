# Comparing `tmp/deployment_package-0.0.7.tar.gz` & `tmp/deployment_package-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deployment_package-0.0.7.tar", last modified: Thu Aug  3 19:43:56 2023, max compression
+gzip compressed data, was "deployment_package-0.0.8.tar", last modified: Thu Aug  3 20:04:05 2023, max compression
```

## Comparing `deployment_package-0.0.7.tar` & `deployment_package-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 19:43:56.055656 deployment_package-0.0.7/
--rw-rw-rw-   0        0        0      435 2023-08-03 19:43:56.055162 deployment_package-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 19:43:56.041874 deployment_package-0.0.7/app/
--rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.7/app/README.md
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.7/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:43:56.046746 deployment_package-0.0.7/app/deployment_package.egg-info/
--rw-rw-rw-   0        0        0      435 2023-08-03 19:43:55.000000 deployment_package-0.0.7/app/deployment_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-08-03 19:43:55.000000 deployment_package-0.0.7/app/deployment_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 19:43:55.000000 deployment_package-0.0.7/app/deployment_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-03 19:43:55.000000 deployment_package-0.0.7/app/deployment_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-03 19:43:55.000000 deployment_package-0.0.7/app/deployment_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 19:43:56.046746 deployment_package-0.0.7/app/deployment_utils/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.7/app/deployment_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:43:56.049906 deployment_package-0.0.7/app/deployment_utils/src/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.7/app/deployment_utils/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:43:56.051079 deployment_package-0.0.7/app/deployment_utils/src/__pycache__/
--rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.7/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.7/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
--rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.7/app/deployment_utils/src/preprocessing.py
--rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.7/app/deployment_utils/src/schemas.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:43:56.054084 deployment_package-0.0.7/app/deployment_utils/test/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.7/app/deployment_utils/test/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-08-03 16:16:43.000000 deployment_package-0.0.7/app/deployment_utils/test/test.pkl
--rw-rw-rw-   0        0        0     1748 2023-08-03 19:43:38.000000 deployment_package-0.0.7/app/deployment_utils/test/testing.py
--rw-rw-rw-   0        0        0       42 2023-08-03 19:43:56.055656 deployment_package-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-08-03 19:43:50.000000 deployment_package-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.271022 deployment_package-0.0.8/
+-rw-rw-rw-   0        0        0      435 2023-08-03 20:04:05.271022 deployment_package-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.259032 deployment_package-0.0.8/app/
+-rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/README.md
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.263125 deployment_package-0.0.8/app/deployment_package.egg-info/
+-rw-rw-rw-   0        0        0      435 2023-08-03 20:04:04.000000 deployment_package-0.0.8/app/deployment_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-08-03 20:04:05.000000 deployment_package-0.0.8/app/deployment_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 20:04:04.000000 deployment_package-0.0.8/app/deployment_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-03 20:04:04.000000 deployment_package-0.0.8/app/deployment_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 20:04:04.000000 deployment_package-0.0.8/app/deployment_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.264125 deployment_package-0.0.8/app/deployment_utils/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.8/app/deployment_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.266124 deployment_package-0.0.8/app/deployment_utils/src/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/deployment_utils/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.268406 deployment_package-0.0.8/app/deployment_utils/src/__pycache__/
+-rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.8/app/deployment_utils/src/preprocessing.py
+-rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/deployment_utils/src/schemas.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.270017 deployment_package-0.0.8/app/deployment_utils/test/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/deployment_utils/test/__init__.py
+-rw-rw-rw-   0        0        0     1846 2023-08-03 19:56:54.000000 deployment_package-0.0.8/app/deployment_utils/test/testing.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 20:04:05.272122 deployment_package-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-08-03 20:01:02.000000 deployment_package-0.0.8/setup.py
```

### Comparing `deployment_package-0.0.7/app/deployment_package.egg-info/SOURCES.txt` & `deployment_package-0.0.8/app/deployment_package.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 app/deployment_utils/__init__.py
 app/deployment_utils/src/__init__.py
 app/deployment_utils/src/preprocessing.py
 app/deployment_utils/src/schemas.py
 app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
 app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
 app/deployment_utils/test/__init__.py
-app/deployment_utils/test/test.pkl
 app/deployment_utils/test/testing.py
```

### Comparing `deployment_package-0.0.7/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc` & `deployment_package-0.0.8/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.7/app/deployment_utils/src/preprocessing.py` & `deployment_package-0.0.8/app/deployment_utils/src/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.7/app/deployment_utils/src/schemas.py` & `deployment_package-0.0.8/app/deployment_utils/src/schemas.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.7/app/deployment_utils/test/testing.py` & `deployment_package-0.0.8/app/deployment_utils/test/testing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest import TestCase, mock 
 import deployment_utils.src.preprocessing as prep
 import pandas as pd
+import os
 
 class DataPreprocessTest(TestCase):
     def test_drop_columns_function(self):
         instance = prep.DataPreprocess("","","")
         data = pd.DataFrame(columns=["age","sex","on_thyroxine","query_on_thyroxine","on_antithyroid_medication","sick","pregnant","thyroid_surgery","I131_treatment",
                                             "query_hypothyroid","query_hyperthyroid","lithium","goitre","tumor","hypopituitary","psych","TSH_measured","TSH","T3_measured","T3",
                                             "TT4_measured","TT4","T4U_measured","T4U","FTI_measured","FTI","TBG_measured","TBG","referral_source","Class"])
@@ -16,14 +17,16 @@
 
     def test_wrong_artifact_path(self):
         instance = prep.DataPreprocess("wrongPath","wrongPath","wrongPath")
         with self.assertRaises(FileNotFoundError):
             encoder, scaler = instance.loadTransformers()
 
     def test_good_artifact_path(self):
-        PATH = "app/deployment_utils/test/test.pkl"
-        instance = prep.DataPreprocess(model_path=PATH,
-                                       encoder_path=PATH,
-                                       scaler_path=PATH)
+        this_dir, this_filename = os.path.split(__file__)
+        DATA_PATH = os.path.join(this_dir, "data", "test.pkl")
+
+        instance = prep.DataPreprocess(model_path=DATA_PATH,
+                                       encoder_path=DATA_PATH,
+                                       scaler_path=DATA_PATH)
         scaler, encoder = instance.loadTransformers()
         self.assertIsNotNone(scaler)
         self.assertIsNotNone(encoder)
```

### Comparing `deployment_package-0.0.7/setup.py` & `deployment_package-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="deployment_package",
-    version="0.0.7",
+    version="0.0.8",
     description="Package for preprocessing functions used during Model Deployment module",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/davidbognar201/Model_deployment_package",
     author="David Bognar",
     author_email="david.bognar@gmail.com",
     install_requires=["bson", "pandas", "scikit-learn", "numpy", "pydantic"],
     extras_require={
         "dev": ["pytest", "twine"],
     },
     python_requires=">=3.8",
+    include_package_data=True
 )
```

