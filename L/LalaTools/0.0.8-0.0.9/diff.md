# Comparing `tmp/LalaTools-0.0.8-py3-none-any.whl.zip` & `tmp/LalaTools-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4815 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      187 b- defN 22-Nov-16 13:57 lalatools/__init__.py
--rw-rw-rw-  2.0 fat     3814 b- defN 22-Nov-17 01:39 lalatools/DigitalImageProcessing/ImageProcess.py
--rw-rw-rw-  2.0 fat      240 b- defN 22-Nov-17 01:40 lalatools/DigitalImageProcessing/__init__.py
+Zip file size: 4769 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       14 b- defN 22-Nov-17 02:03 lalatools/__init__.py
+-rw-rw-rw-  2.0 fat     3959 b- defN 22-Nov-17 02:02 lalatools/DigitalImageProcessing/ImageProcess.py
+-rw-rw-rw-  2.0 fat      240 b- defN 22-Nov-17 02:03 lalatools/DigitalImageProcessing/__init__.py
 -rw-rw-rw-  2.0 fat     2795 b- defN 22-Nov-17 01:37 lalatools/ManageFileSystem/FileSystem.py
--rw-rw-rw-  2.0 fat      122 b- defN 22-Nov-17 01:40 lalatools/ManageFileSystem/__init__.py
--rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-17 01:40 LalaTools-0.0.8.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      286 b- defN 22-Nov-17 01:40 LalaTools-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Nov-17 01:40 LalaTools-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 22-Nov-17 01:40 LalaTools-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      869 b- defN 22-Nov-17 01:40 LalaTools-0.0.8.dist-info/RECORD
-10 files, 8424 bytes uncompressed, 3305 bytes compressed:  60.8%
+-rw-rw-rw-  2.0 fat      120 b- defN 22-Nov-17 02:03 lalatools/ManageFileSystem/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-17 02:04 LalaTools-0.0.9.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      286 b- defN 22-Nov-17 02:04 LalaTools-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Nov-17 02:04 LalaTools-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 22-Nov-17 02:04 LalaTools-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      868 b- defN 22-Nov-17 02:04 LalaTools-0.0.9.dist-info/RECORD
+10 files, 8393 bytes uncompressed, 3259 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: lalatools/ManageFileSystem/FileSystem.py
 Comment: 
 
 Filename: lalatools/ManageFileSystem/__init__.py
 Comment: 
 
-Filename: LalaTools-0.0.8.dist-info/LICENSE.txt
+Filename: LalaTools-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: LalaTools-0.0.8.dist-info/METADATA
+Filename: LalaTools-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: LalaTools-0.0.8.dist-info/WHEEL
+Filename: LalaTools-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: LalaTools-0.0.8.dist-info/top_level.txt
+Filename: LalaTools-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: LalaTools-0.0.8.dist-info/RECORD
+Filename: LalaTools-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lalatools/__init__.py

```diff
@@ -1,3 +1 @@
-__all__ = ['']
-# from .DigitalImageProcessing.ImageProcess import Match, MatchWithImage, WindowCapture, Test_Screen
-# from .DigitalImageProcessing.ImageProcess import cv2toPIL, PILtocv2
+__all__ = ['']
```

## lalatools/DigitalImageProcessing/ImageProcess.py

```diff
@@ -1,20 +1,25 @@
 import cv2
 import win32gui, win32ui, win32con
 from ctypes import windll
 from PIL import Image
 import numpy as np
 from mss import mss
 
+def imreadHangul(path):
+    img_array = np.fromfile(path, np.uint8)
+    img = cv2.imdecode(img_array, cv2.IMREAD_COLOR)
+    return img
+
 class MatchProcess():
     
     def __init__(self,large_image,small_image):
-        try: self.large_image = cv2.imread(large_image) # Read the images from the file
+        try: self.large_image = imreadHangul(large_image) # Read the images from the file
         except: self.large_image = large_image
-        try: self.small_image = cv2.imread(small_image) # Read the images from the file
+        try: self.small_image = imreadHangul(small_image) # Read the images from the file
         except: self.small_image = small_image
         
         method = cv2.TM_SQDIFF_NORMED
         result = cv2.matchTemplate(self.small_image, self.large_image, method)
         self.mn,_,self.mnLoc,_ = cv2.minMaxLoc(result) # min_val, max_val, min_loc, max_loc
         self.MPx,self.MPy = self.mnLoc
         self.trows,self.tcols = self.small_image.shape[:2]
```

## lalatools/ManageFileSystem/__init__.py

```diff
@@ -1,4 +1,3 @@
-
 from .FileSystem import delHead, replaceSplitMark, getFileList
 
 __all__ = ['delHead','replaceSplitMark','getFileList']
```

