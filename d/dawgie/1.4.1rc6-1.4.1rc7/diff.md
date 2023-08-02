# Comparing `tmp/dawgie-1.4.1rc6.tar.gz` & `tmp/dawgie-1.4.1rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgie-1.4.1rc6.tar", last modified: Thu Jul 13 20:59:54 2023, max compression
+gzip compressed data, was "dawgie-1.4.1rc7.tar", last modified: Wed Aug  2 23:45:26 2023, max compression
```

## Comparing `dawgie-1.4.1rc6.tar` & `dawgie-1.4.1rc7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 20:59:54.992869 dawgie-1.4.1rc6/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-07-13 20:59:36.000000 dawgie-1.4.1rc6/LICENSE
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 20:59:54.992869 dawgie-1.4.1rc6/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-07-13 20:59:36.000000 dawgie-1.4.1rc6/README.md
-drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-07-13 20:59:54.992869 dawgie-1.4.1rc6/dawgie.egg-info/
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     9505 2023-07-13 20:59:54.000000 dawgie-1.4.1rc6/dawgie.egg-info/PKG-INFO
--rw-rw-r--   0 niessner  (1000) niessner  (1000)     6384 2023-07-13 20:59:54.000000 dawgie-1.4.1rc6/dawgie.egg-info/SOURCES.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-07-13 20:59:54.000000 dawgie-1.4.1rc6/dawgie.egg-info/dependency_links.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-07-13 20:59:54.000000 dawgie-1.4.1rc6/dawgie.egg-info/requires.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-07-13 20:59:54.000000 dawgie-1.4.1rc6/dawgie.egg-info/top_level.txt
--rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-07-13 20:59:54.992869 dawgie-1.4.1rc6/setup.cfg
--rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6368 2023-07-13 20:40:38.000000 dawgie-1.4.1rc6/setup.py
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-08-02 23:45:26.891328 dawgie-1.4.1rc7/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     1615 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/LICENSE
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2023-08-02 23:45:26.891328 dawgie-1.4.1rc7/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     8906 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/README.md
+drwxrwxr-x   0 niessner  (1000) niessner  (1000)        0 2023-08-02 23:45:26.891328 dawgie-1.4.1rc7/dawgie.egg-info/
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     9485 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/dawgie.egg-info/PKG-INFO
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)     6384 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/dawgie.egg-info/SOURCES.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        1 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/dawgie.egg-info/dependency_links.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)      257 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/dawgie.egg-info/requires.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)        7 2023-08-02 23:45:26.000000 dawgie-1.4.1rc7/dawgie.egg-info/top_level.txt
+-rw-rw-r--   0 niessner  (1000) niessner  (1000)       38 2023-08-02 23:45:26.891328 dawgie-1.4.1rc7/setup.cfg
+-rwxrwxr-x   0 niessner  (1000) niessner  (1000)     6368 2023-08-02 23:14:25.000000 dawgie-1.4.1rc7/setup.py
```

### Comparing `dawgie-1.4.1rc6/LICENSE` & `dawgie-1.4.1rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.1rc6/PKG-INFO` & `dawgie-1.4.1rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.1rc6
+Version: 1.4.1rc7
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Free To Use But Restricted
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -141,9 +140,7 @@
 ### Installation
 
 1. `python3 Python/setup.py build install`
 1. `bash install.sh`
 
 ### Use
 
-
-
```

### Comparing `dawgie-1.4.1rc6/README.md` & `dawgie-1.4.1rc7/README.md`

 * *Files identical despite different names*

### Comparing `dawgie-1.4.1rc6/dawgie.egg-info/PKG-INFO` & `dawgie-1.4.1rc7/dawgie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dawgie
-Version: 1.4.1rc6
+Version: 1.4.1rc7
 Summary: Data and Algorithm Work-flow Generation, Introspection, and Execution (DAWGIE)
 Home-page: https://github.com/al-niessner/DAWGIE
 Author: Al Niessner
 Author-email: Al.Niessner@jpl.nasa.gov
 License: see LICENSE file for details
 Keywords: adaptive pipeline
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: Free To Use But Restricted
 Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -141,9 +140,7 @@
 ### Installation
 
 1. `python3 Python/setup.py build install`
 1. `bash install.sh`
 
 ### Use
 
-
-
```

### Comparing `dawgie-1.4.1rc6/setup.py` & `dawgie-1.4.1rc7/setup.py`

 * *Files identical despite different names*

