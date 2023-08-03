# Comparing `tmp/name-of-thrones-0.2.8.tar.gz` & `tmp/name-of-thrones-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "name-of-thrones-0.2.8.tar", last modified: Thu Aug  3 11:42:15 2023, max compression
+gzip compressed data, was "name-of-thrones-0.2.9.tar", last modified: Thu Aug  3 11:44:33 2023, max compression
```

## Comparing `name-of-thrones-0.2.8.tar` & `name-of-thrones-0.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-03 11:42:15.012932 name-of-thrones-0.2.8/
--rw-r--r--   0 matt      (1000) users      (985)      745 2023-08-03 11:07:45.000000 name-of-thrones-0.2.8/LICENCE
--rw-r--r--   0 matt      (1000) users      (985)     2634 2023-08-03 11:42:15.012932 name-of-thrones-0.2.8/PKG-INFO
--rw-r--r--   0 matt      (1000) users      (985)     1592 2023-08-03 11:31:49.000000 name-of-thrones-0.2.8/README.md
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-03 11:42:15.009599 name-of-thrones-0.2.8/game_of_thrones/
--rw-r--r--   0 matt      (1000) users      (985)     5049 2023-08-03 11:38:38.000000 name-of-thrones-0.2.8/game_of_thrones/__init__.py
--rw-r--r--   0 matt      (1000) users      (985)     2067 2016-03-04 21:25:09.000000 name-of-thrones-0.2.8/game_of_thrones/main.py
-drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-03 11:42:15.012932 name-of-thrones-0.2.8/name_of_thrones.egg-info/
--rw-r--r--   0 matt      (1000) users      (985)     2634 2023-08-03 11:42:14.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) users      (985)      314 2023-08-03 11:42:15.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) users      (985)        1 2023-08-03 11:42:14.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) users      (985)       62 2023-08-03 11:42:14.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) users      (985)       30 2023-08-03 11:42:14.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) users      (985)       16 2023-08-03 11:42:14.000000 name-of-thrones-0.2.8/name_of_thrones.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) users      (985)       38 2023-08-03 11:42:15.012932 name-of-thrones-0.2.8/setup.cfg
--rw-r--r--   0 matt      (1000) users      (985)     1521 2023-08-03 11:42:03.000000 name-of-thrones-0.2.8/setup.py
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-03 11:44:33.165780 name-of-thrones-0.2.9/
+-rw-r--r--   0 matt      (1000) users      (985)      745 2023-08-03 11:07:45.000000 name-of-thrones-0.2.9/LICENCE
+-rw-r--r--   0 matt      (1000) users      (985)     2697 2023-08-03 11:44:33.165780 name-of-thrones-0.2.9/PKG-INFO
+-rw-r--r--   0 matt      (1000) users      (985)     1655 2023-08-03 11:43:29.000000 name-of-thrones-0.2.9/README.md
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-03 11:44:33.162446 name-of-thrones-0.2.9/game_of_thrones/
+-rw-r--r--   0 matt      (1000) users      (985)     5049 2023-08-03 11:44:15.000000 name-of-thrones-0.2.9/game_of_thrones/__init__.py
+-rw-r--r--   0 matt      (1000) users      (985)     2067 2016-03-04 21:25:09.000000 name-of-thrones-0.2.9/game_of_thrones/main.py
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2023-08-03 11:44:33.165780 name-of-thrones-0.2.9/name_of_thrones.egg-info/
+-rw-r--r--   0 matt      (1000) users      (985)     2697 2023-08-03 11:44:33.000000 name-of-thrones-0.2.9/name_of_thrones.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) users      (985)      314 2023-08-03 11:44:33.000000 name-of-thrones-0.2.9/name_of_thrones.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) users      (985)        1 2023-08-03 11:44:33.000000 name-of-thrones-0.2.9/name_of_thrones.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) users      (985)       62 2023-08-03 11:44:33.000000 name-of-thrones-0.2.9/name_of_thrones.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) users      (985)       30 2023-08-03 11:44:33.000000 name-of-thrones-0.2.9/name_of_thrones.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) users      (985)       16 2023-08-03 11:44:33.000000 name-of-thrones-0.2.9/name_of_thrones.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) users      (985)       38 2023-08-03 11:44:33.165780 name-of-thrones-0.2.9/setup.cfg
+-rw-r--r--   0 matt      (1000) users      (985)     1521 2023-08-03 11:42:03.000000 name-of-thrones-0.2.9/setup.py
```

### Comparing `name-of-thrones-0.2.8/LICENCE` & `name-of-thrones-0.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `name-of-thrones-0.2.8/PKG-INFO` & `name-of-thrones-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: name-of-thrones
-Version: 0.2.8
+Version: 0.2.9
 Summary: Command line tool to generate words that sound like characters from Game of Thrones. Good for naming projects, servers and stray cats.
 Home-page: https://codeberg.org/Dokana/Name-of-Thrones
 Author: Matt Deacalion Stevens
 Author-email: matt@dirtymonkey.co.uk
 License: MIT
 Keywords: game of thrones naming namer project tools
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,15 @@
 
 # Name of Thrones
 
 Command line tool to generate words that sound like characters from Game of
 Thrones. Useful for unique project names, host names and the occasional stray
 cat.
 
-![Name of Thrones screenshot](screenshot.png)
+![Name of Thrones screenshot](https://codeberg.org/Dokana/Name-of-Thrones/media/branch/trunk/screenshot.png)
 
 
 ## Installation
 
 You can install the **Name of Thrones** using pip:
 
 ```console
```

### Comparing `name-of-thrones-0.2.8/README.md` & `name-of-thrones-0.2.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Name of Thrones
 
 Command line tool to generate words that sound like characters from Game of
 Thrones. Useful for unique project names, host names and the occasional stray
 cat.
 
-![Name of Thrones screenshot](screenshot.png)
+![Name of Thrones screenshot](https://codeberg.org/Dokana/Name-of-Thrones/media/branch/trunk/screenshot.png)
 
 
 ## Installation
 
 You can install the **Name of Thrones** using pip:
 
 ```console
```

### Comparing `name-of-thrones-0.2.8/game_of_thrones/__init__.py` & `name-of-thrones-0.2.9/game_of_thrones/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
 Command line tool to generate words that sound like characters from Game of
 Thrones. Good for naming projects, servers and stray cats.
 """
 __author__ = 'Matt Deacalion Stevens'
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 import random
 import string
 from itertools import islice
 from collections import defaultdict, deque
```

### Comparing `name-of-thrones-0.2.8/game_of_thrones/main.py` & `name-of-thrones-0.2.9/game_of_thrones/main.py`

 * *Files identical despite different names*

### Comparing `name-of-thrones-0.2.8/name_of_thrones.egg-info/PKG-INFO` & `name-of-thrones-0.2.9/name_of_thrones.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: name-of-thrones
-Version: 0.2.8
+Version: 0.2.9
 Summary: Command line tool to generate words that sound like characters from Game of Thrones. Good for naming projects, servers and stray cats.
 Home-page: https://codeberg.org/Dokana/Name-of-Thrones
 Author: Matt Deacalion Stevens
 Author-email: matt@dirtymonkey.co.uk
 License: MIT
 Keywords: game of thrones naming namer project tools
 Classifier: Development Status :: 4 - Beta
@@ -25,15 +25,15 @@
 
 # Name of Thrones
 
 Command line tool to generate words that sound like characters from Game of
 Thrones. Useful for unique project names, host names and the occasional stray
 cat.
 
-![Name of Thrones screenshot](screenshot.png)
+![Name of Thrones screenshot](https://codeberg.org/Dokana/Name-of-Thrones/media/branch/trunk/screenshot.png)
 
 
 ## Installation
 
 You can install the **Name of Thrones** using pip:
 
 ```console
```

### Comparing `name-of-thrones-0.2.8/setup.py` & `name-of-thrones-0.2.9/setup.py`

 * *Files identical despite different names*

