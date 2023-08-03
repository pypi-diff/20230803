# Comparing `tmp/MyOverlay-0.2.1.tar.gz` & `tmp/MyOverlay-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyOverlay-0.2.1.tar", last modified: Wed Aug  2 14:17:31 2023, max compression
+gzip compressed data, was "MyOverlay-0.2.2.tar", last modified: Thu Aug  3 10:45:04 2023, max compression
```

## Comparing `MyOverlay-0.2.1.tar` & `MyOverlay-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 14:17:31.941042 MyOverlay-0.2.1/
--rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      745 2023-08-02 14:17:31.941042 MyOverlay-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.2.1/README.md
--rw-rw-rw-   0        0        0      649 2023-08-02 14:17:03.000000 MyOverlay-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-02 14:17:31.941042 MyOverlay-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-02 14:17:31.914093 MyOverlay-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-02 14:17:31.925042 MyOverlay-0.2.1/src/MyOverlay/
--rw-rw-rw-   0        0        0      409 2023-08-02 14:16:50.000000 MyOverlay-0.2.1/src/MyOverlay/Overlay.py
--rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.2.1/src/MyOverlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:17:31.940042 MyOverlay-0.2.1/src/MyOverlay/funcs/
--rw-rw-rw-   0        0        0     4972 2023-08-02 14:15:51.000000 MyOverlay-0.2.1/src/MyOverlay/funcs/myfunctions.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:17:31.939043 MyOverlay-0.2.1/src/MyOverlay.egg-info/
--rw-rw-rw-   0        0        0      745 2023-08-02 14:17:31.000000 MyOverlay-0.2.1/src/MyOverlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-08-02 14:17:31.000000 MyOverlay-0.2.1/src/MyOverlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 14:17:31.000000 MyOverlay-0.2.1/src/MyOverlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-02 14:17:31.000000 MyOverlay-0.2.1/src/MyOverlay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 10:45:04.321579 MyOverlay-0.2.2/
+-rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-08-03 10:45:04.321579 MyOverlay-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.2.2/README.md
+-rw-rw-rw-   0        0        0      649 2023-08-03 10:44:31.000000 MyOverlay-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 10:45:04.322584 MyOverlay-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 10:45:04.280603 MyOverlay-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 10:45:04.300655 MyOverlay-0.2.2/src/MyOverlay/
+-rw-rw-rw-   0        0        0      409 2023-08-02 14:16:50.000000 MyOverlay-0.2.2/src/MyOverlay/Overlay.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.2.2/src/MyOverlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 10:45:04.320587 MyOverlay-0.2.2/src/MyOverlay/funcs/
+-rw-rw-rw-   0        0        0     5484 2023-08-03 10:13:51.000000 MyOverlay-0.2.2/src/MyOverlay/funcs/myfunctions.py
+drwxrwxrwx   0        0        0        0 2023-08-03 10:45:04.313608 MyOverlay-0.2.2/src/MyOverlay.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-08-03 10:45:04.000000 MyOverlay-0.2.2/src/MyOverlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-08-03 10:45:04.000000 MyOverlay-0.2.2/src/MyOverlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 10:45:04.000000 MyOverlay-0.2.2/src/MyOverlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-03 10:45:04.000000 MyOverlay-0.2.2/src/MyOverlay.egg-info/top_level.txt
```

### Comparing `MyOverlay-0.2.1/LICENSE` & `MyOverlay-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MyOverlay-0.2.1/PKG-INFO` & `MyOverlay-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.2.1
+Version: 0.2.2
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MyOverlay-0.2.1/pyproject.toml` & `MyOverlay-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "MyOverlay"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Erik Reimann", email="erikreimann28@gmail.com" },
 ]
 description = "Customized Text Only Screen Overlay"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `MyOverlay-0.2.1/src/MyOverlay/funcs/myfunctions.py` & `MyOverlay-0.2.2/src/MyOverlay/funcs/myfunctions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from win32api import GetSystemMetrics
 import pygame
 import win32api
 import win32con
 import win32gui
 import ctypes
 import time
+from thefuzz import fuzz
 
 OverlayRunning = False
 white = (255, 255, 255)
 black = (0, 0, 0)
 fuchsia = (255, 0, 128)
 GWL_EXSTYLE = -20
 WS_EX_APPWINDOW = 0x00040000
@@ -121,15 +122,24 @@
     OverlayRunning = False
     
 def StatusOverlay():
     return OverlayRunning
 
 
 def GetJobDirectory(JobName: str):
-    match JobName:
+    database = ['Airline Pilot', 'Bus Driver', 'Business', 'Cargo Pilot', 'EMS', 'Farmer', 'Firefighter', 'Fisherman',
+                'Gambling', 'Garbage', 'Helicopter Pilot',
+                'Hunter', 'Mechanic', 'Miner', 'Player', 'Racer', 'Strength', 'Train Conductor', 'Trucking',   'PostOP']
+    score = 0
+    for f in database:
+        tempscore = fuzz.partial_ratio(f, JobName)
+        if tempscore > score:
+            score = tempscore
+            AJobName = f
+    match AJobName:
         case 'Airline Pilot':
             return 'piloting piloting'
         case 'Bus Driver':
             return 'train bus'
         case 'Business':
             return 'business business'
         case 'Cargo Pilot':
@@ -162,8 +172,9 @@
             return 'physical strength'
         case 'Train Conductor':
             return 'train train'
         case 'Trucking':
             return 'trucking trucking'
         case 'PostOP':
             return 'trucking postop'
-    return None
+    return None
+
```

### Comparing `MyOverlay-0.2.1/src/MyOverlay.egg-info/PKG-INFO` & `MyOverlay-0.2.2/src/MyOverlay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.2.1
+Version: 0.2.2
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

