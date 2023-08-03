# Comparing `tmp/OpenGeodeWeb-Back-0.0.8.tar.gz` & `tmp/OpenGeodeWeb-Back-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenGeodeWeb-Back-0.0.8.tar", last modified: Tue Aug  1 12:56:59 2023, max compression
+gzip compressed data, was "OpenGeodeWeb-Back-0.0.9.tar", last modified: Tue Aug  1 13:36:41 2023, max compression
```

## Comparing `OpenGeodeWeb-Back-0.0.8.tar` & `OpenGeodeWeb-Back-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:59.161331 OpenGeodeWeb-Back-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 12:56:48.000000 OpenGeodeWeb-Back-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 12:56:59.161331 OpenGeodeWeb-Back-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-08-01 12:56:48.000000 OpenGeodeWeb-Back-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-01 12:56:48.000000 OpenGeodeWeb-Back-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:56:59.161331 OpenGeodeWeb-Back-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:59.157331 OpenGeodeWeb-Back-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:59.161331 OpenGeodeWeb-Back-0.0.8/src/OpenGeodeWeb_Back.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 12:56:59.000000 OpenGeodeWeb-Back-0.0.8/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-01 12:56:59.000000 OpenGeodeWeb-Back-0.0.8/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:56:59.000000 OpenGeodeWeb-Back-0.0.8/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 12:56:59.000000 OpenGeodeWeb-Back-0.0.8/src/OpenGeodeWeb_Back.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:59.161331 OpenGeodeWeb-Back-0.0.8/src/opengeodeweb_back/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:56:48.000000 OpenGeodeWeb-Back-0.0.8/src/opengeodeweb_back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-08-01 12:56:48.000000 OpenGeodeWeb-Back-0.0.8/src/opengeodeweb_back/geode_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-08-01 12:56:48.000000 OpenGeodeWeb-Back-0.0.8/src/opengeodeweb_back/geode_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-08-01 12:56:48.000000 OpenGeodeWeb-Back-0.0.8/src/opengeodeweb_back/inspector_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:36:41.821655 OpenGeodeWeb-Back-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-01 13:36:34.000000 OpenGeodeWeb-Back-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 13:36:41.821655 OpenGeodeWeb-Back-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-08-01 13:36:34.000000 OpenGeodeWeb-Back-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-01 13:36:34.000000 OpenGeodeWeb-Back-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 13:36:41.821655 OpenGeodeWeb-Back-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:36:41.821655 OpenGeodeWeb-Back-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:36:41.821655 OpenGeodeWeb-Back-0.0.9/src/OpenGeodeWeb_Back.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 13:36:41.000000 OpenGeodeWeb-Back-0.0.9/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-01 13:36:41.000000 OpenGeodeWeb-Back-0.0.9/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:36:41.000000 OpenGeodeWeb-Back-0.0.9/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-01 13:36:41.000000 OpenGeodeWeb-Back-0.0.9/src/OpenGeodeWeb_Back.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 13:36:41.000000 OpenGeodeWeb-Back-0.0.9/src/OpenGeodeWeb_Back.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:36:41.821655 OpenGeodeWeb-Back-0.0.9/src/opengeodeweb_back/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:36:34.000000 OpenGeodeWeb-Back-0.0.9/src/opengeodeweb_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-08-01 13:36:34.000000 OpenGeodeWeb-Back-0.0.9/src/opengeodeweb_back/geode_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-08-01 13:36:34.000000 OpenGeodeWeb-Back-0.0.9/src/opengeodeweb_back/geode_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15554 2023-08-01 13:36:34.000000 OpenGeodeWeb-Back-0.0.9/src/opengeodeweb_back/inspector_functions.py
```

### Comparing `OpenGeodeWeb-Back-0.0.8/LICENSE` & `OpenGeodeWeb-Back-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Back-0.0.8/PKG-INFO` & `OpenGeodeWeb-Back-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 0.0.8
+Version: 0.0.9
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <contact@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `OpenGeodeWeb-Back-0.0.8/README.md` & `OpenGeodeWeb-Back-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Back-0.0.8/pyproject.toml` & `OpenGeodeWeb-Back-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OpenGeodeWeb-Back"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Geode-solutions", email="contact@geode-solutions.com" },
 ]
 description = "OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "geode-common==26.1.3",
+    "geode-viewables==2.0.3",
+    "opengeode-core==14.4.1",
+    "opengeode-geosciences==7.1.1",
+    "opengeode-geosciencesio==4.1.6",
+    "opengeode-inspector==3.0.7",
+    "opengeode-io==6.0.10"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/Geode-solutions/OpenGeodeWeb-Back"
 "Bug Tracker" = "https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `OpenGeodeWeb-Back-0.0.8/src/OpenGeodeWeb_Back.egg-info/PKG-INFO` & `OpenGeodeWeb-Back-0.0.9/src/OpenGeodeWeb_Back.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 0.0.8
+Version: 0.0.9
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <contact@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `OpenGeodeWeb-Back-0.0.8/src/opengeodeweb_back/geode_functions.py` & `OpenGeodeWeb-Back-0.0.9/src/opengeodeweb_back/geode_functions.py`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Back-0.0.8/src/opengeodeweb_back/geode_objects.py` & `OpenGeodeWeb-Back-0.0.9/src/opengeodeweb_back/geode_objects.py`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Back-0.0.8/src/opengeodeweb_back/inspector_functions.py` & `OpenGeodeWeb-Back-0.0.9/src/opengeodeweb_back/inspector_functions.py`

 * *Files identical despite different names*

