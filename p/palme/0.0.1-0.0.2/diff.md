# Comparing `tmp/palme-0.0.1.tar.gz` & `tmp/palme-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palme-0.0.1.tar", last modified: Fri Jul 28 15:58:23 2023, max compression
+gzip compressed data, was "palme-0.0.2.tar", last modified: Thu Aug  3 12:28:47 2023, max compression
```

## Comparing `palme-0.0.1.tar` & `palme-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:58:23.230935 palme-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 15:58:13.000000 palme-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-28 15:58:23.230935 palme-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-28 15:58:13.000000 palme-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:58:23.230935 palme-0.0.1/palme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-28 15:58:23.000000 palme-0.0.1/palme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-28 15:58:23.000000 palme-0.0.1/palme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:58:23.000000 palme-0.0.1/palme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-28 15:58:23.000000 palme-0.0.1/palme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:58:23.000000 palme-0.0.1/palme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 15:58:23.230935 palme-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-28 15:58:13.000000 palme-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:28:47.575534 palme-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 12:28:33.000000 palme-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-03 12:28:47.575534 palme-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-08-03 12:28:33.000000 palme-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:28:47.575534 palme-0.0.2/palme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-03 12:28:47.000000 palme-0.0.2/palme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-03 12:28:47.000000 palme-0.0.2/palme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:28:47.000000 palme-0.0.2/palme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 12:28:47.000000 palme-0.0.2/palme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:28:47.000000 palme-0.0.2/palme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:28:47.575534 palme-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-03 12:28:33.000000 palme-0.0.2/setup.py
```

### Comparing `palme-0.0.1/LICENSE` & `palme-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `palme-0.0.1/PKG-INFO` & `palme-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palme
-Version: 0.0.1
+Version: 0.0.2
 Summary: palme - Pytorch
 Home-page: https://github.com/kyegomez/palme
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `palme-0.0.1/palme.egg-info/PKG-INFO` & `palme-0.0.2/palme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palme
-Version: 0.0.1
+Version: 0.0.2
 Summary: palme - Pytorch
 Home-page: https://github.com/kyegomez/palme
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `palme-0.0.1/setup.py` & `palme-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'palme',
   packages = find_packages(exclude=['examples']),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'palme - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/palme',
   long_description_content_type = 'text/markdown',
   keywords = [
```

