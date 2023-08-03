# Comparing `tmp/aind_codeocean_api-0.2.3.tar.gz` & `tmp/aind_codeocean_api-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_codeocean_api-0.2.3.tar", last modified: Fri Jun 30 23:24:53 2023, max compression
+gzip compressed data, was "aind_codeocean_api-0.2.4.tar", last modified: Thu Aug  3 17:02:21 2023, max compression
```

## Comparing `aind_codeocean_api-0.2.3.tar` & `aind_codeocean_api-0.2.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.207109 aind_codeocean_api-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.211109 aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.211109 aind_codeocean_api-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.211109 aind_codeocean_api-0.2.3/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/aind_codeocean_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.207109 aind_codeocean_api-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/src/aind_codeocean_api/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-30 23:24:38.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20676 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api/codeocean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-30 23:24:53.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-30 23:24:53.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 23:24:53.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-30 23:24:53.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 23:24:53.000000 aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:24:53.215109 aind_codeocean_api-0.2.3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/tests/resources/fake_credentials.json
--rw-r--r--   0 runner    (1001) docker     (123)    28173 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/tests/test_codeocean_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-30 23:24:37.000000 aind_codeocean_api-0.2.3/tests/test_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.388740 aind_codeocean_api-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.380740 aind_codeocean_api-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.384739 aind_codeocean_api-0.2.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.384739 aind_codeocean_api-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-03 17:02:21.388740 aind_codeocean_api-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.384739 aind_codeocean_api-0.2.4/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.384739 aind_codeocean_api-0.2.4/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.384739 aind_codeocean_api-0.2.4/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   259838 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/doc_template/source/aind_codeocean_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 17:02:21.388740 aind_codeocean_api-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.380740 aind_codeocean_api-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.384739 aind_codeocean_api-0.2.4/src/aind_codeocean_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 17:02:00.000000 aind_codeocean_api-0.2.4/src/aind_codeocean_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21442 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/src/aind_codeocean_api/codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/src/aind_codeocean_api/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.388740 aind_codeocean_api-0.2.4/src/aind_codeocean_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-03 17:02:21.000000 aind_codeocean_api-0.2.4/src/aind_codeocean_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-03 17:02:21.000000 aind_codeocean_api-0.2.4/src/aind_codeocean_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 17:02:21.000000 aind_codeocean_api-0.2.4/src/aind_codeocean_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 17:02:21.000000 aind_codeocean_api-0.2.4/src/aind_codeocean_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 17:02:21.000000 aind_codeocean_api-0.2.4/src/aind_codeocean_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.388740 aind_codeocean_api-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 17:02:21.388740 aind_codeocean_api-0.2.4/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/tests/resources/fake_credentials.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28636 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/tests/test_codeocean_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-08-03 17:01:59.000000 aind_codeocean_api-0.2.4/tests/test_credentials.py
```

### Comparing `aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_codeocean_api-0.2.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_codeocean_api-0.2.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/.github/ISSUE_TEMPLATE/user-story.md` & `aind_codeocean_api-0.2.4/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/.github/workflows/lint_and_test.yml` & `aind_codeocean_api-0.2.4/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/.github/workflows/tag_and_publish.yml` & `aind_codeocean_api-0.2.4/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/.gitignore` & `aind_codeocean_api-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/LICENSE` & `aind_codeocean_api-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/PKG-INFO` & `aind_codeocean_api-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_codeocean_api
-Version: 0.2.3
+Version: 0.2.4
 Summary: CodeOcean API manager in Python
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_codeocean_api-0.2.3/README.md` & `aind_codeocean_api-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/doc_template/Makefile` & `aind_codeocean_api-0.2.4/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/doc_template/make.bat` & `aind_codeocean_api-0.2.4/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/doc_template/source/_static/dark-logo.svg` & `aind_codeocean_api-0.2.4/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/doc_template/source/_static/favicon.ico` & `aind_codeocean_api-0.2.4/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/doc_template/source/_static/light-logo.svg` & `aind_codeocean_api-0.2.4/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/doc_template/source/aind_codeocean_api.rst` & `aind_codeocean_api-0.2.4/doc_template/source/aind_codeocean_api.rst`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/doc_template/source/conf.py` & `aind_codeocean_api-0.2.4/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/pyproject.toml` & `aind_codeocean_api-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 readme = "README.md"
 dynamic = ["version"]
 
 dependencies = [
-    'requests'
+    'requests',
+    'pydantic<2.0',
+    'boto3'
 ]
 
 [project.optional-dependencies]
 dev = [
     'black',
     'coverage',
     'flake8',
```

### Comparing `aind_codeocean_api-0.2.3/src/aind_codeocean_api/codeocean.py` & `aind_codeocean_api-0.2.4/src/aind_codeocean_api/codeocean.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import logging
 from enum import Enum
 from inspect import signature
 from typing import Dict, List, Optional
 
 import requests
 
+from aind_codeocean_api.credentials import CodeOceanCredentials
+
 
 class CodeOceanClient:
     """Client that will connect to Code Ocean"""
 
     _MAX_SEARCH_BATCH_REQUEST = 1000
 
     class _URLStrings(Enum):
@@ -61,31 +63,60 @@
         domain : str
             VPC domain
         token : str
             API token
         api_version : int
             Code Ocean API version
         """
-        self.domain = domain
+        self.domain = domain.strip("/")
         self.token = token
         self.api_version = api_version
         self.logger = logging.getLogger("aind-codeocean-api")
-        self.asset_url = (
+
+    @property
+    def asset_url(self):
+        """Asset url property."""
+        return (
             f"{self.domain}/api/v{self.api_version}/"
             f"{self._URLStrings.DATA_ASSETS.value}"
         )
-        self.capsule_url = (
+
+    @property
+    def capsule_url(self):
+        """Capsule url property."""
+        return (
             f"{self.domain}/api/v{self.api_version}/"
             f"{self._URLStrings.CAPSULES.value}"
         )
-        self.computation_url = (
+
+    @property
+    def computation_url(self):
+        """Computation url property."""
+        return (
             f"{self.domain}/api/v{self.api_version}/"
             f"{self._URLStrings.COMPUTATIONS.value}"
         )
 
+    @classmethod
+    def from_credentials(
+        cls, credentials: CodeOceanCredentials, api_version: int = 1
+    ):
+        """
+        Create client using credentials object.
+        Parameters
+        ----------
+        credentials : CodeOceanCredentials
+        api_version :
+          Code Ocean API version
+
+        """
+        domain = credentials.domain
+        token = credentials.token.get_secret_value()
+        return cls(domain=domain, token=token, api_version=api_version)
+
     def get_data_asset(self, data_asset_id: str) -> requests.models.Response:
         """
         This will get data from a GET request to Code Ocean API.
 
         Parameters
         ---------------
         data_asset_id : string
```

### Comparing `aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/PKG-INFO` & `aind_codeocean_api-0.2.4/src/aind_codeocean_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-codeocean-api
-Version: 0.2.3
+Version: 0.2.4
 Summary: CodeOcean API manager in Python
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_codeocean_api-0.2.3/src/aind_codeocean_api.egg-info/SOURCES.txt` & `aind_codeocean_api-0.2.4/src/aind_codeocean_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.2.3/tests/test_codeocean_requests.py` & `aind_codeocean_api-0.2.4/tests/test_codeocean_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any, Callable, List
 from unittest import mock
 from unittest.mock import call
 
 import requests
 
 from aind_codeocean_api.codeocean import CodeOceanClient
+from aind_codeocean_api.credentials import CodeOceanCredentials
 
 
 class MockResponse:
     """Mocks a rest request response"""
 
     def __init__(self, content: dict, status_code: int, url: str) -> None:
         """
@@ -154,14 +155,22 @@
             prefix=prefix,
             access_key_id=access_key_id,
             secret_access_key=secret_access_key,
         )
         self.assertEqual(response.content, expected_request_response)
         self.assertEqual(response.status_code, 200)
 
+    def test_create_from_credentials(self):
+        """Tests that the client can be constructed from a
+        CodeOceanCredentials object"""
+        creds = CodeOceanCredentials(domain="some_domain", token="some_token")
+        client = CodeOceanClient.from_credentials(credentials=creds)
+        self.assertEqual("some_domain", client.domain)
+        self.assertEqual("some_token", client.token)
+
     @mock.patch("requests.get")
     def test_get_data_asset(
         self, mock_api_get: unittest.mock.MagicMock
     ) -> None:
         """Tests get_data_asset method."""
 
         def map_to_success_message(url: str) -> dict:
```

