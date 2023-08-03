# Comparing `tmp/fusion-engine-1.0.1.tar.gz` & `tmp/fusion-engine-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-1.0.1.tar", last modified: Thu Aug  3 19:11:56 2023, max compression
+gzip compressed data, was "fusion-engine-1.0.2.tar", last modified: Thu Aug  3 19:18:30 2023, max compression
```

## Comparing `fusion-engine-1.0.1.tar` & `fusion-engine-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:11:56.769359 fusion-engine-1.0.1/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-1.0.1/LICENCE.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     6323 2023-08-03 19:11:56.768477 fusion-engine-1.0.1/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5064 2023-08-03 19:10:42.000000 fusion-engine-1.0.1/README.md
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1638 2023-08-03 19:06:27.000000 fusion-engine-1.0.1/pyproject.toml
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2326 2023-07-27 11:42:53.000000 fusion-engine-1.0.1/release.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       27 2023-07-30 20:07:05.000000 fusion-engine-1.0.1/requirements.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-08-03 19:11:56.769684 fusion-engine-1.0.1/setup.cfg
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2490 2023-07-27 11:51:55.000000 fusion-engine-1.0.1/setup.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:11:56.734288 fusion-engine-1.0.1/src/
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:11:56.747340 fusion-engine-1.0.1/src/fusion_engine.egg-info/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     6323 2023-08-03 19:11:56.000000 fusion-engine-1.0.1/src/fusion_engine.egg-info/PKG-INFO
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      925 2023-08-03 19:11:56.000000 fusion-engine-1.0.1/src/fusion_engine.egg-info/SOURCES.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-08-03 19:11:56.000000 fusion-engine-1.0.1/src/fusion_engine.egg-info/dependency_links.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       28 2023-08-03 19:11:56.000000 fusion-engine-1.0.1/src/fusion_engine.egg-info/requires.txt
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-08-03 19:11:56.000000 fusion-engine-1.0.1/src/fusion_engine.egg-info/top_level.txt
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:11:56.748007 fusion-engine-1.0.1/src/fusionengine/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      760 2023-08-03 19:07:19.000000 fusion-engine-1.0.1/src/fusionengine/__init__.py
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:11:56.748626 fusion-engine-1.0.1/src/fusionengine/debugfiles/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-1.0.1/src/fusionengine/debugfiles/fe.png
-drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:11:56.766964 fusion-engine-1.0.1/src/fusionengine/files/
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3593 2023-07-28 15:12:56.000000 fusion-engine-1.0.1/src/fusionengine/files/body.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1694 2023-07-28 15:13:05.000000 fusion-engine-1.0.1/src/fusionengine/files/color.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      451 2023-07-28 15:13:01.000000 fusion-engine-1.0.1/src/fusionengine/files/data.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      162 2023-07-28 15:12:38.000000 fusion-engine-1.0.1/src/fusionengine/files/debug.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1764 2023-07-29 16:08:23.000000 fusion-engine-1.0.1/src/fusionengine/files/draw.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      374 2023-07-28 15:13:11.000000 fusion-engine-1.0.1/src/fusionengine/files/enums.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5093 2023-08-03 08:53:02.000000 fusion-engine-1.0.1/src/fusionengine/files/event.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      252 2023-07-28 14:45:31.000000 fusion-engine-1.0.1/src/fusionengine/files/exceptions.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      172 2023-07-28 16:40:29.000000 fusion-engine-1.0.1/src/fusionengine/files/fonts.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1035 2023-07-29 16:32:15.000000 fusion-engine-1.0.1/src/fusionengine/files/image.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      592 2023-07-30 20:07:05.000000 fusion-engine-1.0.1/src/fusionengine/files/imports.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-1.0.1/src/fusionengine/files/physics.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      882 2023-08-03 18:48:17.000000 fusion-engine-1.0.1/src/fusionengine/files/shape.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5586 2023-07-28 14:51:13.000000 fusion-engine-1.0.1/src/fusionengine/files/storage.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      144 2023-07-29 10:00:10.000000 fusion-engine-1.0.1/src/fusionengine/files/systems.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1722 2023-08-03 18:38:41.000000 fusion-engine-1.0.1/src/fusionengine/files/ui.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      600 2023-07-28 14:51:26.000000 fusion-engine-1.0.1/src/fusionengine/files/vector.py
--rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2843 2023-08-03 08:52:11.000000 fusion-engine-1.0.1/src/fusionengine/files/window.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:18:30.090565 fusion-engine-1.0.2/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1071 2023-07-02 09:01:28.000000 fusion-engine-1.0.2/LICENCE.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     6332 2023-08-03 19:18:30.089720 fusion-engine-1.0.2/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5073 2023-08-03 19:18:08.000000 fusion-engine-1.0.2/README.md
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1638 2023-08-03 19:06:27.000000 fusion-engine-1.0.2/pyproject.toml
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2326 2023-07-27 11:42:53.000000 fusion-engine-1.0.2/release.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       27 2023-07-30 20:07:05.000000 fusion-engine-1.0.2/requirements.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       38 2023-08-03 19:18:30.090818 fusion-engine-1.0.2/setup.cfg
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2490 2023-07-27 11:51:55.000000 fusion-engine-1.0.2/setup.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:18:30.047892 fusion-engine-1.0.2/src/
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:18:30.059489 fusion-engine-1.0.2/src/fusion_engine.egg-info/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     6332 2023-08-03 19:18:29.000000 fusion-engine-1.0.2/src/fusion_engine.egg-info/PKG-INFO
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      925 2023-08-03 19:18:29.000000 fusion-engine-1.0.2/src/fusion_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        1 2023-08-03 19:18:29.000000 fusion-engine-1.0.2/src/fusion_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       28 2023-08-03 19:18:29.000000 fusion-engine-1.0.2/src/fusion_engine.egg-info/requires.txt
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)       13 2023-08-03 19:18:29.000000 fusion-engine-1.0.2/src/fusion_engine.egg-info/top_level.txt
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:18:30.060443 fusion-engine-1.0.2/src/fusionengine/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      760 2023-08-03 19:18:19.000000 fusion-engine-1.0.2/src/fusionengine/__init__.py
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:18:30.061393 fusion-engine-1.0.2/src/fusionengine/debugfiles/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)    64239 2023-07-07 11:13:39.000000 fusion-engine-1.0.2/src/fusionengine/debugfiles/fe.png
+drwxr-xr-x   0 dmarhitych-pro   (501) staff       (20)        0 2023-08-03 19:18:30.081828 fusion-engine-1.0.2/src/fusionengine/files/
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     3593 2023-07-28 15:12:56.000000 fusion-engine-1.0.2/src/fusionengine/files/body.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1694 2023-07-28 15:13:05.000000 fusion-engine-1.0.2/src/fusionengine/files/color.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      451 2023-07-28 15:13:01.000000 fusion-engine-1.0.2/src/fusionengine/files/data.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      162 2023-07-28 15:12:38.000000 fusion-engine-1.0.2/src/fusionengine/files/debug.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1764 2023-07-29 16:08:23.000000 fusion-engine-1.0.2/src/fusionengine/files/draw.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      374 2023-07-28 15:13:11.000000 fusion-engine-1.0.2/src/fusionengine/files/enums.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5093 2023-08-03 08:53:02.000000 fusion-engine-1.0.2/src/fusionengine/files/event.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      252 2023-07-28 14:45:31.000000 fusion-engine-1.0.2/src/fusionengine/files/exceptions.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      172 2023-07-28 16:40:29.000000 fusion-engine-1.0.2/src/fusionengine/files/fonts.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1035 2023-07-29 16:32:15.000000 fusion-engine-1.0.2/src/fusionengine/files/image.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      592 2023-07-30 20:07:05.000000 fusion-engine-1.0.2/src/fusionengine/files/imports.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)        0 2023-06-11 19:02:09.000000 fusion-engine-1.0.2/src/fusionengine/files/physics.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      882 2023-08-03 18:48:17.000000 fusion-engine-1.0.2/src/fusionengine/files/shape.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     5586 2023-07-28 14:51:13.000000 fusion-engine-1.0.2/src/fusionengine/files/storage.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      144 2023-07-29 10:00:10.000000 fusion-engine-1.0.2/src/fusionengine/files/systems.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     1722 2023-08-03 18:38:41.000000 fusion-engine-1.0.2/src/fusionengine/files/ui.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)      600 2023-07-28 14:51:26.000000 fusion-engine-1.0.2/src/fusionengine/files/vector.py
+-rw-r--r--   0 dmarhitych-pro   (501) staff       (20)     2843 2023-08-03 08:52:11.000000 fusion-engine-1.0.2/src/fusionengine/files/window.py
```

### Comparing `fusion-engine-1.0.1/LICENCE.md` & `fusion-engine-1.0.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/PKG-INFO` & `fusion-engine-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 1.0.1
+Version: 1.0.2
 Summary: A custom open-source game engine on Python and PySDL2, it's written in pure Python! It's easy and fast!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: MIT
 Keywords: game,python,gamedev,game-engine,pygame,game-development,pure-python,pygame-mixer,pygame-ttf,pygame-image,python-game,pygame-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -26,17 +26,15 @@
 License-File: LICENCE.md
 
 <h1 align="center">🚀 Fusion Engine</h1>
 
 <p align="center">
 <a href="https://pypi.org/project/fusion-engine"><img alt="PyPI" src="https://img.shields.io/pypi/v/fusion-engine"></a>
 <a href="https://pypi.org/project/fusion-engine"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/fusion-engine"></a>
-<a href="https://pypi.org/project/fusion-engine"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/fusion-engine"></a>
-
-
+<a href="https://pypi.org/project/fusion-engine"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/fusion-engine?color=blue"></a>
 </p>
 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png" alt="logo">
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fusion-engine Version: 1.0.1 Summary: A custom
+Metadata-Version: 2.1 Name: fusion-engine Version: 1.0.2 Summary: A custom
 open-source game engine on Python and PySDL2, it's written in pure Python! It's
 easy and fast! Author-email: Dimkauzh
 gmail.com> License: MIT Keywords: game,python,gamedev,game-engine,pygame,game-
 development,pure-python,pygame-mixer,pygame-ttf,pygame-image,python-
 game,pygame-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
```

### Comparing `fusion-engine-1.0.1/README.md` & `fusion-engine-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 <h1 align="center">🚀 Fusion Engine</h1>
 
 <p align="center">
 <a href="https://pypi.org/project/fusion-engine"><img alt="PyPI" src="https://img.shields.io/pypi/v/fusion-engine"></a>
 <a href="https://pypi.org/project/fusion-engine"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/fusion-engine"></a>
-<a href="https://pypi.org/project/fusion-engine"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/fusion-engine"></a>
-
-
+<a href="https://pypi.org/project/fusion-engine"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/fusion-engine?color=blue"></a>
 </p>
 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png" alt="logo">
 </p>
```

### Comparing `fusion-engine-1.0.1/pyproject.toml` & `fusion-engine-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/release.py` & `fusion-engine-1.0.2/release.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/setup.py` & `fusion-engine-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusion_engine.egg-info/PKG-INFO` & `fusion-engine-1.0.2/src/fusion_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine
-Version: 1.0.1
+Version: 1.0.2
 Summary: A custom open-source game engine on Python and PySDL2, it's written in pure Python! It's easy and fast!
 Author-email: Dimkauzh <uzhdimka@gmail.com>
 License: MIT
 Keywords: game,python,gamedev,game-engine,pygame,game-development,pure-python,pygame-mixer,pygame-ttf,pygame-image,python-game,pygame-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -26,17 +26,15 @@
 License-File: LICENCE.md
 
 <h1 align="center">🚀 Fusion Engine</h1>
 
 <p align="center">
 <a href="https://pypi.org/project/fusion-engine"><img alt="PyPI" src="https://img.shields.io/pypi/v/fusion-engine"></a>
 <a href="https://pypi.org/project/fusion-engine"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/fusion-engine"></a>
-<a href="https://pypi.org/project/fusion-engine"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/fusion-engine"></a>
-
-
+<a href="https://pypi.org/project/fusion-engine"><img alt="PyPI - License" src="https://img.shields.io/pypi/l/fusion-engine?color=blue"></a>
 </p>
 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/106883655/233103547-5693b2a3-22b9-4b68-ac2a-7220f16d48df.png" alt="logo">
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fusion-engine Version: 1.0.1 Summary: A custom
+Metadata-Version: 2.1 Name: fusion-engine Version: 1.0.2 Summary: A custom
 open-source game engine on Python and PySDL2, it's written in pure Python! It's
 easy and fast! Author-email: Dimkauzh
 gmail.com> License: MIT Keywords: game,python,gamedev,game-engine,pygame,game-
 development,pure-python,pygame-mixer,pygame-ttf,pygame-image,python-
 game,pygame-library,python-game-library,python-game-engine,python-games
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
```

### Comparing `fusion-engine-1.0.1/src/fusion_engine.egg-info/SOURCES.txt` & `fusion-engine-1.0.2/src/fusion_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/__init__.py` & `fusion-engine-1.0.2/src/fusionengine/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Dimkauzh"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 from fusionengine.files.imports import *
 import fusionengine.files.systems as sysconfig
 
 
 class Main:
     def __init__(self):
```

### Comparing `fusion-engine-1.0.1/src/fusionengine/debugfiles/fe.png` & `fusion-engine-1.0.2/src/fusionengine/debugfiles/fe.png`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/body.py` & `fusion-engine-1.0.2/src/fusionengine/files/body.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/color.py` & `fusion-engine-1.0.2/src/fusionengine/files/color.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/draw.py` & `fusion-engine-1.0.2/src/fusionengine/files/draw.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/event.py` & `fusion-engine-1.0.2/src/fusionengine/files/event.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/image.py` & `fusion-engine-1.0.2/src/fusionengine/files/image.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/imports.py` & `fusion-engine-1.0.2/src/fusionengine/files/imports.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/shape.py` & `fusion-engine-1.0.2/src/fusionengine/files/shape.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/storage.py` & `fusion-engine-1.0.2/src/fusionengine/files/storage.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/ui.py` & `fusion-engine-1.0.2/src/fusionengine/files/ui.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/vector.py` & `fusion-engine-1.0.2/src/fusionengine/files/vector.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-1.0.1/src/fusionengine/files/window.py` & `fusion-engine-1.0.2/src/fusionengine/files/window.py`

 * *Files identical despite different names*

