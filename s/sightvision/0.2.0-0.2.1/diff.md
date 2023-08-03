# Comparing `tmp/sightvision-0.2.0.tar.gz` & `tmp/sightvision-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sightvision-0.2.0.tar", last modified: Sat Jul 22 21:37:14 2023, max compression
+gzip compressed data, was "sightvision-0.2.1.tar", last modified: Thu Aug  3 16:48:40 2023, max compression
```

## Comparing `sightvision-0.2.0.tar` & `sightvision-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 21:37:14.630082 sightvision-0.2.0/
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1065 2023-07-21 19:53:53.000000 sightvision-0.2.0/LICENSE.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)      914 2023-07-22 21:37:14.633415 sightvision-0.2.0/PKG-INFO
--rw-r--r--   0 dragon    (1000) dragon    (1000)      987 2023-07-22 15:23:42.000000 sightvision-0.2.0/README.md
--rw-r--r--   0 dragon    (1000) dragon    (1000)       79 2023-07-22 21:37:14.633415 sightvision-0.2.0/setup.cfg
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1981 2023-07-22 21:37:09.000000 sightvision-0.2.0/setup.py
-drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 21:37:14.630082 sightvision-0.2.0/sightvision/
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2265 2023-07-22 21:28:26.000000 sightvision-0.2.0/sightvision/ClassificationModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     3756 2023-07-22 02:24:49.000000 sightvision-0.2.0/sightvision/ColorModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1559 2023-07-22 15:47:17.000000 sightvision-0.2.0/sightvision/FPS.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2361 2023-07-22 02:20:18.000000 sightvision-0.2.0/sightvision/FaceDetectionModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     3607 2023-07-21 23:32:34.000000 sightvision-0.2.0/sightvision/FaceMeshModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     7350 2023-07-22 02:19:49.000000 sightvision-0.2.0/sightvision/HandTrackingModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2235 2023-07-22 16:03:23.000000 sightvision-0.2.0/sightvision/PIDModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     3423 2023-07-22 02:22:52.000000 sightvision-0.2.0/sightvision/PlotModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     5536 2023-07-22 02:22:27.000000 sightvision-0.2.0/sightvision/PoseModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     1670 2023-07-22 02:21:53.000000 sightvision-0.2.0/sightvision/SelfiSegmentationModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     2213 2023-07-22 02:21:28.000000 sightvision-0.2.0/sightvision/SerialModule.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)     6541 2023-07-22 02:20:48.000000 sightvision-0.2.0/sightvision/Utils.py
--rw-r--r--   0 dragon    (1000) dragon    (1000)      663 2023-07-22 21:31:02.000000 sightvision-0.2.0/sightvision/__init__.py
-drwxr-xr-x   0 dragon    (1000) dragon    (1000)        0 2023-07-22 21:37:14.630082 sightvision-0.2.0/sightvision.egg-info/
--rw-r--r--   0 dragon    (1000) dragon    (1000)      914 2023-07-22 21:37:14.000000 sightvision-0.2.0/sightvision.egg-info/PKG-INFO
--rw-r--r--   0 dragon    (1000) dragon    (1000)      584 2023-07-22 21:37:14.000000 sightvision-0.2.0/sightvision.egg-info/SOURCES.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)        1 2023-07-22 21:37:14.000000 sightvision-0.2.0/sightvision.egg-info/dependency_links.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)       57 2023-07-22 21:37:14.000000 sightvision-0.2.0/sightvision.egg-info/requires.txt
--rw-r--r--   0 dragon    (1000) dragon    (1000)       12 2023-07-22 21:37:14.000000 sightvision-0.2.0/sightvision.egg-info/top_level.txt
+drwxrwxr-x   0 rexionmars  (1000) rexionmars  (1000)        0 2023-08-03 16:48:40.770466 sightvision-0.2.1/
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     1065 2023-07-21 15:53:52.000000 sightvision-0.2.1/LICENSE.txt
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     5769 2023-08-03 16:48:40.770466 sightvision-0.2.1/PKG-INFO
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     4814 2023-07-25 01:46:28.000000 sightvision-0.2.1/README.md
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)       79 2023-08-03 16:48:40.770466 sightvision-0.2.1/setup.cfg
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     2123 2023-08-03 16:48:35.000000 sightvision-0.2.1/setup.py
+drwxrwxr-x   0 rexionmars  (1000) rexionmars  (1000)        0 2023-08-03 16:48:40.766466 sightvision-0.2.1/sightvision/
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     2265 2023-07-22 17:28:26.000000 sightvision-0.2.1/sightvision/ClassificationModule.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     3756 2023-07-21 22:24:48.000000 sightvision-0.2.1/sightvision/ColorModule.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     1559 2023-07-22 11:47:16.000000 sightvision-0.2.1/sightvision/FPS.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     3360 2023-07-31 22:14:02.000000 sightvision-0.2.1/sightvision/FaceDetectionModule.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     3607 2023-07-21 19:32:34.000000 sightvision-0.2.1/sightvision/FaceMeshModule.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     7350 2023-07-21 22:19:48.000000 sightvision-0.2.1/sightvision/HandTrackingModule.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     2235 2023-07-22 12:03:22.000000 sightvision-0.2.1/sightvision/PIDModule.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     3423 2023-07-21 22:22:52.000000 sightvision-0.2.1/sightvision/PlotModule.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     5536 2023-07-21 22:22:26.000000 sightvision-0.2.1/sightvision/PoseModule.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     1670 2023-07-21 22:21:52.000000 sightvision-0.2.1/sightvision/SelfiSegmentationModule.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     2213 2023-07-21 22:21:28.000000 sightvision-0.2.1/sightvision/SerialModule.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     6541 2023-07-21 22:20:48.000000 sightvision-0.2.1/sightvision/Utils.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)      663 2023-07-22 17:31:02.000000 sightvision-0.2.1/sightvision/__init__.py
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)       34 2023-07-28 23:19:22.000000 sightvision-0.2.1/sightvision/config.py
+drwxrwxr-x   0 rexionmars  (1000) rexionmars  (1000)        0 2023-08-03 16:48:40.766466 sightvision-0.2.1/sightvision.egg-info/
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)     5769 2023-08-03 16:48:40.000000 sightvision-0.2.1/sightvision.egg-info/PKG-INFO
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)      606 2023-08-03 16:48:40.000000 sightvision-0.2.1/sightvision.egg-info/SOURCES.txt
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)        1 2023-08-03 16:48:40.000000 sightvision-0.2.1/sightvision.egg-info/dependency_links.txt
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)       57 2023-08-03 16:48:40.000000 sightvision-0.2.1/sightvision.egg-info/requires.txt
+-rw-rw-r--   0 rexionmars  (1000) rexionmars  (1000)       12 2023-08-03 16:48:40.000000 sightvision-0.2.1/sightvision.egg-info/top_level.txt
```

### Comparing `sightvision-0.2.0/LICENSE.txt` & `sightvision-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/setup.py` & `sightvision-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from distutils.core import setup
+
+
+with open("README.md", "r") as rd:
+  long_desc = rd.read()
+
+
 setup(
   name = 'sightvision',         # How you named your package folder (MyLib)
   packages = ['sightvision'],   # Chose the same as "name"
-  version = '0.2.0',      # Start with a small number and increase it with every change you make
+  version = '0.2.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a Computer vision package that makes its easy to run Image processing and AI functions.',   # Give a short description about your library
+  long_description=long_desc,
+  long_description_content_type='text/markdown',
   author = 'Leonardi Melo',                   # Type in your name
   author_email = 'opensource.leonardi@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/rexionmars/SightVision',   # Provide either the link to your github or to your website
   #download_url = 'https://github.com/rexionmars/SightVision/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Computervision', 'Imageutils', 'Imageprocessing'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'opencv-python',
```

### Comparing `sightvision-0.2.0/sightvision/ClassificationModule.py` & `sightvision-0.2.1/sightvision/ClassificationModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/ColorModule.py` & `sightvision-0.2.1/sightvision/ColorModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/FPS.py` & `sightvision-0.2.1/sightvision/FPS.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/FaceMeshModule.py` & `sightvision-0.2.1/sightvision/FaceMeshModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/HandTrackingModule.py` & `sightvision-0.2.1/sightvision/HandTrackingModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/PIDModule.py` & `sightvision-0.2.1/sightvision/PIDModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/PlotModule.py` & `sightvision-0.2.1/sightvision/PlotModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/PoseModule.py` & `sightvision-0.2.1/sightvision/PoseModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/SelfiSegmentationModule.py` & `sightvision-0.2.1/sightvision/SelfiSegmentationModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/SerialModule.py` & `sightvision-0.2.1/sightvision/SerialModule.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/Utils.py` & `sightvision-0.2.1/sightvision/Utils.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision/__init__.py` & `sightvision-0.2.1/sightvision/__init__.py`

 * *Files identical despite different names*

### Comparing `sightvision-0.2.0/sightvision.egg-info/SOURCES.txt` & `sightvision-0.2.1/sightvision.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 sightvision/PIDModule.py
 sightvision/PlotModule.py
 sightvision/PoseModule.py
 sightvision/SelfiSegmentationModule.py
 sightvision/SerialModule.py
 sightvision/Utils.py
 sightvision/__init__.py
+sightvision/config.py
 sightvision.egg-info/PKG-INFO
 sightvision.egg-info/SOURCES.txt
 sightvision.egg-info/dependency_links.txt
 sightvision.egg-info/requires.txt
 sightvision.egg-info/top_level.txt
```

