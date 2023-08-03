# Comparing `tmp/image2layout_computer_vision-0.0.8.tar.gz` & `tmp/image2layout_computer_vision-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2layout_computer_vision-0.0.8.tar", last modified: Fri Jul 28 10:25:07 2023, max compression
+gzip compressed data, was "image2layout_computer_vision-0.0.9.tar", last modified: Mon Jul 31 07:07:25 2023, max compression
```

## Comparing `image2layout_computer_vision-0.0.8.tar` & `image2layout_computer_vision-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 10:25:07.259292 image2layout_computer_vision-0.0.8/
--rw-r--r--   0 felixdo    (501) staff       (20)     1073 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.8/LICENSE
--rw-r--r--   0 felixdo    (501) staff       (20)     2963 2023-07-28 10:25:07.259142 image2layout_computer_vision-0.0.8/PKG-INFO
--rw-r--r--   0 felixdo    (501) staff       (20)     2393 2023-07-28 02:48:08.000000 image2layout_computer_vision-0.0.8/README.md
--rw-r--r--   0 felixdo    (501) staff       (20)      637 2023-07-28 10:24:49.000000 image2layout_computer_vision-0.0.8/pyproject.toml
--rw-r--r--   0 felixdo    (501) staff       (20)       38 2023-07-28 10:25:07.259340 image2layout_computer_vision-0.0.8/setup.cfg
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 10:25:07.254143 image2layout_computer_vision-0.0.8/src/
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 10:25:07.254476 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/
--rw-r--r--   0 felixdo    (501) staff       (20)      416 2023-07-27 04:43:37.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/__init__.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 10:25:07.255715 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/color_extract/
--rw-r--r--   0 felixdo    (501) staff       (20)       95 2023-07-26 08:56:49.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/color_extract/__init__.py
--rw-r--r--   0 felixdo    (501) staff       (20)     8737 2023-07-28 02:57:52.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/color_extract/main.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 10:25:07.256991 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/ocr/
--rw-r--r--   0 felixdo    (501) staff       (20)      212 2023-07-27 04:43:44.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/ocr/__init__.py
--rw-r--r--   0 felixdo    (501) staff       (20)    14270 2023-07-28 10:22:11.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/ocr/imagebox.py
--rw-r--r--   0 felixdo    (501) staff       (20)     2679 2023-07-28 02:55:46.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/ocr/main.py
--rw-r--r--   0 felixdo    (501) staff       (20)     6286 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 10:25:07.258731 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/utils/
--rw-r--r--   0 felixdo    (501) staff       (20)      227 2023-07-27 11:28:42.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/utils/__init__.py
--rw-r--r--   0 felixdo    (501) staff       (20)     2221 2023-07-27 11:32:07.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/utils/annotation.py
--rw-r--r--   0 felixdo    (501) staff       (20)     4896 2023-07-26 08:33:29.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/utils/color_system.py
--rw-r--r--   0 felixdo    (501) staff       (20)     1398 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/utils/imaging.py
--rw-r--r--   0 felixdo    (501) staff       (20)     1900 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/utils/pixel_mask.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-28 10:25:07.255284 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision.egg-info/
--rw-r--r--   0 felixdo    (501) staff       (20)     2963 2023-07-28 10:25:07.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision.egg-info/PKG-INFO
--rw-r--r--   0 felixdo    (501) staff       (20)      923 2023-07-28 10:25:07.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision.egg-info/SOURCES.txt
--rw-r--r--   0 felixdo    (501) staff       (20)        1 2023-07-28 10:25:07.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision.egg-info/dependency_links.txt
--rw-r--r--   0 felixdo    (501) staff       (20)       54 2023-07-28 10:25:07.000000 image2layout_computer_vision-0.0.8/src/image2layout_computer_vision.egg-info/top_level.txt
--rw-r--r--   0 felixdo    (501) staff       (20)    13593 2023-07-27 10:41:57.000000 image2layout_computer_vision-0.0.8/src/sandbox.py
--rw-r--r--   0 felixdo    (501) staff       (20)     8862 2023-07-27 11:39:27.000000 image2layout_computer_vision-0.0.8/src/sandbox_ocr.py
--rw-r--r--   0 felixdo    (501) staff       (20)      747 2023-07-26 09:01:24.000000 image2layout_computer_vision-0.0.8/src/test.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.610577 image2layout_computer_vision-0.0.9/
+-rw-r--r--   0 felixdo    (501) staff       (20)     1073 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.9/LICENSE
+-rw-r--r--   0 felixdo    (501) staff       (20)     2963 2023-07-31 07:07:25.610320 image2layout_computer_vision-0.0.9/PKG-INFO
+-rw-r--r--   0 felixdo    (501) staff       (20)     2393 2023-07-28 02:48:08.000000 image2layout_computer_vision-0.0.9/README.md
+-rw-r--r--   0 felixdo    (501) staff       (20)      637 2023-07-31 07:05:05.000000 image2layout_computer_vision-0.0.9/pyproject.toml
+-rw-r--r--   0 felixdo    (501) staff       (20)       38 2023-07-31 07:07:25.610644 image2layout_computer_vision-0.0.9/setup.cfg
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.604968 image2layout_computer_vision-0.0.9/src/
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.605313 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/
+-rw-r--r--   0 felixdo    (501) staff       (20)      416 2023-07-27 04:43:37.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/__init__.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.606769 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/color_extract/
+-rw-r--r--   0 felixdo    (501) staff       (20)       95 2023-07-26 08:56:49.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/color_extract/__init__.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     8737 2023-07-28 02:57:52.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/color_extract/main.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.608260 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/
+-rw-r--r--   0 felixdo    (501) staff       (20)      212 2023-07-27 04:43:44.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/__init__.py
+-rw-r--r--   0 felixdo    (501) staff       (20)    14270 2023-07-28 10:22:11.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/imagebox.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     2652 2023-07-31 07:04:17.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/main.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     6286 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.609885 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/
+-rw-r--r--   0 felixdo    (501) staff       (20)      227 2023-07-27 11:28:42.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/__init__.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     2221 2023-07-27 11:32:07.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/annotation.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     4896 2023-07-26 08:33:29.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/color_system.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     1398 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/imaging.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     1900 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/pixel_mask.py
+drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.606272 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/
+-rw-r--r--   0 felixdo    (501) staff       (20)     2963 2023-07-31 07:07:25.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/PKG-INFO
+-rw-r--r--   0 felixdo    (501) staff       (20)      923 2023-07-31 07:07:25.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 felixdo    (501) staff       (20)        1 2023-07-31 07:07:25.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 felixdo    (501) staff       (20)       54 2023-07-31 07:07:25.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/top_level.txt
+-rw-r--r--   0 felixdo    (501) staff       (20)    13593 2023-07-27 10:41:57.000000 image2layout_computer_vision-0.0.9/src/sandbox.py
+-rw-r--r--   0 felixdo    (501) staff       (20)     8978 2023-07-31 07:03:32.000000 image2layout_computer_vision-0.0.9/src/sandbox_ocr.py
+-rw-r--r--   0 felixdo    (501) staff       (20)      747 2023-07-26 09:01:24.000000 image2layout_computer_vision-0.0.9/src/test.py
```

### Comparing `image2layout_computer_vision-0.0.8/LICENSE` & `image2layout_computer_vision-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/PKG-INFO` & `image2layout_computer_vision-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout_computer_vision
-Version: 0.0.8
+Version: 0.0.9
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `image2layout_computer_vision-0.0.8/README.md` & `image2layout_computer_vision-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/pyproject.toml` & `image2layout_computer_vision-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "Pillow",
   "numpy",
   "pandas",
 ]
 
 [project]
 name = "image2layout_computer_vision"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Felix Do", email="felix.do.1030@gmail.com" },
 ]
 description = "image processing and stuff"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/color_extract/main.py` & `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/color_extract/main.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/ocr/imagebox.py` & `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/imagebox.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/ocr/main.py` & `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,19 +48,20 @@
     '''predict boxes for text in the image
     Parameters: (same as detect_text)
     Returns:
         boxes_merged: (np.ndarray) [M, 4] text boxes detected, merged boxes
         boxes_raw:    (np.ndarray) [N, 4] text boxes detected, all individual boxes (N >= M)
     '''
     imageboxes = detect_text(image, **kwargs)
-    boxes = np.array(list(imageboxes.df['box'])).astype(int)
     
     boxes_merged = np.array(imageboxes.boxes_top, int)
     boxes_raw = np.array(imageboxes.boxes, int)
     return boxes_merged, boxes_raw
 
 # %%
 if __name__ == '__main__':
     imageboxes = detect_text('data/inputs/SCR-20230710-ixfw.jpeg')
+    
     imageboxes.draw_anno(width=3)
-    imageboxes.df
-    boxes = np.array(list(imageboxes.df['box'])).astype(int)
+    
+    boxes_merged = np.array(imageboxes.boxes_top, int)
+    boxes_raw = np.array(imageboxes.boxes, int)
```

### Comparing `image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/ocr/model_layoutmlv2.py` & `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/model_layoutmlv2.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/utils/annotation.py` & `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/utils/color_system.py` & `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/color_system.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/utils/imaging.py` & `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/src/image2layout_computer_vision/utils/pixel_mask.py` & `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/pixel_mask.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/src/image2layout_computer_vision.egg-info/PKG-INFO` & `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout-computer-vision
-Version: 0.0.8
+Version: 0.0.9
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `image2layout_computer_vision-0.0.8/src/image2layout_computer_vision.egg-info/SOURCES.txt` & `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/src/sandbox.py` & `image2layout_computer_vision-0.0.9/src/sandbox.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.8/src/sandbox_ocr.py` & `image2layout_computer_vision-0.0.9/src/sandbox_ocr.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from PIL import Image, ImageFont, ImageDraw
 import plotly.express as px
 import plotly.io as pio
 pio.templates.default = 'plotly_dark'
 from typing import Union, Any, List, Dict, Tuple
 
 # %%
-from image2layout_computer_vision import (
+from src.image2layout_computer_vision import (
     ImageBoxes, detect_text, detect_text_boxes, BoxMerge, get_image
 )
 
 
 # %%
 boxes_top, boxes_bottom = detect_text_boxes(
-    '/Users/felixdo/Documents/Code/AI/image2layout-computer-vision/data/inputs/SCR-20230710-jhbw.png',
+    # '/Users/felixdo/Documents/Code/AI/image2layout-computer-vision/data/inputs/SCR-20230710-jhbw.png',
+    '/Users/felixdo/Documents/Code/AI/image2layout-computer-vision/data/inputs/section_capturenmvqljbvbg.png',
 )
 boxes_top, boxes_bottom
 
-
 # %%
 IB = detect_text(
     '/Users/felixdo/Documents/Code/AI/image2layout-computer-vision/data/inputs/SCR-20230710-jhbw.png',
     grouping=False,
 )
 IB
```

### Comparing `image2layout_computer_vision-0.0.8/src/test.py` & `image2layout_computer_vision-0.0.9/src/test.py`

 * *Files identical despite different names*

