# Comparing `tmp/lares-0.0.1.tar.gz` & `tmp/lares-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lares-0.0.1.tar", last modified: Thu Aug  3 03:40:43 2023, max compression
+gzip compressed data, was "lares-0.0.2.tar", last modified: Thu Aug  3 05:23:13 2023, max compression
```

## Comparing `lares-0.0.1.tar` & `lares-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 03:40:43.288094 lares-0.0.1/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-08-03 03:26:16.000000 lares-0.0.1/LICENSE
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-08-03 03:26:16.000000 lares-0.0.1/MANIFEST.in
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 03:40:43.288094 lares-0.0.1/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       65 2023-08-03 03:28:06.000000 lares-0.0.1/README.md
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 03:40:43.284094 lares-0.0.1/__pycache__/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     2802 2023-08-03 03:26:16.000000 lares-0.0.1/__pycache__/inviz.cpython-310.pyc
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 03:40:43.284094 lares-0.0.1/lares/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1645 2023-08-03 03:33:01.000000 lares-0.0.1/lares/evaluate.py
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 03:40:43.288094 lares-0.0.1/lares/lares.egg-info/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 03:40:43.000000 lares-0.0.1/lares/lares.egg-info/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      297 2023-08-03 03:40:43.000000 lares-0.0.1/lares/lares.egg-info/SOURCES.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-08-03 03:40:43.000000 lares-0.0.1/lares/lares.egg-info/dependency_links.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       91 2023-08-03 03:40:43.000000 lares-0.0.1/lares/lares.egg-info/requires.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-08-03 03:40:43.000000 lares-0.0.1/lares/lares.egg-info/top_level.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1972 2023-08-03 03:34:34.000000 lares-0.0.1/lares/lares.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1818 2023-08-03 03:34:00.000000 lares-0.0.1/lares/validate.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-08-03 03:40:43.288094 lares-0.0.1/setup.cfg
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      997 2023-08-03 03:36:17.000000 lares-0.0.1/setup.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:23:13.064268 lares-0.0.2/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-08-03 03:26:16.000000 lares-0.0.2/LICENSE
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-08-03 03:26:16.000000 lares-0.0.2/MANIFEST.in
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 05:23:13.064268 lares-0.0.2/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       65 2023-08-03 03:28:06.000000 lares-0.0.2/README.md
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:23:13.064268 lares-0.0.2/__pycache__/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     2802 2023-08-03 03:26:16.000000 lares-0.0.2/__pycache__/inviz.cpython-310.pyc
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:23:13.064268 lares-0.0.2/lares/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1645 2023-08-03 03:33:01.000000 lares-0.0.2/lares/evaluate.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:23:13.064268 lares-0.0.2/lares/lares.egg-info/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 05:23:13.000000 lares-0.0.2/lares/lares.egg-info/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      297 2023-08-03 05:23:13.000000 lares-0.0.2/lares/lares.egg-info/SOURCES.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-08-03 05:23:13.000000 lares-0.0.2/lares/lares.egg-info/dependency_links.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       91 2023-08-03 05:23:13.000000 lares-0.0.2/lares/lares.egg-info/requires.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-08-03 05:23:13.000000 lares-0.0.2/lares/lares.egg-info/top_level.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     2005 2023-08-03 05:08:42.000000 lares-0.0.2/lares/lares.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1818 2023-08-03 03:34:00.000000 lares-0.0.2/lares/validate.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-08-03 05:23:13.064268 lares-0.0.2/setup.cfg
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      997 2023-08-03 05:22:49.000000 lares-0.0.2/setup.py
```

### Comparing `lares-0.0.1/LICENSE` & `lares-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lares-0.0.1/PKG-INFO` & `lares-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lares
-Version: 0.0.1
+Version: 0.0.2
 Summary: LARES: vaLidation, evAluation and REliability Solutions
 Home-page: http://packages.python.org/lares
 Author: Karime Maamari
 Author-email: maamari@usc.edu
 License: MIT
 Keywords: evaluation,validation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lares-0.0.1/__pycache__/inviz.cpython-310.pyc` & `lares-0.0.2/__pycache__/inviz.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lares-0.0.1/lares/evaluate.py` & `lares-0.0.2/lares/evaluate.py`

 * *Files identical despite different names*

### Comparing `lares-0.0.1/lares/lares.egg-info/PKG-INFO` & `lares-0.0.2/lares/lares.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lares
-Version: 0.0.1
+Version: 0.0.2
 Summary: LARES: vaLidation, evAluation and REliability Solutions
 Home-page: http://packages.python.org/lares
 Author: Karime Maamari
 Author-email: maamari@usc.edu
 License: MIT
 Keywords: evaluation,validation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lares-0.0.1/lares/lares.py` & `lares-0.0.2/lares/lares.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import evaluate
+import validate
+
 def generate(prompt, reference, max_iterations=10, task_type = None):
     """
     Generate a response, evaluate it, and ensure it is safe.
 
     Args:
     prompt (str): The input prompt for the model.
     reference (str): The reference solution.
```

### Comparing `lares-0.0.1/lares/validate.py` & `lares-0.0.2/lares/validate.py`

 * *Files identical despite different names*

### Comparing `lares-0.0.1/setup.py` & `lares-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "lares",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Karime Maamari",
     author_email = "maamari@usc.edu",
     description = ("LARES: vaLidation, evAluation and REliability Solutions"),
     license = "MIT",
     keywords = "evaluation, validation",
     url = "http://packages.python.org/lares",
     py_modules=["lares"],
```

