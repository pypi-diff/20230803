# Comparing `tmp/sequentialPSS-0.0.1.tar.gz` & `tmp/sequentialPSS-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentialPSS-0.0.1.tar", last modified: Thu Aug  3 02:52:36 2023, max compression
+gzip compressed data, was "sequentialPSS-0.0.2.tar", last modified: Thu Aug  3 03:05:36 2023, max compression
```

## Comparing `sequentialPSS-0.0.1.tar` & `sequentialPSS-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 02:52:36.012256 sequentialPSS-0.0.1/
--rw-rw-rw-   0        0        0      273 2023-08-03 02:52:36.011258 sequentialPSS-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       89 2023-08-03 02:22:05.000000 sequentialPSS-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 02:52:35.960395 sequentialPSS-0.0.1/seqPSS/
--rw-rw-rw-   0        0        0      826 2023-08-03 02:33:55.000000 sequentialPSS-0.0.1/seqPSS/__init__.py
--rw-rw-rw-   0        0        0     1877 2023-08-03 02:51:30.000000 sequentialPSS-0.0.1/seqPSS/seqPSS.py
-drwxrwxrwx   0        0        0        0 2023-08-03 02:52:36.007269 sequentialPSS-0.0.1/sequentialPSS.egg-info/
--rw-rw-rw-   0        0        0      273 2023-08-03 02:52:34.000000 sequentialPSS-0.0.1/sequentialPSS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-08-03 02:52:35.000000 sequentialPSS-0.0.1/sequentialPSS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 02:52:35.000000 sequentialPSS-0.0.1/sequentialPSS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-08-03 02:52:35.000000 sequentialPSS-0.0.1/sequentialPSS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-03 02:52:35.000000 sequentialPSS-0.0.1/sequentialPSS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 02:52:36.013253 sequentialPSS-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1148 2023-08-03 02:52:19.000000 sequentialPSS-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:05:36.399202 sequentialPSS-0.0.2/
+-rw-rw-rw-   0        0        0      273 2023-08-03 03:05:36.398204 sequentialPSS-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2023-08-03 02:22:05.000000 sequentialPSS-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 03:05:36.362259 sequentialPSS-0.0.2/seqPSS/
+-rw-rw-rw-   0        0        0      826 2023-08-03 02:33:55.000000 sequentialPSS-0.0.2/seqPSS/__init__.py
+-rw-rw-rw-   0        0        0     1872 2023-08-03 02:58:33.000000 sequentialPSS-0.0.2/seqPSS/sequentialPSS.py
+drwxrwxrwx   0        0        0        0 2023-08-03 03:05:36.395182 sequentialPSS-0.0.2/sequentialPSS.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-08-03 03:05:01.000000 sequentialPSS-0.0.2/sequentialPSS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-08-03 03:05:36.000000 sequentialPSS-0.0.2/sequentialPSS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 03:05:01.000000 sequentialPSS-0.0.2/sequentialPSS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-03 03:05:02.000000 sequentialPSS-0.0.2/sequentialPSS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 03:05:02.000000 sequentialPSS-0.0.2/sequentialPSS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 03:05:36.400169 sequentialPSS-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2023-08-03 03:04:47.000000 sequentialPSS-0.0.2/setup.py
```

### Comparing `sequentialPSS-0.0.1/seqPSS/__init__.py` & `sequentialPSS-0.0.2/seqPSS/__init__.py`

 * *Files identical despite different names*

### Comparing `sequentialPSS-0.0.1/seqPSS/seqPSS.py` & `sequentialPSS-0.0.2/seqPSS/sequentialPSS.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import numpy as np
 import pandas as pd
 import random2
 
 
 # ## data
 
-# In[5]:
+# In[6]:
 
 
-path = "seqPSS/sampleData/concatenated_df.csv"
+path = "./sampleData/concatenated_df.csv"
 simul_data = pd.read_csv(path)
 
 
 # ## simulation code
 
 # In[3]:
```

### Comparing `sequentialPSS-0.0.1/setup.py` & `sequentialPSS-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'sequentialPSS',
-    version = '0.0.1',
+    version = '0.0.2',
     description = "algorithm for sequential parameter searching with GSA",
     url = 'https://github.com/MG-Choi/seqPSS',
     author = 'MoongiChoi',
     author_email = 'u1316663@utah.edu',
     packages = find_packages(),
+    package_data = {'seqentialPSS': ['sampleData/concatenated_df.csv']},
+    include_package_data = True,
     install_requires = ['numpy==1.24.3', 'pandas==1.5.3', 'random2==1.0.1']
 )
 
 
+
 '''
 note: How to make library
 - 모두 seqC -> py로 저장.
 
 - cmd (administrator) -> cd repository
 - python setup.py bdist_wheel
 - cd dist
```

