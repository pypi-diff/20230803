# Comparing `tmp/pyzjr-1.0.1.tar.gz` & `tmp/pyzjr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-1.0.1.tar", last modified: Thu Jul 27 10:31:55 2023, max compression
+gzip compressed data, was "dist\pyzjr-1.0.2.tar", last modified: Thu Aug  3 09:12:55 2023, max compression
```

## Comparing `pyzjr-1.0.1.tar` & `pyzjr-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 10:31:55.000000 pyzjr-1.0.1/
--rw-rw-rw-   0        0        0     2838 2023-07-27 10:31:55.000000 pyzjr-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1634 2023-07-27 10:30:52.000000 pyzjr-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr/
--rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-1.0.1/pyzjr/ColorModule.py
--rw-rw-rw-   0        0        0    17203 2023-07-11 01:30:30.000000 pyzjr-1.0.1/pyzjr/Enimage.py
--rw-rw-rw-   0        0        0     3932 2023-07-21 17:30:08.000000 pyzjr-1.0.1/pyzjr/FM.py
--rw-rw-rw-   0        0        0     9085 2023-07-15 12:01:54.000000 pyzjr-1.0.1/pyzjr/MinIO.py
--rw-rw-rw-   0        0        0     7019 2023-07-26 16:37:00.000000 pyzjr-1.0.1/pyzjr/PIC.py
--rw-rw-rw-   0        0        0     6505 2023-07-26 16:48:15.000000 pyzjr-1.0.1/pyzjr/Showimage.py
--rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-1.0.1/pyzjr/TrackBar.py
--rw-rw-rw-   0        0        0      312 2023-07-12 11:15:25.000000 pyzjr-1.0.1/pyzjr/Z.py
--rw-rw-rw-   0        0        0      976 2023-07-27 10:31:48.000000 pyzjr-1.0.1/pyzjr/__init__.py
--rw-rw-rw-   0        0        0     6164 2023-07-22 02:13:00.000000 pyzjr-1.0.1/pyzjr/definition.py
--rw-rw-rw-   0        0        0     2356 2023-07-16 02:19:11.000000 pyzjr-1.0.1/pyzjr/utils.py
--rw-rw-rw-   0        0        0     4832 2023-07-24 15:58:50.000000 pyzjr-1.0.1/pyzjr/video.py
--rw-rw-rw-   0        0        0     3637 2023-07-27 04:09:54.000000 pyzjr-1.0.1/pyzjr/zmath.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/
--rw-rw-rw-   0        0        0     2838 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 10:31:55.000000 pyzjr-1.0.1/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 10:31:55.000000 pyzjr-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2044 2023-07-27 10:31:46.000000 pyzjr-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 09:12:55.000000 pyzjr-1.0.2/
+-rw-rw-rw-   0        0        0     2838 2023-08-03 09:12:55.000000 pyzjr-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1634 2023-07-27 10:30:52.000000 pyzjr-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 09:12:55.000000 pyzjr-1.0.2/pyzjr/
+-rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-1.0.2/pyzjr/ColorModule.py
+-rw-rw-rw-   0        0        0    17203 2023-07-11 01:30:30.000000 pyzjr-1.0.2/pyzjr/Enimage.py
+-rw-rw-rw-   0        0        0     3654 2023-08-03 09:11:06.000000 pyzjr-1.0.2/pyzjr/FM.py
+-rw-rw-rw-   0        0        0     9085 2023-07-15 12:01:54.000000 pyzjr-1.0.2/pyzjr/MinIO.py
+-rw-rw-rw-   0        0        0     7996 2023-08-02 11:13:43.000000 pyzjr-1.0.2/pyzjr/PIC.py
+-rw-rw-rw-   0        0        0     6505 2023-07-26 16:48:15.000000 pyzjr-1.0.2/pyzjr/Showimage.py
+-rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-1.0.2/pyzjr/TrackBar.py
+-rw-rw-rw-   0        0        0      312 2023-07-12 11:15:25.000000 pyzjr-1.0.2/pyzjr/Z.py
+-rw-rw-rw-   0        0        0      976 2023-08-03 09:12:37.000000 pyzjr-1.0.2/pyzjr/__init__.py
+-rw-rw-rw-   0        0        0     6168 2023-08-02 08:10:51.000000 pyzjr-1.0.2/pyzjr/definition.py
+-rw-rw-rw-   0        0        0     2491 2023-08-02 10:24:51.000000 pyzjr-1.0.2/pyzjr/utils.py
+-rw-rw-rw-   0        0        0     4832 2023-07-24 15:58:50.000000 pyzjr-1.0.2/pyzjr/video.py
+-rw-rw-rw-   0        0        0     3637 2023-07-27 04:09:54.000000 pyzjr-1.0.2/pyzjr/zmath.py
+drwxrwxrwx   0        0        0        0 2023-08-03 09:12:55.000000 pyzjr-1.0.2/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-08-03 09:12:54.000000 pyzjr-1.0.2/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-08-03 09:12:55.000000 pyzjr-1.0.2/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 09:12:54.000000 pyzjr-1.0.2/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-08-03 09:12:54.000000 pyzjr-1.0.2/pyzjr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-03 09:12:54.000000 pyzjr-1.0.2/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 09:12:55.000000 pyzjr-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2044 2023-08-03 09:11:55.000000 pyzjr-1.0.2/setup.py
```

### Comparing `pyzjr-1.0.1/PKG-INFO` & `pyzjr-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.0.1
+Version: 1.0.2
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
```

### Comparing `pyzjr-1.0.1/README.md` & `pyzjr-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.1/pyzjr/ColorModule.py` & `pyzjr-1.0.2/pyzjr/ColorModule.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.1/pyzjr/Enimage.py` & `pyzjr-1.0.2/pyzjr/Enimage.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.1/pyzjr/MinIO.py` & `pyzjr-1.0.2/pyzjr/MinIO.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.1/pyzjr/PIC.py` & `pyzjr-1.0.2/pyzjr/PIC.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,33 @@
 import pyzjr.Z as Z
 
 from skimage.morphology import skeletonize
 from skimage.filters import threshold_otsu
 from skimage.color import rgb2gray
 from skimage import measure
 
-import torch
 from torchvision import transforms
 
+def addnoisy(image, n=10000):
+    """
+    :param image: 原始图像
+    :param n: 添加椒盐的次数,默认为10000
+    :return: 返回被椒盐处理后的图像
+    """
+    result = image.copy()
+    w, h = image.shape[:2]
+    for i in range(n):
+        x = np.random.randint(0, w)
+        y = np.random.randint(0, h)
+        if np.random.randint(0, 2) == 0: 
+            result[x, y] = 0
+        else:
+            result[x, y] = 255
+    return result
+
 def repairImg(img,r=5,flags=Z.repair_NS,mode=0):
     """
     * 用于修复图像
     :param img: 输入图像
     :param r: 修复半径，即掩膜的像素周围需要参考的区域半径
     :param flags: 修复算法的标志,有Z.repair_NS、Z.repair_TELEA,默认为Z.repair_NS
     :param mode: 是否采用HSV例模式,默认为0,自定义模式,可通过Color下的TrackBar文件中获得
@@ -157,20 +173,36 @@
     """转化为RGB格式"""
     if len(np.shape(image)) == 3 and np.shape(image)[2] == 3:
         return image
     else:
         img = image.convert('RGB')
         return img
 
-def imtensor(image):
+def imtensor(image,dim=0):
     """转化为tensor格式
     image1 = Image.open(path).convert('L')
     image2 = pz.imtensor(image1)
     """
     preprocess = transforms.ToTensor()
-    image_tensor = preprocess(image).unsqueeze(0)
+    image_tensor = preprocess(image).unsqueeze(dim=dim)
     return image_tensor
 
-def impillow(input_tensor):
+def impillow(input_tensor,dim=0):
     """将tensor再转化为PIL"""
-    output_image = transforms.ToPILImage()(input_tensor.squeeze(0))
-    return output_image
+    output_image = transforms.ToPILImage()(input_tensor.squeeze(dim=dim))
+    return output_image
+
+def Rectangle_mask(image, boxes):
+    """
+    创建矩形蒙版
+    :param image: 原始图像。
+    :param boxes: [x1, y1, x2, y2]
+    :return: 蒙版与应用蒙版
+    """
+    mask = np.zeros(image.shape, dtype=np.uint8)
+    for box in boxes:
+        x1, y1, x2, y2 = box
+        mask[y1:y2, x1:x2] = 255
+    if mask.ndim == 3 and mask.shape[-1] > 1:
+        mask = mask[:, :, 0]
+    masked_image = cv2.bitwise_and(image, image, mask=mask)
+    return mask, masked_image
```

### Comparing `pyzjr-1.0.1/pyzjr/Showimage.py` & `pyzjr-1.0.2/pyzjr/Showimage.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.1/pyzjr/TrackBar.py` & `pyzjr-1.0.2/pyzjr/TrackBar.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.1/pyzjr/__init__.py` & `pyzjr-1.0.2/pyzjr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   At present, it is only for my personal use. If you want to
   use it, please contact me. Here are my email and WeChat.
 - WeChat: z15583909992
 - Email: zjricetea@gmail.com
 - Note: Currently still being updated, please refer to the latest version for any changes that may occur
 """
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 import cv2
 
 from pyzjr.Enimage import Filter,Enhance,Random_Enhance,Retinex
 from pyzjr.definition import *
 from pyzjr.ColorModule import *
 from pyzjr.definition import *
```

### Comparing `pyzjr-1.0.1/pyzjr/definition.py` & `pyzjr-1.0.2/pyzjr/definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,16 +120,16 @@
 
     def getThr(self,pathTest = "./ces/test",pathStd = "./ces/Standards"):
         """
         :param pathTest:测试的数据集文件夹位置
         :param pathStd: 标准图的数据文件夹位置
         :return: 模糊判定未知区间
         """
-        imgfile1 = getPhotopath(pathTest)
-        imgfile2 = getPhotopath(pathStd)
+        imgfile1,_ = getPhotopath(pathTest)
+        imgfile2,_ = getPhotopath(pathStd)
         a = self.getTest(imgfile1)
         b = self.getTest(imgfile2)
         thr = (a[0], b[0])
         # print(thr)
         return thr
 
 def vagueJudge(img, show_minandmax=True):
@@ -177,12 +177,12 @@
         M1 = np.sum(im_sharp[slices])
         M2 = np.sum(T[slices])
         blur_metric.append(np.abs((M1 - M2)) / M1)
 
     return np.max(blur_metric) if len(blur_metric) > 0 else 0.0
 
 if __name__ == "__main__":
-    image="./ces/test/01.jpg"   #需要进行测试的图片
+    image=r".ces\test\02.jpg"   #需要进行测试的图片
     image=cv2.imread(image)
     img=vagueJudge(image)
     cv2.imshow("img", img)
     k = cv2.waitKey(0) & 0xFF
```

### Comparing `pyzjr-1.0.1/pyzjr/video.py` & `pyzjr-1.0.2/pyzjr/video.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.1/pyzjr/zmath.py` & `pyzjr-1.0.2/pyzjr/zmath.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.1/pyzjr.egg-info/PKG-INFO` & `pyzjr-1.0.2/pyzjr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.0.1
+Version: 1.0.2
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
```

### Comparing `pyzjr-1.0.1/setup.py` & `pyzjr-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = ' A computer vision library that supports Win, packaged with patches for visual libraries such as \
                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui) \
                 engineering code experience. '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports Win'
 
 setup(
     name="pyzjr",
```

