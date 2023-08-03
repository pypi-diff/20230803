# Comparing `tmp/lares-0.0.3.tar.gz` & `tmp/lares-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lares-0.0.3.tar", last modified: Thu Aug  3 05:29:13 2023, max compression
+gzip compressed data, was "lares-0.0.4.tar", last modified: Thu Aug  3 05:31:47 2023, max compression
```

## Comparing `lares-0.0.3.tar` & `lares-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:29:13.928278 lares-0.0.3/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-08-03 03:26:16.000000 lares-0.0.3/LICENSE
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-08-03 03:26:16.000000 lares-0.0.3/MANIFEST.in
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 05:29:13.928278 lares-0.0.3/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       65 2023-08-03 03:28:06.000000 lares-0.0.3/README.md
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:29:13.928278 lares-0.0.3/lares/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       68 2023-08-03 05:26:08.000000 lares-0.0.3/lares/__init__.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1645 2023-08-03 03:33:01.000000 lares-0.0.3/lares/evaluate.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     2005 2023-08-03 05:08:42.000000 lares-0.0.3/lares/generate.py
--rw-rw-r--   0 maamari   (1000) maamari   (1000)     1818 2023-08-03 03:34:00.000000 lares-0.0.3/lares/validate.py
-drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:29:13.928278 lares-0.0.3/lares.egg-info/
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 05:29:13.000000 lares-0.0.3/lares.egg-info/PKG-INFO
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      254 2023-08-03 05:29:13.000000 lares-0.0.3/lares.egg-info/SOURCES.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-08-03 05:29:13.000000 lares-0.0.3/lares.egg-info/dependency_links.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       91 2023-08-03 05:29:13.000000 lares-0.0.3/lares.egg-info/requires.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-08-03 05:29:13.000000 lares-0.0.3/lares.egg-info/top_level.txt
--rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-08-03 05:29:13.928278 lares-0.0.3/setup.cfg
--rw-rw-r--   0 maamari   (1000) maamari   (1000)      903 2023-08-03 05:28:40.000000 lares-0.0.3/setup.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:31:47.992283 lares-0.0.4/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1066 2023-08-03 03:26:16.000000 lares-0.0.4/LICENSE
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       42 2023-08-03 03:26:16.000000 lares-0.0.4/MANIFEST.in
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 05:31:47.992283 lares-0.0.4/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       65 2023-08-03 03:28:06.000000 lares-0.0.4/README.md
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:31:47.992283 lares-0.0.4/lares/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       72 2023-08-03 05:30:19.000000 lares-0.0.4/lares/__init__.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1645 2023-08-03 03:33:01.000000 lares-0.0.4/lares/evaluate.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     2005 2023-08-03 05:08:42.000000 lares-0.0.4/lares/generate.py
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)     1818 2023-08-03 03:34:00.000000 lares-0.0.4/lares/validate.py
+drwxrwxr-x   0 maamari   (1000) maamari   (1000)        0 2023-08-03 05:31:47.992283 lares-0.0.4/lares.egg-info/
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      553 2023-08-03 05:31:47.000000 lares-0.0.4/lares.egg-info/PKG-INFO
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      254 2023-08-03 05:31:47.000000 lares-0.0.4/lares.egg-info/SOURCES.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        1 2023-08-03 05:31:47.000000 lares-0.0.4/lares.egg-info/dependency_links.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       91 2023-08-03 05:31:47.000000 lares-0.0.4/lares.egg-info/requires.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)        6 2023-08-03 05:31:47.000000 lares-0.0.4/lares.egg-info/top_level.txt
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)       38 2023-08-03 05:31:47.992283 lares-0.0.4/setup.cfg
+-rw-rw-r--   0 maamari   (1000) maamari   (1000)      903 2023-08-03 05:31:20.000000 lares-0.0.4/setup.py
```

### Comparing `lares-0.0.3/LICENSE` & `lares-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lares-0.0.3/PKG-INFO` & `lares-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lares
-Version: 0.0.3
+Version: 0.0.4
 Summary: LARES: vaLidation, evAluation and REliability Solutions
 Home-page: http://packages.python.org/lares
 Author: Karime Maamari
 Author-email: maamari@usc.edu
 License: MIT
 Keywords: evaluation,validation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lares-0.0.3/lares/evaluate.py` & `lares-0.0.4/lares/evaluate.py`

 * *Files identical despite different names*

### Comparing `lares-0.0.3/lares/generate.py` & `lares-0.0.4/lares/generate.py`

 * *Files identical despite different names*

### Comparing `lares-0.0.3/lares/validate.py` & `lares-0.0.4/lares/validate.py`

 * *Files identical despite different names*

### Comparing `lares-0.0.3/lares.egg-info/PKG-INFO` & `lares-0.0.4/lares.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lares
-Version: 0.0.3
+Version: 0.0.4
 Summary: LARES: vaLidation, evAluation and REliability Solutions
 Home-page: http://packages.python.org/lares
 Author: Karime Maamari
 Author-email: maamari@usc.edu
 License: MIT
 Keywords: evaluation,validation
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lares-0.0.3/setup.py` & `lares-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lares",
-    version="0.0.3",
+    version="0.0.4",
     author="Karime Maamari",
     author_email="maamari@usc.edu",
     description="LARES: vaLidation, evAluation and REliability Solutions",
     license="MIT",
     keywords="evaluation, validation",
     url="http://packages.python.org/lares",
     packages=setuptools.find_packages(),
```

