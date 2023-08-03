# Comparing `tmp/pytmpdir-1.0.4.tar.gz` & `tmp/pytmpdir-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmpdir-1.0.4.tar", last modified: Sun Jul 30 12:44:37 2023, max compression
+gzip compressed data, was "pytmpdir-1.0.5.tar", last modified: Thu Aug  3 05:50:57 2023, max compression
```

## Comparing `pytmpdir-1.0.4.tar` & `pytmpdir-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-07-30 12:44:37.460578 pytmpdir-1.0.4/
--rw-r--r--   0 jchesney   (501) staff       (20)     1068 2021-09-22 06:19:18.000000 pytmpdir-1.0.4/LICENSE.rst
--rw-r--r--   0 jchesney   (501) staff       (20)      441 2023-07-30 12:44:37.460737 pytmpdir-1.0.4/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)      816 2021-09-22 06:19:18.000000 pytmpdir-1.0.4/README.rst
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-07-30 12:44:37.458723 pytmpdir-1.0.4/pytmpdir/
--rw-r--r--   0 jchesney   (501) staff       (20)      102 2023-07-30 12:44:34.000000 pytmpdir-1.0.4/pytmpdir/__init__.py
--rw-r--r--   0 jchesney   (501) staff       (20)      222 2023-07-30 12:38:57.000000 pytmpdir-1.0.4/pytmpdir/dir_setting.py
--rw-r--r--   0 jchesney   (501) staff       (20)     9026 2022-02-12 23:54:48.000000 pytmpdir-1.0.4/pytmpdir/directory_.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4034 2022-01-12 14:15:13.000000 pytmpdir-1.0.4/pytmpdir/directory_test.py
--rw-r--r--   0 jchesney   (501) staff       (20)     8335 2022-02-12 08:23:56.000000 pytmpdir-1.0.4/pytmpdir/file_.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2286 2022-01-10 23:27:28.000000 pytmpdir-1.0.4/pytmpdir/named_temp_file_reader.py
--rw-r--r--   0 jchesney   (501) staff       (20)      259 2022-01-10 23:14:45.000000 pytmpdir-1.0.4/pytmpdir/pytmpdir_exception.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3037 2022-01-12 13:04:58.000000 pytmpdir-1.0.4/pytmpdir/spooled_named_temporary_file.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-07-30 12:44:37.460308 pytmpdir-1.0.4/pytmpdir.egg-info/
--rw-r--r--   0 jchesney   (501) staff       (20)      441 2023-07-30 12:44:37.000000 pytmpdir-1.0.4/pytmpdir.egg-info/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)      420 2023-07-30 12:44:37.000000 pytmpdir-1.0.4/pytmpdir.egg-info/SOURCES.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-07-30 12:44:37.000000 pytmpdir-1.0.4/pytmpdir.egg-info/dependency_links.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       26 2023-07-30 12:44:37.000000 pytmpdir-1.0.4/pytmpdir.egg-info/requires.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        9 2023-07-30 12:44:37.000000 pytmpdir-1.0.4/pytmpdir.egg-info/top_level.txt
--rw-r--r--   0 jchesney   (501) staff       (20)       80 2023-07-30 12:44:37.461374 pytmpdir-1.0.4/setup.cfg
--rw-r--r--   0 jchesney   (501) staff       (20)      799 2023-07-30 12:44:34.000000 pytmpdir-1.0.4/setup.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-08-03 05:50:57.531448 pytmpdir-1.0.5/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1068 2021-09-22 06:19:18.000000 pytmpdir-1.0.5/LICENSE.rst
+-rw-r--r--   0 jchesney   (501) staff       (20)      441 2023-08-03 05:50:57.531563 pytmpdir-1.0.5/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)      816 2021-09-22 06:19:18.000000 pytmpdir-1.0.5/README.rst
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-08-03 05:50:57.529564 pytmpdir-1.0.5/pytmpdir/
+-rw-r--r--   0 jchesney   (501) staff       (20)      102 2023-08-03 05:50:55.000000 pytmpdir-1.0.5/pytmpdir/__init__.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      232 2023-08-03 05:48:47.000000 pytmpdir-1.0.5/pytmpdir/dir_setting.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     9026 2022-02-12 23:54:48.000000 pytmpdir-1.0.5/pytmpdir/directory_.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4034 2022-01-12 14:15:13.000000 pytmpdir-1.0.5/pytmpdir/directory_test.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     8335 2022-02-12 08:23:56.000000 pytmpdir-1.0.5/pytmpdir/file_.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2286 2022-01-10 23:27:28.000000 pytmpdir-1.0.5/pytmpdir/named_temp_file_reader.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      259 2022-01-10 23:14:45.000000 pytmpdir-1.0.5/pytmpdir/pytmpdir_exception.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3037 2022-01-12 13:04:58.000000 pytmpdir-1.0.5/pytmpdir/spooled_named_temporary_file.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2023-08-03 05:50:57.531182 pytmpdir-1.0.5/pytmpdir.egg-info/
+-rw-r--r--   0 jchesney   (501) staff       (20)      441 2023-08-03 05:50:57.000000 pytmpdir-1.0.5/pytmpdir.egg-info/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)      420 2023-08-03 05:50:57.000000 pytmpdir-1.0.5/pytmpdir.egg-info/SOURCES.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2023-08-03 05:50:57.000000 pytmpdir-1.0.5/pytmpdir.egg-info/dependency_links.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       26 2023-08-03 05:50:57.000000 pytmpdir-1.0.5/pytmpdir.egg-info/requires.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        9 2023-08-03 05:50:57.000000 pytmpdir-1.0.5/pytmpdir.egg-info/top_level.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)       80 2023-08-03 05:50:57.532017 pytmpdir-1.0.5/setup.cfg
+-rw-r--r--   0 jchesney   (501) staff       (20)      799 2023-08-03 05:50:55.000000 pytmpdir-1.0.5/setup.py
```

### Comparing `pytmpdir-1.0.4/LICENSE.rst` & `pytmpdir-1.0.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.4/README.rst` & `pytmpdir-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.4/pytmpdir/directory_.py` & `pytmpdir-1.0.5/pytmpdir/directory_.py`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.4/pytmpdir/directory_test.py` & `pytmpdir-1.0.5/pytmpdir/directory_test.py`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.4/pytmpdir/file_.py` & `pytmpdir-1.0.5/pytmpdir/file_.py`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.4/pytmpdir/named_temp_file_reader.py` & `pytmpdir-1.0.5/pytmpdir/named_temp_file_reader.py`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.4/pytmpdir/spooled_named_temporary_file.py` & `pytmpdir-1.0.5/pytmpdir/spooled_named_temporary_file.py`

 * *Files identical despite different names*

### Comparing `pytmpdir-1.0.4/setup.py` & `pytmpdir-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 package_name = "pytmpdir"
-package_version = '1.0.4'
+package_version = '1.0.5'
 
 setup(
     name=package_name,
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     install_requires=["sphinx_rtd_theme", "sphinx<4"],
     version=package_version,
     description='A class representing a file system directory, that deletes on '
```

