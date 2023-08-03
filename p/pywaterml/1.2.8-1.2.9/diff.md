# Comparing `tmp/pywaterml-1.2.8.tar.gz` & `tmp/pywaterml-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywaterml-1.2.8.tar", last modified: Tue Mar  2 18:22:00 2021, max compression
+gzip compressed data, was "dist/pywaterml-1.2.9.tar", last modified: Tue Mar  2 18:46:20 2021, max compression
```

## Comparing `pywaterml-1.2.8.tar` & `pywaterml-1.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-02 18:22:00.000000 pywaterml-1.2.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2021-03-02 18:13:09.000000 pywaterml-1.2.8/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-02 18:22:00.000000 pywaterml-1.2.8/pywaterml.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      882 2021-03-02 18:22:00.000000 pywaterml-1.2.8/pywaterml.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-02 18:22:00.000000 pywaterml-1.2.8/pywaterml.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2021-03-02 18:22:00.000000 pywaterml-1.2.8/pywaterml.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-02 18:22:00.000000 pywaterml-1.2.8/pywaterml.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      442 2021-03-02 18:22:00.000000 pywaterml-1.2.8/pywaterml.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2021-03-02 18:22:00.000000 pywaterml-1.2.8/pywaterml.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2021-03-02 18:22:00.000000 pywaterml-1.2.8/pywaterml.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    70144 2021-03-02 18:13:09.000000 pywaterml-1.2.8/versioneer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      882 2021-03-02 18:22:00.000000 pywaterml-1.2.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-02 18:22:00.000000 pywaterml-1.2.8/pywaterml/
--rw-rw-r--   0 travis    (2000) travis    (2000)      498 2021-03-02 18:22:00.000000 pywaterml-1.2.8/pywaterml/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3801 2021-03-02 18:13:09.000000 pywaterml-1.2.8/pywaterml/analyzeData.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      900 2021-03-02 18:13:09.000000 pywaterml-1.2.8/pywaterml/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44487 2021-03-02 18:13:09.000000 pywaterml-1.2.8/pywaterml/waterML.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       37 2021-03-02 18:13:09.000000 pywaterml-1.2.8/pywaterml/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      330 2021-03-02 18:13:09.000000 pywaterml-1.2.8/pywaterml/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40907 2021-03-02 18:13:09.000000 pywaterml-1.2.8/pywaterml/auxiliaryMod.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2021-03-02 18:22:00.000000 pywaterml-1.2.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     3831 2021-03-02 18:13:09.000000 pywaterml-1.2.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2021-03-02 18:13:09.000000 pywaterml-1.2.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-02 18:46:20.000000 pywaterml-1.2.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       81 2021-03-02 18:37:21.000000 pywaterml-1.2.9/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-02 18:46:20.000000 pywaterml-1.2.9/pywaterml.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      882 2021-03-02 18:46:20.000000 pywaterml-1.2.9/pywaterml.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-02 18:46:20.000000 pywaterml-1.2.9/pywaterml.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       10 2021-03-02 18:46:20.000000 pywaterml-1.2.9/pywaterml.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-02 18:46:20.000000 pywaterml-1.2.9/pywaterml.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      442 2021-03-02 18:46:20.000000 pywaterml-1.2.9/pywaterml.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2021-03-02 18:46:20.000000 pywaterml-1.2.9/pywaterml.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       49 2021-03-02 18:46:20.000000 pywaterml-1.2.9/pywaterml.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70144 2021-03-02 18:37:21.000000 pywaterml-1.2.9/versioneer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      882 2021-03-02 18:46:20.000000 pywaterml-1.2.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-02 18:46:20.000000 pywaterml-1.2.9/pywaterml/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      498 2021-03-02 18:46:20.000000 pywaterml-1.2.9/pywaterml/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3801 2021-03-02 18:37:21.000000 pywaterml-1.2.9/pywaterml/analyzeData.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      900 2021-03-02 18:37:21.000000 pywaterml-1.2.9/pywaterml/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44488 2021-03-02 18:37:21.000000 pywaterml-1.2.9/pywaterml/waterML.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       37 2021-03-02 18:37:21.000000 pywaterml-1.2.9/pywaterml/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      330 2021-03-02 18:37:21.000000 pywaterml-1.2.9/pywaterml/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40907 2021-03-02 18:37:21.000000 pywaterml-1.2.9/pywaterml/auxiliaryMod.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2021-03-02 18:46:20.000000 pywaterml-1.2.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3831 2021-03-02 18:37:21.000000 pywaterml-1.2.9/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1377 2021-03-02 18:37:21.000000 pywaterml-1.2.9/setup.py
```

### Comparing `pywaterml-1.2.8/pywaterml.egg-info/PKG-INFO` & `pywaterml-1.2.9/pywaterml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pywaterml
-Version: 1.2.8
+Version: 1.2.9
 Summary: The pywaterml is a package that lets you handle WaterML functions such as GetValues, GetSitesInfo, etc. In addition it lets offers extra functions such as mean interpolation for data with gaps
 Home-page: https://github.com/romer8/pywaterml
 Author: Elkin Giovanni Romero Bustamante
 Author-email: gio.rombus@gmail.com
 License: BSD 3-Clause
 Description: UNKNOWN
 Keywords: WaterML
```

### Comparing `pywaterml-1.2.8/versioneer.py` & `pywaterml-1.2.9/versioneer.py`

 * *Files identical despite different names*

### Comparing `pywaterml-1.2.8/PKG-INFO` & `pywaterml-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pywaterml
-Version: 1.2.8
+Version: 1.2.9
 Summary: The pywaterml is a package that lets you handle WaterML functions such as GetValues, GetSitesInfo, etc. In addition it lets offers extra functions such as mean interpolation for data with gaps
 Home-page: https://github.com/romer8/pywaterml
 Author: Elkin Giovanni Romero Bustamante
 Author-email: gio.rombus@gmail.com
 License: BSD 3-Clause
 Description: UNKNOWN
 Keywords: WaterML
```

### Comparing `pywaterml-1.2.8/pywaterml/analyzeData.py` & `pywaterml-1.2.9/pywaterml/analyzeData.py`

 * *Files identical despite different names*

### Comparing `pywaterml-1.2.8/pywaterml/cli.py` & `pywaterml-1.2.9/pywaterml/cli.py`

 * *Files identical despite different names*

### Comparing `pywaterml-1.2.8/pywaterml/waterML.py` & `pywaterml-1.2.9/pywaterml/waterML.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pyproj import Proj, transform
 import xml.etree.ElementTree as ET
 import pandas as pd
 from datetime import datetime
 from tslearn.metrics import dtw
 from tslearn.clustering import TimeSeriesKMeans
 from tslearn.utils import to_time_series, to_time_series_dataset
+
 class WaterMLOperations():
     """
     This class represents the WaterML object that will be able to fetch and analyze Data from 'WaterML' and 'WaterOneFlow' Web Services
 
     Args:
         url: WaterOneFlow web service that complies to the SOAP protocol
     """
```

### Comparing `pywaterml-1.2.8/pywaterml/auxiliaryMod.py` & `pywaterml-1.2.9/pywaterml/auxiliaryMod.py`

 * *Files identical despite different names*

### Comparing `pywaterml-1.2.8/setup.cfg` & `pywaterml-1.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pywaterml-1.2.8/README.rst` & `pywaterml-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `pywaterml-1.2.8/setup.py` & `pywaterml-1.2.9/setup.py`

 * *Files identical despite different names*

