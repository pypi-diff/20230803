# Comparing `tmp/bfscale-1.0a2.tar.gz` & `tmp/bfscale-1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfscale-1.0a2.tar", last modified: Wed Aug  2 07:04:39 2023, max compression
+gzip compressed data, was "bfscale-1.0a3.tar", last modified: Wed Aug  2 16:05:12 2023, max compression
```

## Comparing `bfscale-1.0a2.tar` & `bfscale-1.0a3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:04:39.415613 bfscale-1.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 07:04:16.000000 bfscale-1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-08-02 07:04:39.415613 bfscale-1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-08-02 07:04:16.000000 bfscale-1.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-02 07:04:16.000000 bfscale-1.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 07:04:39.415613 bfscale-1.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:04:39.411613 bfscale-1.0a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:04:39.415613 bfscale-1.0a2/src/bfscale/
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-08-02 07:04:16.000000 bfscale-1.0a2/src/bfscale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:04:39.415613 bfscale-1.0a2/src/bfscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-08-02 07:04:39.000000 bfscale-1.0a2/src/bfscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-02 07:04:39.000000 bfscale-1.0a2/src/bfscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 07:04:39.000000 bfscale-1.0a2/src/bfscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 07:04:39.000000 bfscale-1.0a2/src/bfscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 07:04:39.000000 bfscale-1.0a2/src/bfscale.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:04:39.415613 bfscale-1.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-02 07:04:16.000000 bfscale-1.0a2/tests/test_resize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:12.051074 bfscale-1.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 16:04:50.000000 bfscale-1.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-02 16:05:12.051074 bfscale-1.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-02 16:04:50.000000 bfscale-1.0a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-02 16:04:50.000000 bfscale-1.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:05:12.051074 bfscale-1.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:12.051074 bfscale-1.0a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:12.051074 bfscale-1.0a3/src/bfscale/
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-08-02 16:04:50.000000 bfscale-1.0a3/src/bfscale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:12.051074 bfscale-1.0a3/src/bfscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-08-02 16:05:12.000000 bfscale-1.0a3/src/bfscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-02 16:05:12.000000 bfscale-1.0a3/src/bfscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:05:12.000000 bfscale-1.0a3/src/bfscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 16:05:12.000000 bfscale-1.0a3/src/bfscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 16:05:12.000000 bfscale-1.0a3/src/bfscale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:05:12.051074 bfscale-1.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-02 16:04:50.000000 bfscale-1.0a3/tests/test_resize.py
```

### Comparing `bfscale-1.0a2/LICENSE` & `bfscale-1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `bfscale-1.0a2/PKG-INFO` & `bfscale-1.0a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 Metadata-Version: 2.1
 Name: bfscale
-Version: 1.0a2
+Version: 1.0a3
 Summary: Best fit image scaling
 Author-email: GroveDG <grovedgdev@gmail.com>
 Project-URL: Homepage, https://github.com/GroveDG/bfscale
 Project-URL: Bug Tracker, https://github.com/GroveDG/bfscale/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bfscale
 
-Best Fit Scale (bfscale) is a image downscaling method to create the highest possible image quality upon upscaling/upsampling with a certain scaling method (in this instance bilinear). This is achieved by curve fitting the sections of the original image that correspond to pixels in the downscaled image.
+Best Fit Scale (bfscale) is a image downscaling method to create the highest possible image quality upon upscaling/upsampling with a certain scaling method (in this instance bilinear). This is achieved by fitting the parameters of the upscaling model to sections of the original image. In the case of bilinear, this can be done with a simple linear regression.
 
 Bfscale was originally developed for improved Signed Distance Fields (SDFs), but was separated due to its broader usefulness.
 
 
 ## Dependencies
 <ul>
   <li>Numpy</li>
   <li>Numba</li>
   <li>ImageIO</li>
   <li>PySimpleGUI</li>
 </ul>
 
 ## Image Comparison
 
-<center>
-  <table>
-    <tr>
-      <th>Unscaled</th>
-      <th>Bfscale 20% Scale</th>
-      <th>Linear 20% Scale</th>
-    </tr>
-    <tr>
-      <td><img alt="Billiard Balls A. Unscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/c7cd6e43-19ee-42fd-b5c6-9bda1a5ca9cf" width="10000"></td>
-      <td><img alt="Billiard Balls A. Bfscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/2d009578-bb3e-41f2-9a61-929046fa8b24" width="10000"></td>
-      <td><img alt="Billiard Balls A. Linear Scaled" src="https://github.com/GroveDG/bfscale/assets/87248833/d3e676e0-0d85-48b9-bbfa-8424deb805b1" width="10000"></td>
-    </tr>
-    <tr>
-      <td><img alt="Billiard Balls A. Unscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/694e895e-371f-46f2-b402-e73b217b4e3e" width="10000"></td>
-      <td><img alt="Billiard Balls A. Bfscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/4c58f538-9e88-4f3a-a81c-8d1a4ab37437" width="10000"></td>
-      <td><img alt="Billiard Balls A. Linear Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/85bd749a-caa5-43a2-bd15-056542cfe61c" width="10000"></td>
-    </tr>
-  </table>
-  <details>
-    <summary>Image Source</summary>
-    <p>Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD</p>
-    <p>The images shown are part of the TESTIMAGES project: http://testimages.tecnick.com</p>
-  </details>
-</center>
+<table>
+  <tr>
+    <th>Unscaled</th>
+    <th>Bfscale 20% Scale</th>
+    <th>Linear 20% Scale</th>
+  </tr>
+  <tr>
+    <td><img alt="Billiard Balls A. Unscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/c7cd6e43-19ee-42fd-b5c6-9bda1a5ca9cf" width="10000"></td>
+    <td><img alt="Billiard Balls A. Bfscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/2d009578-bb3e-41f2-9a61-929046fa8b24" width="10000"></td>
+    <td><img alt="Billiard Balls A. Linear Scaled" src="https://github.com/GroveDG/bfscale/assets/87248833/d3e676e0-0d85-48b9-bbfa-8424deb805b1" width="10000"></td>
+  </tr>
+  <tr>
+    <td><img alt="Billiard Balls A. Unscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/694e895e-371f-46f2-b402-e73b217b4e3e" width="10000"></td>
+    <td><img alt="Billiard Balls A. Bfscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/4c58f538-9e88-4f3a-a81c-8d1a4ab37437" width="10000"></td>
+    <td><img alt="Billiard Balls A. Linear Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/85bd749a-caa5-43a2-bd15-056542cfe61c" width="10000"></td>
+  </tr>
+</table>
+<details>
+  <summary>Image Source</summary>
+  <p>Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD</p>
+  <p>The images shown are part of the TESTIMAGES project: http://testimages.tecnick.com</p>
+</details>
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1 Name: bfscale Version: 1.0a2 Summary: Best fit image
+Metadata-Version: 2.1 Name: bfscale Version: 1.0a3 Summary: Best fit image
 scaling Author-email: GroveDG
 gmail.com> Project-URL: Homepage, https://github.com/GroveDG/bfscale Project-
 URL: Bug Tracker, https://github.com/GroveDG/bfscale/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE # bfscale Best
 Fit Scale (bfscale) is a image downscaling method to create the highest
 possible image quality upon upscaling/upsampling with a certain scaling method
-(in this instance bilinear). This is achieved by curve fitting the sections of
-the original image that correspond to pixels in the downscaled image. Bfscale
-was originally developed for improved Signed Distance Fields (SDFs), but was
-separated due to its broader usefulness. ## Dependencies
+(in this instance bilinear). This is achieved by fitting the parameters of the
+upscaling model to sections of the original image. In the case of bilinear,
+this can be done with a simple linear regression. Bfscale was originally
+developed for improved Signed Distance Fields (SDFs), but was separated due to
+its broader usefulness. ## Dependencies
     * Numpy
     * Numba
     * ImageIO
     * PySimpleGUI
 ## Image Comparison
-   Unscaled           Bfscale 20% Scale           Linear 20% Scale
-   [Billiard Balls A. [Billiard Balls A.          [Billiard Balls A. Linear
-   Unscaled]          Bfscaled]                   Scaled]
-   [Billiard Balls A. [Billiard Balls A. Bfscaled [Billiard Balls A. Linear
-   Unscaled Cropped]  Cropped]                    Cropped]
-                                  Image Source
-            Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD
-         The images shown are part of the TESTIMAGES project: http://
-                            testimages.tecnick.com
+Unscaled           Bfscale 20% Scale           Linear 20% Scale
+[Billiard Balls A. [Billiard Balls A.          [Billiard Balls A. Linear
+Unscaled]          Bfscaled]                   Scaled]
+[Billiard Balls A. [Billiard Balls A. Bfscaled [Billiard Balls A. Linear
+Unscaled Cropped]  Cropped]                    Cropped]
+ Image Source
+Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD
+The images shown are part of the TESTIMAGES project: http://
+testimages.tecnick.com
+
```

### Comparing `bfscale-1.0a2/README.md` & `bfscale-1.0a3/src/bfscale.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,53 @@
+Metadata-Version: 2.1
+Name: bfscale
+Version: 1.0a3
+Summary: Best fit image scaling
+Author-email: GroveDG <grovedgdev@gmail.com>
+Project-URL: Homepage, https://github.com/GroveDG/bfscale
+Project-URL: Bug Tracker, https://github.com/GroveDG/bfscale/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # bfscale
 
-Best Fit Scale (bfscale) is a image downscaling method to create the highest possible image quality upon upscaling/upsampling with a certain scaling method (in this instance bilinear). This is achieved by curve fitting the sections of the original image that correspond to pixels in the downscaled image.
+Best Fit Scale (bfscale) is a image downscaling method to create the highest possible image quality upon upscaling/upsampling with a certain scaling method (in this instance bilinear). This is achieved by fitting the parameters of the upscaling model to sections of the original image. In the case of bilinear, this can be done with a simple linear regression.
 
 Bfscale was originally developed for improved Signed Distance Fields (SDFs), but was separated due to its broader usefulness.
 
 
 ## Dependencies
 <ul>
   <li>Numpy</li>
   <li>Numba</li>
   <li>ImageIO</li>
   <li>PySimpleGUI</li>
 </ul>
 
 ## Image Comparison
 
-<center>
-  <table>
-    <tr>
-      <th>Unscaled</th>
-      <th>Bfscale 20% Scale</th>
-      <th>Linear 20% Scale</th>
-    </tr>
-    <tr>
-      <td><img alt="Billiard Balls A. Unscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/c7cd6e43-19ee-42fd-b5c6-9bda1a5ca9cf" width="10000"></td>
-      <td><img alt="Billiard Balls A. Bfscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/2d009578-bb3e-41f2-9a61-929046fa8b24" width="10000"></td>
-      <td><img alt="Billiard Balls A. Linear Scaled" src="https://github.com/GroveDG/bfscale/assets/87248833/d3e676e0-0d85-48b9-bbfa-8424deb805b1" width="10000"></td>
-    </tr>
-    <tr>
-      <td><img alt="Billiard Balls A. Unscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/694e895e-371f-46f2-b402-e73b217b4e3e" width="10000"></td>
-      <td><img alt="Billiard Balls A. Bfscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/4c58f538-9e88-4f3a-a81c-8d1a4ab37437" width="10000"></td>
-      <td><img alt="Billiard Balls A. Linear Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/85bd749a-caa5-43a2-bd15-056542cfe61c" width="10000"></td>
-    </tr>
-  </table>
-  <details>
-    <summary>Image Source</summary>
-    <p>Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD</p>
-    <p>The images shown are part of the TESTIMAGES project: http://testimages.tecnick.com</p>
-  </details>
-</center>
+<table>
+  <tr>
+    <th>Unscaled</th>
+    <th>Bfscale 20% Scale</th>
+    <th>Linear 20% Scale</th>
+  </tr>
+  <tr>
+    <td><img alt="Billiard Balls A. Unscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/c7cd6e43-19ee-42fd-b5c6-9bda1a5ca9cf" width="10000"></td>
+    <td><img alt="Billiard Balls A. Bfscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/2d009578-bb3e-41f2-9a61-929046fa8b24" width="10000"></td>
+    <td><img alt="Billiard Balls A. Linear Scaled" src="https://github.com/GroveDG/bfscale/assets/87248833/d3e676e0-0d85-48b9-bbfa-8424deb805b1" width="10000"></td>
+  </tr>
+  <tr>
+    <td><img alt="Billiard Balls A. Unscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/694e895e-371f-46f2-b402-e73b217b4e3e" width="10000"></td>
+    <td><img alt="Billiard Balls A. Bfscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/4c58f538-9e88-4f3a-a81c-8d1a4ab37437" width="10000"></td>
+    <td><img alt="Billiard Balls A. Linear Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/85bd749a-caa5-43a2-bd15-056542cfe61c" width="10000"></td>
+  </tr>
+</table>
+<details>
+  <summary>Image Source</summary>
+  <p>Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD</p>
+  <p>The images shown are part of the TESTIMAGES project: http://testimages.tecnick.com</p>
+</details>
```

#### html2text {}

```diff
@@ -1,20 +1,29 @@
-# bfscale Best Fit Scale (bfscale) is a image downscaling method to create the
-highest possible image quality upon upscaling/upsampling with a certain scaling
-method (in this instance bilinear). This is achieved by curve fitting the
-sections of the original image that correspond to pixels in the downscaled
-image. Bfscale was originally developed for improved Signed Distance Fields
-(SDFs), but was separated due to its broader usefulness. ## Dependencies
+Metadata-Version: 2.1 Name: bfscale Version: 1.0a3 Summary: Best fit image
+scaling Author-email: GroveDG
+gmail.com> Project-URL: Homepage, https://github.com/GroveDG/bfscale Project-
+URL: Bug Tracker, https://github.com/GroveDG/bfscale/issues Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE # bfscale Best
+Fit Scale (bfscale) is a image downscaling method to create the highest
+possible image quality upon upscaling/upsampling with a certain scaling method
+(in this instance bilinear). This is achieved by fitting the parameters of the
+upscaling model to sections of the original image. In the case of bilinear,
+this can be done with a simple linear regression. Bfscale was originally
+developed for improved Signed Distance Fields (SDFs), but was separated due to
+its broader usefulness. ## Dependencies
     * Numpy
     * Numba
     * ImageIO
     * PySimpleGUI
 ## Image Comparison
-   Unscaled           Bfscale 20% Scale           Linear 20% Scale
-   [Billiard Balls A. [Billiard Balls A.          [Billiard Balls A. Linear
-   Unscaled]          Bfscaled]                   Scaled]
-   [Billiard Balls A. [Billiard Balls A. Bfscaled [Billiard Balls A. Linear
-   Unscaled Cropped]  Cropped]                    Cropped]
-                                  Image Source
-            Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD
-         The images shown are part of the TESTIMAGES project: http://
-                            testimages.tecnick.com
+Unscaled           Bfscale 20% Scale           Linear 20% Scale
+[Billiard Balls A. [Billiard Balls A.          [Billiard Balls A. Linear
+Unscaled]          Bfscaled]                   Scaled]
+[Billiard Balls A. [Billiard Balls A. Bfscaled [Billiard Balls A. Linear
+Unscaled Cropped]  Cropped]                    Cropped]
+ Image Source
+Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD
+The images shown are part of the TESTIMAGES project: http://
+testimages.tecnick.com
+
```

### Comparing `bfscale-1.0a2/pyproject.toml` & `bfscale-1.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "numba"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bfscale"
-version = "1.0a2"
+version = "1.0a3"
 authors = [
 	{ name="GroveDG", email="grovedgdev@gmail.com"}
 ]
 description = "Best fit image scaling"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `bfscale-1.0a2/src/bfscale/__init__.py` & `bfscale-1.0a3/src/bfscale/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,31 +55,30 @@
 	X = np.tile(indicies, scale)
 	Y = np.repeat(indicies, scale)
 
 	yx_indices = np.column_stack(((1-Y)*(1-X), (1-X)*Y, X*(1-Y), X*Y))
 
 	parameters, _, _, _ = np.linalg.lstsq(yx_indices, data, rcond=None)
 
-	out_img = np.pad(np.clip(parameters, 0, 255).transpose().reshape(out_img_shape), ((0,1), (0,1), (0,0), (0,0)), 'constant', constant_values=-1)
+	out_img = np.pad(parameters.transpose().reshape(out_img_shape), ((0,1), (0,1), (0,0), (0,0)), 'constant', constant_values=-1)
 	# This ↓↓↓ is what this line ↑↑↑ is doing
 	# ---------------------------------------
-	# out_img = np.clip(parameters, 0, 255)
 	# out_img = out_img.transpose()
 	# out_img = out_img.reshape(out_img_shape)
 	# out_img = np.pad(out_img, ((0,1), (0,1), (0,0), (0,0)), 'constant', constant_values=-1)
 
 	out_img[:, 1:, :, 1] = out_img[:, :-1, :, 1]
 	out_img[1:, :, :, 2] = out_img[:-1, :, :, 2]
 	out_img[1:, 1:, :, 3] = out_img[:-1, :-1, :, 3]
 	out_img[:, 0, :, 1] = -1
 	out_img[0, :, :, 2] = -1
 	out_img[0, 0, :, 3] = -1
 
 	out_img = np.ma.median(np.ma.masked_values(out_img, -1), axis=-1)
-	out_img = np.uint8(np.round(np.ma.getdata(out_img)))
+	out_img = np.uint8(np.clip(np.round(np.ma.getdata(out_img)), 0, 255))
 	return out_img
 
 def _scales_of(size):
 	scales = []
 	for n in range(1, floor(sqrt(size[0]))+1):
 		if size[0] % n == 0 and size[1] % n == 0:
 			scales.append(n)
```

### Comparing `bfscale-1.0a2/src/bfscale.egg-info/PKG-INFO` & `bfscale-1.0a3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,39 @@
-Metadata-Version: 2.1
-Name: bfscale
-Version: 1.0a2
-Summary: Best fit image scaling
-Author-email: GroveDG <grovedgdev@gmail.com>
-Project-URL: Homepage, https://github.com/GroveDG/bfscale
-Project-URL: Bug Tracker, https://github.com/GroveDG/bfscale/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # bfscale
 
-Best Fit Scale (bfscale) is a image downscaling method to create the highest possible image quality upon upscaling/upsampling with a certain scaling method (in this instance bilinear). This is achieved by curve fitting the sections of the original image that correspond to pixels in the downscaled image.
+Best Fit Scale (bfscale) is a image downscaling method to create the highest possible image quality upon upscaling/upsampling with a certain scaling method (in this instance bilinear). This is achieved by fitting the parameters of the upscaling model to sections of the original image. In the case of bilinear, this can be done with a simple linear regression.
 
 Bfscale was originally developed for improved Signed Distance Fields (SDFs), but was separated due to its broader usefulness.
 
 
 ## Dependencies
 <ul>
   <li>Numpy</li>
   <li>Numba</li>
   <li>ImageIO</li>
   <li>PySimpleGUI</li>
 </ul>
 
 ## Image Comparison
 
-<center>
-  <table>
-    <tr>
-      <th>Unscaled</th>
-      <th>Bfscale 20% Scale</th>
-      <th>Linear 20% Scale</th>
-    </tr>
-    <tr>
-      <td><img alt="Billiard Balls A. Unscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/c7cd6e43-19ee-42fd-b5c6-9bda1a5ca9cf" width="10000"></td>
-      <td><img alt="Billiard Balls A. Bfscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/2d009578-bb3e-41f2-9a61-929046fa8b24" width="10000"></td>
-      <td><img alt="Billiard Balls A. Linear Scaled" src="https://github.com/GroveDG/bfscale/assets/87248833/d3e676e0-0d85-48b9-bbfa-8424deb805b1" width="10000"></td>
-    </tr>
-    <tr>
-      <td><img alt="Billiard Balls A. Unscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/694e895e-371f-46f2-b402-e73b217b4e3e" width="10000"></td>
-      <td><img alt="Billiard Balls A. Bfscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/4c58f538-9e88-4f3a-a81c-8d1a4ab37437" width="10000"></td>
-      <td><img alt="Billiard Balls A. Linear Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/85bd749a-caa5-43a2-bd15-056542cfe61c" width="10000"></td>
-    </tr>
-  </table>
-  <details>
-    <summary>Image Source</summary>
-    <p>Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD</p>
-    <p>The images shown are part of the TESTIMAGES project: http://testimages.tecnick.com</p>
-  </details>
-</center>
+<table>
+  <tr>
+    <th>Unscaled</th>
+    <th>Bfscale 20% Scale</th>
+    <th>Linear 20% Scale</th>
+  </tr>
+  <tr>
+    <td><img alt="Billiard Balls A. Unscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/c7cd6e43-19ee-42fd-b5c6-9bda1a5ca9cf" width="10000"></td>
+    <td><img alt="Billiard Balls A. Bfscaled" src="https://github.com/GroveDG/bfscale/assets/87248833/2d009578-bb3e-41f2-9a61-929046fa8b24" width="10000"></td>
+    <td><img alt="Billiard Balls A. Linear Scaled" src="https://github.com/GroveDG/bfscale/assets/87248833/d3e676e0-0d85-48b9-bbfa-8424deb805b1" width="10000"></td>
+  </tr>
+  <tr>
+    <td><img alt="Billiard Balls A. Unscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/694e895e-371f-46f2-b402-e73b217b4e3e" width="10000"></td>
+    <td><img alt="Billiard Balls A. Bfscaled Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/4c58f538-9e88-4f3a-a81c-8d1a4ab37437" width="10000"></td>
+    <td><img alt="Billiard Balls A. Linear Cropped" src="https://github.com/GroveDG/bfscale/assets/87248833/85bd749a-caa5-43a2-bd15-056542cfe61c" width="10000"></td>
+  </tr>
+</table>
+<details>
+  <summary>Image Source</summary>
+  <p>Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD</p>
+  <p>The images shown are part of the TESTIMAGES project: http://testimages.tecnick.com</p>
+</details>
```

#### html2text {}

```diff
@@ -1,27 +1,22 @@
-Metadata-Version: 2.1 Name: bfscale Version: 1.0a2 Summary: Best fit image
-scaling Author-email: GroveDG
-gmail.com> Project-URL: Homepage, https://github.com/GroveDG/bfscale Project-
-URL: Bug Tracker, https://github.com/GroveDG/bfscale/issues Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE # bfscale Best
-Fit Scale (bfscale) is a image downscaling method to create the highest
-possible image quality upon upscaling/upsampling with a certain scaling method
-(in this instance bilinear). This is achieved by curve fitting the sections of
-the original image that correspond to pixels in the downscaled image. Bfscale
-was originally developed for improved Signed Distance Fields (SDFs), but was
+# bfscale Best Fit Scale (bfscale) is a image downscaling method to create the
+highest possible image quality upon upscaling/upsampling with a certain scaling
+method (in this instance bilinear). This is achieved by fitting the parameters
+of the upscaling model to sections of the original image. In the case of
+bilinear, this can be done with a simple linear regression. Bfscale was
+originally developed for improved Signed Distance Fields (SDFs), but was
 separated due to its broader usefulness. ## Dependencies
     * Numpy
     * Numba
     * ImageIO
     * PySimpleGUI
 ## Image Comparison
-   Unscaled           Bfscale 20% Scale           Linear 20% Scale
-   [Billiard Balls A. [Billiard Balls A.          [Billiard Balls A. Linear
-   Unscaled]          Bfscaled]                   Scaled]
-   [Billiard Balls A. [Billiard Balls A. Bfscaled [Billiard Balls A. Linear
-   Unscaled Cropped]  Cropped]                    Cropped]
-                                  Image Source
-            Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD
-         The images shown are part of the TESTIMAGES project: http://
-                            testimages.tecnick.com
+Unscaled           Bfscale 20% Scale           Linear 20% Scale
+[Billiard Balls A. [Billiard Balls A.          [Billiard Balls A. Linear
+Unscaled]          Bfscaled]                   Scaled]
+[Billiard Balls A. [Billiard Balls A. Bfscaled [Billiard Balls A. Linear
+Unscaled Cropped]  Cropped]                    Cropped]
+ Image Source
+Copyright (C) 2011-2014 Nicola Asuni - Tecnick.com LTD
+The images shown are part of the TESTIMAGES project: http://
+testimages.tecnick.com
+
```

### Comparing `bfscale-1.0a2/tests/test_resize.py` & `bfscale-1.0a3/tests/test_resize.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,12 +20,13 @@
 
 	return tmpdir
 
 def test_resize(datadir):
 	img_test = imread(os.path.realpath(datadir.join("billiards.tif")))
 	img_test = bf.resize(img_test, 5)
 	img_sample = imread(os.path.realpath(datadir.join("billiards-scaled.tif")))
-	diff = img_sample-img_test
+	diff = np.intc(img_sample)-np.intc(img_test)
 	print(diff.nonzero())
-	print(diff[diff != 0])
-	print(np.count_nonzero(diff))
-	assert np.all(img_sample == img_test)
+	print(diff[diff > 1])
+	print(img_test[diff > 1])
+	print(img_sample[diff > 1])
+	assert np.all(abs(diff) <= 1)
```

