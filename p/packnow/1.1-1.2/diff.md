# Comparing `tmp/packnow-1.1.tar.gz` & `tmp/packnow-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packnow-1.1.tar", last modified: Thu Aug  3 12:44:55 2023, max compression
+gzip compressed data, was "packnow-1.2.tar", last modified: Thu Aug  3 12:49:22 2023, max compression
```

## Comparing `packnow-1.1.tar` & `packnow-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:44:55.743173 packnow-1.1/
--rw-r--r--   0 runner    (1000) runner    (1000)      743 2023-08-03 12:44:55.743173 packnow-1.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      313 2023-08-03 12:38:54.000000 packnow-1.1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:44:55.739173 packnow-1.1/packnow/
--rw-r--r--   0 runner    (1000) runner    (1000)      162 2023-08-03 08:47:41.000000 packnow-1.1/packnow/__main__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9120 2023-08-03 12:34:30.000000 packnow-1.1/packnow/main.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:44:55.743173 packnow-1.1/packnow.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      743 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      242 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       57 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-08-03 12:44:55.743173 packnow-1.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      848 2023-08-03 12:43:14.000000 packnow-1.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:49:22.906686 packnow-1.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      743 2023-08-03 12:49:22.906686 packnow-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      313 2023-08-03 12:38:54.000000 packnow-1.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:49:22.826678 packnow-1.2/packnow/
+-rw-r--r--   0 runner    (1000) runner    (1000)      162 2023-08-03 08:47:41.000000 packnow-1.2/packnow/__main__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9120 2023-08-03 12:46:02.000000 packnow-1.2/packnow/main.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:49:22.906686 packnow-1.2/packnow.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      743 2023-08-03 12:49:22.000000 packnow-1.2/packnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      252 2023-08-03 12:49:22.000000 packnow-1.2/packnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-08-03 12:49:22.000000 packnow-1.2/packnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2023-08-03 12:49:22.000000 packnow-1.2/packnow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       57 2023-08-03 12:49:22.000000 packnow-1.2/packnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-08-03 12:49:22.000000 packnow-1.2/packnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       79 2023-08-03 12:49:22.906686 packnow-1.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      848 2023-08-03 12:49:10.000000 packnow-1.2/setup.py
```

### Comparing `packnow-1.1/PKG-INFO` & `packnow-1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packnow
-Version: 1.1
+Version: 1.2
 Summary: Pack everything, now. Cross-platform.
 Author: AWeirdDev
 Author-email: aweirdscratcher@gmail.com
 License: MIT License
 Keywords: pack,packing,packnow
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `packnow-1.1/packnow/main.py` & `packnow-1.2/packnow/main.py`

 * *Files identical despite different names*

### Comparing `packnow-1.1/packnow.egg-info/PKG-INFO` & `packnow-1.2/packnow.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packnow
-Version: 1.1
+Version: 1.2
 Summary: Pack everything, now. Cross-platform.
 Author: AWeirdDev
 Author-email: aweirdscratcher@gmail.com
 License: MIT License
 Keywords: pack,packing,packnow
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `packnow-1.1/setup.py` & `packnow-1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
   name="packnow",
   author="AWeirdDev",
-  version="1.1",
+  version="1.2",
   license="MIT License",
   description="Pack everything, now. Cross-platform.",
   long_description=readme,
   long_description_content_type="text/markdown",
   author_email="aweirdscratcher@gmail.com",
   packages=['packnow'],
   classifiers=[
```

