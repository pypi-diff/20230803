# Comparing `tmp/deployment_package-0.0.3.tar.gz` & `tmp/deployment_package-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deployment_package-0.0.3.tar", last modified: Thu Aug  3 19:24:18 2023, max compression
+gzip compressed data, was "deployment_package-0.0.4.tar", last modified: Thu Aug  3 19:33:35 2023, max compression
```

## Comparing `deployment_package-0.0.3.tar` & `deployment_package-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.294216 deployment_package-0.0.3/
--rw-rw-rw-   0        0        0      435 2023-08-03 19:24:18.294216 deployment_package-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.281668 deployment_package-0.0.3/app/
--rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/README.md
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.285723 deployment_package-0.0.3/app/deployment_package.egg-info/
--rw-rw-rw-   0        0        0      435 2023-08-03 19:24:18.000000 deployment_package-0.0.3/app/deployment_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-08-03 19:24:18.000000 deployment_package-0.0.3/app/deployment_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 19:24:18.000000 deployment_package-0.0.3/app/deployment_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-03 19:24:18.000000 deployment_package-0.0.3/app/deployment_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-03 19:24:18.000000 deployment_package-0.0.3/app/deployment_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.286621 deployment_package-0.0.3/app/deployment_utils/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.3/app/deployment_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.288635 deployment_package-0.0.3/app/deployment_utils/src/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.290926 deployment_package-0.0.3/app/deployment_utils/src/__pycache__/
--rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
--rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.3/app/deployment_utils/src/preprocessing.py
--rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/src/schemas.py
-drwxrwxrwx   0        0        0        0 2023-08-03 19:24:18.292929 deployment_package-0.0.3/app/deployment_utils/test/
--rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/test/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-08-03 16:16:43.000000 deployment_package-0.0.3/app/deployment_utils/test/test.pkl
--rw-rw-rw-   0        0        0     1610 2023-08-03 19:23:46.000000 deployment_package-0.0.3/app/deployment_utils/test/testing.py
--rw-rw-rw-   0        0        0       42 2023-08-03 19:24:18.294216 deployment_package-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-08-03 19:24:09.000000 deployment_package-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.500661 deployment_package-0.0.4/
+-rw-rw-rw-   0        0        0      435 2023-08-03 19:33:35.499664 deployment_package-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.484632 deployment_package-0.0.4/app/
+-rw-rw-rw-   0        0        0       67 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/README.md
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.489969 deployment_package-0.0.4/app/deployment_package.egg-info/
+-rw-rw-rw-   0        0        0      435 2023-08-03 19:33:35.000000 deployment_package-0.0.4/app/deployment_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-08-03 19:33:35.000000 deployment_package-0.0.4/app/deployment_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 19:33:35.000000 deployment_package-0.0.4/app/deployment_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-03 19:33:35.000000 deployment_package-0.0.4/app/deployment_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-03 19:33:35.000000 deployment_package-0.0.4/app/deployment_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.491013 deployment_package-0.0.4/app/deployment_utils/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:26:35.000000 deployment_package-0.0.4/app/deployment_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.492864 deployment_package-0.0.4/app/deployment_utils/src/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.495785 deployment_package-0.0.4/app/deployment_utils/src/__pycache__/
+-rw-rw-rw-   0        0        0      165 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/src/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2153 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1985 2023-08-03 19:03:39.000000 deployment_package-0.0.4/app/deployment_utils/src/preprocessing.py
+-rw-rw-rw-   0        0        0      690 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/src/schemas.py
+drwxrwxrwx   0        0        0        0 2023-08-03 19:33:35.498655 deployment_package-0.0.4/app/deployment_utils/test/
+-rw-rw-rw-   0        0        0        0 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/test/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-08-03 16:16:43.000000 deployment_package-0.0.4/app/deployment_utils/test/test.pkl
+-rw-rw-rw-   0        0        0     1744 2023-08-03 19:33:15.000000 deployment_package-0.0.4/app/deployment_utils/test/testing.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 19:33:35.500661 deployment_package-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-08-03 19:33:30.000000 deployment_package-0.0.4/setup.py
```

### Comparing `deployment_package-0.0.3/app/deployment_package.egg-info/SOURCES.txt` & `deployment_package-0.0.4/app/deployment_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.3/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc` & `deployment_package-0.0.4/app/deployment_utils/src/__pycache__/preprocessing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.3/app/deployment_utils/src/preprocessing.py` & `deployment_package-0.0.4/app/deployment_utils/src/preprocessing.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.3/app/deployment_utils/src/schemas.py` & `deployment_package-0.0.4/app/deployment_utils/src/schemas.py`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.3/app/deployment_utils/test/test.pkl` & `deployment_package-0.0.4/app/deployment_utils/test/test.pkl`

 * *Files identical despite different names*

### Comparing `deployment_package-0.0.3/setup.py` & `deployment_package-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="deployment_package",
-    version="0.0.3",
+    version="0.0.4",
     description="Package for preprocessing functions used during Model Deployment module",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/davidbognar201/Model_deployment_package",
     author="David Bognar",
```

