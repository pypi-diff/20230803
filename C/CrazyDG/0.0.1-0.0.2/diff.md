# Comparing `tmp/CrazyDG-0.0.1.tar.gz` & `tmp/CrazyDG-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrazyDG-0.0.1.tar", last modified: Thu Aug  3 01:47:13 2023, max compression
+gzip compressed data, was "CrazyDG-0.0.2.tar", last modified: Thu Aug  3 01:59:38 2023, max compression
```

## Comparing `CrazyDG-0.0.1.tar` & `CrazyDG-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:47:13.156260 CrazyDG-0.0.1/
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:47:13.150165 CrazyDG-0.0.1/CrazyDG/
--rw-r--r--   0 daegeun    (501) staff       (20)      154 2023-08-03 01:43:02.000000 CrazyDG-0.0.1/CrazyDG/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:47:13.152210 CrazyDG-0.0.1/CrazyDG/control/
--rw-r--r--   0 daegeun    (501) staff       (20)     2003 2023-08-03 01:28:34.000000 CrazyDG-0.0.1/CrazyDG/control/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 00:57:59.000000 CrazyDG-0.0.1/CrazyDG/control/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:13:03.000000 CrazyDG-0.0.1/CrazyDG/control/integral_loop.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 00:58:20.000000 CrazyDG-0.0.1/CrazyDG/control/optimus_prime.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:47:13.152767 CrazyDG-0.0.1/CrazyDG/crazy/
--rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:07:36.000000 CrazyDG-0.0.1/CrazyDG/crazy/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:07:19.000000 CrazyDG-0.0.1/CrazyDG/crazy/crazy.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:47:13.153007 CrazyDG-0.0.1/CrazyDG/guidance/
--rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 01:27:22.000000 CrazyDG-0.0.1/CrazyDG/guidance/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:47:13.154756 CrazyDG-0.0.1/CrazyDG/guidance/utils/
--rw-r--r--   0 daegeun    (501) staff       (20)      109 2023-08-03 01:05:27.000000 CrazyDG-0.0.1/CrazyDG/guidance/utils/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)       86 2023-08-03 01:05:27.000000 CrazyDG-0.0.1/CrazyDG/guidance/utils/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      947 2023-08-03 01:23:17.000000 CrazyDG-0.0.1/CrazyDG/guidance/utils/goto.py
--rw-r--r--   0 daegeun    (501) staff       (20)      826 2023-08-03 01:21:00.000000 CrazyDG-0.0.1/CrazyDG/guidance/utils/hover.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1101 2023-08-03 01:25:53.000000 CrazyDG-0.0.1/CrazyDG/guidance/utils/landing.py
--rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:05:27.000000 CrazyDG-0.0.1/CrazyDG/guidance/utils/smoother.py
--rw-r--r--   0 daegeun    (501) staff       (20)      970 2023-08-03 01:18:19.000000 CrazyDG-0.0.1/CrazyDG/guidance/utils/takeoff.py
--rw-r--r--   0 daegeun    (501) staff       (20)      805 2023-08-03 01:35:20.000000 CrazyDG-0.0.1/CrazyDG/main_example.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:47:13.155675 CrazyDG-0.0.1/CrazyDG/navigation/
--rw-r--r--   0 daegeun    (501) staff       (20)      518 2023-08-03 01:29:45.000000 CrazyDG-0.0.1/CrazyDG/navigation/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1658 2023-08-03 01:09:38.000000 CrazyDG-0.0.1/CrazyDG/navigation/imu.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2096 2023-08-03 01:11:38.000000 CrazyDG-0.0.1/CrazyDG/navigation/imu_setup.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:03:19.000000 CrazyDG-0.0.1/CrazyDG/navigation/qualisys.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:47:13.151239 CrazyDG-0.0.1/CrazyDG.egg-info/
--rw-r--r--   0 daegeun    (501) staff       (20)      507 2023-08-03 01:47:12.000000 CrazyDG-0.0.1/CrazyDG.egg-info/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      764 2023-08-03 01:47:13.000000 CrazyDG-0.0.1/CrazyDG.egg-info/SOURCES.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 01:47:12.000000 CrazyDG-0.0.1/CrazyDG.egg-info/dependency_links.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 01:47:12.000000 CrazyDG-0.0.1/CrazyDG.egg-info/not-zip-safe
--rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 01:47:12.000000 CrazyDG-0.0.1/CrazyDG.egg-info/top_level.txt
--rw-r--r--   0 daegeun    (501) staff       (20)      507 2023-08-03 01:47:13.156031 CrazyDG-0.0.1/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 01:47:13.156345 CrazyDG-0.0.1/setup.cfg
--rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 01:40:39.000000 CrazyDG-0.0.1/setup.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.346844 CrazyDG-0.0.2/
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.340749 CrazyDG-0.0.2/CrazyDG/
+-rw-r--r--   0 daegeun    (501) staff       (20)      183 2023-08-03 01:58:56.000000 CrazyDG-0.0.2/CrazyDG/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.342946 CrazyDG-0.0.2/CrazyDG/control/
+-rw-r--r--   0 daegeun    (501) staff       (20)     2003 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/control/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/control/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/control/integral_loop.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/control/optimus_prime.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.343413 CrazyDG-0.0.2/CrazyDG/crazy/
+-rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/crazy/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/crazy/crazy.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.343670 CrazyDG-0.0.2/CrazyDG/guidance/
+-rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.345311 CrazyDG-0.0.2/CrazyDG/guidance/utils/
+-rw-r--r--   0 daegeun    (501) staff       (20)      109 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       86 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      947 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/goto.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      826 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/hover.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1101 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/landing.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/smoother.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      970 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/takeoff.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      805 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/main_example.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.346276 CrazyDG-0.0.2/CrazyDG/navigation/
+-rw-r--r--   0 daegeun    (501) staff       (20)      518 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/navigation/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1658 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/navigation/imu.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2096 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/navigation/imu_setup.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/navigation/qualisys.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.341940 CrazyDG-0.0.2/CrazyDG.egg-info/
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 01:59:38.000000 CrazyDG-0.0.2/CrazyDG.egg-info/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      774 2023-08-03 01:59:38.000000 CrazyDG-0.0.2/CrazyDG.egg-info/SOURCES.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 01:59:38.000000 CrazyDG-0.0.2/CrazyDG.egg-info/dependency_links.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 01:59:38.000000 CrazyDG-0.0.2/CrazyDG.egg-info/not-zip-safe
+-rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 01:59:38.000000 CrazyDG-0.0.2/CrazyDG.egg-info/top_level.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 01:59:38.346589 CrazyDG-0.0.2/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/README.md
+-rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 01:59:38.346910 CrazyDG-0.0.2/setup.cfg
+-rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 01:59:00.000000 CrazyDG-0.0.2/setup.py
```

### Comparing `CrazyDG-0.0.1/CrazyDG/control/__init__.py` & `CrazyDG-0.0.2/CrazyDG/control/__init__.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG/control/optimus_prime.py` & `CrazyDG-0.0.2/CrazyDG/control/optimus_prime.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG/guidance/utils/goto.py` & `CrazyDG-0.0.2/CrazyDG/guidance/utils/goto.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG/guidance/utils/hover.py` & `CrazyDG-0.0.2/CrazyDG/guidance/utils/hover.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG/guidance/utils/landing.py` & `CrazyDG-0.0.2/CrazyDG/guidance/utils/landing.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG/guidance/utils/takeoff.py` & `CrazyDG-0.0.2/CrazyDG/guidance/utils/takeoff.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG/main_example.py` & `CrazyDG-0.0.2/CrazyDG/main_example.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG/navigation/__init__.py` & `CrazyDG-0.0.2/CrazyDG/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG/navigation/imu.py` & `CrazyDG-0.0.2/CrazyDG/navigation/imu.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG/navigation/imu_setup.py` & `CrazyDG-0.0.2/CrazyDG/navigation/imu_setup.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG/navigation/qualisys.py` & `CrazyDG-0.0.2/CrazyDG/navigation/qualisys.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.1/CrazyDG.egg-info/SOURCES.txt` & `CrazyDG-0.0.2/CrazyDG.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 CrazyDG/__init__.py
 CrazyDG/main_example.py
 CrazyDG.egg-info/PKG-INFO
 CrazyDG.egg-info/SOURCES.txt
 CrazyDG.egg-info/dependency_links.txt
 CrazyDG.egg-info/not-zip-safe
```

### Comparing `CrazyDG-0.0.1/setup.py` & `CrazyDG-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='CrazyDG',
-    version='0.0.1',
+    version='0.0.2',
     description='CrazyDG is for convenience',
     author='Daegeun02',
     author_email='redhawkdg02@gmail.com',
     url='https://github.com/Daegeun02/CrazyDG.git',
     install_requires=[],
     packages=find_packages( exclude=[] ),
     keywords=['CrazyDG', 'by daegeun', 'for convenience'],
```

