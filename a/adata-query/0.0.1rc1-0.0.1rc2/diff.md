# Comparing `tmp/adata_query-0.0.1rc1.tar.gz` & `tmp/adata_query-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata_query-0.0.1rc1.tar", last modified: Thu Aug  3 14:28:03 2023, max compression
+gzip compressed data, was "adata_query-0.0.1rc2.tar", last modified: Thu Aug  3 14:33:41 2023, max compression
```

## Comparing `adata_query-0.0.1rc1.tar` & `adata_query-0.0.1rc2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:28:03.038113 adata_query-0.0.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 14:27:53.000000 adata_query-0.0.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 14:28:03.038113 adata_query-0.0.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-03 14:27:53.000000 adata_query-0.0.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:28:03.038113 adata_query-0.0.1rc1/adata_query/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-03 14:27:53.000000 adata_query-0.0.1rc1/adata_query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:28:03.038113 adata_query-0.0.1rc1/adata_query/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 14:27:53.000000 adata_query-0.0.1rc1/adata_query/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-08-03 14:27:53.000000 adata_query-0.0.1rc1/adata_query/_core/_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-03 14:27:53.000000 adata_query-0.0.1rc1/adata_query/_core/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-03 14:27:53.000000 adata_query-0.0.1rc1/adata_query/_core/_locator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:28:03.038113 adata_query-0.0.1rc1/adata_query/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 14:27:53.000000 adata_query-0.0.1rc1/adata_query/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 14:27:53.000000 adata_query-0.0.1rc1/adata_query/_utils/_info_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:28:03.038113 adata_query-0.0.1rc1/adata_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 14:28:02.000000 adata_query-0.0.1rc1/adata_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 14:28:03.000000 adata_query-0.0.1rc1/adata_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:28:02.000000 adata_query-0.0.1rc1/adata_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 14:28:02.000000 adata_query-0.0.1rc1/adata_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 14:28:02.000000 adata_query-0.0.1rc1/adata_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:28:03.038113 adata_query-0.0.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-03 14:27:53.000000 adata_query-0.0.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:33:41.080381 adata_query-0.0.1rc2/adata_query/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/adata_query/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_core/_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_core/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_core/_locator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/adata_query/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/adata_query/_utils/_info_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/adata_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 14:33:41.000000 adata_query-0.0.1rc2/adata_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-03 14:33:41.000000 adata_query-0.0.1rc2/adata_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:33:41.000000 adata_query-0.0.1rc2/adata_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 14:33:41.000000 adata_query-0.0.1rc2/adata_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 14:33:41.000000 adata_query-0.0.1rc2/adata_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:33:41.084382 adata_query-0.0.1rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-03 14:33:27.000000 adata_query-0.0.1rc2/setup.py
```

### Comparing `adata_query-0.0.1rc1/LICENSE` & `adata_query-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc1/PKG-INFO` & `adata_query-0.0.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata_query
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Fetch and format data matrices from AnnData.
 Home-page: https://github.com/mvinyard/AnnDataQuery
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `adata_query-0.0.1rc1/README.md` & `adata_query-0.0.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc1/adata_query/_core/_fetcher.py` & `adata_query-0.0.1rc2/adata_query/_core/_fetcher.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc1/adata_query/_core/_formatter.py` & `adata_query-0.0.1rc2/adata_query/_core/_formatter.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc1/adata_query/_core/_locator.py` & `adata_query-0.0.1rc2/adata_query/_core/_locator.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc1/adata_query/_utils/_info_message.py` & `adata_query-0.0.1rc2/adata_query/_utils/_info_message.py`

 * *Files identical despite different names*

### Comparing `adata_query-0.0.1rc1/adata_query.egg-info/PKG-INFO` & `adata_query-0.0.1rc2/adata_query.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata-query
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Fetch and format data matrices from AnnData.
 Home-page: https://github.com/mvinyard/AnnDataQuery
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `adata_query-0.0.1rc1/setup.py` & `adata_query-0.0.1rc2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 import os
 import sys
 
 
 # -- run setup: ----------------------------------------------------------------
 setuptools.setup(
     name="adata_query",
-    version="0.0.1rc1",
+    version="0.0.1rc2",
     python_requires=">3.9.0",
     author="Michael E. Vinyard",
     author_email="mvinyard.ai@gmail.com",
     url="https://github.com/mvinyard/AnnDataQuery",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="Fetch and format data matrices from AnnData.",
     packages=setuptools.find_packages(),
     install_requires=[
         "anndata>=0.9.1",
         "torch>=2.0.1",
         "autodevice>=0.0.2",
         "ABCParse>=0.0.6",
+        "licorice_font>=0.0.3",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3.9",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
```

