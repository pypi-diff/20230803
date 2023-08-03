# Comparing `tmp/CrazyDG-0.0.3.tar.gz` & `tmp/CrazyDG-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrazyDG-0.0.3.tar", last modified: Thu Aug  3 02:09:15 2023, max compression
+gzip compressed data, was "CrazyDG-0.0.4.tar", last modified: Thu Aug  3 02:18:10 2023, max compression
```

## Comparing `CrazyDG-0.0.3.tar` & `CrazyDG-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.804783 CrazyDG-0.0.3/
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.798351 CrazyDG-0.0.3/CrazyDG/
--rw-r--r--   0 daegeun    (501) staff       (20)      183 2023-08-03 02:08:55.000000 CrazyDG-0.0.3/CrazyDG/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.800667 CrazyDG-0.0.3/CrazyDG/control/
--rw-r--r--   0 daegeun    (501) staff       (20)     2003 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/control/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/control/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/control/integral_loop.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/control/optimus_prime.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.801163 CrazyDG-0.0.3/CrazyDG/crazy/
--rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/crazy/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/crazy/crazy.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.801402 CrazyDG-0.0.3/CrazyDG/guidance/
--rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.3/CrazyDG/guidance/__init__.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.803146 CrazyDG-0.0.3/CrazyDG/guidance/utils/
--rw-r--r--   0 daegeun    (501) staff       (20)      114 2023-08-03 02:08:21.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)      948 2023-08-03 02:04:57.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/_goto.py
--rw-r--r--   0 daegeun    (501) staff       (20)      827 2023-08-03 02:05:05.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/_hover.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1102 2023-08-03 02:05:11.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/_landing.py
--rw-r--r--   0 daegeun    (501) staff       (20)      971 2023-08-03 02:05:20.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/_takeoff.py
--rw-r--r--   0 daegeun    (501) staff       (20)       86 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/constants.py
--rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/guidance/utils/smoother.py
--rw-r--r--   0 daegeun    (501) staff       (20)      805 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/main_example.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.804163 CrazyDG-0.0.3/CrazyDG/navigation/
--rw-r--r--   0 daegeun    (501) staff       (20)      518 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/navigation/__init__.py
--rw-r--r--   0 daegeun    (501) staff       (20)     1658 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/navigation/imu.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2096 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/navigation/imu_setup.py
--rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/CrazyDG/navigation/qualisys.py
-drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:09:15.799591 CrazyDG-0.0.3/CrazyDG.egg-info/
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 02:09:15.000000 CrazyDG-0.0.3/CrazyDG.egg-info/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)      778 2023-08-03 02:09:15.000000 CrazyDG-0.0.3/CrazyDG.egg-info/SOURCES.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:09:15.000000 CrazyDG-0.0.3/CrazyDG.egg-info/dependency_links.txt
--rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:09:15.000000 CrazyDG-0.0.3/CrazyDG.egg-info/not-zip-safe
--rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 02:09:15.000000 CrazyDG-0.0.3/CrazyDG.egg-info/top_level.txt
--rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 02:09:15.804508 CrazyDG-0.0.3/PKG-INFO
--rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.3/README.md
--rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 02:09:15.804854 CrazyDG-0.0.3/setup.cfg
--rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 02:09:00.000000 CrazyDG-0.0.3/setup.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.810583 CrazyDG-0.0.4/
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.802767 CrazyDG-0.0.4/CrazyDG/
+-rw-r--r--   0 daegeun    (501) staff       (20)      183 2023-08-03 02:12:58.000000 CrazyDG-0.0.4/CrazyDG/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.805042 CrazyDG-0.0.4/CrazyDG/control/
+-rw-r--r--   0 daegeun    (501) staff       (20)     2003 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/control/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       69 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/control/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      459 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/control/integral_loop.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1548 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/control/optimus_prime.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.805554 CrazyDG-0.0.4/CrazyDG/crazy/
+-rw-r--r--   0 daegeun    (501) staff       (20)       30 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/crazy/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      428 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/crazy/crazy.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.805788 CrazyDG-0.0.4/CrazyDG/guidance/
+-rw-r--r--   0 daegeun    (501) staff       (20)      185 2023-08-03 02:04:21.000000 CrazyDG-0.0.4/CrazyDG/guidance/__init__.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.807558 CrazyDG-0.0.4/CrazyDG/guidance/utils/
+-rw-r--r--   0 daegeun    (501) staff       (20)      114 2023-08-03 02:08:21.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      948 2023-08-03 02:04:57.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/_goto.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      827 2023-08-03 02:05:05.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/_hover.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1102 2023-08-03 02:05:11.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/_landing.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      971 2023-08-03 02:05:20.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/_takeoff.py
+-rw-r--r--   0 daegeun    (501) staff       (20)       86 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/constants.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      349 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/guidance/utils/smoother.py
+-rw-r--r--   0 daegeun    (501) staff       (20)      971 2023-08-03 02:17:42.000000 CrazyDG-0.0.4/CrazyDG/main_example.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.809048 CrazyDG-0.0.4/CrazyDG/navigation/
+-rw-r--r--   0 daegeun    (501) staff       (20)      518 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/navigation/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     1658 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/navigation/imu.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2096 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/navigation/imu_setup.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2394 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/CrazyDG/navigation/qualisys.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.809954 CrazyDG-0.0.4/CrazyDG/recorder/
+-rw-r--r--   0 daegeun    (501) staff       (20)       63 2023-08-03 02:12:37.000000 CrazyDG-0.0.4/CrazyDG/recorder/__init__.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     3146 2023-08-03 02:15:01.000000 CrazyDG-0.0.4/CrazyDG/recorder/recorder.py
+-rw-r--r--   0 daegeun    (501) staff       (20)     2451 2023-08-03 02:12:37.000000 CrazyDG-0.0.4/CrazyDG/recorder/visualizer.py
+drwxr-xr-x   0 daegeun    (501) staff       (20)        0 2023-08-03 02:18:10.803962 CrazyDG-0.0.4/CrazyDG.egg-info/
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 02:18:10.000000 CrazyDG-0.0.4/CrazyDG.egg-info/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)      867 2023-08-03 02:18:10.000000 CrazyDG-0.0.4/CrazyDG.egg-info/SOURCES.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:18:10.000000 CrazyDG-0.0.4/CrazyDG.egg-info/dependency_links.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)        1 2023-08-03 02:18:10.000000 CrazyDG-0.0.4/CrazyDG.egg-info/not-zip-safe
+-rw-r--r--   0 daegeun    (501) staff       (20)        8 2023-08-03 02:18:10.000000 CrazyDG-0.0.4/CrazyDG.egg-info/top_level.txt
+-rw-r--r--   0 daegeun    (501) staff       (20)      462 2023-08-03 02:18:10.810293 CrazyDG-0.0.4/PKG-INFO
+-rw-r--r--   0 daegeun    (501) staff       (20)       44 2023-08-03 01:51:19.000000 CrazyDG-0.0.4/README.md
+-rw-r--r--   0 daegeun    (501) staff       (20)       38 2023-08-03 02:18:10.810651 CrazyDG-0.0.4/setup.cfg
+-rw-r--r--   0 daegeun    (501) staff       (20)      678 2023-08-03 02:12:53.000000 CrazyDG-0.0.4/setup.py
```

### Comparing `CrazyDG-0.0.3/CrazyDG/control/__init__.py` & `CrazyDG-0.0.4/CrazyDG/control/__init__.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.3/CrazyDG/control/optimus_prime.py` & `CrazyDG-0.0.4/CrazyDG/control/optimus_prime.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.3/CrazyDG/guidance/utils/_goto.py` & `CrazyDG-0.0.4/CrazyDG/guidance/utils/_goto.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.3/CrazyDG/guidance/utils/_hover.py` & `CrazyDG-0.0.4/CrazyDG/guidance/utils/_hover.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.3/CrazyDG/guidance/utils/_landing.py` & `CrazyDG-0.0.4/CrazyDG/guidance/utils/_landing.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.3/CrazyDG/guidance/utils/_takeoff.py` & `CrazyDG-0.0.4/CrazyDG/guidance/utils/_takeoff.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.3/CrazyDG/main_example.py` & `CrazyDG-0.0.4/CrazyDG/main_example.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from navigation import Navigation
 
 from control import Controller
 
+from recorder import Recorder
+
 from crazy import CrazyDragon
 
 from cflib.crazyflie.syncCrazyflie import SyncCrazyflie
 from cflib.utils                   import uri_helper
 
 from numpy import array
 
@@ -27,18 +29,26 @@
     
     _cf = CrazyDragon()
 
     with SyncCrazyflie( uri, cf=_cf ) as scf:
 
         NAV = Navigation( _cf, nav_config )
         CTR = Controller( _cf, ctr_config )
+        RCD = Recorder( _cf, CTR )
 
         NAV.start()
         CTR.start()
+        RCD.start()
 
         ## your guidance function ##
         CTR.init_send_setpoint()
         ##       from here        ##
 
         ############################
 
-        CTR.stop_send_setpoint()
+        CTR.stop_send_setpoint()
+
+        NAV.join()
+        CTR.join()
+        RCD.join()
+
+    NAV.qtm.close()
```

### Comparing `CrazyDG-0.0.3/CrazyDG/navigation/__init__.py` & `CrazyDG-0.0.4/CrazyDG/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.3/CrazyDG/navigation/imu.py` & `CrazyDG-0.0.4/CrazyDG/navigation/imu.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.3/CrazyDG/navigation/imu_setup.py` & `CrazyDG-0.0.4/CrazyDG/navigation/imu_setup.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.3/CrazyDG/navigation/qualisys.py` & `CrazyDG-0.0.4/CrazyDG/navigation/qualisys.py`

 * *Files identical despite different names*

### Comparing `CrazyDG-0.0.3/CrazyDG.egg-info/SOURCES.txt` & `CrazyDG-0.0.4/CrazyDG.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -20,8 +20,11 @@
 CrazyDG/guidance/utils/_landing.py
 CrazyDG/guidance/utils/_takeoff.py
 CrazyDG/guidance/utils/constants.py
 CrazyDG/guidance/utils/smoother.py
 CrazyDG/navigation/__init__.py
 CrazyDG/navigation/imu.py
 CrazyDG/navigation/imu_setup.py
-CrazyDG/navigation/qualisys.py
+CrazyDG/navigation/qualisys.py
+CrazyDG/recorder/__init__.py
+CrazyDG/recorder/recorder.py
+CrazyDG/recorder/visualizer.py
```

### Comparing `CrazyDG-0.0.3/setup.py` & `CrazyDG-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
     name='CrazyDG',
-    version='0.0.3',
+    version='0.0.4',
     description='CrazyDG is for convenience',
     author='Daegeun02',
     author_email='redhawkdg02@gmail.com',
     url='https://github.com/Daegeun02/CrazyDG.git',
     install_requires=[],
     packages=find_packages( exclude=[] ),
     keywords=['CrazyDG', 'by daegeun', 'for convenience'],
```

