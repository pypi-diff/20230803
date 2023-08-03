# Comparing `tmp/yolov8face-0.0.3.tar.gz` & `tmp/yolov8face-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolov8face-0.0.3.tar", last modified: Thu Aug  3 09:52:17 2023, max compression
+gzip compressed data, was "yolov8face-0.1.1.tar", last modified: Thu Aug  3 10:20:04 2023, max compression
```

## Comparing `yolov8face-0.0.3.tar` & `yolov8face-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-08-03 09:52:17.018980 yolov8face-0.0.3/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)    35149 2023-07-22 13:32:13.000000 yolov8face-0.0.3/LICENSE
--rw-rw-r--   0 harsh     (1000) harsh     (1000)     1585 2023-08-03 09:52:17.018980 yolov8face-0.0.3/PKG-INFO
--rw-rw-r--   0 harsh     (1000) harsh     (1000)     1424 2023-07-25 19:45:20.000000 yolov8face-0.0.3/README.md
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       38 2023-08-03 09:52:17.018980 yolov8face-0.0.3/setup.cfg
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      543 2023-08-03 09:52:02.000000 yolov8face-0.0.3/setup.py
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-08-03 09:52:17.018980 yolov8face-0.0.3/yolov8face.egg-info/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)     1585 2023-08-03 09:52:17.000000 yolov8face-0.0.3/yolov8face.egg-info/PKG-INFO
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      195 2023-08-03 09:52:17.000000 yolov8face-0.0.3/yolov8face.egg-info/SOURCES.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-08-03 09:52:17.000000 yolov8face-0.0.3/yolov8face.egg-info/dependency_links.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       12 2023-08-03 09:52:17.000000 yolov8face-0.0.3/yolov8face.egg-info/requires.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-08-03 09:52:17.000000 yolov8face-0.0.3/yolov8face.egg-info/top_level.txt
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-08-03 10:20:04.034444 yolov8face-0.1.1/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)    35149 2023-07-22 13:32:13.000000 yolov8face-0.1.1/LICENSE
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       61 2023-08-03 10:08:53.000000 yolov8face-0.1.1/MANIFEST.in
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     1816 2023-08-03 10:20:04.034444 yolov8face-0.1.1/PKG-INFO
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     1424 2023-07-25 19:45:20.000000 yolov8face-0.1.1/README.md
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)   357459 2023-07-23 19:16:35.000000 yolov8face-0.1.1/detected_faces.png
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       38 2023-08-03 10:20:04.034444 yolov8face-0.1.1/setup.cfg
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      657 2023-08-03 10:19:12.000000 yolov8face-0.1.1/setup.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-08-03 10:20:04.034444 yolov8face-0.1.1/yolov8face/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       32 2023-07-21 10:47:47.000000 yolov8face-0.1.1/yolov8face/__init__.py
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     1569 2023-07-21 10:58:09.000000 yolov8face-0.1.1/yolov8face/yolo_model.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-08-03 10:20:04.034444 yolov8face-0.1.1/yolov8face.egg-info/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     1816 2023-08-03 10:20:04.000000 yolov8face-0.1.1/yolov8face.egg-info/PKG-INFO
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      274 2023-08-03 10:20:04.000000 yolov8face-0.1.1/yolov8face.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-08-03 10:20:04.000000 yolov8face-0.1.1/yolov8face.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       12 2023-08-03 10:20:04.000000 yolov8face-0.1.1/yolov8face.egg-info/requires.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       11 2023-08-03 10:20:04.000000 yolov8face-0.1.1/yolov8face.egg-info/top_level.txt
```

### Comparing `yolov8face-0.0.3/LICENSE` & `yolov8face-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yolov8face-0.0.3/PKG-INFO` & `yolov8face-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: yolov8face
-Version: 0.0.3
-Summary: A wrapper to YOLOv8 face detector.
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # yolov8face
 Yolov8face is a Python wrapper of Ultrlytics that simplifies the process of detecting faces in images using the yolov8n-face model. It takes care of pre-trained model downloading, loading and postprocessing, allowing you to detect faces in images with just a few lines of code. 
 
 ## Installation
 ```bash
 pip install yolov8face
 ```
```

### Comparing `yolov8face-0.0.3/README.md` & `yolov8face-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: yolov8face
+Version: 0.1.1
+Summary: Yolov8face is a Python wrapper of Ultrlytics that simplifies the process of detecting faces in images using the yolov8n-face model. It takes care of model downloading, loading and postprocessing, allowing you to detect faces in images with just a few lines of code.
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # yolov8face
 Yolov8face is a Python wrapper of Ultrlytics that simplifies the process of detecting faces in images using the yolov8n-face model. It takes care of pre-trained model downloading, loading and postprocessing, allowing you to detect faces in images with just a few lines of code. 
 
 ## Installation
 ```bash
 pip install yolov8face
 ```
```

### Comparing `yolov8face-0.0.3/yolov8face.egg-info/PKG-INFO` & `yolov8face-0.1.1/yolov8face.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: yolov8face
-Version: 0.0.3
-Summary: A wrapper to YOLOv8 face detector.
+Version: 0.1.1
+Summary: Yolov8face is a Python wrapper of Ultrlytics that simplifies the process of detecting faces in images using the yolov8n-face model. It takes care of model downloading, loading and postprocessing, allowing you to detect faces in images with just a few lines of code.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yolov8face
 Yolov8face is a Python wrapper of Ultrlytics that simplifies the process of detecting faces in images using the yolov8n-face model. It takes care of pre-trained model downloading, loading and postprocessing, allowing you to detect faces in images with just a few lines of code. 
 
 ## Installation
```

