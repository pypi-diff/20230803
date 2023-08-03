# Comparing `tmp/deployment_package-0.0.4.tar.gz` & `tmp/deployment_package-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deployment_package-0.0.4.tar", last modified: Thu Aug  3 19:33:35 2023, max compression
+gzip compressed data, was "deployment_package-0.0.5.tar", last modified: Thu Aug  3 19:37:12 2023, max compression
```

## Comparing `deployment_package-0.0.4.tar` & `deployment_package-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.500661 deployment_package-0.0.4/
--rw-rw-rw-   0        0        0      435 2023-08-03 19:33:35.499664 deployment_package-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.484632 deployment_package-0.0.4/app/
--rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/README.md
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.489969 deployment_package-0.0.4/app/deployment_package.egg-info/
--rw-rw-rw-   0        0        0      435 2023-08-03 19:33:35.000000 deployment_package-0.0.4/app/deployment_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-08-03 19:33:35.000000 deployment_package-0.0.4/app/deployment_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 19:33:35.000000 deployment_package-0.0.4/app/deployment_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-03 19:33:35.000000 deployment_package-0.0.4/app/deployment_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-03 19:33:35.000000 deployment_package-0.0.4/app/deployment_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.491013 deployment_package-0.0.4/app/deployment_utils/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.4/app/deployment_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.492864 deployment_package-0.0.4/app/deployment_utils/src/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.495785 deployment_package-0.0.4/app/deployment_utils/src/__pycache__/
--rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
--rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.4/app/deployment_utils/src/preprocessing.py
--rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/src/schemas.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.498655 deployment_package-0.0.4/app/deployment_utils/test/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/test/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/test/test.pkl
--rw-rw-rw-   0        0        0     1744 2023-08-03 19:33:15.000000 deployment_package-0.0.4/app/deployment_utils/test/testing.py
--rw-rw-rw-   0        0        0       42 2023-08-03 19:33:35.500661 deployment_package-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-08-03 19:33:30.000000 deployment_package-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:37:12.064776 deployment_package-0.0.5/
+-rw-rw-rw-   0        0        0      435 2023-08-03 19:37:12.064776 deployment_package-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 19:37:12.051891 deployment_package-0.0.5/app/
+-rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.5/app/README.md
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.5/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:37:12.056406 deployment_package-0.0.5/app/deployment_package.egg-info/
+-rw-rw-rw-   0        0        0      435 2023-08-03 19:37:11.000000 deployment_package-0.0.5/app/deployment_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-08-03 19:37:11.000000 deployment_package-0.0.5/app/deployment_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 19:37:11.000000 deployment_package-0.0.5/app/deployment_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-03 19:37:11.000000 deployment_package-0.0.5/app/deployment_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 19:37:11.000000 deployment_package-0.0.5/app/deployment_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 19:37:12.057402 deployment_package-0.0.5/app/deployment_utils/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.5/app/deployment_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:37:12.058766 deployment_package-0.0.5/app/deployment_utils/src/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.5/app/deployment_utils/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:37:12.061276 deployment_package-0.0.5/app/deployment_utils/src/__pycache__/
+-rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.5/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.5/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.5/app/deployment_utils/src/preprocessing.py
+-rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.5/app/deployment_utils/src/schemas.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:37:12.063768 deployment_package-0.0.5/app/deployment_utils/test/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.5/app/deployment_utils/test/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-08-03 16:16:43.000000 deployment_package-0.0.5/app/deployment_utils/test/test.pkl
+-rw-rw-rw-   0        0        0     1745 2023-08-03 19:36:34.000000 deployment_package-0.0.5/app/deployment_utils/test/testing.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 19:37:12.065912 deployment_package-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-08-03 19:37:07.000000 deployment_package-0.0.5/setup.py
```

### Comparing `deployment_package-0.0.4/app/deployment_package.egg-info/SOURCES.txt` & `deployment_package-0.0.5/app/deployment_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.4/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc` & `deployment_package-0.0.5/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.4/app/deployment_utils/src/preprocessing.py` & `deployment_package-0.0.5/app/deployment_utils/src/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.4/app/deployment_utils/src/schemas.py` & `deployment_package-0.0.5/app/deployment_utils/src/schemas.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.4/app/deployment_utils/test/test.pkl` & `deployment_package-0.0.5/app/deployment_utils/test/test.pkl`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.4/app/deployment_utils/test/testing.py` & `deployment_package-0.0.5/app/deployment_utils/test/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 
     def test_wrong_artifact_path(self):
         instance = prep.DataPreprocess("wrongPath","wrongPath","wrongPath")
         with self.assertRaises(FileNotFoundError):
             encoder, scaler = instance.loadTransformers()
 
     def test_good_artifact_path(self):
-        PATH = "deployment_utils/test/test.pkl"
+        PATH = "/deployment_utils/test/test.pkl"
         instance = prep.DataPreprocess(model_path=PATH,
                                        encoder_path=PATH,
                                        scaler_path=PATH)
         scaler, encoder = instance.loadTransformers()
         self.assertIsNotNone(scaler)
         self.assertIsNotNone(encoder)
```

### Comparing `deployment_package-0.0.4/setup.py` & `deployment_package-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="deployment_package",
-    version="0.0.4",
+    version="0.0.5",
     description="Package for preprocessing functions used during Model Deployment module",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/davidbognar201/Model_deployment_package",
     author="David Bognar",
```

