# Comparing `tmp/general-superstaq-0.4.8.tar.gz` & `tmp/general-superstaq-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general-superstaq-0.4.8.tar", last modified: Fri Jul 28 17:44:10 2023, max compression
+gzip compressed data, was "general-superstaq-0.4.9.tar", last modified: Fri Jul 28 21:48:04 2023, max compression
```

## Comparing `general-superstaq-0.4.8.tar` & `general-superstaq-0.4.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:10.084422 general-superstaq-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 17:44:10.084422 general-superstaq-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:10.080422 general-superstaq-0.4.8/general_superstaq/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/_init_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/_version_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:10.084422 general-superstaq-0.4.8/general_superstaq/check/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/all_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/check_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/checks-pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/coverage_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/flake8_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/format_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/mypy_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/pylint_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/pytest_.py
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/qubo.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/qubo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/resource_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/resource_estimate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23178 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/superstaq_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25714 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/superstaq_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/superstaq_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/superstaq_exceptions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/validation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:10.080422 general-superstaq-0.4.8/general_superstaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 17:44:10.000000 general-superstaq-0.4.8/general_superstaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-28 17:44:10.000000 general-superstaq-0.4.8/general_superstaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:44:10.000000 general-superstaq-0.4.8/general_superstaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-28 17:44:10.000000 general-superstaq-0.4.8/general_superstaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 17:44:10.000000 general-superstaq-0.4.8/general_superstaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:44:10.084422 general-superstaq-0.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:04.966916 general-superstaq-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 21:48:04.966916 general-superstaq-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:04.962916 general-superstaq-0.4.9/general_superstaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/_init_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/_version_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:04.966916 general-superstaq-0.4.9/general_superstaq/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/all_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/check_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/checks-pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/coverage_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/flake8_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/format_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/mypy_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/pylint_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/pytest_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/check/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/qubo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/qubo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/resource_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/resource_estimate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23178 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/superstaq_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25714 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/superstaq_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/superstaq_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/superstaq_exceptions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/general_superstaq/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:48:04.962916 general-superstaq-0.4.9/general_superstaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 21:48:04.000000 general-superstaq-0.4.9/general_superstaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-28 21:48:04.000000 general-superstaq-0.4.9/general_superstaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:48:04.000000 general-superstaq-0.4.9/general_superstaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-28 21:48:04.000000 general-superstaq-0.4.9/general_superstaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 21:48:04.000000 general-superstaq-0.4.9/general_superstaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 21:47:42.000000 general-superstaq-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 21:48:04.966916 general-superstaq-0.4.9/setup.cfg
```

### Comparing `general-superstaq-0.4.8/PKG-INFO` & `general-superstaq-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general-superstaq
-Version: 0.4.8
+Version: 0.4.9
 Summary: The general module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `general-superstaq-0.4.8/general_superstaq/__init__.py` & `general-superstaq-0.4.9/general_superstaq/__init__.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/all_.py` & `general-superstaq-0.4.9/general_superstaq/check/all_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/build_docs.py` & `general-superstaq-0.4.9/general_superstaq/check/build_docs.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/check_utils.py` & `general-superstaq-0.4.9/general_superstaq/check/check_utils.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/checks-pyproject.toml` & `general-superstaq-0.4.9/general_superstaq/check/checks-pyproject.toml`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/configs.py` & `general-superstaq-0.4.9/general_superstaq/check/configs.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/coverage_.py` & `general-superstaq-0.4.9/general_superstaq/check/coverage_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/flake8_.py` & `general-superstaq-0.4.9/general_superstaq/check/flake8_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/format_.py` & `general-superstaq-0.4.9/general_superstaq/check/format_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/mypy_.py` & `general-superstaq-0.4.9/general_superstaq/check/mypy_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/pylint_.py` & `general-superstaq-0.4.9/general_superstaq/check/pylint_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/pytest_.py` & `general-superstaq-0.4.9/general_superstaq/check/pytest_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/check/requirements.py` & `general-superstaq-0.4.9/general_superstaq/check/requirements.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/qubo.py` & `general-superstaq-0.4.9/general_superstaq/qubo.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/qubo_test.py` & `general-superstaq-0.4.9/general_superstaq/qubo_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/resource_estimate.py` & `general-superstaq-0.4.9/general_superstaq/resource_estimate.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/serialization.py` & `general-superstaq-0.4.9/general_superstaq/serialization.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/service.py` & `general-superstaq-0.4.9/general_superstaq/service.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/service_test.py` & `general-superstaq-0.4.9/general_superstaq/service_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/superstaq_client.py` & `general-superstaq-0.4.9/general_superstaq/superstaq_client.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/superstaq_client_test.py` & `general-superstaq-0.4.9/general_superstaq/superstaq_client_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/superstaq_exceptions.py` & `general-superstaq-0.4.9/general_superstaq/superstaq_exceptions.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/superstaq_exceptions_test.py` & `general-superstaq-0.4.9/general_superstaq/superstaq_exceptions_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/typing.py` & `general-superstaq-0.4.9/general_superstaq/typing.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/validation.py` & `general-superstaq-0.4.9/general_superstaq/validation.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq/validation_test.py` & `general-superstaq-0.4.9/general_superstaq/validation_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/general_superstaq.egg-info/PKG-INFO` & `general-superstaq-0.4.9/general_superstaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general-superstaq
-Version: 0.4.8
+Version: 0.4.9
 Summary: The general module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `general-superstaq-0.4.8/general_superstaq.egg-info/SOURCES.txt` & `general-superstaq-0.4.9/general_superstaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.8/pyproject.toml` & `general-superstaq-0.4.9/pyproject.toml`

 * *Files identical despite different names*

