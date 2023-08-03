# Comparing `tmp/chalk-harness-1.1.8.tar.gz` & `tmp/chalk-harness-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalk-harness-1.1.8.tar", last modified: Thu Aug  3 18:52:32 2023, max compression
+gzip compressed data, was "chalk-harness-1.1.9.tar", last modified: Thu Aug  3 19:58:33 2023, max compression
```

## Comparing `chalk-harness-1.1.8.tar` & `chalk-harness-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:32.861335 chalk-harness-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 18:52:16.000000 chalk-harness-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 18:52:32.857335 chalk-harness-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 18:52:16.000000 chalk-harness-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:16.000000 chalk-harness-1.1.8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 18:52:16.000000 chalk-harness-1.1.8/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:32.857335 chalk-harness-1.1.8/chalk_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 18:52:32.000000 chalk-harness-1.1.8/chalk_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-03 18:52:32.000000 chalk-harness-1.1.8/chalk_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:52:32.000000 chalk-harness-1.1.8/chalk_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 18:52:32.000000 chalk-harness-1.1.8/chalk_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 18:52:32.000000 chalk-harness-1.1.8/chalk_harness.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:32.857335 chalk-harness-1.1.8/chalkharness/
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-03 18:52:16.000000 chalk-harness-1.1.8/chalkharness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:16.000000 chalk-harness-1.1.8/chalkharness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 18:52:16.000000 chalk-harness-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 18:52:32.861335 chalk-harness-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-03 18:52:16.000000 chalk-harness-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:32.857335 chalk-harness-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-03 18:52:16.000000 chalk-harness-1.1.8/tests/SanityTestCase.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:16.000000 chalk-harness-1.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:58:33.682510 chalk-harness-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-03 19:58:18.000000 chalk-harness-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 19:58:33.682510 chalk-harness-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-03 19:58:18.000000 chalk-harness-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:58:18.000000 chalk-harness-1.1.9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 19:58:18.000000 chalk-harness-1.1.9/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:58:33.682510 chalk-harness-1.1.9/chalk_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 19:58:33.000000 chalk-harness-1.1.9/chalk_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-03 19:58:33.000000 chalk-harness-1.1.9/chalk_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 19:58:33.000000 chalk-harness-1.1.9/chalk_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 19:58:33.000000 chalk-harness-1.1.9/chalk_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 19:58:33.000000 chalk-harness-1.1.9/chalk_harness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:58:33.682510 chalk-harness-1.1.9/chalkharness/
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-03 19:58:18.000000 chalk-harness-1.1.9/chalkharness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:58:18.000000 chalk-harness-1.1.9/chalkharness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 19:58:18.000000 chalk-harness-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 19:58:33.682510 chalk-harness-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-08-03 19:58:18.000000 chalk-harness-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 19:58:33.682510 chalk-harness-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-03 19:58:18.000000 chalk-harness-1.1.9/tests/SanityTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 19:58:18.000000 chalk-harness-1.1.9/tests/__init__.py
```

### Comparing `chalk-harness-1.1.8/PKG-INFO` & `chalk-harness-1.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalk-harness
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python wrapper for Chalk's CLI
 Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
```

### Comparing `chalk-harness-1.1.8/README.md` & `chalk-harness-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.1.8/chalk_harness.egg-info/PKG-INFO` & `chalk-harness-1.1.9/chalk_harness.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalk-harness
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python wrapper for Chalk's CLI
 Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
```

### Comparing `chalk-harness-1.1.8/chalkharness/__init__.py` & `chalk-harness-1.1.9/chalkharness/__init__.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.1.8/setup.py` & `chalk-harness-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.1.8/tests/SanityTestCase.py` & `chalk-harness-1.1.9/tests/SanityTestCase.py`

 * *Files identical despite different names*

