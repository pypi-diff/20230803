# Comparing `tmp/packnow-1.4.tar.gz` & `tmp/packnow-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packnow-1.4.tar", last modified: Thu Aug  3 13:01:12 2023, max compression
+gzip compressed data, was "packnow-1.5.tar", last modified: Thu Aug  3 13:02:35 2023, max compression
```

## Comparing `packnow-1.4.tar` & `packnow-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:01:12.811793 packnow-1.4/
--rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-08-03 12:54:35.000000 packnow-1.4/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2110 2023-08-03 13:01:12.811793 packnow-1.4/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      313 2023-08-03 12:51:15.000000 packnow-1.4/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:01:12.803792 packnow-1.4/packnow/
--rw-r--r--   0 runner    (1000) runner    (1000)       19 2023-08-03 12:59:55.000000 packnow-1.4/packnow/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      162 2023-08-03 08:47:41.000000 packnow-1.4/packnow/__main__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9120 2023-08-03 12:46:02.000000 packnow-1.4/packnow/main.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:01:12.811793 packnow-1.4/packnow.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2110 2023-08-03 13:01:12.000000 packnow-1.4/packnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      295 2023-08-03 13:01:12.000000 packnow-1.4/packnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-08-03 13:01:12.000000 packnow-1.4/packnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2023-08-03 13:01:12.000000 packnow-1.4/packnow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       57 2023-08-03 13:01:12.000000 packnow-1.4/packnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-08-03 13:01:12.000000 packnow-1.4/packnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      768 2023-08-03 13:01:08.000000 packnow-1.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       79 2023-08-03 13:01:12.811793 packnow-1.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      707 2023-08-03 13:01:05.000000 packnow-1.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:02:35.312289 packnow-1.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1070 2023-08-03 12:54:35.000000 packnow-1.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2110 2023-08-03 13:02:35.316290 packnow-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      313 2023-08-03 12:51:15.000000 packnow-1.5/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:02:35.220280 packnow-1.5/packnow/
+-rw-r--r--   0 runner    (1000) runner    (1000)       19 2023-08-03 12:59:55.000000 packnow-1.5/packnow/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      162 2023-08-03 08:47:41.000000 packnow-1.5/packnow/__main__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9120 2023-08-03 12:46:02.000000 packnow-1.5/packnow/main.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 13:02:35.312289 packnow-1.5/packnow.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2110 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      295 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       49 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-08-03 13:02:34.000000 packnow-1.5/packnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      754 2023-08-03 13:02:28.000000 packnow-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       79 2023-08-03 13:02:35.316290 packnow-1.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      707 2023-08-03 13:02:33.000000 packnow-1.5/setup.py
```

### Comparing `packnow-1.4/LICENSE` & `packnow-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `packnow-1.4/PKG-INFO` & `packnow-1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packnow
-Version: 1.4
+Version: 1.5
 Summary: Pack everything, now.
 Author: AWeirdDev
 Author-email: AWeirdDev <aweirdscratcher@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 AWeirdDev @ tw
```

### Comparing `packnow-1.4/packnow/main.py` & `packnow-1.5/packnow/main.py`

 * *Files identical despite different names*

### Comparing `packnow-1.4/packnow.egg-info/PKG-INFO` & `packnow-1.5/packnow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packnow
-Version: 1.4
+Version: 1.5
 Summary: Pack everything, now.
 Author: AWeirdDev
 Author-email: AWeirdDev <aweirdscratcher@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 AWeirdDev @ tw
```

### Comparing `packnow-1.4/pyproject.toml` & `packnow-1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "packnow"
-version = "1.4"
+version = "1.5"
 description = "Pack everything, now."
 keywords = ["pack", "packing", "packnow"]
 authors = [
   { name = "AWeirdDev", email = "aweirdscratcher@gmail.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.9"
 dependencies = [
-  "zipfile", 
   "termcolor", 
   "fastapi", 
   "questionary", 
   "websockets", 
   "uvicorn",
 ]
```

### Comparing `packnow-1.4/setup.py` & `packnow-1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
   name="packnow",
   author="AWeirdDev",
-  version="1.4",
+  version="1.5",
   license="MIT License",
   description="Pack everything, now. Cross-platform.",
   long_description=readme,
   long_description_content_type="text/markdown",
   author_email="aweirdscratcher@gmail.com",
   packages=['packnow'],
   classifiers=[
```

