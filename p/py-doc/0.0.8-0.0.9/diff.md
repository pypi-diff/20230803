# Comparing `tmp/py-doc-0.0.8.tar.gz` & `tmp/py-doc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-doc-0.0.8.tar", last modified: Tue Aug  1 21:49:15 2023, max compression
+gzip compressed data, was "py-doc-0.0.9.tar", last modified: Wed Aug  2 00:09:34 2023, max compression
```

## Comparing `py-doc-0.0.8.tar` & `py-doc-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 21:49:15.307024 py-doc-0.0.8/
--rw-r--r--   0 connor    (1000) connor    (1000)     1119 2023-08-01 21:49:15.307024 py-doc-0.0.8/PKG-INFO
--rw-r--r--   0 connor    (1000) connor    (1000)      457 2023-08-01 20:49:33.000000 py-doc-0.0.8/README.md
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 21:49:15.307024 py-doc-0.0.8/py_doc/
--rw-r--r--   0 connor    (1000) connor    (1000)      126 2023-08-01 21:47:22.000000 py-doc-0.0.8/py_doc/__init__.py
--rw-r--r--   0 connor    (1000) connor    (1000)      369 2023-08-01 21:46:07.000000 py-doc-0.0.8/py_doc/document.py
--rw-r--r--   0 connor    (1000) connor    (1000)      923 2023-08-01 18:20:38.000000 py-doc-0.0.8/py_doc/multiplication.py
-drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-01 21:49:15.307024 py-doc-0.0.8/py_doc.egg-info/
--rw-r--r--   0 connor    (1000) connor    (1000)     1119 2023-08-01 21:49:15.000000 py-doc-0.0.8/py_doc.egg-info/PKG-INFO
--rw-r--r--   0 connor    (1000) connor    (1000)      230 2023-08-01 21:49:15.000000 py-doc-0.0.8/py_doc.egg-info/SOURCES.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        1 2023-08-01 21:49:15.000000 py-doc-0.0.8/py_doc.egg-info/dependency_links.txt
--rw-r--r--   0 connor    (1000) connor    (1000)       13 2023-08-01 21:49:15.000000 py-doc-0.0.8/py_doc.egg-info/requires.txt
--rw-r--r--   0 connor    (1000) connor    (1000)        7 2023-08-01 21:49:15.000000 py-doc-0.0.8/py_doc.egg-info/top_level.txt
--rw-r--r--   0 connor    (1000) connor    (1000)       38 2023-08-01 21:49:15.307024 py-doc-0.0.8/setup.cfg
--rw-r--r--   0 connor    (1000) connor    (1000)     1281 2023-08-01 21:46:52.000000 py-doc-0.0.8/setup.py
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-02 00:09:34.333424 py-doc-0.0.9/
+-rw-r--r--   0 connor    (1000) connor    (1000)     1119 2023-08-02 00:09:34.333424 py-doc-0.0.9/PKG-INFO
+-rw-r--r--   0 connor    (1000) connor    (1000)      457 2023-08-01 20:49:33.000000 py-doc-0.0.9/README.md
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-02 00:09:34.332424 py-doc-0.0.9/py_doc/
+-rw-r--r--   0 connor    (1000) connor    (1000)      126 2023-08-01 21:47:22.000000 py-doc-0.0.9/py_doc/__init__.py
+-rw-r--r--   0 connor    (1000) connor    (1000)      646 2023-08-02 00:00:33.000000 py-doc-0.0.9/py_doc/document.py
+-rw-r--r--   0 connor    (1000) connor    (1000)      923 2023-08-01 18:20:38.000000 py-doc-0.0.9/py_doc/multiplication.py
+drwxr-xr-x   0 connor    (1000) connor    (1000)        0 2023-08-02 00:09:34.332424 py-doc-0.0.9/py_doc.egg-info/
+-rw-r--r--   0 connor    (1000) connor    (1000)     1119 2023-08-02 00:09:34.000000 py-doc-0.0.9/py_doc.egg-info/PKG-INFO
+-rw-r--r--   0 connor    (1000) connor    (1000)      230 2023-08-02 00:09:34.000000 py-doc-0.0.9/py_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        1 2023-08-02 00:09:34.000000 py-doc-0.0.9/py_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)      280 2023-08-02 00:09:34.000000 py-doc-0.0.9/py_doc.egg-info/requires.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)        7 2023-08-02 00:09:34.000000 py-doc-0.0.9/py_doc.egg-info/top_level.txt
+-rw-r--r--   0 connor    (1000) connor    (1000)       38 2023-08-02 00:09:34.333424 py-doc-0.0.9/setup.cfg
+-rw-r--r--   0 connor    (1000) connor    (1000)     1393 2023-08-02 00:09:28.000000 py-doc-0.0.9/setup.py
```

### Comparing `py-doc-0.0.8/PKG-INFO` & `py-doc-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-doc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Used for working with documentations in Python.
 Home-page: 
 Author: Connor Holm
 Author-email: connorjholm@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-doc-0.0.8/py_doc/multiplication.py` & `py-doc-0.0.9/py_doc/multiplication.py`

 * *Files identical despite different names*

### Comparing `py-doc-0.0.8/py_doc.egg-info/PKG-INFO` & `py-doc-0.0.9/py_doc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-doc
-Version: 0.0.8
+Version: 0.0.9
 Summary: Used for working with documentations in Python.
 Home-page: 
 Author: Connor Holm
 Author-email: connorjholm@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py-doc-0.0.8/setup.py` & `py-doc-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
+
 # To use a consistent encoding
 from codecs import open
+import os
 from os import path
 
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
+with open("requirements.txt") as f:
+    requirements = f.read().splitlines()
+requirements.append("py-doc")
+
 # This call to setup() does all the work
 setup(
     name="py-doc",
-    version="0.0.8",
+    version="0.0.9",
     description="Used for working with documentations in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Connor Holm",
     author_email="connorjholm@gmail.com",
     license="MIT",
@@ -32,9 +38,9 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["py_doc"],
     include_package_data=True,
-    install_requires=["numpy", "py-doc"]
+    install_requires=requirements
 )
```

