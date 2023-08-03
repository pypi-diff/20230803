# Comparing `tmp/heif-image-plugin-0.5.1.tar.gz` & `tmp/heif-image-plugin-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/heif-image-plugin-0.5.1.tar", last modified: Fri Jun 17 10:50:29 2022, max compression
+gzip compressed data, was "heif-image-plugin-0.6.0.tar", last modified: Thu Aug  3 20:31:13 2023, max compression
```

## Comparing `heif-image-plugin-0.5.1.tar` & `heif-image-plugin-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 Master     (501) staff       (20)        0 2022-06-17 10:50:29.000000 heif-image-plugin-0.5.1/
--rw-r--r--   0 Master     (501) staff       (20)     7837 2022-06-17 10:49:36.000000 heif-image-plugin-0.5.1/HeifImagePlugin.py
--rw-r--r--   0 Master     (501) staff       (20)     1130 2021-11-25 08:39:53.000000 heif-image-plugin-0.5.1/LICENSE
--rw-r--r--   0 Master     (501) staff       (20)       34 2021-11-25 08:39:53.000000 heif-image-plugin-0.5.1/MANIFEST.in
--rw-r--r--   0 Master     (501) staff       (20)     3984 2022-06-17 10:50:29.000000 heif-image-plugin-0.5.1/PKG-INFO
--rw-r--r--   0 Master     (501) staff       (20)     2939 2022-05-25 10:05:33.000000 heif-image-plugin-0.5.1/README.md
-drwxr-xr-x   0 Master     (501) staff       (20)        0 2022-06-17 10:50:29.000000 heif-image-plugin-0.5.1/heif_image_plugin.egg-info/
--rw-rw-r--   0 Master     (501) staff       (20)     3984 2022-06-17 10:50:29.000000 heif-image-plugin-0.5.1/heif_image_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 Master     (501) staff       (20)      271 2022-06-17 10:50:29.000000 heif-image-plugin-0.5.1/heif_image_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 Master     (501) staff       (20)        1 2022-06-17 10:50:29.000000 heif-image-plugin-0.5.1/heif_image_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 Master     (501) staff       (20)       82 2022-06-17 10:50:29.000000 heif-image-plugin-0.5.1/heif_image_plugin.egg-info/requires.txt
--rw-rw-r--   0 Master     (501) staff       (20)       16 2022-06-17 10:50:29.000000 heif-image-plugin-0.5.1/heif_image_plugin.egg-info/top_level.txt
--rw-r--r--   0 Master     (501) staff       (20)      308 2022-06-17 10:50:29.000000 heif-image-plugin-0.5.1/setup.cfg
--rwxr-xr-x   0 Master     (501) staff       (20)     1687 2022-06-17 10:49:46.000000 heif-image-plugin-0.5.1/setup.py
+drwxr-xr-x   0 master     (501) staff       (20)        0 2023-08-03 20:31:13.225281 heif-image-plugin-0.6.0/
+-rw-r--r--   0 master     (501) staff       (20)     8113 2023-08-03 14:13:20.000000 heif-image-plugin-0.6.0/HeifImagePlugin.py
+-rw-r--r--   0 master     (501) staff       (20)     1130 2021-11-25 08:39:53.000000 heif-image-plugin-0.6.0/LICENSE
+-rw-r--r--   0 master     (501) staff       (20)       34 2021-11-25 08:39:53.000000 heif-image-plugin-0.6.0/MANIFEST.in
+-rw-r--r--   0 master     (501) staff       (20)     4224 2023-08-03 20:31:13.225338 heif-image-plugin-0.6.0/PKG-INFO
+-rw-r--r--   0 master     (501) staff       (20)     3179 2023-08-03 14:17:28.000000 heif-image-plugin-0.6.0/README.md
+drwxr-xr-x   0 master     (501) staff       (20)        0 2023-08-03 20:31:13.225163 heif-image-plugin-0.6.0/heif_image_plugin.egg-info/
+-rw-rw-r--   0 master     (501) staff       (20)     4224 2023-08-03 20:31:13.000000 heif-image-plugin-0.6.0/heif_image_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 master     (501) staff       (20)      271 2023-08-03 20:31:13.000000 heif-image-plugin-0.6.0/heif_image_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 master     (501) staff       (20)        1 2023-08-03 20:31:13.000000 heif-image-plugin-0.6.0/heif_image_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 master     (501) staff       (20)       82 2023-08-03 20:31:13.000000 heif-image-plugin-0.6.0/heif_image_plugin.egg-info/requires.txt
+-rw-rw-r--   0 master     (501) staff       (20)       16 2023-08-03 20:31:13.000000 heif-image-plugin-0.6.0/heif_image_plugin.egg-info/top_level.txt
+-rw-r--r--   0 master     (501) staff       (20)      308 2023-08-03 20:31:13.225647 heif-image-plugin-0.6.0/setup.cfg
+-rwxr-xr-x   0 master     (501) staff       (20)     1687 2023-08-03 14:14:17.000000 heif-image-plugin-0.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `heif-image-plugin-0.5.1/HeifImagePlugin.py` & `heif-image-plugin-0.6.0/HeifImagePlugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-import inspect
 import subprocess
 import tempfile
 from copy import copy
 from weakref import WeakKeyDictionary
 
 import piexif
 import pyheif
 from cffi import FFI
 from PIL import Image, ImageFile
 from pyheif.error import HeifError
 
 
+try:
+    from pyheif.transformations import Transformations
+except ImportError:
+    Transformations = None
+
+
 ffi = FFI()
 _keep_refs = WeakKeyDictionary()
-pyheif_supports_transformations = (
-    'transformations' in inspect.signature(pyheif.HeifFile).parameters
-)
 HEIF_ENC_BIN = 'heif-enc'
 
 
 def _crop_heif_file(heif):
     # Zero-copy crop before loading. Just shifts data pointer and updates meta.
-    crop = heif.transformations['crop']
+    crop = heif.transformations.crop
     if crop == (0, 0) + heif.size:
         return heif
 
     if heif.mode not in ("L", "RGB", "RGBA"):
         raise ValueError("Unknown mode")
     pixel_size = len(heif.mode)
 
@@ -36,15 +38,16 @@
     # Keep reference to the original data as long as "cdata + offset" is alive.
     # Normally ffi.from_buffer should hold it for us but unfortunately
     # cdata + offset creates a new cdata object without reference.
     _keep_refs[cdata] = heif.data
 
     new_heif = copy(heif)
     new_heif.size = crop[2:4]
-    new_heif.transformations = dict(heif.transformations, crop=(0, 0) + crop[2:4])
+    new_heif.transformations = copy(heif.transformations)
+    new_heif.transformations.crop = (0, 0) + crop[2:4]
     new_heif.data = data
     return new_heif
 
 
 def _rotate_heif_file(heif):
     """
     Heif files already contain transformation chunks imir and irot which are
@@ -52,28 +55,29 @@
 
     This is not aligned with other formats behaviour and we MUST fix EXIF after
     loading to prevent unexpected rotation after resaving in other formats.
 
     And we come up to there is no reasons to force rotation of HEIF images
     after loading since we need update EXIF anyway.
     """
-    orientation = heif.transformations['orientation_tag']
+    orientation = heif.transformations.orientation_tag
     if not (1 <= orientation <= 8):
         return heif
 
     exif = {'0th': {piexif.ImageIFD.Orientation: orientation}}
     if heif.exif:
         try:
             exif = piexif.load(heif.exif)
             exif['0th'][piexif.ImageIFD.Orientation] = orientation
         except Exception:
             pass
 
     new_heif = copy(heif)
-    new_heif.transformations = dict(heif.transformations, orientation_tag=0)
+    new_heif.transformations = copy(heif.transformations)
+    new_heif.transformations.orientation_tag = 0
     new_heif.exif = piexif.dump(exif)
     return new_heif
 
 
 def _extract_heif_exif(heif_file):
     """
     Unlike other helper functions, this alters heif_file in-place.
@@ -94,23 +98,23 @@
 class HeifImageFile(ImageFile.ImageFile):
     format = 'HEIF'
     format_description = "HEIF/HEIC image"
 
     def _open(self):
         try:
             heif_file = pyheif.open(
-                self.fp, apply_transformations=not pyheif_supports_transformations)
+                self.fp, apply_transformations=Transformations is None)
         except HeifError as e:
             raise SyntaxError(str(e))
 
         _extract_heif_exif(heif_file)
 
-        if pyheif_supports_transformations:
+        if Transformations is not None:
             heif_file = _rotate_heif_file(heif_file)
-            self._size = heif_file.transformations['crop'][2:4]
+            self._size = heif_file.transformations.crop[2:4]
         else:
             self._size = heif_file.size
 
         self.mode = heif_file.mode
 
         if heif_file.exif:
             self.info['exif'] = heif_file.exif
@@ -140,15 +144,15 @@
                 if not cropped_file or not ImageFile.LOAD_TRUNCATED_IMAGES:
                     raise
                 # Ignore EOF error and return blank image otherwise
 
             self.load_prepare()
 
             if heif_file.data:
-                if pyheif_supports_transformations:
+                if Transformations is not None:
                     heif_file = _crop_heif_file(heif_file)
                 self.frombytes(heif_file.data, "raw", (self.mode, heif_file.stride))
 
             heif_file.data = None
 
         return super().load()
 
@@ -186,14 +190,19 @@
 
         if info.get('encoder'):
             cmd.extend(['-e', info['encoder']])
 
         if info.get('quality') is not None:
             cmd.extend(['-q', str(info['quality'])])
 
+        if info.get('downsampling') is not None:
+            if info['downsampling'] not in ('nn', 'average', 'sharp-yuv'):
+                raise ValueError(f"Unknown downsampling: {info['downsampling']}")
+            cmd.extend(['-C', info['downsampling']])
+
         subsampling = info.get('subsampling')
         if subsampling is not None:
             if subsampling == 0:
                 subsampling = '444'
             elif subsampling == 1:
                 subsampling = '422'
             elif subsampling == 2:
```

### Comparing `heif-image-plugin-0.5.1/LICENSE` & `heif-image-plugin-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heif-image-plugin-0.5.1/PKG-INFO` & `heif-image-plugin-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: heif-image-plugin
-Version: 0.5.1
+Version: 0.6.0
 Summary: Simple HEIF/HEIC images plugin for Pillow base on pyhief library.
 Home-page: https://github.com/uploadcare/heif-image-plugin
 Author: Alexander Karpinsky
 Author-email: homm86@gmail.com
 License: MIT
-Download-URL: https://github.com/uploadcare/heif-image-plugin/archive/v0.5.1.tar.gz
+Download-URL: https://github.com/uploadcare/heif-image-plugin/archive/v0.6.0.tar.gz
 Keywords: heif,heic,Pillow,plugin,pyhief
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -64,14 +64,24 @@
  1. do your fixes or add new awesome features (with tests)
  1. run the tests `make test`
  1. commit in new branch and make a pull request
 
 
 ## Changelog
 
+### 0.6.0
+
+* Minimal supported pyheif is 0.7.1
+* Added `downsampling` parameter for saving. Works only with `subsampling` == 2.
+* Transformations support updated to the latest libheif and pyheif
+
+### 0.5.1
+
+* Fixed HEIF saving in '1' mode
+
 ### 0.5.0
 
 * Added HEIF saving support if `heif-enc` is installed (part of libheif)
 * Fixed `HeifImageFile.verify()` call
 * Extensions .heic, .avif, .heif, .hif are handled by the plugin
 
 ### 0.4.0
```

### Comparing `heif-image-plugin-0.5.1/README.md` & `heif-image-plugin-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,24 @@
  1. do your fixes or add new awesome features (with tests)
  1. run the tests `make test`
  1. commit in new branch and make a pull request
 
 
 ## Changelog
 
+### 0.6.0
+
+* Minimal supported pyheif is 0.7.1
+* Added `downsampling` parameter for saving. Works only with `subsampling` == 2.
+* Transformations support updated to the latest libheif and pyheif
+
+### 0.5.1
+
+* Fixed HEIF saving in '1' mode
+
 ### 0.5.0
 
 * Added HEIF saving support if `heif-enc` is installed (part of libheif)
 * Fixed `HeifImageFile.verify()` call
 * Extensions .heic, .avif, .heif, .hif are handled by the plugin
 
 ### 0.4.0
```

### Comparing `heif-image-plugin-0.5.1/heif_image_plugin.egg-info/PKG-INFO` & `heif-image-plugin-0.6.0/heif_image_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: heif-image-plugin
-Version: 0.5.1
+Version: 0.6.0
 Summary: Simple HEIF/HEIC images plugin for Pillow base on pyhief library.
 Home-page: https://github.com/uploadcare/heif-image-plugin
 Author: Alexander Karpinsky
 Author-email: homm86@gmail.com
 License: MIT
-Download-URL: https://github.com/uploadcare/heif-image-plugin/archive/v0.5.1.tar.gz
+Download-URL: https://github.com/uploadcare/heif-image-plugin/archive/v0.6.0.tar.gz
 Keywords: heif,heic,Pillow,plugin,pyhief
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -64,14 +64,24 @@
  1. do your fixes or add new awesome features (with tests)
  1. run the tests `make test`
  1. commit in new branch and make a pull request
 
 
 ## Changelog
 
+### 0.6.0
+
+* Minimal supported pyheif is 0.7.1
+* Added `downsampling` parameter for saving. Works only with `subsampling` == 2.
+* Transformations support updated to the latest libheif and pyheif
+
+### 0.5.1
+
+* Fixed HEIF saving in '1' mode
+
 ### 0.5.0
 
 * Added HEIF saving support if `heif-enc` is installed (part of libheif)
 * Fixed `HeifImageFile.verify()` call
 * Extensions .heic, .avif, .heif, .hif are handled by the plugin
 
 ### 0.4.0
```

### Comparing `heif-image-plugin-0.5.1/setup.py` & `heif-image-plugin-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import os.path
 
 from setuptools import setup
 
 
-__version__ = '0.5.1'
+__version__ = '0.6.0'
 
 github_url = 'https://github.com/uploadcare'
 package_name = 'heif-image-plugin'
 package_path = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(package_path, 'README.md')) as f:
     long_description = f.read()
@@ -22,15 +22,15 @@
     long_description_content_type='text/markdown',
     author='Alexander Karpinsky',
     author_email='homm86@gmail.com',
     url='%s/%s' % (github_url, package_name),
     download_url='%s/%s/archive/v%s.tar.gz' % (github_url, package_name, __version__),
     keywords=['heif', 'heic', 'Pillow', 'plugin', 'pyhief'],
     install_requires=[
-        "pyheif>=0.6.1",
+        "pyheif>=0.7.1",
         "piexif>=1.1.3",
     ],
     extras_require={
         'test': [
             'pillow>=6.0.0',
             'pytest>=4.6.5',
             'pytest-cov>=2.8.1',
```

