# Comparing `tmp/pymeten-0.0.2.tar.gz` & `tmp/pymeten-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeten-0.0.2.tar", last modified: Mon Jul 17 12:29:50 2023, max compression
+gzip compressed data, was "pymeten-0.0.3.tar", last modified: Thu Aug  3 11:22:08 2023, max compression
```

## Comparing `pymeten-0.0.2.tar` & `pymeten-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-17 12:29:50.688396 pymeten-0.0.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2023-07-17 12:29:50.688396 pymeten-0.0.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-07-17 12:29:50.000000 pymeten-0.0.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-17 12:29:50.688396 pymeten-0.0.2/pymeten/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-17 12:29:50.000000 pymeten-0.0.2/pymeten/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1859 2023-07-17 12:29:50.000000 pymeten-0.0.2/pymeten/itutils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-17 12:29:50.688396 pymeten-0.0.2/pymeten.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2023-07-17 12:29:50.000000 pymeten-0.0.2/pymeten.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-07-17 12:29:50.000000 pymeten-0.0.2/pymeten.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-17 12:29:50.000000 pymeten-0.0.2/pymeten.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-07-17 12:29:50.000000 pymeten-0.0.2/pymeten.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-07-17 12:29:50.000000 pymeten-0.0.2/pymeten.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-17 12:29:50.688396 pymeten-0.0.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      830 2023-07-17 12:29:50.000000 pymeten-0.0.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 11:22:08.516557 pymeten-0.0.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2023-08-03 11:22:08.516557 pymeten-0.0.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      780 2023-08-03 11:22:08.000000 pymeten-0.0.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 11:22:08.516557 pymeten-0.0.3/pymeten/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-08-03 11:22:08.000000 pymeten-0.0.3/pymeten/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3803 2023-08-03 11:22:08.000000 pymeten-0.0.3/pymeten/itutils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 11:22:08.516557 pymeten-0.0.3/pymeten.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2023-08-03 11:22:08.000000 pymeten-0.0.3/pymeten.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-08-03 11:22:08.000000 pymeten-0.0.3/pymeten.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 11:22:08.000000 pymeten-0.0.3/pymeten.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2023-08-03 11:22:08.000000 pymeten-0.0.3/pymeten.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-03 11:22:08.000000 pymeten-0.0.3/pymeten.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-03 11:22:08.516557 pymeten-0.0.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2023-08-03 11:22:08.000000 pymeten-0.0.3/setup.py
```

### Comparing `pymeten-0.0.2/setup.py` & `pymeten-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A tool for metrics of tensors'
 LONG_DESCRIPTION = 'Measure the different aspects of your tensor program efficiency'
 
 requirements = []
 devRequirements = [
     'numpy==1.25.1',
-    'pytest'
+    'sphinx',
+    'sphinx_rtd_theme',
+    'pytest',
 ]
 
 setup(
     name="pymeten",
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

