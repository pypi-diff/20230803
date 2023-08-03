# Comparing `tmp/ABCParse-0.0.6.tar.gz` & `tmp/ABCParse-0.0.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABCParse-0.0.6.tar", last modified: Thu Aug  3 02:51:32 2023, max compression
+gzip compressed data, was "ABCParse-0.0.6rc0.tar", last modified: Tue Aug  1 03:27:40 2023, max compression
```

## Comparing `ABCParse-0.0.6.tar` & `ABCParse-0.0.6rc0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:51:32.372701 ABCParse-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:51:32.368701 ABCParse-0.0.6/ABCParse/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 02:51:21.000000 ABCParse-0.0.6/ABCParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-03 02:51:21.000000 ABCParse-0.0.6/ABCParse/_abc_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-03 02:51:21.000000 ABCParse-0.0.6/ABCParse/_function_kwargs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 02:51:32.372701 ABCParse-0.0.6/ABCParse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-03 02:51:32.000000 ABCParse-0.0.6/ABCParse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-03 02:51:32.000000 ABCParse-0.0.6/ABCParse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 02:51:32.000000 ABCParse-0.0.6/ABCParse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 02:51:32.000000 ABCParse-0.0.6/ABCParse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-03 02:51:21.000000 ABCParse-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-03 02:51:32.372701 ABCParse-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-03 02:51:21.000000 ABCParse-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 02:51:32.372701 ABCParse-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-03 02:51:21.000000 ABCParse-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:27:40.781231 ABCParse-0.0.6rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:27:40.781231 ABCParse-0.0.6rc0/ABCParse/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 03:27:28.000000 ABCParse-0.0.6rc0/ABCParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-01 03:27:28.000000 ABCParse-0.0.6rc0/ABCParse/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-08-01 03:27:28.000000 ABCParse-0.0.6rc0/ABCParse/_function_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 03:27:40.781231 ABCParse-0.0.6rc0/ABCParse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 03:27:40.000000 ABCParse-0.0.6rc0/ABCParse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-01 03:27:40.000000 ABCParse-0.0.6rc0/ABCParse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 03:27:40.000000 ABCParse-0.0.6rc0/ABCParse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 03:27:40.000000 ABCParse-0.0.6rc0/ABCParse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-01 03:27:28.000000 ABCParse-0.0.6rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 03:27:40.781231 ABCParse-0.0.6rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-08-01 03:27:28.000000 ABCParse-0.0.6rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 03:27:40.781231 ABCParse-0.0.6rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-01 03:27:28.000000 ABCParse-0.0.6rc0/setup.py
```

### Comparing `ABCParse-0.0.6/ABCParse/_abc_parse.py` & `ABCParse-0.0.6rc0/ABCParse/_abc_parse.py`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.6/ABCParse/_function_kwargs.py` & `ABCParse-0.0.6rc0/ABCParse/_function_kwargs.py`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.6/ABCParse.egg-info/PKG-INFO` & `ABCParse-0.0.6rc0/ABCParse.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ABCParse
-Version: 0.0.6
+Version: 0.0.6rc0
 Summary: A better base class to automatically parse local args.
 Author: Michael E. Vinyard
-Author-email: mvinyard.ai@gmail.com
+Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `ABCParse-0.0.6/LICENSE` & `ABCParse-0.0.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.6/PKG-INFO` & `ABCParse-0.0.6rc0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ABCParse
-Version: 0.0.6
+Version: 0.0.6rc0
 Summary: A better base class to automatically parse local args.
 Author: Michael E. Vinyard
-Author-email: mvinyard.ai@gmail.com
+Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `ABCParse-0.0.6/README.md` & `ABCParse-0.0.6rc0/README.md`

 * *Files identical despite different names*

