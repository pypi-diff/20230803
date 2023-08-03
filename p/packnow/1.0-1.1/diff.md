# Comparing `tmp/packnow-1.0.tar.gz` & `tmp/packnow-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packnow-1.0.tar", last modified: Thu Aug  3 12:40:59 2023, max compression
+gzip compressed data, was "packnow-1.1.tar", last modified: Thu Aug  3 12:44:55 2023, max compression
```

## Comparing `packnow-1.0.tar` & `packnow-1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:40:59.626858 packnow-1.0/
--rw-r--r--   0 runner    (1000) runner    (1000)      743 2023-08-03 12:40:59.626858 packnow-1.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      313 2023-08-03 12:38:54.000000 packnow-1.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:40:59.622857 packnow-1.0/packnow/
--rw-r--r--   0 runner    (1000) runner    (1000)      162 2023-08-03 08:47:41.000000 packnow-1.0/packnow/__main__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9120 2023-08-03 12:34:30.000000 packnow-1.0/packnow/main.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:40:59.626858 packnow-1.0/packnow.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      743 2023-08-03 12:40:59.000000 packnow-1.0/packnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      257 2023-08-03 12:40:59.000000 packnow-1.0/packnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-08-03 12:40:59.000000 packnow-1.0/packnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       46 2023-08-03 12:40:59.000000 packnow-1.0/packnow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       57 2023-08-03 12:40:59.000000 packnow-1.0/packnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-08-03 12:40:59.000000 packnow-1.0/packnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      836 2023-08-03 12:16:00.000000 packnow-1.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-08-03 12:40:59.626858 packnow-1.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      848 2023-08-03 12:39:36.000000 packnow-1.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:44:55.743173 packnow-1.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)      743 2023-08-03 12:44:55.743173 packnow-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      313 2023-08-03 12:38:54.000000 packnow-1.1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:44:55.739173 packnow-1.1/packnow/
+-rw-r--r--   0 runner    (1000) runner    (1000)      162 2023-08-03 08:47:41.000000 packnow-1.1/packnow/__main__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9120 2023-08-03 12:34:30.000000 packnow-1.1/packnow/main.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-08-03 12:44:55.743173 packnow-1.1/packnow.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      743 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      242 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       46 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       57 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-08-03 12:44:55.000000 packnow-1.1/packnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-08-03 12:44:55.743173 packnow-1.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      848 2023-08-03 12:43:14.000000 packnow-1.1/setup.py
```

### Comparing `packnow-1.0/PKG-INFO` & `packnow-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packnow
-Version: 1.0
+Version: 1.1
 Summary: Pack everything, now. Cross-platform.
 Author: AWeirdDev
 Author-email: aweirdscratcher@gmail.com
 License: MIT License
 Keywords: pack,packing,packnow
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `packnow-1.0/packnow/main.py` & `packnow-1.1/packnow/main.py`

 * *Files identical despite different names*

### Comparing `packnow-1.0/packnow.egg-info/PKG-INFO` & `packnow-1.1/packnow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packnow
-Version: 1.0
+Version: 1.1
 Summary: Pack everything, now. Cross-platform.
 Author: AWeirdDev
 Author-email: aweirdscratcher@gmail.com
 License: MIT License
 Keywords: pack,packing,packnow
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `packnow-1.0/setup.py` & `packnow-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
   name="packnow",
   author="AWeirdDev",
-  version="1.0",
+  version="1.1",
   license="MIT License",
   description="Pack everything, now. Cross-platform.",
   long_description=readme,
   long_description_content_type="text/markdown",
   author_email="aweirdscratcher@gmail.com",
   packages=['packnow'],
   classifiers=[
```

