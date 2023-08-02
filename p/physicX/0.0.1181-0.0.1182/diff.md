# Comparing `tmp/physicX-0.0.1181.tar.gz` & `tmp/physicX-0.0.1182.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicX-0.0.1181.tar", last modified: Wed Aug  2 03:45:22 2023, max compression
+gzip compressed data, was "physicX-0.0.1182.tar", last modified: Wed Aug  2 22:49:41 2023, max compression
```

## Comparing `physicX-0.0.1181.tar` & `physicX-0.0.1182.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 03:45:22.560827 physicX-0.0.1181/
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      830 2023-08-02 03:45:22.560827 physicX-0.0.1181/PKG-INFO
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      263 2023-08-02 03:10:34.000000 physicX-0.0.1181/README.md
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      772 2023-08-02 03:45:07.000000 physicX-0.0.1181/pyproject.toml
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       31 2023-08-02 03:10:34.000000 physicX-0.0.1181/requirements.txt
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       38 2023-08-02 03:45:22.560827 physicX-0.0.1181/setup.cfg
-drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 03:45:22.560827 physicX-0.0.1181/src/
-drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 03:45:22.560827 physicX-0.0.1181/src/physicX/
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       76 2023-08-02 03:35:22.000000 physicX-0.0.1181/src/physicX/__init__.py
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      880 2023-08-02 03:33:42.000000 physicX-0.0.1181/src/physicX/constants.py
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      101 2023-08-02 03:44:30.000000 physicX-0.0.1181/src/physicX/law.py
-drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 03:45:22.560827 physicX-0.0.1181/src/physicX.egg-info/
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      830 2023-08-02 03:45:22.000000 physicX-0.0.1181/src/physicX.egg-info/PKG-INFO
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      283 2023-08-02 03:45:22.000000 physicX-0.0.1181/src/physicX.egg-info/SOURCES.txt
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)        1 2023-08-02 03:45:22.000000 physicX-0.0.1181/src/physicX.egg-info/dependency_links.txt
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       31 2023-08-02 03:45:22.000000 physicX-0.0.1181/src/physicX.egg-info/requires.txt
--rw-rw-r--   0 cunknown  (1000) cunknown  (1000)        8 2023-08-02 03:45:22.000000 physicX-0.0.1181/src/physicX.egg-info/top_level.txt
+drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 22:49:41.041921 physicX-0.0.1182/
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      830 2023-08-02 22:49:41.041921 physicX-0.0.1182/PKG-INFO
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      263 2023-08-02 22:44:43.000000 physicX-0.0.1182/README.md
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      772 2023-08-02 22:49:18.000000 physicX-0.0.1182/pyproject.toml
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       31 2023-08-02 22:44:43.000000 physicX-0.0.1182/requirements.txt
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       38 2023-08-02 22:49:41.041921 physicX-0.0.1182/setup.cfg
+drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 22:49:41.037921 physicX-0.0.1182/src/
+drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 22:49:41.037921 physicX-0.0.1182/src/physicX/
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       77 2023-08-02 22:44:43.000000 physicX-0.0.1182/src/physicX/__init__.py
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      880 2023-08-02 22:44:43.000000 physicX-0.0.1182/src/physicX/constants.py
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       94 2023-08-02 22:45:39.000000 physicX-0.0.1182/src/physicX/law.py
+drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 22:49:41.041921 physicX-0.0.1182/src/physicX.egg-info/
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      830 2023-08-02 22:49:41.000000 physicX-0.0.1182/src/physicX.egg-info/PKG-INFO
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      283 2023-08-02 22:49:41.000000 physicX-0.0.1182/src/physicX.egg-info/SOURCES.txt
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)        1 2023-08-02 22:49:41.000000 physicX-0.0.1182/src/physicX.egg-info/dependency_links.txt
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       31 2023-08-02 22:49:41.000000 physicX-0.0.1182/src/physicX.egg-info/requires.txt
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)        8 2023-08-02 22:49:41.000000 physicX-0.0.1182/src/physicX.egg-info/top_level.txt
```

### Comparing `physicX-0.0.1181/PKG-INFO` & `physicX-0.0.1182/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicX
-Version: 0.0.1181
+Version: 0.0.1182
 Summary: mathematics and physics library
 Author-email: anonymous14725 <anonymous14725@yahoo.com>
 Project-URL: Homepage, https://github.com/anonymous14725/physicX
 Project-URL: Bug Tracker, https://github.com/anonymous14725/physicX/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Other OS
```

### Comparing `physicX-0.0.1181/pyproject.toml` & `physicX-0.0.1182/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy>=1.24.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["dependencies"]
 name = "physicX"
-version = "0.0.1181"
+version = "0.0.1182"
 authors = [
   { name="anonymous14725", email="anonymous14725@yahoo.com" },
 ]
 description = "mathematics and physics library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `physicX-0.0.1181/src/physicX/constants.py` & `physicX-0.0.1182/src/physicX/constants.py`

 * *Files identical despite different names*

### Comparing `physicX-0.0.1181/src/physicX.egg-info/PKG-INFO` & `physicX-0.0.1182/src/physicX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicX
-Version: 0.0.1181
+Version: 0.0.1182
 Summary: mathematics and physics library
 Author-email: anonymous14725 <anonymous14725@yahoo.com>
 Project-URL: Homepage, https://github.com/anonymous14725/physicX
 Project-URL: Bug Tracker, https://github.com/anonymous14725/physicX/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Other OS
```

