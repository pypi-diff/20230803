# Comparing `tmp/CUDG-0.0.1.tar.gz` & `tmp/CUDG-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUDG-0.0.1.tar", last modified: Thu Aug  3 02:46:22 2023, max compression
+gzip compressed data, was "CUDG-0.0.2.tar", last modified: Thu Aug  3 02:49:37 2023, max compression
```

## Comparing `CUDG-0.0.1.tar` & `CUDG-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:46:22.771150 CUDG-0.0.1/
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:46:22.766540 CUDG-0.0.1/CUDG.egg-info/
--rw-r--r--   0 daegeun    (501) staff       (20)      468 2023-08-03 02:46:22.000000 CUDG-0.0.1/CUDG.egg-info/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      384 2023-08-03 02:46:22.000000 CUDG-0.0.1/CUDG.egg-info/SOURCES.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:46:22.000000 CUDG-0.0.1/CUDG.egg-info/dependency_links.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:46:22.000000 CUDG-0.0.1/CUDG.egg-info/not-zip-safe
--rw-r--r--   0 daegeun    (501) staff       (20)       34 2023-08-03 02:46:22.000000 CUDG-0.0.1/CUDG.egg-info/top_level.txt
--rw-r--r--   0 daegeun    (501) staff       (20)      468 2023-08-03 02:46:22.770875 CUDG-0.0.1/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      172 2023-05-19 05:03:17.000000 CUDG-0.0.1/README.md
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:46:22.767928 CUDG-0.0.1/VRAManager/
--rw-r--r--   0 daegeun    (501) staff       (20)      120 2023-05-21 14:59:59.000000 CUDG-0.0.1/VRAManager/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)       28 2023-05-21 14:13:48.000000 CUDG-0.0.1/VRAManager/assigner.py
--rw-r--r--   0 daegeun    (501) staff       (20)       27 2023-05-21 14:14:26.000000 CUDG-0.0.1/VRAManager/cleaner.py
--rw-r--r--   0 daegeun    (501) staff       (20)      567 2023-05-22 04:02:27.000000 CUDG-0.0.1/VRAManager/memory.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:46:22.768657 CUDG-0.0.1/gpuarray/
--rw-r--r--   0 daegeun    (501) staff       (20)       32 2023-05-21 14:59:49.000000 CUDG-0.0.1/gpuarray/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1572 2023-07-30 06:08:09.000000 CUDG-0.0.1/gpuarray/gpuarray.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:46:22.769718 CUDG-0.0.1/linalg/
--rw-r--r--   0 daegeun    (501) staff       (20)       24 2023-07-30 01:42:39.000000 CUDG-0.0.1/linalg/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1930 2023-07-30 03:31:27.000000 CUDG-0.0.1/linalg/linalg.py
--rw-r--r--   0 daegeun    (501) staff       (20)     3117 2023-07-30 01:45:19.000000 CUDG-0.0.1/linalg/linalgcore.py
--rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 02:46:22.771228 CUDG-0.0.1/setup.cfg
--rw-r--r--   0 daegeun    (501) staff       (20)      684 2023-08-03 02:45:37.000000 CUDG-0.0.1/setup.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:46:22.770439 CUDG-0.0.1/sparse/
--rw-r--r--   0 daegeun    (501) staff       (20)       17 2023-05-19 05:03:17.000000 CUDG-0.0.1/sparse/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1416 2023-05-22 04:06:14.000000 CUDG-0.0.1/sparse/gpusparse.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:49:37.340268 CUDG-0.0.2/
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:49:37.333936 CUDG-0.0.2/CUDG/
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:49:37.337046 CUDG-0.0.2/CUDG/VRAManager/
+-rw-r--r--   0 daegeun    (501) staff       (20)      120 2023-05-21 14:59:59.000000 CUDG-0.0.2/CUDG/VRAManager/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       28 2023-05-21 14:13:48.000000 CUDG-0.0.2/CUDG/VRAManager/assigner.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       27 2023-05-21 14:14:26.000000 CUDG-0.0.2/CUDG/VRAManager/cleaner.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      567 2023-05-22 04:02:27.000000 CUDG-0.0.2/CUDG/VRAManager/memory.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      145 2023-08-03 02:49:04.000000 CUDG-0.0.2/CUDG/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:49:37.337689 CUDG-0.0.2/CUDG/gpuarray/
+-rw-r--r--   0 daegeun    (501) staff       (20)       32 2023-05-21 14:59:49.000000 CUDG-0.0.2/CUDG/gpuarray/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1572 2023-07-30 06:08:09.000000 CUDG-0.0.2/CUDG/gpuarray/gpuarray.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:49:37.338718 CUDG-0.0.2/CUDG/linalg/
+-rw-r--r--   0 daegeun    (501) staff       (20)       24 2023-07-30 01:42:39.000000 CUDG-0.0.2/CUDG/linalg/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1930 2023-07-30 03:31:27.000000 CUDG-0.0.2/CUDG/linalg/linalg.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     3117 2023-07-30 01:45:19.000000 CUDG-0.0.2/CUDG/linalg/linalgcore.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:49:37.339452 CUDG-0.0.2/CUDG/sparse/
+-rw-r--r--   0 daegeun    (501) staff       (20)       17 2023-05-19 05:03:17.000000 CUDG-0.0.2/CUDG/sparse/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1416 2023-05-22 04:06:14.000000 CUDG-0.0.2/CUDG/sparse/gpusparse.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:49:37.335717 CUDG-0.0.2/CUDG.egg-info/
+-rw-r--r--   0 daegeun    (501) staff       (20)      468 2023-08-03 02:49:37.000000 CUDG-0.0.2/CUDG.egg-info/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      456 2023-08-03 02:49:37.000000 CUDG-0.0.2/CUDG.egg-info/SOURCES.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:49:37.000000 CUDG-0.0.2/CUDG.egg-info/dependency_links.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:46:22.000000 CUDG-0.0.2/CUDG.egg-info/not-zip-safe
+-rw-r--r--   0 daegeun    (501) staff       (20)        5 2023-08-03 02:49:37.000000 CUDG-0.0.2/CUDG.egg-info/top_level.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)      468 2023-08-03 02:49:37.339904 CUDG-0.0.2/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      172 2023-05-19 05:03:17.000000 CUDG-0.0.2/README.md
+-rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 02:49:37.340366 CUDG-0.0.2/setup.cfg
+-rw-r--r--   0 daegeun    (501) staff       (20)      684 2023-08-03 02:49:13.000000 CUDG-0.0.2/setup.py
```

### Comparing `CUDG-0.0.1/VRAManager/memory.py` & `CUDG-0.0.2/CUDG/VRAManager/memory.py`

 * *Files identical despite different names*

### Comparing `CUDG-0.0.1/gpuarray/gpuarray.py` & `CUDG-0.0.2/CUDG/gpuarray/gpuarray.py`

 * *Files identical despite different names*

### Comparing `CUDG-0.0.1/linalg/linalg.py` & `CUDG-0.0.2/CUDG/linalg/linalg.py`

 * *Files identical despite different names*

### Comparing `CUDG-0.0.1/linalg/linalgcore.py` & `CUDG-0.0.2/CUDG/linalg/linalgcore.py`

 * *Files identical despite different names*

### Comparing `CUDG-0.0.1/setup.py` & `CUDG-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='CUDG',
-    version='0.0.1',
+    version='0.0.2',
     description='CUDG is for gpuarray type for convenience',
     author='Daegeun02',
     author_email='redhawkdg02@gmail.com',
     url='https://github.com/Daegeun02/cudg.git',
     install_requires=[],
     packages=find_packages( exclude=[] ),
     keywords=['CUDG', 'by daegeun', 'for convenience'],
```

### Comparing `CUDG-0.0.1/sparse/gpusparse.py` & `CUDG-0.0.2/CUDG/sparse/gpusparse.py`

 * *Files identical despite different names*

