# Comparing `tmp/deployment_package-0.0.1.tar.gz` & `tmp/deployment_package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deployment_package-0.0.1.tar", last modified: Thu Aug  3 16:27:25 2023, max compression
+gzip compressed data, was "deployment_package-0.0.2.tar", last modified: Thu Aug  3 19:06:31 2023, max compression
```

## Comparing `deployment_package-0.0.1.tar` & `deployment_package-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 16:27:25.475969 deployment_package-0.0.1/
--rw-rw-rw-   0        0        0      435 2023-08-03 16:27:25.475969 deployment_package-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 16:27:25.461809 deployment_package-0.0.1/app/
--rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.1/app/README.md
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.1/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 16:27:25.467413 deployment_package-0.0.1/app/deployment_package.egg-info/
--rw-rw-rw-   0        0        0      435 2023-08-03 16:27:25.000000 deployment_package-0.0.1/app/deployment_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-08-03 16:27:25.000000 deployment_package-0.0.1/app/deployment_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 16:27:25.000000 deployment_package-0.0.1/app/deployment_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-03 16:27:25.000000 deployment_package-0.0.1/app/deployment_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-03 16:27:25.000000 deployment_package-0.0.1/app/deployment_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 16:27:25.468409 deployment_package-0.0.1/app/deployment_utils/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.1/app/deployment_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 16:27:25.470410 deployment_package-0.0.1/app/deployment_utils/src/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.1/app/deployment_utils/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 16:27:25.472525 deployment_package-0.0.1/app/deployment_utils/src/__pycache__/
--rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.1/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.1/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
--rw-rw-rw-   0        0        0     2020 2023-08-03 16:16:43.000000 deployment_package-0.0.1/app/deployment_utils/src/preprocessing.py
--rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.1/app/deployment_utils/src/schemas.py
-drwxrwxrwx   0        0        0        0 2023-08-03 16:27:25.474962 deployment_package-0.0.1/app/deployment_utils/test/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.1/app/deployment_utils/test/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-08-03 16:16:43.000000 deployment_package-0.0.1/app/deployment_utils/test/test.pkl
--rw-rw-rw-   0        0        0     1593 2023-08-03 16:16:43.000000 deployment_package-0.0.1/app/deployment_utils/test/testing.py
--rw-rw-rw-   0        0        0       42 2023-08-03 16:27:25.475969 deployment_package-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-08-03 16:18:30.000000 deployment_package-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.456105 deployment_package-0.0.2/
+-rw-rw-rw-   0        0        0      435 2023-08-03 19:06:31.454932 deployment_package-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.441043 deployment_package-0.0.2/app/
+-rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/README.md
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.446071 deployment_package-0.0.2/app/deployment_package.egg-info/
+-rw-rw-rw-   0        0        0      435 2023-08-03 19:06:31.000000 deployment_package-0.0.2/app/deployment_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-08-03 19:06:31.000000 deployment_package-0.0.2/app/deployment_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 19:06:31.000000 deployment_package-0.0.2/app/deployment_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-03 19:06:31.000000 deployment_package-0.0.2/app/deployment_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 19:06:31.000000 deployment_package-0.0.2/app/deployment_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.446071 deployment_package-0.0.2/app/deployment_utils/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.2/app/deployment_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.449392 deployment_package-0.0.2/app/deployment_utils/src/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.450401 deployment_package-0.0.2/app/deployment_utils/src/__pycache__/
+-rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.2/app/deployment_utils/src/preprocessing.py
+-rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/src/schemas.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:06:31.453920 deployment_package-0.0.2/app/deployment_utils/test/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/test/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/test/test.pkl
+-rw-rw-rw-   0        0        0     1593 2023-08-03 16:16:43.000000 deployment_package-0.0.2/app/deployment_utils/test/testing.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 19:06:31.456105 deployment_package-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-08-03 19:03:59.000000 deployment_package-0.0.2/setup.py
```

### Comparing `deployment_package-0.0.1/app/deployment_package.egg-info/SOURCES.txt` & `deployment_package-0.0.2/app/deployment_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.1/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc` & `deployment_package-0.0.2/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.1/app/deployment_utils/src/preprocessing.py` & `deployment_package-0.0.2/app/deployment_utils/src/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def dropColumns(self, inputData:pd.DataFrame):
         return inputData.drop(labels=["TBG", "referral_source", "TBG_measured", "FTI_measured", "query_on_thyroxine", "query_hyperthyroid", 
                             "query_hypothyroid", "T4U_measured", "TT4_measured", "T3_measured", "TSH_measured"], 
                             axis=1)
     
     def preprocessInput(self, inputData:pd.DataFrame):
         cleaned_input = self.dropColumns(inputData)
-        encoder, scaler = self.loadTransformers(self.ENCODER_PATH, self.SCALER_PATH)
+        encoder, scaler = self.loadTransformers()
         numeric_features = cleaned_input.select_dtypes("number").columns
         categorical_features = cleaned_input.select_dtypes(object).columns
 
         numericProcessed = pd.DataFrame(data=scaler.transform(cleaned_input[numeric_features]),
                                         columns=numeric_features)
 
         categoricalPreprocessed = pd.DataFrame(encoder.transform(cleaned_input[categorical_features]).toarray(),
```

### Comparing `deployment_package-0.0.1/app/deployment_utils/src/schemas.py` & `deployment_package-0.0.2/app/deployment_utils/src/schemas.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.1/app/deployment_utils/test/test.pkl` & `deployment_package-0.0.2/app/deployment_utils/test/test.pkl`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.1/app/deployment_utils/test/testing.py` & `deployment_package-0.0.2/app/deployment_utils/test/testing.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.1/setup.py` & `deployment_package-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import find_packages, setup
 
+
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="deployment_package",
-    version="0.0.1",
+    version="0.0.2",
     description="Package for preprocessing functions used during Model Deployment module",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/davidbognar201/Model_deployment_package",
     author="David Bognar",
```

