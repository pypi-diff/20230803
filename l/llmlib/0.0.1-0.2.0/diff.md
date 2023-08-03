# Comparing `tmp/llmlib-0.0.1.tar.gz` & `tmp/llmlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmlib-0.0.1.tar", last modified: Thu Aug  3 15:50:28 2023, max compression
+gzip compressed data, was "llmlib-0.2.0.tar", last modified: Thu Aug  3 16:02:52 2023, max compression
```

## Comparing `llmlib-0.0.1.tar` & `llmlib-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 markwatson   (501) staff       (20)        0 2023-08-03 15:50:28.279633 llmlib-0.0.1/
--rw-r--r--   0 markwatson   (501) staff       (20)    11357 2023-07-01 17:56:05.000000 llmlib-0.0.1/LICENSE
--rw-r--r--   0 markwatson   (501) staff       (20)     2159 2023-08-03 15:50:28.279500 llmlib-0.0.1/PKG-INFO
--rw-r--r--   0 markwatson   (501) staff       (20)     1509 2023-08-03 15:47:20.000000 llmlib-0.0.1/README.md
-drwxr-xr-x   0 markwatson   (501) staff       (20)        0 2023-08-03 15:50:28.278664 llmlib-0.0.1/llmlib/
--rw-r--r--   0 markwatson   (501) staff       (20)      484 2023-07-07 18:06:51.000000 llmlib-0.0.1/llmlib/base_model_wrapper.py
--rw-r--r--   0 markwatson   (501) staff       (20)     3261 2023-08-03 15:28:32.000000 llmlib-0.0.1/llmlib/huggingface.py
--rw-r--r--   0 markwatson   (501) staff       (20)     2966 2023-07-07 18:07:04.000000 llmlib-0.0.1/llmlib/openai.py
-drwxr-xr-x   0 markwatson   (501) staff       (20)        0 2023-08-03 15:50:28.279347 llmlib-0.0.1/llmlib.egg-info/
--rw-r--r--   0 markwatson   (501) staff       (20)     2159 2023-08-03 15:50:28.000000 llmlib-0.0.1/llmlib.egg-info/PKG-INFO
--rw-r--r--   0 markwatson   (501) staff       (20)      258 2023-08-03 15:50:28.000000 llmlib-0.0.1/llmlib.egg-info/SOURCES.txt
--rw-r--r--   0 markwatson   (501) staff       (20)        1 2023-08-03 15:50:28.000000 llmlib-0.0.1/llmlib.egg-info/dependency_links.txt
--rw-r--r--   0 markwatson   (501) staff       (20)        7 2023-08-03 15:50:28.000000 llmlib-0.0.1/llmlib.egg-info/requires.txt
--rw-r--r--   0 markwatson   (501) staff       (20)        7 2023-08-03 15:50:28.000000 llmlib-0.0.1/llmlib.egg-info/top_level.txt
--rw-r--r--   0 markwatson   (501) staff       (20)      529 2023-07-01 18:34:52.000000 llmlib-0.0.1/pyproject.toml
--rw-r--r--   0 markwatson   (501) staff       (20)       38 2023-08-03 15:50:28.279677 llmlib-0.0.1/setup.cfg
--rw-r--r--   0 markwatson   (501) staff       (20)      947 2023-07-01 18:05:06.000000 llmlib-0.0.1/setup.py
+drwxr-xr-x   0 markwatson   (501) staff       (20)        0 2023-08-03 16:02:52.629013 llmlib-0.2.0/
+-rw-r--r--   0 markwatson   (501) staff       (20)    11357 2023-07-01 17:56:05.000000 llmlib-0.2.0/LICENSE
+-rw-r--r--   0 markwatson   (501) staff       (20)     2159 2023-08-03 16:02:52.628880 llmlib-0.2.0/PKG-INFO
+-rw-r--r--   0 markwatson   (501) staff       (20)     1509 2023-08-03 15:47:20.000000 llmlib-0.2.0/README.md
+drwxr-xr-x   0 markwatson   (501) staff       (20)        0 2023-08-03 16:02:52.628071 llmlib-0.2.0/llmlib/
+-rw-r--r--   0 markwatson   (501) staff       (20)      484 2023-07-07 18:06:51.000000 llmlib-0.2.0/llmlib/base_model_wrapper.py
+-rw-r--r--   0 markwatson   (501) staff       (20)     3261 2023-08-03 15:28:32.000000 llmlib-0.2.0/llmlib/huggingface.py
+-rw-r--r--   0 markwatson   (501) staff       (20)     2966 2023-07-07 18:07:04.000000 llmlib-0.2.0/llmlib/openai.py
+drwxr-xr-x   0 markwatson   (501) staff       (20)        0 2023-08-03 16:02:52.628730 llmlib-0.2.0/llmlib.egg-info/
+-rw-r--r--   0 markwatson   (501) staff       (20)     2159 2023-08-03 16:02:52.000000 llmlib-0.2.0/llmlib.egg-info/PKG-INFO
+-rw-r--r--   0 markwatson   (501) staff       (20)      258 2023-08-03 16:02:52.000000 llmlib-0.2.0/llmlib.egg-info/SOURCES.txt
+-rw-r--r--   0 markwatson   (501) staff       (20)        1 2023-08-03 16:02:52.000000 llmlib-0.2.0/llmlib.egg-info/dependency_links.txt
+-rw-r--r--   0 markwatson   (501) staff       (20)        7 2023-08-03 16:02:52.000000 llmlib-0.2.0/llmlib.egg-info/requires.txt
+-rw-r--r--   0 markwatson   (501) staff       (20)        7 2023-08-03 16:02:52.000000 llmlib-0.2.0/llmlib.egg-info/top_level.txt
+-rw-r--r--   0 markwatson   (501) staff       (20)      529 2023-08-03 16:02:21.000000 llmlib-0.2.0/pyproject.toml
+-rw-r--r--   0 markwatson   (501) staff       (20)       38 2023-08-03 16:02:52.629060 llmlib-0.2.0/setup.cfg
+-rw-r--r--   0 markwatson   (501) staff       (20)      946 2023-08-03 16:02:12.000000 llmlib-0.2.0/setup.py
```

### Comparing `llmlib-0.0.1/LICENSE` & `llmlib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmlib-0.0.1/PKG-INFO` & `llmlib-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmlib
-Version: 0.0.1
+Version: 0.2.0
 Summary: Portability lib for OpenAI, Hugging Face, and FastChat local model APIs
 Home-page: https://github.com/mark-watson/llmlib
 Author: Mark Watson
 Author-email: Mark Watson <markw@markwatson.com>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/mark-watson/llmlib
 Project-URL: Bug Tracker, https://github.com/mark-watson/llmlib/issues
```

### Comparing `llmlib-0.0.1/README.md` & `llmlib-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `llmlib-0.0.1/llmlib/huggingface.py` & `llmlib-0.2.0/llmlib/huggingface.py`

 * *Files identical despite different names*

### Comparing `llmlib-0.0.1/llmlib/openai.py` & `llmlib-0.2.0/llmlib/openai.py`

 * *Files identical despite different names*

### Comparing `llmlib-0.0.1/llmlib.egg-info/PKG-INFO` & `llmlib-0.2.0/llmlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmlib
-Version: 0.0.1
+Version: 0.2.0
 Summary: Portability lib for OpenAI, Hugging Face, and FastChat local model APIs
 Home-page: https://github.com/mark-watson/llmlib
 Author: Mark Watson
 Author-email: Mark Watson <markw@markwatson.com>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/mark-watson/llmlib
 Project-URL: Bug Tracker, https://github.com/mark-watson/llmlib/issues
```

### Comparing `llmlib-0.0.1/pyproject.toml` & `llmlib-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmlib"
-version = "0.0.1"
+version = "0.2.0"
 authors = [
   { name="Mark Watson", email="markw@markwatson.com" },
 ]
 description = "Portability lib for OpenAI, Hugging Face, and FastChat local model APIs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `llmlib-0.0.1/setup.py` & `llmlib-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.01"
+VERSION = "0.2"
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
         return fp.read()
```

