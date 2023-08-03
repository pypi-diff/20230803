# Comparing `tmp/text2hologram-0.0.4.tar.gz` & `tmp/text2hologram-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2hologram-0.0.4.tar", last modified: Fri Jul 28 21:13:19 2023, max compression
+gzip compressed data, was "text2hologram-0.1.0.tar", last modified: Thu Aug  3 01:44:22 2023, max compression
```

## Comparing `text2hologram-0.0.4.tar` & `text2hologram-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 21:13:19.222856 text2hologram-0.0.4/
--rw-rw-rw-   0        0        0       20 2023-07-26 18:34:11.000000 text2hologram-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      698 2023-07-28 21:13:19.221855 text2hologram-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-22 16:43:03.000000 text2hologram-0.0.4/README.md
--rw-rw-rw-   0        0        0      826 2023-07-28 21:12:55.000000 text2hologram-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 21:13:19.222856 text2hologram-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-28 21:13:19.195856 text2hologram-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-28 21:13:19.211856 text2hologram-0.0.4/src/text2hologram/
--rw-rw-rw-   0        0        0     2473 2023-07-28 21:11:19.000000 text2hologram-0.0.4/src/text2hologram/__main__.py
--rw-rw-rw-   0        0        0      964 2023-07-28 18:01:04.000000 text2hologram-0.0.4/src/text2hologram/config.json
--rw-rw-rw-   0        0        0      487 2023-07-28 17:36:58.000000 text2hologram-0.0.4/src/text2hologram/device_setup.py
--rw-rw-rw-   0        0        0      920 2023-07-28 21:11:30.000000 text2hologram-0.0.4/src/text2hologram/image_generation.py
--rw-rw-rw-   0        0        0     2191 2023-07-28 17:51:12.000000 text2hologram-0.0.4/src/text2hologram/model.py
--rw-rw-rw-   0        0        0     7070 2023-07-26 18:37:12.000000 text2hologram-0.0.4/src/text2hologram/post_processing.py
--rw-rw-rw-   0        0        0      454 2023-07-28 17:26:17.000000 text2hologram-0.0.4/src/text2hologram/read_all.py
--rw-rw-rw-   0        0        0      711 2023-07-28 17:42:08.000000 text2hologram-0.0.4/src/text2hologram/settings.py
--rw-rw-rw-   0        0        0      340 2023-07-26 18:37:12.000000 text2hologram-0.0.4/src/text2hologram/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 21:13:19.219858 text2hologram-0.0.4/src/text2hologram.egg-info/
--rw-rw-rw-   0        0        0      698 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-28 21:13:19.000000 text2hologram-0.0.4/src/text2hologram.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 01:44:22.043526 text2hologram-0.1.0/
+-rw-rw-rw-   0        0        0       20 2023-07-26 18:34:11.000000 text2hologram-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2119 2023-08-03 01:44:22.042526 text2hologram-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1673 2023-08-03 01:40:03.000000 text2hologram-0.1.0/README.md
+-rw-rw-rw-   0        0        0      824 2023-08-03 01:44:14.000000 text2hologram-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 01:44:22.043526 text2hologram-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 01:44:22.015504 text2hologram-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 01:44:22.033018 text2hologram-0.1.0/src/text2hologram/
+-rw-rw-rw-   0        0        0     2473 2023-07-28 21:17:16.000000 text2hologram-0.1.0/src/text2hologram/__main__.py
+-rw-rw-rw-   0        0        0      964 2023-07-28 18:01:04.000000 text2hologram-0.1.0/src/text2hologram/config.json
+-rw-rw-rw-   0        0        0      487 2023-07-28 17:36:58.000000 text2hologram-0.1.0/src/text2hologram/device_setup.py
+-rw-rw-rw-   0        0        0      920 2023-07-28 21:11:30.000000 text2hologram-0.1.0/src/text2hologram/image_generation.py
+-rw-rw-rw-   0        0        0     2191 2023-07-28 17:51:12.000000 text2hologram-0.1.0/src/text2hologram/model.py
+-rw-rw-rw-   0        0        0     7070 2023-07-26 18:37:12.000000 text2hologram-0.1.0/src/text2hologram/post_processing.py
+-rw-rw-rw-   0        0        0      454 2023-07-28 17:26:17.000000 text2hologram-0.1.0/src/text2hologram/read_all.py
+-rw-rw-rw-   0        0        0      711 2023-07-28 17:42:08.000000 text2hologram-0.1.0/src/text2hologram/settings.py
+-rw-rw-rw-   0        0        0      340 2023-07-26 18:37:12.000000 text2hologram-0.1.0/src/text2hologram/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-03 01:44:22.041528 text2hologram-0.1.0/src/text2hologram.egg-info/
+-rw-rw-rw-   0        0        0     2119 2023-08-03 01:44:21.000000 text2hologram-0.1.0/src/text2hologram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-08-03 01:44:22.000000 text2hologram-0.1.0/src/text2hologram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 01:44:21.000000 text2hologram-0.1.0/src/text2hologram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-08-03 01:44:21.000000 text2hologram-0.1.0/src/text2hologram.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-08-03 01:44:21.000000 text2hologram-0.1.0/src/text2hologram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-03 01:44:21.000000 text2hologram-0.1.0/src/text2hologram.egg-info/top_level.txt
```

### Comparing `text2hologram-0.0.4/pyproject.toml` & `text2hologram-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text2hologram"
-version = "0.0.4"
+version = "0.1.0"
 description = "Generate holograms from text"
 readme = "README.md"
 authors = [{ name = "Pengze Li", email = "linsonng@163.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -28,8 +28,8 @@
 requires-python = ">=3.9"
 
 
 [project.urls]
 Homepage = "https://github.com/Linsonng/text2hologram"
 
 [project.scripts]
-text2hologram = "text2hologram.__main__:main"
+text2hologram = "text2hologram.__main__:main"
```

### Comparing `text2hologram-0.0.4/src/text2hologram/__main__.py` & `text2hologram-0.1.0/src/text2hologram/__main__.py`

 * *Files identical despite different names*

### Comparing `text2hologram-0.0.4/src/text2hologram/config.json` & `text2hologram-0.1.0/src/text2hologram/config.json`

 * *Files identical despite different names*

### Comparing `text2hologram-0.0.4/src/text2hologram/image_generation.py` & `text2hologram-0.1.0/src/text2hologram/image_generation.py`

 * *Files identical despite different names*

### Comparing `text2hologram-0.0.4/src/text2hologram/model.py` & `text2hologram-0.1.0/src/text2hologram/model.py`

 * *Files identical despite different names*

### Comparing `text2hologram-0.0.4/src/text2hologram/post_processing.py` & `text2hologram-0.1.0/src/text2hologram/post_processing.py`

 * *Files identical despite different names*

### Comparing `text2hologram-0.0.4/src/text2hologram/settings.py` & `text2hologram-0.1.0/src/text2hologram/settings.py`

 * *Files identical despite different names*

### Comparing `text2hologram-0.0.4/src/text2hologram.egg-info/SOURCES.txt` & `text2hologram-0.1.0/src/text2hologram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

