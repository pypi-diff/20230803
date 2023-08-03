# Comparing `tmp/aEye-1.2.1.tar.gz` & `tmp/aEye-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aEye-1.2.1.tar", last modified: Thu Aug  3 16:27:50 2023, max compression
+gzip compressed data, was "aEye-1.2.2.tar", last modified: Thu Aug  3 16:30:40 2023, max compression
```

## Comparing `aEye-1.2.1.tar` & `aEye-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:27:50.231902 aEye-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 16:27:36.000000 aEye-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-03 16:27:50.231902 aEye-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-08-03 16:27:36.000000 aEye-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:27:50.227902 aEye-1.2.1/aEye/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-03 16:27:36.000000 aEye-1.2.1/aEye/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-08-03 16:27:36.000000 aEye-1.2.1/aEye/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-03 16:27:36.000000 aEye-1.2.1/aEye/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-08-03 16:27:36.000000 aEye-1.2.1/aEye/labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-08-03 16:27:36.000000 aEye-1.2.1/aEye/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:27:50.231902 aEye-1.2.1/aEye.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-03 16:27:50.000000 aEye-1.2.1/aEye.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-03 16:27:50.000000 aEye-1.2.1/aEye.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:27:50.000000 aEye-1.2.1/aEye.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 16:27:50.000000 aEye-1.2.1/aEye.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 16:27:50.000000 aEye-1.2.1/aEye.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:27:50.231902 aEye-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-03 16:27:36.000000 aEye-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:27:50.231902 aEye-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-03 16:27:36.000000 aEye-1.2.1/tests/test_extract_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:30:40.410541 aEye-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 16:30:26.000000 aEye-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-03 16:30:40.410541 aEye-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-08-03 16:30:26.000000 aEye-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:30:40.410541 aEye-1.2.2/aEye/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-03 16:30:26.000000 aEye-1.2.2/aEye/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-08-03 16:30:26.000000 aEye-1.2.2/aEye/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-03 16:30:26.000000 aEye-1.2.2/aEye/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-08-03 16:30:26.000000 aEye-1.2.2/aEye/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-08-03 16:30:26.000000 aEye-1.2.2/aEye/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:30:40.410541 aEye-1.2.2/aEye.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-08-03 16:30:40.000000 aEye-1.2.2/aEye.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-03 16:30:40.000000 aEye-1.2.2/aEye.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:30:40.000000 aEye-1.2.2/aEye.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 16:30:40.000000 aEye-1.2.2/aEye.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 16:30:40.000000 aEye-1.2.2/aEye.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 16:30:40.410541 aEye-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-03 16:30:26.000000 aEye-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:30:40.410541 aEye-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-03 16:30:26.000000 aEye-1.2.2/tests/test_extract_metadata.py
```

### Comparing `aEye-1.2.1/LICENSE` & `aEye-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aEye-1.2.1/PKG-INFO` & `aEye-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.2.1
+Version: 1.2.2
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aEye-1.2.1/README.md` & `aEye-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aEye-1.2.1/aEye/auxiliary.py` & `aEye-1.2.2/aEye/auxiliary.py`

 * *Files identical despite different names*

### Comparing `aEye-1.2.1/aEye/extractor.py` & `aEye-1.2.2/aEye/extractor.py`

 * *Files identical despite different names*

### Comparing `aEye-1.2.1/aEye/labeler.py` & `aEye-1.2.2/aEye/labeler.py`

 * *Files identical despite different names*

### Comparing `aEye-1.2.1/aEye/video.py` & `aEye-1.2.2/aEye/video.py`

 * *Files identical despite different names*

### Comparing `aEye-1.2.1/aEye.egg-info/PKG-INFO` & `aEye-1.2.2/aEye.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aEye
-Version: 1.2.1
+Version: 1.2.2
 Summary: Extensible Video Processing Framework
 Home-page: https://github.com/DISHDevEx/aEye
 Author-email: devex@dish.com
 License: Dish Wireless
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aEye-1.2.1/setup.py` & `aEye-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 
 def get_version():
     """
     Checks commandline arguments for a user specified Version number.
     If the --version flag is not given at run time, then the version number is defaulted to
-    v1.2.1, which will later be replaced with a git tag when performing
+    v1.2.2, which will later be replaced with a git tag when performing
     version releases.
 
     Returns
     -------
     when the bdist_wheel command is given a version flag and version number, such as:
 
     --version 1.x.x
@@ -36,15 +36,15 @@
     If the --version flag is given, but no version number is supplied, such as:
 
     --version
 
     then an IndexError will be thrown and the build will exit with exit status 1.
 
     """
-    version = 'v1.2.1'
+    version = 'v1.2.2'
     if "--version" in sys.argv:
         try:
             version = sys.argv[3]
             sys.argv.remove(sys.argv[3])
         except IndexError as e:
             print("error:  " + str(e))
             print("supply a version number i.e. --version 1.x.x")
```

### Comparing `aEye-1.2.1/tests/test_extract_metadata.py` & `aEye-1.2.2/tests/test_extract_metadata.py`

 * *Files identical despite different names*

