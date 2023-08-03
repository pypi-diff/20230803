# Comparing `tmp/CrazyDG-0.0.7.tar.gz` & `tmp/CrazyDG-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrazyDG-0.0.7.tar", last modified: Thu Aug  3 14:21:26 2023, max compression
+gzip compressed data, was "CrazyDG-0.0.8.tar", last modified: Thu Aug  3 14:24:42 2023, max compression
```

## Comparing `CrazyDG-0.0.7.tar` & `CrazyDG-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:21:26.282470 CrazyDG-0.0.7/
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:21:26.274400 CrazyDG-0.0.7/CrazyDG/
--rw-r--r--   0 daegeun    (501) staff       (20)      215 2023-08-03 14:21:12.000000 CrazyDG-0.0.7/CrazyDG/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:21:26.277114 CrazyDG-0.0.7/CrazyDG/control/
--rw-r--r--   0 daegeun    (501) staff       (20)     2159 2023-08-03 10:11:52.000000 CrazyDG-0.0.7/CrazyDG/control/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.7/CrazyDG/control/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.7/CrazyDG/control/integral_loop.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.7/CrazyDG/control/optimus_prime.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:21:26.277639 CrazyDG-0.0.7/CrazyDG/crazy/
--rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.7/CrazyDG/crazy/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.7/CrazyDG/crazy/crazy.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:21:26.277878 CrazyDG-0.0.7/CrazyDG/guidance/
--rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.7/CrazyDG/guidance/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:21:26.279993 CrazyDG-0.0.7/CrazyDG/guidance/utils/
--rw-r--r--   0 daegeun    (501) staff       (20)      165 2023-08-03 10:28:33.000000 CrazyDG-0.0.7/CrazyDG/guidance/utils/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      953 2023-08-03 14:12:26.000000 CrazyDG-0.0.7/CrazyDG/guidance/utils/_goto.py
--rw-r--r--   0 daegeun    (501) staff       (20)      807 2023-08-03 10:28:10.000000 CrazyDG-0.0.7/CrazyDG/guidance/utils/_hover.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1172 2023-08-03 11:08:07.000000 CrazyDG-0.0.7/CrazyDG/guidance/utils/_landing.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1011 2023-08-03 10:09:19.000000 CrazyDG-0.0.7/CrazyDG/guidance/utils/_landing_supporter.py
--rw-r--r--   0 daegeun    (501) staff       (20)      967 2023-08-03 10:28:22.000000 CrazyDG-0.0.7/CrazyDG/guidance/utils/_takeoff.py
--rw-r--r--   0 daegeun    (501) staff       (20)      157 2023-08-03 14:18:14.000000 CrazyDG-0.0.7/CrazyDG/guidance/utils/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.7/CrazyDG/guidance/utils/smoother.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1018 2023-08-03 10:19:59.000000 CrazyDG-0.0.7/CrazyDG/main_example.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:21:26.281094 CrazyDG-0.0.7/CrazyDG/navigation/
--rw-r--r--   0 daegeun    (501) staff       (20)      968 2023-08-03 10:28:03.000000 CrazyDG-0.0.7/CrazyDG/navigation/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1660 2023-08-03 10:27:51.000000 CrazyDG-0.0.7/CrazyDG/navigation/imu.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2098 2023-08-03 10:27:54.000000 CrazyDG-0.0.7/CrazyDG/navigation/imu_setup.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.7/CrazyDG/navigation/qualisys.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:21:26.281817 CrazyDG-0.0.7/CrazyDG/recorder/
--rw-r--r--   0 daegeun    (501) staff       (20)       63 2023-08-03 02:12:37.000000 CrazyDG-0.0.7/CrazyDG/recorder/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     3209 2023-08-03 10:30:11.000000 CrazyDG-0.0.7/CrazyDG/recorder/recorder.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2451 2023-08-03 02:12:37.000000 CrazyDG-0.0.7/CrazyDG/recorder/visualizer.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:21:26.275843 CrazyDG-0.0.7/CrazyDG.egg-info/
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 14:21:26.000000 CrazyDG-0.0.7/CrazyDG.egg-info/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      912 2023-08-03 14:21:26.000000 CrazyDG-0.0.7/CrazyDG.egg-info/SOURCES.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 14:21:26.000000 CrazyDG-0.0.7/CrazyDG.egg-info/dependency_links.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 14:21:26.000000 CrazyDG-0.0.7/CrazyDG.egg-info/not-zip-safe
--rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 14:21:26.000000 CrazyDG-0.0.7/CrazyDG.egg-info/top_level.txt
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 14:21:26.282168 CrazyDG-0.0.7/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.7/README.md
--rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 14:21:26.282544 CrazyDG-0.0.7/setup.cfg
--rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 14:21:18.000000 CrazyDG-0.0.7/setup.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.335681 CrazyDG-0.0.8/
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.325900 CrazyDG-0.0.8/CrazyDG/
+-rw-r--r--   0 daegeun    (501) staff       (20)      215 2023-08-03 14:24:27.000000 CrazyDG-0.0.8/CrazyDG/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.329045 CrazyDG-0.0.8/CrazyDG/control/
+-rw-r--r--   0 daegeun    (501) staff       (20)     2159 2023-08-03 10:11:52.000000 CrazyDG-0.0.8/CrazyDG/control/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/control/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/control/integral_loop.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/control/optimus_prime.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.329720 CrazyDG-0.0.8/CrazyDG/crazy/
+-rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/crazy/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/crazy/crazy.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.330015 CrazyDG-0.0.8/CrazyDG/guidance/
+-rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.8/CrazyDG/guidance/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.332590 CrazyDG-0.0.8/CrazyDG/guidance/utils/
+-rw-r--r--   0 daegeun    (501) staff       (20)      165 2023-08-03 10:28:33.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      953 2023-08-03 14:12:26.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/_goto.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      807 2023-08-03 10:28:10.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/_hover.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1172 2023-08-03 11:08:07.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/_landing.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      874 2023-08-03 14:24:11.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/_landing_supporter.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      967 2023-08-03 10:28:22.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/_takeoff.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      157 2023-08-03 14:18:14.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/guidance/utils/smoother.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1018 2023-08-03 10:19:59.000000 CrazyDG-0.0.8/CrazyDG/main_example.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.334051 CrazyDG-0.0.8/CrazyDG/navigation/
+-rw-r--r--   0 daegeun    (501) staff       (20)      968 2023-08-03 10:28:03.000000 CrazyDG-0.0.8/CrazyDG/navigation/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1660 2023-08-03 10:27:51.000000 CrazyDG-0.0.8/CrazyDG/navigation/imu.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2098 2023-08-03 10:27:54.000000 CrazyDG-0.0.8/CrazyDG/navigation/imu_setup.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/CrazyDG/navigation/qualisys.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.334960 CrazyDG-0.0.8/CrazyDG/recorder/
+-rw-r--r--   0 daegeun    (501) staff       (20)       63 2023-08-03 02:12:37.000000 CrazyDG-0.0.8/CrazyDG/recorder/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     3209 2023-08-03 10:30:11.000000 CrazyDG-0.0.8/CrazyDG/recorder/recorder.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2451 2023-08-03 02:12:37.000000 CrazyDG-0.0.8/CrazyDG/recorder/visualizer.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 14:24:42.327614 CrazyDG-0.0.8/CrazyDG.egg-info/
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 14:24:42.000000 CrazyDG-0.0.8/CrazyDG.egg-info/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      912 2023-08-03 14:24:42.000000 CrazyDG-0.0.8/CrazyDG.egg-info/SOURCES.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 14:24:42.000000 CrazyDG-0.0.8/CrazyDG.egg-info/dependency_links.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 14:24:42.000000 CrazyDG-0.0.8/CrazyDG.egg-info/not-zip-safe
+-rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 14:24:42.000000 CrazyDG-0.0.8/CrazyDG.egg-info/top_level.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 14:24:42.335352 CrazyDG-0.0.8/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.8/README.md
+-rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 14:24:42.335760 CrazyDG-0.0.8/setup.cfg
+-rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 14:24:25.000000 CrazyDG-0.0.8/setup.py
```

### Comparing `CrazyDG-0.0.7/CrazyDG/control/__init__.py` & `CrazyDG-0.0.8/CrazyDG/control/__init__.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/control/optimus_prime.py` & `CrazyDG-0.0.8/CrazyDG/control/optimus_prime.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/guidance/utils/_goto.py` & `CrazyDG-0.0.8/CrazyDG/guidance/utils/_goto.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/guidance/utils/_hover.py` & `CrazyDG-0.0.8/CrazyDG/guidance/utils/_hover.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/guidance/utils/_landing.py` & `CrazyDG-0.0.8/CrazyDG/guidance/utils/_landing.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/guidance/utils/_takeoff.py` & `CrazyDG-0.0.8/CrazyDG/guidance/utils/_takeoff.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/main_example.py` & `CrazyDG-0.0.8/CrazyDG/main_example.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/navigation/__init__.py` & `CrazyDG-0.0.8/CrazyDG/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/navigation/imu.py` & `CrazyDG-0.0.8/CrazyDG/navigation/imu.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/navigation/imu_setup.py` & `CrazyDG-0.0.8/CrazyDG/navigation/imu_setup.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/navigation/qualisys.py` & `CrazyDG-0.0.8/CrazyDG/navigation/qualisys.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/recorder/recorder.py` & `CrazyDG-0.0.8/CrazyDG/recorder/recorder.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG/recorder/visualizer.py` & `CrazyDG-0.0.8/CrazyDG/recorder/visualizer.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/CrazyDG.egg-info/SOURCES.txt` & `CrazyDG-0.0.8/CrazyDG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.7/setup.py` & `CrazyDG-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='CrazyDG',
-    version='0.0.7',
+    version='0.0.8',
     description='CrazyDG is for convenience',
     author='Daegeun02',
     author_email='redhawkdg02@gmail.com',
     url='https://github.com/Daegeun02/CrazyDG.git',
     install_requires=[],
     packages=find_packages( exclude=[] ),
     keywords=['CrazyDG', 'by daegeun', 'for convenience'],
```

