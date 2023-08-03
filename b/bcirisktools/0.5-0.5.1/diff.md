# Comparing `tmp/bcirisktools-0.5.tar.gz` & `tmp/bcirisktools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcirisktools-0.5.tar", last modified: Wed Aug  2 19:15:30 2023, max compression
+gzip compressed data, was "bcirisktools-0.5.1.tar", last modified: Wed Aug  2 19:27:30 2023, max compression
```

## Comparing `bcirisktools-0.5.tar` & `bcirisktools-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:15:30.033000 bcirisktools-0.5/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-07-27 13:56:43.000000 bcirisktools-0.5/LICENCE
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      571 2023-08-02 19:15:30.026000 bcirisktools-0.5/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-07-27 13:56:43.000000 bcirisktools-0.5/README.md
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:15:29.902000 bcirisktools-0.5/bcirisktools/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      385 2023-08-02 19:08:07.000000 bcirisktools-0.5/bcirisktools/__init__.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/input_filters.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/metrics_bci.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/modeling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    16808 2023-08-02 19:01:12.000000 bcirisktools-0.5/bcirisktools/profiling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/shapley_report.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/stability.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/tree_crt.py
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:15:30.000000 bcirisktools-0.5/bcirisktools.egg-info/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      571 2023-08-02 19:15:29.000000 bcirisktools-0.5/bcirisktools.egg-info/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-02 19:15:29.000000 bcirisktools-0.5/bcirisktools.egg-info/SOURCES.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-02 19:15:29.000000 bcirisktools-0.5/bcirisktools.egg-info/dependency_links.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-08-02 19:15:29.000000 bcirisktools-0.5/bcirisktools.egg-info/requires.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-02 19:15:29.000000 bcirisktools-0.5/bcirisktools.egg-info/top_level.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-07-27 13:56:43.000000 bcirisktools-0.5/pyproject.toml
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-02 19:15:30.036000 bcirisktools-0.5/setup.cfg
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1016 2023-08-02 19:15:11.000000 bcirisktools-0.5/setup.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:27:30.658000 bcirisktools-0.5.1/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-07-27 13:56:43.000000 bcirisktools-0.5.1/LICENCE
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-02 19:27:30.652000 bcirisktools-0.5.1/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-07-27 13:56:43.000000 bcirisktools-0.5.1/README.md
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:27:30.530000 bcirisktools-0.5.1/bcirisktools/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      385 2023-08-02 19:08:07.000000 bcirisktools-0.5.1/bcirisktools/__init__.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-07-27 13:56:43.000000 bcirisktools-0.5.1/bcirisktools/input_filters.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-07-27 13:56:43.000000 bcirisktools-0.5.1/bcirisktools/metrics_bci.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-07-27 13:56:43.000000 bcirisktools-0.5.1/bcirisktools/modeling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    16951 2023-08-02 19:27:19.000000 bcirisktools-0.5.1/bcirisktools/profiling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-07-27 13:56:43.000000 bcirisktools-0.5.1/bcirisktools/shapley_report.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-07-27 13:56:43.000000 bcirisktools-0.5.1/bcirisktools/stability.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-07-27 13:56:43.000000 bcirisktools-0.5.1/bcirisktools/tree_crt.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:27:30.629000 bcirisktools-0.5.1/bcirisktools.egg-info/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-02 19:27:30.000000 bcirisktools-0.5.1/bcirisktools.egg-info/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-02 19:27:30.000000 bcirisktools-0.5.1/bcirisktools.egg-info/SOURCES.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-02 19:27:30.000000 bcirisktools-0.5.1/bcirisktools.egg-info/dependency_links.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-08-02 19:27:30.000000 bcirisktools-0.5.1/bcirisktools.egg-info/requires.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-02 19:27:30.000000 bcirisktools-0.5.1/bcirisktools.egg-info/top_level.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-07-27 13:56:43.000000 bcirisktools-0.5.1/pyproject.toml
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-02 19:27:30.663000 bcirisktools-0.5.1/setup.cfg
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1018 2023-08-02 19:27:23.000000 bcirisktools-0.5.1/setup.py
```

### Comparing `bcirisktools-0.5/LICENCE` & `bcirisktools-0.5.1/LICENCE`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5/PKG-INFO` & `bcirisktools-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.5
+Version: 0.5.1
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.5/README.md` & `bcirisktools-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5/bcirisktools/input_filters.py` & `bcirisktools-0.5.1/bcirisktools/input_filters.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5/bcirisktools/metrics_bci.py` & `bcirisktools-0.5.1/bcirisktools/metrics_bci.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5/bcirisktools/modeling.py` & `bcirisktools-0.5.1/bcirisktools/modeling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5/bcirisktools/profiling.py` & `bcirisktools-0.5.1/bcirisktools/profiling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,13 @@
+import pandas as pd
+import numpy as np
 from PIL import Image
+import plotly.express as px
+from plotly.subplots import make_subplots
+import plotly.graph_objects as go
 
 
 def modify_interval(interval1, interval2):
     if interval2 > interval1:
         return pd.Interval(interval1.left, interval2.right, closed="right")
     else:
         return pd.Interval(interval2.left, interval1.right, closed="right")
```

### Comparing `bcirisktools-0.5/bcirisktools/shapley_report.py` & `bcirisktools-0.5.1/bcirisktools/shapley_report.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5/bcirisktools/stability.py` & `bcirisktools-0.5.1/bcirisktools/stability.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5/bcirisktools/tree_crt.py` & `bcirisktools-0.5.1/bcirisktools/tree_crt.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5/bcirisktools.egg-info/PKG-INFO` & `bcirisktools-0.5.1/bcirisktools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.5
+Version: 0.5.1
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.5/setup.py` & `bcirisktools-0.5.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.5"
+VERSION = "0.5.1"
 DESCRIPTION = "BCI risks tools"
 LONG_DESCRIPTION = "A package that compiles different risk tools used by BCI bank."
 
 # Setting up
 setup(
     name="bcirisktools",
     version=VERSION,
```

