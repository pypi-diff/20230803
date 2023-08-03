# Comparing `tmp/CrazyDG-0.0.2.tar.gz` & `tmp/CrazyDG-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrazyDG-0.0.2.tar", last modified: Thu Aug  3 01:59:38 2023, max compression
+gzip compressed data, was "CrazyDG-0.0.3.tar", last modified: Thu Aug  3 02:09:15 2023, max compression
```

## Comparing `CrazyDG-0.0.2.tar` & `CrazyDG-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.346844 CrazyDG-0.0.2/
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.340749 CrazyDG-0.0.2/CrazyDG/
--rw-r--r--   0 daegeun    (501) staff       (20)      183 2023-08-03 01:58:56.000000 CrazyDG-0.0.2/CrazyDG/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.342946 CrazyDG-0.0.2/CrazyDG/control/
--rw-r--r--   0 daegeun    (501) staff       (20)     2003 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/control/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/control/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/control/integral_loop.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/control/optimus_prime.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.343413 CrazyDG-0.0.2/CrazyDG/crazy/
--rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/crazy/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/crazy/crazy.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.343670 CrazyDG-0.0.2/CrazyDG/guidance/
--rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.345311 CrazyDG-0.0.2/CrazyDG/guidance/utils/
--rw-r--r--   0 daegeun    (501) staff       (20)      109 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)       86 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      947 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/goto.py
--rw-r--r--   0 daegeun    (501) staff       (20)      826 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/hover.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1101 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/landing.py
--rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/smoother.py
--rw-r--r--   0 daegeun    (501) staff       (20)      970 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/guidance/utils/takeoff.py
--rw-r--r--   0 daegeun    (501) staff       (20)      805 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/main_example.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.346276 CrazyDG-0.0.2/CrazyDG/navigation/
--rw-r--r--   0 daegeun    (501) staff       (20)      518 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/navigation/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1658 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/navigation/imu.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2096 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/navigation/imu_setup.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/CrazyDG/navigation/qualisys.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 01:59:38.341940 CrazyDG-0.0.2/CrazyDG.egg-info/
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 01:59:38.000000 CrazyDG-0.0.2/CrazyDG.egg-info/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      774 2023-08-03 01:59:38.000000 CrazyDG-0.0.2/CrazyDG.egg-info/SOURCES.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 01:59:38.000000 CrazyDG-0.0.2/CrazyDG.egg-info/dependency_links.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 01:59:38.000000 CrazyDG-0.0.2/CrazyDG.egg-info/not-zip-safe
--rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 01:59:38.000000 CrazyDG-0.0.2/CrazyDG.egg-info/top_level.txt
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 01:59:38.346589 CrazyDG-0.0.2/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.2/README.md
--rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 01:59:38.346910 CrazyDG-0.0.2/setup.cfg
--rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 01:59:00.000000 CrazyDG-0.0.2/setup.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.804783 CrazyDG-0.0.3/
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.798351 CrazyDG-0.0.3/CrazyDG/
+-rw-r--r--   0 daegeun    (501) staff       (20)      183 2023-08-03 02:08:55.000000 CrazyDG-0.0.3/CrazyDG/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.800667 CrazyDG-0.0.3/CrazyDG/control/
+-rw-r--r--   0 daegeun    (501) staff       (20)     2003 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/control/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/control/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/control/integral_loop.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/control/optimus_prime.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.801163 CrazyDG-0.0.3/CrazyDG/crazy/
+-rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/crazy/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/crazy/crazy.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.801402 CrazyDG-0.0.3/CrazyDG/guidance/
+-rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.3/CrazyDG/guidance/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.803146 CrazyDG-0.0.3/CrazyDG/guidance/utils/
+-rw-r--r--   0 daegeun    (501) staff       (20)      114 2023-08-03 02:08:21.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      948 2023-08-03 02:04:57.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/_goto.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      827 2023-08-03 02:05:05.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/_hover.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1102 2023-08-03 02:05:11.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/_landing.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      971 2023-08-03 02:05:20.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/_takeoff.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       86 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/smoother.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      805 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/main_example.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.804163 CrazyDG-0.0.3/CrazyDG/navigation/
+-rw-r--r--   0 daegeun    (501) staff       (20)      518 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/navigation/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1658 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/navigation/imu.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2096 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/navigation/imu_setup.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/navigation/qualisys.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.799591 CrazyDG-0.0.3/CrazyDG.egg-info/
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 02:09:15.000000 CrazyDG-0.0.3/CrazyDG.egg-info/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      778 2023-08-03 02:09:15.000000 CrazyDG-0.0.3/CrazyDG.egg-info/SOURCES.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:09:15.000000 CrazyDG-0.0.3/CrazyDG.egg-info/dependency_links.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:09:15.000000 CrazyDG-0.0.3/CrazyDG.egg-info/not-zip-safe
+-rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 02:09:15.000000 CrazyDG-0.0.3/CrazyDG.egg-info/top_level.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 02:09:15.804508 CrazyDG-0.0.3/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/README.md
+-rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 02:09:15.804854 CrazyDG-0.0.3/setup.cfg
+-rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 02:09:00.000000 CrazyDG-0.0.3/setup.py
```

### Comparing `CrazyDG-0.0.2/CrazyDG/control/__init__.py` & `CrazyDG-0.0.3/CrazyDG/control/__init__.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.2/CrazyDG/control/optimus_prime.py` & `CrazyDG-0.0.3/CrazyDG/control/optimus_prime.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.2/CrazyDG/guidance/utils/goto.py` & `CrazyDG-0.0.3/CrazyDG/guidance/utils/_goto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from crazy import CrazyDragon
 
 from .smoother import smooth_command
 
+from .constants import Kp, Kd, g
+
 from numpy import array, zeros
 
 from time import sleep
 
-from constants import Kp, Kd, g
-
 
 
 def goto( cf: CrazyDragon, destination, T, dt=0.1 ):
 
     cur     = zeros(3)
     des     = zeros(3)
     des_cmd = zeros(3)
```

### Comparing `CrazyDG-0.0.2/CrazyDG/guidance/utils/hover.py` & `CrazyDG-0.0.3/CrazyDG/guidance/utils/_hover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from crazy import CrazyDragon
 
 from .smoother import smooth_command
 
+from .constants import Kp, Kd, g
+
 from numpy import array, zeros
 
 from time import sleep
 
-from constants import Kp, Kd, g
-
 
 
 def hover( cf: CrazyDragon, T, dt=0.1 ):
 
     cur     = zeros(3)
     des     = zeros(3)
     des_cmd = zeros(3)
```

### Comparing `CrazyDG-0.0.2/CrazyDG/guidance/utils/landing.py` & `CrazyDG-0.0.3/CrazyDG/guidance/utils/_landing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from crazy import CrazyDragon
 
 from .smoother import smooth_command
 
+from .constants import Kp, Kd, g
+
 from numpy        import array, zeros
 from numpy.linalg import norm
 
 from time import sleep
 
-from constants import Kp, Kd, g
-
 
 
 def landing( cf: CrazyDragon, h=0.2, T=3, dt=0.1, step=0.075 ):
 
     cur     = zeros(3)
     des     = zeros(3)
     des_cmd = zeros(3)
```

### Comparing `CrazyDG-0.0.2/CrazyDG/guidance/utils/takeoff.py` & `CrazyDG-0.0.3/CrazyDG/guidance/utils/_takeoff.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from crazy import CrazyDragon
 
 from .smoother import smooth_command
 
+from .constants import Kp, Kd, g
+
 from numpy import array, zeros
 
 from time import sleep
 
-from constants import Kp, Kd, g
-
 
 
 def takeoff( cf: CrazyDragon, h=1.5, T=3, dt=0.1 ):
 
     cur     = zeros(3)
     des     = zeros(3)
     des_cmd = zeros(3)
```

### Comparing `CrazyDG-0.0.2/CrazyDG/main_example.py` & `CrazyDG-0.0.3/CrazyDG/main_example.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.2/CrazyDG/navigation/__init__.py` & `CrazyDG-0.0.3/CrazyDG/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.2/CrazyDG/navigation/imu.py` & `CrazyDG-0.0.3/CrazyDG/navigation/imu.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.2/CrazyDG/navigation/imu_setup.py` & `CrazyDG-0.0.3/CrazyDG/navigation/imu_setup.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.2/CrazyDG/navigation/qualisys.py` & `CrazyDG-0.0.3/CrazyDG/navigation/qualisys.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.2/CrazyDG.egg-info/SOURCES.txt` & `CrazyDG-0.0.3/CrazyDG.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 CrazyDG/control/constants.py
 CrazyDG/control/integral_loop.py
 CrazyDG/control/optimus_prime.py
 CrazyDG/crazy/__init__.py
 CrazyDG/crazy/crazy.py
 CrazyDG/guidance/__init__.py
 CrazyDG/guidance/utils/__init__.py
+CrazyDG/guidance/utils/_goto.py
+CrazyDG/guidance/utils/_hover.py
+CrazyDG/guidance/utils/_landing.py
+CrazyDG/guidance/utils/_takeoff.py
 CrazyDG/guidance/utils/constants.py
-CrazyDG/guidance/utils/goto.py
-CrazyDG/guidance/utils/hover.py
-CrazyDG/guidance/utils/landing.py
 CrazyDG/guidance/utils/smoother.py
-CrazyDG/guidance/utils/takeoff.py
 CrazyDG/navigation/__init__.py
 CrazyDG/navigation/imu.py
 CrazyDG/navigation/imu_setup.py
 CrazyDG/navigation/qualisys.py
```

### Comparing `CrazyDG-0.0.2/setup.py` & `CrazyDG-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='CrazyDG',
-    version='0.0.2',
+    version='0.0.3',
     description='CrazyDG is for convenience',
     author='Daegeun02',
     author_email='redhawkdg02@gmail.com',
     url='https://github.com/Daegeun02/CrazyDG.git',
     install_requires=[],
     packages=find_packages( exclude=[] ),
     keywords=['CrazyDG', 'by daegeun', 'for convenience'],
```

