# Comparing `tmp/AlgDiff-2.1.1.1.tar.gz` & `tmp/AlgDiff-2.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgDiff-2.1.1.1.tar", last modified: Thu Aug  3 09:23:13 2023, max compression
+gzip compressed data, was "AlgDiff-2.1.1.2.tar", last modified: Thu Aug  3 09:25:41 2023, max compression
```

## Comparing `AlgDiff-2.1.1.1.tar` & `AlgDiff-2.1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-08-03 09:23:13.633016 AlgDiff-2.1.1.1/
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-08-03 09:23:13.633016 AlgDiff-2.1.1.1/AlgDiff/
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.000000 AlgDiff-2.1.1.1/AlgDiff/__init__.py
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41484 2023-08-03 08:24:37.000000 AlgDiff-2.1.1.1/AlgDiff/algebraicDifferentiator.py
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-08-03 09:23:13.633016 AlgDiff-2.1.1.1/AlgDiff.egg-info/
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    15188 2023-08-03 09:23:13.000000 AlgDiff-2.1.1.1/AlgDiff.egg-info/PKG-INFO
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      260 2023-08-03 09:23:13.000000 AlgDiff-2.1.1.1/AlgDiff.egg-info/SOURCES.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        1 2023-08-03 09:23:13.000000 AlgDiff-2.1.1.1/AlgDiff.egg-info/dependency_links.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       19 2023-08-03 09:23:13.000000 AlgDiff-2.1.1.1/AlgDiff.egg-info/requires.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        8 2023-08-03 09:23:13.000000 AlgDiff-2.1.1.1/AlgDiff.egg-info/top_level.txt
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1458 2023-06-06 12:55:23.000000 AlgDiff-2.1.1.1/LICENSE
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    15188 2023-08-03 09:23:13.633016 AlgDiff-2.1.1.1/PKG-INFO
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    12724 2023-06-16 13:57:29.000000 AlgDiff-2.1.1.1/README.md
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      875 2023-08-03 09:22:50.000000 AlgDiff-2.1.1.1/pyproject.toml
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       79 2023-08-03 09:23:13.633016 AlgDiff-2.1.1.1/setup.cfg
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1121 2023-08-03 09:23:02.000000 AlgDiff-2.1.1.1/setup.py
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-08-03 09:25:41.177026 AlgDiff-2.1.1.2/
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-08-03 09:25:41.177026 AlgDiff-2.1.1.2/AlgDiff/
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.000000 AlgDiff-2.1.1.2/AlgDiff/__init__.py
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41484 2023-08-03 08:24:37.000000 AlgDiff-2.1.1.2/AlgDiff/algebraicDifferentiator.py
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-08-03 09:25:41.177026 AlgDiff-2.1.1.2/AlgDiff.egg-info/
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    15188 2023-08-03 09:25:41.000000 AlgDiff-2.1.1.2/AlgDiff.egg-info/PKG-INFO
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      260 2023-08-03 09:25:41.000000 AlgDiff-2.1.1.2/AlgDiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        1 2023-08-03 09:25:41.000000 AlgDiff-2.1.1.2/AlgDiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       19 2023-08-03 09:25:41.000000 AlgDiff-2.1.1.2/AlgDiff.egg-info/requires.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        8 2023-08-03 09:25:41.000000 AlgDiff-2.1.1.2/AlgDiff.egg-info/top_level.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1458 2023-06-06 12:55:23.000000 AlgDiff-2.1.1.2/LICENSE
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    15188 2023-08-03 09:25:41.177026 AlgDiff-2.1.1.2/PKG-INFO
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    12724 2023-06-16 13:57:29.000000 AlgDiff-2.1.1.2/README.md
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      875 2023-08-03 09:25:26.000000 AlgDiff-2.1.1.2/pyproject.toml
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       79 2023-08-03 09:25:41.177026 AlgDiff-2.1.1.2/setup.cfg
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1121 2023-08-03 09:25:31.000000 AlgDiff-2.1.1.2/setup.py
```

### Comparing `AlgDiff-2.1.1.1/AlgDiff/algebraicDifferentiator.py` & `AlgDiff-2.1.1.2/AlgDiff/algebraicDifferentiator.py`

 * *Files identical despite different names*

### Comparing `AlgDiff-2.1.1.1/AlgDiff.egg-info/PKG-INFO` & `AlgDiff-2.1.1.2/AlgDiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgDiff
-Version: 2.1.1.1
+Version: 2.1.1.2
 Summary: AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.
 Home-page: https://github.com/aothmane-control/Algebraic-differentiators
 Download-URL: https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.1.1
 Author: Amine Othmane
 Author-email: Amine Othmane <amine.othmane@uni-saarland.de>
 License: Copyright 2021 Amine Othmane
```

### Comparing `AlgDiff-2.1.1.1/LICENSE` & `AlgDiff-2.1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgDiff-2.1.1.1/PKG-INFO` & `AlgDiff-2.1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgDiff
-Version: 2.1.1.1
+Version: 2.1.1.2
 Summary: AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.
 Home-page: https://github.com/aothmane-control/Algebraic-differentiators
 Download-URL: https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.1.1
 Author: Amine Othmane
 Author-email: Amine Othmane <amine.othmane@uni-saarland.de>
 License: Copyright 2021 Amine Othmane
```

### Comparing `AlgDiff-2.1.1.1/README.md` & `AlgDiff-2.1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `AlgDiff-2.1.1.1/pyproject.toml` & `AlgDiff-2.1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "AlgDiff"
-version = "2.1.1.1"
+version = "2.1.1.2"
 authors = [
   { name="Amine Othmane", email="amine.othmane@uni-saarland.de" },
 ]
 description = "AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided."
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `AlgDiff-2.1.1.1/setup.py` & `AlgDiff-2.1.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "docs/source/usage.rst").read_text()
 
 setup(
   name = 'AlgDiff',
   packages = ['AlgDiff'],
-  version = '2.1.1.1',
+  version = '2.1.1.2',
   license='bsd-3-clause',
   description = 'AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.',
   
   long_description = long_description,
   long_description_content_type='text/x-rst',
   
   author = 'Amine Othmane',
```

