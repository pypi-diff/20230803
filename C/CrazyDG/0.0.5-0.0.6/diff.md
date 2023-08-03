# Comparing `tmp/CrazyDG-0.0.5.tar.gz` & `tmp/CrazyDG-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrazyDG-0.0.5.tar", last modified: Thu Aug  3 10:21:59 2023, max compression
+gzip compressed data, was "CrazyDG-0.0.6.tar", last modified: Thu Aug  3 10:30:42 2023, max compression
```

## Comparing `CrazyDG-0.0.5.tar` & `CrazyDG-0.0.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.213108 CrazyDG-0.0.5/
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.204178 CrazyDG-0.0.5/CrazyDG/
--rw-r--r--   0 daegeun    (501) staff       (20)      215 2023-08-03 10:12:32.000000 CrazyDG-0.0.5/CrazyDG/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.206744 CrazyDG-0.0.5/CrazyDG/control/
--rw-r--r--   0 daegeun    (501) staff       (20)     2159 2023-08-03 10:11:52.000000 CrazyDG-0.0.5/CrazyDG/control/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/control/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/control/integral_loop.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/control/optimus_prime.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.207297 CrazyDG-0.0.5/CrazyDG/crazy/
--rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/crazy/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/crazy/crazy.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.207574 CrazyDG-0.0.5/CrazyDG/guidance/
--rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.5/CrazyDG/guidance/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.210269 CrazyDG-0.0.5/CrazyDG/guidance/utils/
--rw-r--r--   0 daegeun    (501) staff       (20)      114 2023-08-03 02:08:21.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      944 2023-08-03 10:00:35.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/_goto.py
--rw-r--r--   0 daegeun    (501) staff       (20)      804 2023-08-03 10:01:00.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/_hover.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1169 2023-08-03 10:02:43.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/_landing.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1011 2023-08-03 10:09:19.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/_landing_supporter.py
--rw-r--r--   0 daegeun    (501) staff       (20)      964 2023-08-03 10:03:33.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/_takeoff.py
--rw-r--r--   0 daegeun    (501) staff       (20)       86 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/guidance/utils/smoother.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1018 2023-08-03 10:19:59.000000 CrazyDG-0.0.5/CrazyDG/main_example.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.211391 CrazyDG-0.0.5/CrazyDG/navigation/
--rw-r--r--   0 daegeun    (501) staff       (20)      966 2023-08-03 10:11:41.000000 CrazyDG-0.0.5/CrazyDG/navigation/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1658 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/navigation/imu.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2096 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/navigation/imu_setup.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/CrazyDG/navigation/qualisys.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.212459 CrazyDG-0.0.5/CrazyDG/recorder/
--rw-r--r--   0 daegeun    (501) staff       (20)       63 2023-08-03 02:12:37.000000 CrazyDG-0.0.5/CrazyDG/recorder/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     3205 2023-08-03 10:13:00.000000 CrazyDG-0.0.5/CrazyDG/recorder/recorder.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2451 2023-08-03 02:12:37.000000 CrazyDG-0.0.5/CrazyDG/recorder/visualizer.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:21:59.205460 CrazyDG-0.0.5/CrazyDG.egg-info/
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 10:21:59.000000 CrazyDG-0.0.5/CrazyDG.egg-info/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      912 2023-08-03 10:21:59.000000 CrazyDG-0.0.5/CrazyDG.egg-info/SOURCES.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 10:21:59.000000 CrazyDG-0.0.5/CrazyDG.egg-info/dependency_links.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 10:21:59.000000 CrazyDG-0.0.5/CrazyDG.egg-info/not-zip-safe
--rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 10:21:59.000000 CrazyDG-0.0.5/CrazyDG.egg-info/top_level.txt
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 10:21:59.212850 CrazyDG-0.0.5/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.5/README.md
--rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 10:21:59.213174 CrazyDG-0.0.5/setup.cfg
--rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 10:20:43.000000 CrazyDG-0.0.5/setup.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:30:42.846955 CrazyDG-0.0.6/
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:30:42.836233 CrazyDG-0.0.6/CrazyDG/
+-rw-r--r--   0 daegeun    (501) staff       (20)      215 2023-08-03 10:30:38.000000 CrazyDG-0.0.6/CrazyDG/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:30:42.839161 CrazyDG-0.0.6/CrazyDG/control/
+-rw-r--r--   0 daegeun    (501) staff       (20)     2159 2023-08-03 10:11:52.000000 CrazyDG-0.0.6/CrazyDG/control/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.6/CrazyDG/control/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.6/CrazyDG/control/integral_loop.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.6/CrazyDG/control/optimus_prime.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:30:42.839843 CrazyDG-0.0.6/CrazyDG/crazy/
+-rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.6/CrazyDG/crazy/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.6/CrazyDG/crazy/crazy.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:30:42.840275 CrazyDG-0.0.6/CrazyDG/guidance/
+-rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.6/CrazyDG/guidance/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:30:42.843239 CrazyDG-0.0.6/CrazyDG/guidance/utils/
+-rw-r--r--   0 daegeun    (501) staff       (20)      165 2023-08-03 10:28:33.000000 CrazyDG-0.0.6/CrazyDG/guidance/utils/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      944 2023-08-03 10:00:35.000000 CrazyDG-0.0.6/CrazyDG/guidance/utils/_goto.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      807 2023-08-03 10:28:10.000000 CrazyDG-0.0.6/CrazyDG/guidance/utils/_hover.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1172 2023-08-03 10:28:18.000000 CrazyDG-0.0.6/CrazyDG/guidance/utils/_landing.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1011 2023-08-03 10:09:19.000000 CrazyDG-0.0.6/CrazyDG/guidance/utils/_landing_supporter.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      967 2023-08-03 10:28:22.000000 CrazyDG-0.0.6/CrazyDG/guidance/utils/_takeoff.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       86 2023-08-03 01:51:19.000000 CrazyDG-0.0.6/CrazyDG/guidance/utils/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.6/CrazyDG/guidance/utils/smoother.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1018 2023-08-03 10:19:59.000000 CrazyDG-0.0.6/CrazyDG/main_example.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:30:42.844491 CrazyDG-0.0.6/CrazyDG/navigation/
+-rw-r--r--   0 daegeun    (501) staff       (20)      968 2023-08-03 10:28:03.000000 CrazyDG-0.0.6/CrazyDG/navigation/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1660 2023-08-03 10:27:51.000000 CrazyDG-0.0.6/CrazyDG/navigation/imu.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2098 2023-08-03 10:27:54.000000 CrazyDG-0.0.6/CrazyDG/navigation/imu_setup.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.6/CrazyDG/navigation/qualisys.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:30:42.846205 CrazyDG-0.0.6/CrazyDG/recorder/
+-rw-r--r--   0 daegeun    (501) staff       (20)       63 2023-08-03 02:12:37.000000 CrazyDG-0.0.6/CrazyDG/recorder/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     3209 2023-08-03 10:30:11.000000 CrazyDG-0.0.6/CrazyDG/recorder/recorder.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2451 2023-08-03 02:12:37.000000 CrazyDG-0.0.6/CrazyDG/recorder/visualizer.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 10:30:42.837833 CrazyDG-0.0.6/CrazyDG.egg-info/
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 10:30:42.000000 CrazyDG-0.0.6/CrazyDG.egg-info/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      912 2023-08-03 10:30:42.000000 CrazyDG-0.0.6/CrazyDG.egg-info/SOURCES.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 10:30:42.000000 CrazyDG-0.0.6/CrazyDG.egg-info/dependency_links.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 10:30:42.000000 CrazyDG-0.0.6/CrazyDG.egg-info/not-zip-safe
+-rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 10:30:42.000000 CrazyDG-0.0.6/CrazyDG.egg-info/top_level.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 10:30:42.846625 CrazyDG-0.0.6/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.6/README.md
+-rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 10:30:42.847034 CrazyDG-0.0.6/setup.cfg
+-rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 10:30:27.000000 CrazyDG-0.0.6/setup.py
```

### Comparing `CrazyDG-0.0.5/CrazyDG/control/__init__.py` & `CrazyDG-0.0.6/CrazyDG/control/__init__.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.5/CrazyDG/control/optimus_prime.py` & `CrazyDG-0.0.6/CrazyDG/control/optimus_prime.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.5/CrazyDG/guidance/utils/_goto.py` & `CrazyDG-0.0.6/CrazyDG/guidance/utils/_goto.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.5/CrazyDG/guidance/utils/_hover.py` & `CrazyDG-0.0.6/CrazyDG/guidance/utils/_hover.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from crazy import CrazyDragon
+from ...crazy import CrazyDragon
 
 from .smoother import smooth_command
 
 from .constants import Kp, Kd, g
 
 from numpy import array, zeros
```

### Comparing `CrazyDG-0.0.5/CrazyDG/guidance/utils/_landing.py` & `CrazyDG-0.0.6/CrazyDG/guidance/utils/_landing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from crazy import CrazyDragon
+from ...crazy import CrazyDragon
 
 from .smoother import smooth_command
 
 from .constants import Kp, Kd, g
 
 from numpy        import array, zeros
 from numpy.linalg import norm
```

### Comparing `CrazyDG-0.0.5/CrazyDG/guidance/utils/_landing_supporter.py` & `CrazyDG-0.0.6/CrazyDG/guidance/utils/_landing_supporter.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.5/CrazyDG/guidance/utils/_takeoff.py` & `CrazyDG-0.0.6/CrazyDG/guidance/utils/_takeoff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from crazy import CrazyDragon
+from ...crazy import CrazyDragon
 
 from .smoother import smooth_command
 
 from .constants import Kp, Kd, g
 
 from numpy import array, zeros
```

### Comparing `CrazyDG-0.0.5/CrazyDG/main_example.py` & `CrazyDG-0.0.6/CrazyDG/main_example.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.5/CrazyDG/navigation/__init__.py` & `CrazyDG-0.0.6/CrazyDG/navigation/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from crazy import CrazyDragon
+from ..crazy import CrazyDragon
 
 from threading import Thread
 
 from .imu       import IMU
 from .qualisys  import Qualisys
 
 from time import sleep
```

### Comparing `CrazyDG-0.0.5/CrazyDG/navigation/imu.py` & `CrazyDG-0.0.6/CrazyDG/navigation/imu.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from crazy import CrazyDragon
+from ..crazy import CrazyDragon
 
 from .imu_setup import *
 
 from cflib.crazyflie.log import LogConfig
```

### Comparing `CrazyDG-0.0.5/CrazyDG/navigation/imu_setup.py` & `CrazyDG-0.0.6/CrazyDG/navigation/imu_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from crazy import CrazyDragon
+from ..crazy import CrazyDragon
 
 import time
 
 from cflib.crazyflie.log        import LogConfig
 from cflib.crazyflie.syncLogger import SyncLogger
```

### Comparing `CrazyDG-0.0.5/CrazyDG/navigation/qualisys.py` & `CrazyDG-0.0.6/CrazyDG/navigation/qualisys.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.5/CrazyDG/recorder/recorder.py` & `CrazyDG-0.0.6/CrazyDG/recorder/recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from crazy import CrazyDragon
+from ..crazy import CrazyDragon
 
 from threading import Thread
 
 from numpy import zeros, array
 
 from time  import sleep
 
-from control import alpha
+from ..control import alpha
 
 from .visualizer import *
 
 
 
 class Recorder( Thread ):
```

### Comparing `CrazyDG-0.0.5/CrazyDG/recorder/visualizer.py` & `CrazyDG-0.0.6/CrazyDG/recorder/visualizer.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.5/CrazyDG.egg-info/SOURCES.txt` & `CrazyDG-0.0.6/CrazyDG.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.5/setup.py` & `CrazyDG-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='CrazyDG',
-    version='0.0.5',
+    version='0.0.6',
     description='CrazyDG is for convenience',
     author='Daegeun02',
     author_email='redhawkdg02@gmail.com',
     url='https://github.com/Daegeun02/CrazyDG.git',
     install_requires=[],
     packages=find_packages( exclude=[] ),
     keywords=['CrazyDG', 'by daegeun', 'for convenience'],
```

