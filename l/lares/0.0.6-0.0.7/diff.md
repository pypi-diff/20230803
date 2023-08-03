# Comparing `tmp/lares-0.0.6.tar.gz` & `tmp/lares-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lares-0.0.6.tar", last modified: Thu Aug  3 05:56:39 2023, max compression
+gzip compressed data, was "lares-0.0.7.tar", last modified: Thu Aug  3 06:02:35 2023, max compression
```

## Comparing `lares-0.0.6.tar` & `lares-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:56:39.932325 lares-0.0.6/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-08-03 03:26:16.000000 lares-0.0.6/LICENSE
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-08-03 03:26:16.000000 lares-0.0.6/MANIFEST.in
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 05:56:39.932325 lares-0.0.6/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       65 2023-08-03 03:28:06.000000 lares-0.0.6/README.md
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:56:39.932325 lares-0.0.6/lares/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:52:38.000000 lares-0.0.6/lares/__init__.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1645 2023-08-03 03:33:01.000000 lares-0.0.6/lares/evaluate.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1972 2023-08-03 05:40:16.000000 lares-0.0.6/lares/generate.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1818 2023-08-03 03:34:00.000000 lares-0.0.6/lares/validate.py
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:56:39.932325 lares-0.0.6/lares.egg-info/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 05:56:39.000000 lares-0.0.6/lares.egg-info/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      254 2023-08-03 05:56:39.000000 lares-0.0.6/lares.egg-info/SOURCES.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-08-03 05:56:39.000000 lares-0.0.6/lares.egg-info/dependency_links.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       91 2023-08-03 05:56:39.000000 lares-0.0.6/lares.egg-info/requires.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-08-03 05:56:39.000000 lares-0.0.6/lares.egg-info/top_level.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-08-03 05:56:39.932325 lares-0.0.6/setup.cfg
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      903 2023-08-03 05:56:18.000000 lares-0.0.6/setup.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 06:02:35.788335 lares-0.0.7/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-08-03 03:26:16.000000 lares-0.0.7/LICENSE
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-08-03 03:26:16.000000 lares-0.0.7/MANIFEST.in
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 06:02:35.788335 lares-0.0.7/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       65 2023-08-03 03:28:06.000000 lares-0.0.7/README.md
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 06:02:35.788335 lares-0.0.7/lares/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:52:38.000000 lares-0.0.7/lares/__init__.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1645 2023-08-03 03:33:01.000000 lares-0.0.7/lares/evaluate.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     3100 2023-08-03 06:01:41.000000 lares-0.0.7/lares/generate.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1818 2023-08-03 03:34:00.000000 lares-0.0.7/lares/validate.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 06:02:35.788335 lares-0.0.7/lares.egg-info/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 06:02:35.000000 lares-0.0.7/lares.egg-info/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      254 2023-08-03 06:02:35.000000 lares-0.0.7/lares.egg-info/SOURCES.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-08-03 06:02:35.000000 lares-0.0.7/lares.egg-info/dependency_links.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       91 2023-08-03 06:02:35.000000 lares-0.0.7/lares.egg-info/requires.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-08-03 06:02:35.000000 lares-0.0.7/lares.egg-info/top_level.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-08-03 06:02:35.788335 lares-0.0.7/setup.cfg
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      903 2023-08-03 06:02:19.000000 lares-0.0.7/setup.py
```

### Comparing `lares-0.0.6/LICENSE` & `lares-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lares-0.0.6/PKG-INFO` & `lares-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lares
-Version: 0.0.6
+Version: 0.0.7
 Summary: LARES: vaLidation, evAluation and REliability Solutions
 Home-page: http://packages.python.org/lares
 Author: Karime Maamari
 Author-email: maamari@usc.edu
 License: MIT
 Keywords: evaluation,validation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lares-0.0.6/lares/evaluate.py` & `lares-0.0.7/lares/evaluate.py`

 * *Files identical despite different names*

### Comparing `lares-0.0.6/lares/generate.py` & `lares-0.0.7/lares/generate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,48 @@
+from .validate import *
+from .generate import *
+
+def get_response(prompt):
+    """
+    Get a response to a given prompt using the text-davinci-003 engine.
+
+    Args:
+    prompt (str): The input prompt for the model.
+
+    Returns:
+    str: The response generated by the model.
+    """
+    response = openai.Completion.create(
+        engine="text-davinci-003",
+        prompt=prompt,
+        temperature=0.3,
+        max_tokens=100
+    )
+
+    return response.choices[0].text.strip()
+
+
+def determine_task(task_desc):
+    """
+    Determine the evaluation tool most suitable for a given task description.
+
+    Args:
+    task_desc (str): The description of the task.
+
+    Returns:
+    str: The evaluation tool (Translation, Summarization, or Rephrasing).
+    """
+    response = openai.Completion.create(
+        engine="text-davinci-003",
+        prompt=f"The task is: '{task_desc}'. Which evaluation tool is most suitable for this task? Respond with a single word out of the following choices: Translation, Summarization, Rephrasing",
+        temperature=0.3,
+        max_tokens=3
+    )
+    return response.choices[0].text.strip()
+
 def generate(prompt, reference, max_iterations=10, task_type = None):
     """
     Generate a response, evaluate it, and ensure it is safe.
 
     Args:
     prompt (str): The input prompt for the model.
     reference (str): The reference solution.
```

### Comparing `lares-0.0.6/lares/validate.py` & `lares-0.0.7/lares/validate.py`

 * *Files identical despite different names*

### Comparing `lares-0.0.6/lares.egg-info/PKG-INFO` & `lares-0.0.7/lares.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lares
-Version: 0.0.6
+Version: 0.0.7
 Summary: LARES: vaLidation, evAluation and REliability Solutions
 Home-page: http://packages.python.org/lares
 Author: Karime Maamari
 Author-email: maamari@usc.edu
 License: MIT
 Keywords: evaluation,validation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lares-0.0.6/setup.py` & `lares-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lares",
-    version="0.0.6",
+    version="0.0.7",
     author="Karime Maamari",
     author_email="maamari@usc.edu",
     description="LARES: vaLidation, evAluation and REliability Solutions",
     license="MIT",
     keywords="evaluation, validation",
     url="http://packages.python.org/lares",
     packages=setuptools.find_packages(),
```

