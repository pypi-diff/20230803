# Comparing `tmp/multilogue-0.0.6.tar.gz` & `tmp/multilogue-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multilogue-0.0.6.tar", last modified: Sat Jul 29 21:10:56 2023, max compression
+gzip compressed data, was "multilogue-0.0.7.tar", last modified: Thu Aug  3 14:11:24 2023, max compression
```

## Comparing `multilogue-0.0.6.tar` & `multilogue-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.955251 multilogue-0.0.6/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.6/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-07-29 21:10:56.955251 multilogue-0.0.6/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       55 2023-07-02 15:37:04.000000 multilogue-0.0.6/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      689 2023-07-29 20:15:07.000000 multilogue-0.0.6/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-29 21:10:56.955251 multilogue-0.0.6/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.951251 multilogue-0.0.6/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.951251 multilogue-0.0.6/src/multilogue/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-07-29 19:20:27.000000 multilogue-0.0.6/src/multilogue/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1244 2023-07-27 12:09:50.000000 multilogue-0.0.6/src/multilogue/entities.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-07-27 00:36:41.000000 multilogue-0.0.6/src/multilogue/participants.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.951251 multilogue-0.0.6/src/multilogue/utilities/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      246 2023-07-29 19:42:30.000000 multilogue-0.0.6/src/multilogue/utilities/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1762 2023-07-29 21:09:58.000000 multilogue-0.0.6/src/multilogue/utilities/chatgpt.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.951251 multilogue-0.0.6/src/multilogue.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-07-29 21:10:56.000000 multilogue-0.0.6/src/multilogue.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      402 2023-07-29 21:10:56.000000 multilogue-0.0.6/src/multilogue.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-29 21:10:56.000000 multilogue-0.0.6/src/multilogue.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       17 2023-07-29 21:10:56.000000 multilogue-0.0.6/src/multilogue.egg-info/requires.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-07-29 21:10:56.000000 multilogue-0.0.6/src/multilogue.egg-info/top_level.txt
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-29 21:10:56.951251 multilogue-0.0.6/tests/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      345 2023-07-27 12:09:50.000000 multilogue-0.0.6/tests/test_entities.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.596764 multilogue-0.0.7/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.7/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-08-03 14:11:24.596764 multilogue-0.0.7/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       55 2023-07-02 15:37:04.000000 multilogue-0.0.7/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      738 2023-08-03 00:19:59.000000 multilogue-0.0.7/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-08-03 14:11:24.596764 multilogue-0.0.7/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.592764 multilogue-0.0.7/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.592764 multilogue-0.0.7/src/multilogue/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-07-29 19:20:27.000000 multilogue-0.0.7/src/multilogue/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1244 2023-07-27 12:09:50.000000 multilogue-0.0.7/src/multilogue/entities.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-07-27 00:36:41.000000 multilogue-0.0.7/src/multilogue/participants.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.592764 multilogue-0.0.7/src/multilogue/utilities/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      439 2023-07-30 22:20:03.000000 multilogue-0.0.7/src/multilogue/utilities/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1849 2023-07-30 22:14:48.000000 multilogue-0.0.7/src/multilogue/utilities/chatgpt.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4562 2023-08-03 00:18:39.000000 multilogue-0.0.7/src/multilogue/utilities/githublog.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.592764 multilogue-0.0.7/src/multilogue.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-08-03 14:11:24.000000 multilogue-0.0.7/src/multilogue.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      440 2023-08-03 14:11:24.000000 multilogue-0.0.7/src/multilogue.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-08-03 14:11:24.000000 multilogue-0.0.7/src/multilogue.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       49 2023-08-03 14:11:24.000000 multilogue-0.0.7/src/multilogue.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-08-03 14:11:24.000000 multilogue-0.0.7/src/multilogue.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.592764 multilogue-0.0.7/tests/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      345 2023-07-27 12:09:50.000000 multilogue-0.0.7/tests/test_entities.py
```

### Comparing `multilogue-0.0.6/LICENSE` & `multilogue-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.6/PKG-INFO` & `multilogue-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilogue
-Version: 0.0.6
+Version: 0.0.7
 Summary: Multilogue
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/multilogue
 Project-URL: Bug Tracker, https://github.com/multilogue/multilogue/issues
 Keywords: multilogue,multilectic,conversation,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multilogue-0.0.6/pyproject.toml` & `multilogue-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "multilogue"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Multilogue"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
 ]
 keywords = ["multilogue", "multilectic", "conversation", "ai"]
 dependencies = [
     "requests >= 2.30.0",
+    "PyGithub >= 1.59.0",
+    "urllib3 >= 2.0.4"
 ]
 [project.urls]
 "Homepage" = "https://github.com/multilogue/multilogue"
 "Bug Tracker" = "https://github.com/multilogue/multilogue/issues"
```

### Comparing `multilogue-0.0.6/src/multilogue/entities.py` & `multilogue-0.0.7/src/multilogue/entities.py`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.6/src/multilogue/utilities/chatgpt.py` & `multilogue-0.0.7/src/multilogue/utilities/chatgpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 """Copyright (c) Alexander Fedotov.
 This source code is licensed under the license found in the
 LICENSE file in the root directory of this source tree.
 """
 from os import environ
 import requests
 
-api_key         = environ.get("OPENAI_API_KEY")
+api_key         = environ.get("OPENAI_API_KEY"
+                              )
 api_key_path    = environ.get("OPENAI_API_KEY_PATH")
 
 organization    = environ.get("OPENAI_ORGANIZATION")
+organization_id = environ.get("OPENAI_ORGANIZATION_ID")
 api_base        = environ.get("OPENAI_API_BASE", "https://api.openai.com/v1")
 api_type        = environ.get("OPENAI_API_TYPE", "open_ai")
 default_model   = environ.get("OPENAI_DEFAULT_MODEL", "gpt-3.5-turbo-0613")
 
 
 def answer( messages,
             functions=None,
```

### Comparing `multilogue-0.0.6/src/multilogue.egg-info/PKG-INFO` & `multilogue-0.0.7/src/multilogue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilogue
-Version: 0.0.6
+Version: 0.0.7
 Summary: Multilogue
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/multilogue
 Project-URL: Bug Tracker, https://github.com/multilogue/multilogue/issues
 Keywords: multilogue,multilectic,conversation,ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

