# Comparing `tmp/adata_query-0.0.1rc3.tar.gz` & `tmp/adata_query-0.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata_query-0.0.1rc3.tar", last modified: Thu Aug  3 15:24:52 2023, max compression
+gzip compressed data, was "adata_query-0.0.1rc4.tar", last modified: Thu Aug  3 15:49:05 2023, max compression
```

## Comparing `adata_query-0.0.1rc3.tar` & `adata_query-0.0.1rc4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/adata_query/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/adata_query/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_core/_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_core/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_core/_locator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/adata_query/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/adata_query/_utils/_info_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/adata_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 15:24:52.000000 adata_query-0.0.1rc3/adata_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 15:24:52.000000 adata_query-0.0.1rc3/adata_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:24:52.000000 adata_query-0.0.1rc3/adata_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 15:24:52.000000 adata_query-0.0.1rc3/adata_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 15:24:52.000000 adata_query-0.0.1rc3/adata_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:24:52.955311 adata_query-0.0.1rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 15:24:42.000000 adata_query-0.0.1rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:49:05.953601 adata_query-0.0.1rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 15:48:53.000000 adata_query-0.0.1rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-03 15:49:05.953601 adata_query-0.0.1rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-03 15:48:53.000000 adata_query-0.0.1rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:49:05.953601 adata_query-0.0.1rc4/adata_query/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-03 15:48:53.000000 adata_query-0.0.1rc4/adata_query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:49:05.953601 adata_query-0.0.1rc4/adata_query/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 15:48:53.000000 adata_query-0.0.1rc4/adata_query/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-08-03 15:48:53.000000 adata_query-0.0.1rc4/adata_query/_core/_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-03 15:48:53.000000 adata_query-0.0.1rc4/adata_query/_core/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-03 15:48:53.000000 adata_query-0.0.1rc4/adata_query/_core/_locator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:49:05.953601 adata_query-0.0.1rc4/adata_query/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 15:48:53.000000 adata_query-0.0.1rc4/adata_query/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 15:48:53.000000 adata_query-0.0.1rc4/adata_query/_utils/_info_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:49:05.953601 adata_query-0.0.1rc4/adata_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-03 15:49:05.000000 adata_query-0.0.1rc4/adata_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 15:49:05.000000 adata_query-0.0.1rc4/adata_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:49:05.000000 adata_query-0.0.1rc4/adata_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 15:49:05.000000 adata_query-0.0.1rc4/adata_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 15:49:05.000000 adata_query-0.0.1rc4/adata_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:49:05.953601 adata_query-0.0.1rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 15:48:53.000000 adata_query-0.0.1rc4/setup.py
```

### Comparing `adata_query-0.0.1rc3/LICENSE` & `adata_query-0.0.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc3/PKG-INFO` & `adata_query-0.0.1rc4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata_query
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: Fetch and format data matrices from AnnData.
 Home-page: https://github.com/mvinyard/AnnDataQuery
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
@@ -18,8 +18,10 @@
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/adata_query.svg)](https://pypi.python.org/pypi/adata_query/)
 [![PyPI version](https://badge.fury.io/py/adata_query.svg)](https://badge.fury.io/py/adata_query)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Fetch data matrices from AnnData and format as `np.ndarray` or `torch.Tensor`, on any device.
 
+Example: [notebook](https://colab.research.google.com/github/mvinyard/AnnDataQuery/blob/test-release/notebooks/anndata_query_tutorial.ipynb)
+
 For more information, see: [documentation](https://michael-vinyard.gitbook.io/anndataquery/)
```

### Comparing `adata_query-0.0.1rc3/README.md` & `adata_query-0.0.1rc4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,8 +2,10 @@
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/adata_query.svg)](https://pypi.python.org/pypi/adata_query/)
 [![PyPI version](https://badge.fury.io/py/adata_query.svg)](https://badge.fury.io/py/adata_query)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Fetch data matrices from AnnData and format as `np.ndarray` or `torch.Tensor`, on any device.
 
+Example: [notebook](https://colab.research.google.com/github/mvinyard/AnnDataQuery/blob/test-release/notebooks/anndata_query_tutorial.ipynb)
+
 For more information, see: [documentation](https://michael-vinyard.gitbook.io/anndataquery/)
```

### Comparing `adata_query-0.0.1rc3/adata_query/_core/_fetcher.py` & `adata_query-0.0.1rc4/adata_query/_core/_fetcher.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc3/adata_query/_core/_formatter.py` & `adata_query-0.0.1rc4/adata_query/_core/_formatter.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc3/adata_query/_core/_locator.py` & `adata_query-0.0.1rc4/adata_query/_core/_locator.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc3/adata_query/_utils/_info_message.py` & `adata_query-0.0.1rc4/adata_query/_utils/_info_message.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc3/adata_query.egg-info/PKG-INFO` & `adata_query-0.0.1rc4/adata_query.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata-query
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: Fetch and format data matrices from AnnData.
 Home-page: https://github.com/mvinyard/AnnDataQuery
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
@@ -18,8 +18,10 @@
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/adata_query.svg)](https://pypi.python.org/pypi/adata_query/)
 [![PyPI version](https://badge.fury.io/py/adata_query.svg)](https://badge.fury.io/py/adata_query)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Fetch data matrices from AnnData and format as `np.ndarray` or `torch.Tensor`, on any device.
 
+Example: [notebook](https://colab.research.google.com/github/mvinyard/AnnDataQuery/blob/test-release/notebooks/anndata_query_tutorial.ipynb)
+
 For more information, see: [documentation](https://michael-vinyard.gitbook.io/anndataquery/)
```

### Comparing `adata_query-0.0.1rc3/setup.py` & `adata_query-0.0.1rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 
 
 # -- run setup: ----------------------------------------------------------------
 setuptools.setup(
     name="adata_query",
-    version="0.0.1rc3",
+    version="0.0.1rc4",
     python_requires=">3.9.0",
     author="Michael E. Vinyard",
     author_email="mvinyard.ai@gmail.com",
     url="https://github.com/mvinyard/AnnDataQuery",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="Fetch and format data matrices from AnnData.",
```

