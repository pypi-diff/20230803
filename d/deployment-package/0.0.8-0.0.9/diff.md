# Comparing `tmp/deployment_package-0.0.8.tar.gz` & `tmp/deployment_package-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deployment_package-0.0.8.tar", last modified: Thu Aug  3 20:04:05 2023, max compression
+gzip compressed data, was "deployment_package-0.0.9.tar", last modified: Thu Aug  3 20:14:41 2023, max compression
```

## Comparing `deployment_package-0.0.8.tar` & `deployment_package-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.271022 deployment_package-0.0.8/
--rw-rw-rw-   0        0        0      435 2023-08-03 20:04:05.271022 deployment_package-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.259032 deployment_package-0.0.8/app/
--rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/README.md
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.263125 deployment_package-0.0.8/app/deployment_package.egg-info/
--rw-rw-rw-   0        0        0      435 2023-08-03 20:04:04.000000 deployment_package-0.0.8/app/deployment_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-08-03 20:04:05.000000 deployment_package-0.0.8/app/deployment_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 20:04:04.000000 deployment_package-0.0.8/app/deployment_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-03 20:04:04.000000 deployment_package-0.0.8/app/deployment_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-03 20:04:04.000000 deployment_package-0.0.8/app/deployment_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.264125 deployment_package-0.0.8/app/deployment_utils/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.8/app/deployment_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.266124 deployment_package-0.0.8/app/deployment_utils/src/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/deployment_utils/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.268406 deployment_package-0.0.8/app/deployment_utils/src/__pycache__/
--rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
--rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.8/app/deployment_utils/src/preprocessing.py
--rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/deployment_utils/src/schemas.py
-drwxrwxrwx   0        0        0        0 2023-08-03 20:04:05.270017 deployment_package-0.0.8/app/deployment_utils/test/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.8/app/deployment_utils/test/__init__.py
--rw-rw-rw-   0        0        0     1846 2023-08-03 19:56:54.000000 deployment_package-0.0.8/app/deployment_utils/test/testing.py
--rw-rw-rw-   0        0        0       42 2023-08-03 20:04:05.272122 deployment_package-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-08-03 20:01:02.000000 deployment_package-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:14:41.039349 deployment_package-0.0.9/
+-rw-rw-rw-   0        0        0      435 2023-08-03 20:14:41.039349 deployment_package-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 20:14:41.023973 deployment_package-0.0.9/app/
+-rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.9/app/README.md
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.9/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:14:41.025420 deployment_package-0.0.9/app/deployment_utils/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.9/app/deployment_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:14:41.027639 deployment_package-0.0.9/app/deployment_utils/src/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.9/app/deployment_utils/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:14:41.029811 deployment_package-0.0.9/app/deployment_utils/src/__pycache__/
+-rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.9/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.9/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.9/app/deployment_utils/src/preprocessing.py
+-rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.9/app/deployment_utils/src/schemas.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:14:41.032303 deployment_package-0.0.9/app/deployment_utils/test/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.9/app/deployment_utils/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:14:41.032303 deployment_package-0.0.9/app/deployment_utils/test/data/
+-rw-rw-rw-   0        0        0     1099 2023-08-03 16:16:43.000000 deployment_package-0.0.9/app/deployment_utils/test/data/test.pkl
+-rw-rw-rw-   0        0        0     1846 2023-08-03 19:56:54.000000 deployment_package-0.0.9/app/deployment_utils/test/testing.py
+drwxrwxrwx   0        0        0        0 2023-08-03 20:14:41.037401 deployment_package-0.0.9/deployment_package.egg-info/
+-rw-rw-rw-   0        0        0      435 2023-08-03 20:14:40.000000 deployment_package-0.0.9/deployment_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      639 2023-08-03 20:14:40.000000 deployment_package-0.0.9/deployment_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 20:14:40.000000 deployment_package-0.0.9/deployment_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-03 20:14:40.000000 deployment_package-0.0.9/deployment_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-03 20:14:40.000000 deployment_package-0.0.9/deployment_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 20:14:41.039349 deployment_package-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-08-03 20:14:36.000000 deployment_package-0.0.9/setup.py
```

### Comparing `deployment_package-0.0.8/app/deployment_package.egg-info/SOURCES.txt` & `deployment_package-0.0.9/deployment_package.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 setup.py
 app/README.md
 app/__init__.py
-app/deployment_package.egg-info/PKG-INFO
-app/deployment_package.egg-info/SOURCES.txt
-app/deployment_package.egg-info/dependency_links.txt
-app/deployment_package.egg-info/requires.txt
-app/deployment_package.egg-info/top_level.txt
 app/deployment_utils/__init__.py
 app/deployment_utils/src/__init__.py
 app/deployment_utils/src/preprocessing.py
 app/deployment_utils/src/schemas.py
 app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
 app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
 app/deployment_utils/test/__init__.py
-app/deployment_utils/test/testing.py
+app/deployment_utils/test/testing.py
+app/deployment_utils/test/data/test.pkl
+deployment_package.egg-info/PKG-INFO
+deployment_package.egg-info/SOURCES.txt
+deployment_package.egg-info/dependency_links.txt
+deployment_package.egg-info/requires.txt
+deployment_package.egg-info/top_level.txt
```

### Comparing `deployment_package-0.0.8/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc` & `deployment_package-0.0.9/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.8/app/deployment_utils/src/preprocessing.py` & `deployment_package-0.0.9/app/deployment_utils/src/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.8/app/deployment_utils/src/schemas.py` & `deployment_package-0.0.9/app/deployment_utils/src/schemas.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.8/app/deployment_utils/test/testing.py` & `deployment_package-0.0.9/app/deployment_utils/test/testing.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.8/setup.py` & `deployment_package-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="deployment_package",
-    version="0.0.8",
+    version="0.0.9",
     description="Package for preprocessing functions used during Model Deployment module",
-    package_dir={"": "app"},
-    packages=find_packages(where="app"),
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
-    include_package_data=True
+    include_package_data=True,
+    data_files=[("test_data", ["app/deployment_utils/test/data/test.pkl"])]
 )
```

