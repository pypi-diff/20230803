# Comparing `tmp/kedro-telemetry-0.2.4.tar.gz` & `tmp/kedro-telemetry-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-telemetry-0.2.4.tar", last modified: Wed Apr  5 15:33:13 2023, max compression
+gzip compressed data, was "kedro-telemetry-0.2.5.tar", last modified: Thu Aug  3 11:04:23 2023, max compression
```

## Comparing `kedro-telemetry-0.2.4.tar` & `kedro-telemetry-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 15:33:13.304784 kedro-telemetry-0.2.4/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5142 2023-04-05 15:33:13.304784 kedro-telemetry-0.2.4/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4847 2023-04-05 15:32:08.000000 kedro-telemetry-0.2.4/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 15:33:13.304784 kedro-telemetry-0.2.4/kedro_telemetry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-04-05 15:32:08.000000 kedro-telemetry-0.2.4/kedro_telemetry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-04-05 15:32:08.000000 kedro-telemetry-0.2.4/kedro_telemetry/masking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9466 2023-04-05 15:32:08.000000 kedro-telemetry-0.2.4/kedro_telemetry/plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 15:33:13.304784 kedro-telemetry-0.2.4/kedro_telemetry.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5142 2023-04-05 15:33:13.000000 kedro-telemetry-0.2.4/kedro_telemetry.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      431 2023-04-05 15:33:13.000000 kedro-telemetry-0.2.4/kedro_telemetry.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-05 15:33:13.000000 kedro-telemetry-0.2.4/kedro_telemetry.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      139 2023-04-05 15:33:13.000000 kedro-telemetry-0.2.4/kedro_telemetry.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-05 15:33:13.000000 kedro-telemetry-0.2.4/kedro_telemetry.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-04-05 15:33:13.000000 kedro-telemetry-0.2.4/kedro_telemetry.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       16 2023-04-05 15:33:13.000000 kedro-telemetry-0.2.4/kedro_telemetry.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      167 2023-04-05 15:32:08.000000 kedro-telemetry-0.2.4/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       38 2023-04-05 15:33:13.304784 kedro-telemetry-0.2.4/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1309 2023-04-05 15:32:08.000000 kedro-telemetry-0.2.4/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-05 15:33:13.304784 kedro-telemetry-0.2.4/tests/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8026 2023-04-05 15:32:08.000000 kedro-telemetry-0.2.4/tests/test_masking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16674 2023-04-05 15:32:08.000000 kedro-telemetry-0.2.4/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:04:23.207164 kedro-telemetry-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-08-03 11:04:23.207164 kedro-telemetry-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-08-03 11:04:05.000000 kedro-telemetry-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:04:23.207164 kedro-telemetry-0.2.5/kedro_telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-03 11:04:05.000000 kedro-telemetry-0.2.5/kedro_telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-08-03 11:04:05.000000 kedro-telemetry-0.2.5/kedro_telemetry/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-08-03 11:04:05.000000 kedro-telemetry-0.2.5/kedro_telemetry/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:04:23.207164 kedro-telemetry-0.2.5/kedro_telemetry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-08-03 11:04:23.000000 kedro-telemetry-0.2.5/kedro_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 11:04:23.000000 kedro-telemetry-0.2.5/kedro_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:04:23.000000 kedro-telemetry-0.2.5/kedro_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 11:04:23.000000 kedro-telemetry-0.2.5/kedro_telemetry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:04:22.000000 kedro-telemetry-0.2.5/kedro_telemetry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 11:04:23.000000 kedro-telemetry-0.2.5/kedro_telemetry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 11:04:23.000000 kedro-telemetry-0.2.5/kedro_telemetry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-08-03 11:04:05.000000 kedro-telemetry-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:04:23.207164 kedro-telemetry-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:04:23.207164 kedro-telemetry-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-08-03 11:04:05.000000 kedro-telemetry-0.2.5/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16674 2023-08-03 11:04:05.000000 kedro-telemetry-0.2.5/tests/test_plugin.py
```

### Comparing `kedro-telemetry-0.2.4/PKG-INFO` & `kedro-telemetry-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: kedro-telemetry
-Version: 0.2.4
+Version: 0.2.5
 Summary: Kedro-Telemetry
-Home-page: https://github.com/kedro-org/kedro-plugins/tree/main/kedro-telemetry
 Author: Kedro
 License: Apache Software License (Apache 2.0)
-Requires-Python: >=3.7, <3.11
+Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-telemetry
+Project-URL: Documentation, https://github.com/kedro-org/kedro-plugins/blob/main/kedro-telemetry/README.md
+Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 
 # Kedro-Telemetry
 
 [![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-telemetry/)
 [![PyPI version](https://badge.fury.io/py/kedro-telemetry.svg)](https://pypi.org/project/kedro-telemetry/)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
```

### Comparing `kedro-telemetry-0.2.4/README.md` & `kedro-telemetry-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `kedro-telemetry-0.2.4/kedro_telemetry/masking.py` & `kedro-telemetry-0.2.5/kedro_telemetry/masking.py`

 * *Files identical despite different names*

### Comparing `kedro-telemetry-0.2.4/kedro_telemetry/plugin.py` & `kedro-telemetry-0.2.5/kedro_telemetry/plugin.py`

 * *Files identical despite different names*

### Comparing `kedro-telemetry-0.2.4/kedro_telemetry.egg-info/PKG-INFO` & `kedro-telemetry-0.2.5/kedro_telemetry.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: kedro-telemetry
-Version: 0.2.4
+Version: 0.2.5
 Summary: Kedro-Telemetry
-Home-page: https://github.com/kedro-org/kedro-plugins/tree/main/kedro-telemetry
 Author: Kedro
 License: Apache Software License (Apache 2.0)
-Requires-Python: >=3.7, <3.11
+Project-URL: Source, https://github.com/kedro-org/kedro-plugins/tree/main/kedro-telemetry
+Project-URL: Documentation, https://github.com/kedro-org/kedro-plugins/blob/main/kedro-telemetry/README.md
+Project-URL: Tracker, https://github.com/kedro-org/kedro-plugins/issues
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 
 # Kedro-Telemetry
 
 [![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue.svg)](https://pypi.org/project/kedro-telemetry/)
 [![PyPI version](https://badge.fury.io/py/kedro-telemetry.svg)](https://pypi.org/project/kedro-telemetry/)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
```

### Comparing `kedro-telemetry-0.2.4/tests/test_masking.py` & `kedro-telemetry-0.2.5/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `kedro-telemetry-0.2.4/tests/test_plugin.py` & `kedro-telemetry-0.2.5/tests/test_plugin.py`

 * *Files identical despite different names*

