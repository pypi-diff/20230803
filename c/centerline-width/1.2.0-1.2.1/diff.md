# Comparing `tmp/centerline-width-1.2.0.tar.gz` & `tmp/centerline-width-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-1.2.0.tar", last modified: Wed Aug  2 21:47:36 2023, max compression
+gzip compressed data, was "dist/centerline-width-1.2.1.tar", last modified: Wed Aug  2 22:10:41 2023, max compression
```

## Comparing `centerline-width-1.2.0.tar` & `centerline-width-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 21:47:36.907874 centerline-width-1.2.0/
--rw-rw-r--   0 user      (1000) user      (1000)    53896 2023-08-02 21:47:36.903874 centerline-width-1.2.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    47490 2023-08-01 21:45:39.000000 centerline-width-1.2.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 21:47:36.899874 centerline-width-1.2.0/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1981 2023-08-01 00:12:16.000000 centerline-width-1.2.0/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    24559 2023-08-02 21:33:19.000000 centerline-width-1.2.0/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    19456 2023-08-01 21:47:42.000000 centerline-width-1.2.0/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-1.2.0/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    12626 2023-08-02 20:44:38.000000 centerline-width-1.2.0/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-1.2.0/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 21:47:36.903874 centerline-width-1.2.0/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     6529 2023-08-01 21:54:02.000000 centerline-width-1.2.0/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-1.2.0/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    15156 2023-08-01 21:54:05.000000 centerline-width-1.2.0/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-1.2.0/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-1.2.0/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)    11472 2023-08-01 21:54:49.000000 centerline-width-1.2.0/centerline_width/pytests/test_saveOutput.py
--rw-rw-r--   0 user      (1000) user      (1000)     3516 2023-08-02 20:45:43.000000 centerline-width-1.2.0/centerline_width/relativeDistance.py
--rw-rw-r--   0 user      (1000) user      (1000)     9334 2023-08-02 05:58:57.000000 centerline-width-1.2.0/centerline_width/riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     5833 2023-08-01 22:05:26.000000 centerline-width-1.2.0/centerline_width/saveOutput.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 21:47:36.903874 centerline-width-1.2.0/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    53896 2023-08-02 21:47:36.000000 centerline-width-1.2.0/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      812 2023-08-02 21:47:36.000000 centerline-width-1.2.0/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 21:47:36.000000 centerline-width-1.2.0/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      160 2023-08-02 21:47:36.000000 centerline-width-1.2.0/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-08-02 21:47:36.000000 centerline-width-1.2.0/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 21:47:36.907874 centerline-width-1.2.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1846 2023-08-02 21:45:52.000000 centerline-width-1.2.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:10:41.114423 centerline-width-1.2.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    53896 2023-08-02 22:10:41.114423 centerline-width-1.2.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    47490 2023-08-01 21:45:39.000000 centerline-width-1.2.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:10:41.114423 centerline-width-1.2.1/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1981 2023-08-01 00:12:16.000000 centerline-width-1.2.1/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    24570 2023-08-02 21:56:19.000000 centerline-width-1.2.1/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19456 2023-08-01 21:47:42.000000 centerline-width-1.2.1/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-1.2.1/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12626 2023-08-02 20:44:38.000000 centerline-width-1.2.1/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-1.2.1/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:10:41.114423 centerline-width-1.2.1/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     6529 2023-08-01 21:54:02.000000 centerline-width-1.2.1/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-1.2.1/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15156 2023-08-01 21:54:05.000000 centerline-width-1.2.1/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-1.2.1/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-1.2.1/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11472 2023-08-01 21:54:49.000000 centerline-width-1.2.1/centerline_width/pytests/test_saveOutput.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3516 2023-08-02 20:45:43.000000 centerline-width-1.2.1/centerline_width/relativeDistance.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9334 2023-08-02 05:58:57.000000 centerline-width-1.2.1/centerline_width/riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5833 2023-08-01 22:05:26.000000 centerline-width-1.2.1/centerline_width/saveOutput.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 22:10:41.114423 centerline-width-1.2.1/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    53896 2023-08-02 22:10:41.000000 centerline-width-1.2.1/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      812 2023-08-02 22:10:41.000000 centerline-width-1.2.1/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 22:10:41.000000 centerline-width-1.2.1/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      160 2023-08-02 22:10:41.000000 centerline-width-1.2.1/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-08-02 22:10:41.000000 centerline-width-1.2.1/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 22:10:41.114423 centerline-width-1.2.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1846 2023-08-02 22:08:07.000000 centerline-width-1.2.1/setup.py
```

### Comparing `centerline-width-1.2.0/PKG-INFO` & `centerline-width-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.2.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.2.1.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
```

### Comparing `centerline-width-1.2.0/README.md` & `centerline-width-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/__init__.py` & `centerline-width-1.2.1/centerline_width/__init__.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/centerline.py` & `centerline-width-1.2.1/centerline_width/centerline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Built in Python functions
 import math
 import logging
+import csv
 
 # External Python libraries (installed via pip install)
 import numpy as np
 import networkx as nx
 from scipy import interpolate
 from shapely.geometry import Point, LineString
 from shapely.ops import split
```

### Comparing `centerline-width-1.2.0/centerline_width/error_handling.py` & `centerline-width-1.2.1/centerline_width/error_handling.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/getCoordinatesKML.py` & `centerline-width-1.2.1/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/plotDiagrams.py` & `centerline-width-1.2.1/centerline_width/plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/preprocessing.py` & `centerline-width-1.2.1/centerline_width/preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/pytests/test_centerline.py` & `centerline-width-1.2.1/centerline_width/pytests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-1.2.1/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-1.2.1/centerline_width/pytests/test_plotDiagrams.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/pytests/test_preprocessing.py` & `centerline-width-1.2.1/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-1.2.1/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/pytests/test_saveOutput.py` & `centerline-width-1.2.1/centerline_width/pytests/test_saveOutput.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/relativeDistance.py` & `centerline-width-1.2.1/centerline_width/relativeDistance.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/riverCenterlineClass.py` & `centerline-width-1.2.1/centerline_width/riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width/saveOutput.py` & `centerline-width-1.2.1/centerline_width/saveOutput.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/centerline_width.egg-info/PKG-INFO` & `centerline-width-1.2.1/centerline_width.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.2.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.2.1.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
```

### Comparing `centerline-width-1.2.0/centerline_width.egg-info/SOURCES.txt` & `centerline-width-1.2.1/centerline_width.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-width-1.2.0/setup.py` & `centerline-width-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.2.0"
+VERSION="1.2.1"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
```

