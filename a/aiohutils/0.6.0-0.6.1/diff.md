# Comparing `tmp/aiohutils-0.6.0.tar.gz` & `tmp/aiohutils-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohutils-0.6.0.tar", last modified: Thu Aug  3 06:59:06 2023, max compression
+gzip compressed data, was "aiohutils-0.6.1.tar", last modified: Thu Aug  3 07:04:40 2023, max compression
```

## Comparing `aiohutils-0.6.0.tar` & `aiohutils-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 06:59:06.551817 aiohutils-0.6.0/
--rw-rw-rw-   0        0        0      512 2023-08-03 06:59:06.550932 aiohutils-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-08-03 06:55:23.000000 aiohutils-0.6.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-03 06:59:06.532747 aiohutils-0.6.0/aiohutils/
--rw-rw-rw-   0        0        0       22 2023-08-03 06:59:03.000000 aiohutils-0.6.0/aiohutils/__init__.py
--rw-rw-rw-   0        0        0     1304 2023-08-03 06:48:56.000000 aiohutils-0.6.0/aiohutils/session.py
--rw-rw-rw-   0        0        0     2960 2023-08-03 06:48:10.000000 aiohutils-0.6.0/aiohutils/tests.py
-drwxrwxrwx   0        0        0        0 2023-08-03 06:59:06.541725 aiohutils-0.6.0/aiohutils.egg-info/
--rw-rw-rw-   0        0        0      512 2023-08-03 06:59:06.000000 aiohutils-0.6.0/aiohutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-03 06:59:06.000000 aiohutils-0.6.0/aiohutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 06:59:06.000000 aiohutils-0.6.0/aiohutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-08-03 06:59:06.000000 aiohutils-0.6.0/aiohutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-03 06:59:06.000000 aiohutils-0.6.0/aiohutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-08-03 06:59:05.000000 aiohutils-0.6.0/aiohutils.egg-info/zip-safe
--rw-rw-rw-   0        0        0      976 2023-08-03 04:08:05.000000 aiohutils-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 06:59:06.552815 aiohutils-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 07:04:40.211690 aiohutils-0.6.1/
+-rw-rw-rw-   0        0        0      503 2023-08-03 07:04:40.210693 aiohutils-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-08-03 06:55:23.000000 aiohutils-0.6.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-03 07:04:40.202715 aiohutils-0.6.1/aiohutils/
+-rw-rw-rw-   0        0        0       22 2023-08-03 07:04:37.000000 aiohutils-0.6.1/aiohutils/__init__.py
+-rw-rw-rw-   0        0        0     1304 2023-08-03 06:48:56.000000 aiohutils-0.6.1/aiohutils/session.py
+-rw-rw-rw-   0        0        0     2956 2023-08-03 07:04:03.000000 aiohutils-0.6.1/aiohutils/tests.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:04:40.209695 aiohutils-0.6.1/aiohutils.egg-info/
+-rw-rw-rw-   0        0        0      503 2023-08-03 07:04:40.000000 aiohutils-0.6.1/aiohutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-03 07:04:40.000000 aiohutils-0.6.1/aiohutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:04:40.000000 aiohutils-0.6.1/aiohutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-08-03 07:04:40.000000 aiohutils-0.6.1/aiohutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 07:04:40.000000 aiohutils-0.6.1/aiohutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-03 06:59:05.000000 aiohutils-0.6.1/aiohutils.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      967 2023-08-03 07:01:19.000000 aiohutils-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:04:40.211690 aiohutils-0.6.1/setup.cfg
```

### Comparing `aiohutils-0.6.0/aiohutils/session.py` & `aiohutils-0.6.1/aiohutils/session.py`

 * *Files identical despite different names*

### Comparing `aiohutils-0.6.0/aiohutils/tests.py` & `aiohutils-0.6.1/aiohutils/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from itertools import cycle
 from typing import Iterator
 from unittest.mock import patch
 
 from decouple import config
 from pytest import fixture
 
-from aiohutils.session import _SessionManager
+from aiohutils.session import SessionManager
 
 RECORD_MODE = OFFLINE_MODE = TESTS_PATH = REMOVE_UNUSED_TESTDATA = None
 
 
 def init_tests():
     global RECORD_MODE, OFFLINE_MODE, TESTS_PATH, REMOVE_UNUSED_TESTDATA
 
@@ -49,20 +49,20 @@
     if OFFLINE_MODE:
 
         class FakeSession:
             @staticmethod
             async def get(*_, **__):
                 return FakeResponse()
 
-        _SessionManager.session = FakeSession()
+        SessionManager.session = FakeSession()
         yield
-        del _SessionManager.session
+        del SessionManager.session
         return
 
-    sm = _SessionManager()
+    sm = SessionManager()
 
     if RECORD_MODE:
         original_get = sm.get
 
         async def recording_get(*args, **kwargs):
             resp = await original_get(*args, **kwargs)
             content = await resp.read()
```

### Comparing `aiohutils-0.6.0/pyproject.toml` & `aiohutils-0.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=66.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiohutils"
 authors = [{name = "5j9", email = "5j9@users.noreply.github.com"}]
 license = {text = "GNU General Public License v3 (GPLv3)"}
-description = "a small library used for testing aiohttp projects"
+description = "A small library to for aiohttp projects."
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.10",
 ]
 requires-python = ">=3.10"
 dependencies = [
     "pytest",
```

