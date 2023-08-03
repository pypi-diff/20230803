# Comparing `tmp/mcemtools-0.8.4.tar.gz` & `tmp/mcemtools-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.8.4.tar", last modified: Fri Jul 28 04:23:38 2023, max compression
+gzip compressed data, was "mcemtools-0.8.5.tar", last modified: Thu Aug  3 10:44:53 2023, max compression
```

## Comparing `mcemtools-0.8.4.tar` & `mcemtools-0.8.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:23:38.979864 mcemtools-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-28 04:23:28.000000 mcemtools-0.8.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-28 04:23:28.000000 mcemtools-0.8.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-28 04:23:28.000000 mcemtools-0.8.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 04:23:28.000000 mcemtools-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 04:23:28.000000 mcemtools-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-28 04:23:38.979864 mcemtools-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-28 04:23:28.000000 mcemtools-0.8.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:23:38.979864 mcemtools-0.8.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 04:23:28.000000 mcemtools-0.8.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:23:38.979864 mcemtools-0.8.4/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-28 04:23:28.000000 mcemtools-0.8.4/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-28 04:23:28.000000 mcemtools-0.8.4/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 04:23:28.000000 mcemtools-0.8.4/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-28 04:23:28.000000 mcemtools-0.8.4/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-28 04:23:28.000000 mcemtools-0.8.4/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-28 04:23:28.000000 mcemtools-0.8.4/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-28 04:23:28.000000 mcemtools-0.8.4/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:23:38.979864 mcemtools-0.8.4/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-28 04:23:38.000000 mcemtools-0.8.4/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-28 04:23:38.000000 mcemtools-0.8.4/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:23:38.000000 mcemtools-0.8.4/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 04:23:38.000000 mcemtools-0.8.4/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:23:38.000000 mcemtools-0.8.4/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 04:23:38.000000 mcemtools-0.8.4/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 04:23:38.000000 mcemtools-0.8.4/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 04:23:28.000000 mcemtools-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-28 04:23:38.979864 mcemtools-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-28 04:23:28.000000 mcemtools-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:23:38.979864 mcemtools-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 04:23:28.000000 mcemtools-0.8.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 04:23:28.000000 mcemtools-0.8.4/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-28 04:23:28.000000 mcemtools-0.8.4/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-28 04:23:28.000000 mcemtools-0.8.4/tests/test_mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-28 04:23:28.000000 mcemtools-0.8.4/tests/test_tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-28 04:23:28.000000 mcemtools-0.8.4/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:53.505726 mcemtools-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-03 10:44:41.000000 mcemtools-0.8.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-08-03 10:44:41.000000 mcemtools-0.8.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-03 10:44:41.000000 mcemtools-0.8.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-03 10:44:41.000000 mcemtools-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-03 10:44:41.000000 mcemtools-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-03 10:44:53.505726 mcemtools-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-03 10:44:41.000000 mcemtools-0.8.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:53.501726 mcemtools-0.8.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 10:44:41.000000 mcemtools-0.8.5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:53.505726 mcemtools-0.8.5/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-08-03 10:44:41.000000 mcemtools-0.8.5/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:53.505726 mcemtools-0.8.5/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 10:44:53.000000 mcemtools-0.8.5/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 10:44:41.000000 mcemtools-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-03 10:44:53.505726 mcemtools-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-03 10:44:41.000000 mcemtools-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:44:53.505726 mcemtools-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/test_mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/test_tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-03 10:44:41.000000 mcemtools-0.8.5/tests/test_transforms.py
```

### Comparing `mcemtools-0.8.4/CONTRIBUTING.rst` & `mcemtools-0.8.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/HISTORY.rst` & `mcemtools-0.8.5/HISTORY.rst`

 * *Files 15% similar despite different names*

```diff
@@ -53,8 +53,12 @@
 
 0.8.3 (2023-07-28)
 ------------------
 * critical bug was fixed in viewer_4D
 
 0.8.4 (2023-07-28)
 ------------------
-* critical bug was fixed in viewer_4D
+* critical bug was fixed in viewer_4D
+
+0.8.5 (2023-08-03)
+------------------
+* bug fixed in image_by_windows
```

### Comparing `mcemtools-0.8.4/LICENSE` & `mcemtools-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/PKG-INFO` & `mcemtools-0.8.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.8.4
+Version: 0.8.5
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -120,7 +120,11 @@
 0.8.3 (2023-07-28)
 ------------------
 * critical bug was fixed in viewer_4D
 
 0.8.4 (2023-07-28)
 ------------------
 * critical bug was fixed in viewer_4D
+
+0.8.5 (2023-08-03)
+------------------
+* bug fixed in image_by_windows
```

### Comparing `mcemtools-0.8.4/README.rst` & `mcemtools-0.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/docs/Makefile` & `mcemtools-0.8.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/docs/conf.py` & `mcemtools-0.8.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/docs/installation.rst` & `mcemtools-0.8.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/docs/make.bat` & `mcemtools-0.8.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/mcemtools/__init__.py` & `mcemtools-0.8.5/mcemtools/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for mcemtools."""
 
 __author__ = """Alireza Sadri"""
 __email__ = 'Alireza.Sadri@monash.edu'
-__version__ = '0.8.4'
+__version__ = '0.8.5'
 
 from .analysis import pyMSSE, cross_correlation_4D, SymmSTEM
 from .analysis import centre_of_mass_4D, sum_4D
 
 from .masking import annular_mask, image_by_windows, markimage, mask2D_to_4D
 
 from .tensor_svd import svd_fit, svd_eval
 
 from .transforms import get_polar_coords, polar2image, image2polar, bin_4D
-from .transforms import normalize_4D
+from .transforms import normalize_4D, data4D_to_multichannel
 
 from .mcemtools import pltfig_to_numpy, locate_atoms, numbers_as_images
 from .mcemtools import open_muSTEM_binary, viewer_4D
```

### Comparing `mcemtools-0.8.4/mcemtools/analysis.py` & `mcemtools-0.8.5/mcemtools/analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/mcemtools/masking.py` & `mcemtools-0.8.5/mcemtools/masking.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 
     return mask.astype('uint8') 
 
 class image_by_windows:
     def __init__(self, 
                  img_shape: tuple[int, int], 
                  win_shape: tuple[int, int],
-                 skip: tuple[int, int] = (1, 1)):
+                 skip: tuple[int, int] = (1, 1),
+                 method = 'linear'):
         """image by windows
         
             I am using OOP here because the user pretty much always wants to
             transform results back to the original shape. It is different
             from typical transforms, where the processing ends at the other
             space.
         
@@ -70,27 +71,47 @@
             :param img_shape:
                 pass your_data.shape. First two dimensions should be for the
                 image to be cropped.
             :param win_shape:
                 the cropping windows shape
             :param skip:
                 The skipping length of windows
+            :param method:
+                default is linear, it means that if it cannot preserve the skip
+                it will not, but the grid will be spread evenly among windows.
+                If you wish to keep the skip exact, choose fixed. If the size
+                of the image is not dividable by the skip, it will have to
+                change the location of last window such that the entire image
+                is covered. This emans that the location of the grid will be 
+                moved to the left. 
         """
         self.img_shape = img_shape
         self.win_shape = win_shape
         self.skip = skip
-        n_r, n_c = img_shape[:2]
-        rows = np.arange(0, n_r - win_shape[0] + 1, skip[0])
-        clms = np.arange(0, n_c - win_shape[1] + 1, skip[1])
         
-        if rows[-1] < n_r - win_shape[0]:
-            rows = np.concatenate(rows, n_r - win_shape[0])
-        if clms[-1] > n_c - win_shape[1]:
-            clms = np.concatenate(clms, n_c - win_shape[1])
-    
+        assert win_shape[0]<= img_shape[0], 'win must be smaller than the image'
+        assert win_shape[1]<= img_shape[1], 'win must be smaller than the image'
+        
+        n_r, n_c = img_shape[:2]
+
+        if(method == 'fixed'):
+            rows = np.arange(0, n_r - win_shape[0] + 1, skip[0])
+            clms = np.arange(0, n_c - win_shape[1] + 1, skip[1])
+            if rows[-1] < n_r - win_shape[0]:
+                rows = np.concatenate((rows, np.array([n_r - win_shape[0]])))
+            if clms[-1] < n_c - win_shape[1]:
+                clms = np.concatenate((clms, np.array([n_c - win_shape[1]])))
+        if(method == 'linear'):
+            rows = np.linspace(
+                0, n_r - win_shape[0],n_r // skip[0], dtype = 'int')
+            rows = np.unique(rows)
+            clms = np.linspace(
+                0, n_c - win_shape[1],n_r // skip[1], dtype = 'int')
+            clms = np.unique(clms)
+            
         grid_clms, grid_rows = np.meshgrid(clms, rows)
     
         self.grid = np.array([grid_rows.ravel(), grid_clms.ravel()]).T
         self.visited = np.zeros(self.img_shape, dtype='int')
         for grc in self.grid:
             self.visited[grc[0]:grc[0] + self.win_shape[0], 
                          grc[1]:grc[1] + self.win_shape[1]] += 1
```

### Comparing `mcemtools-0.8.4/mcemtools/mcemtools.py` & `mcemtools-0.8.5/mcemtools/mcemtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,18 +165,18 @@
                 sh_type = shape_layer.shape_type[shape_cnt]
                 if sh_type == 'path':
                     if (sh_width < 2):
                         pt_data = shape_layer.data[shape_cnt]
                         _mask2D = polygon2mask(mask_shape ,pt_data)
                     else:
                         _mask2D = label2D.copy()
-                        _mask2D[_mask2D != shape_cnt + 1] = 0
+                        _mask2D[_mask2D != shape_cnt + 1] = 0   ##################################Wrong when overlapping
                 else:
                     _mask2D = label2D.copy()
-                    _mask2D[_mask2D != shape_cnt + 1] = 0
+                    _mask2D[_mask2D != shape_cnt + 1] = 0   ##################################Wrong when overlapping
                 if sh_width == 2:
                     _mask2D_swirl_sum = swirl_and_sum(_mask2D)
                     _mask2D_swirl_sum[_mask2D_swirl_sum >= 7] = 0
                     _mask2D_swirl_sum[_mask2D_swirl_sum>0] = 1
                     _mask2D = _mask2D_swirl_sum.copy()
                 elif sh_width > 2:
                     _mask2D_swirl_sum = swirl_and_sum(_mask2D)
```

### Comparing `mcemtools-0.8.4/mcemtools/tensor_svd.py` & `mcemtools-0.8.5/mcemtools/tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/mcemtools/transforms.py` & `mcemtools-0.8.5/mcemtools/transforms.py`

 * *Files 15% similar despite different names*

```diff
@@ -168,14 +168,28 @@
         polar_mask[a,b] += 1
         polar_maskq[aq,b] += 1
     polar_image[polar_mask>0] /= polar_mask[polar_mask>0]
     polar_imageq[polar_maskq>0] /= polar_maskq[polar_maskq>0]
     
     return (polar_image, polar_imageq, polar_mask, polar_maskq)
 
+class polar_transform:
+    def __init__(self, image_shape, centre, polar_shape):
+        self.image_shape = image_shape
+        self.polar_shape = polar_shape
+        self.centre = centre
+        self.get_polar_coords_output = \
+            get_polar_coords(self.image_shape, self.centre, self.polar_shape)
+    def image2polar(self, data):
+        return image2polar(data, self.polar_shape[0], self.polar_shape[1],
+                           self.centre, self.get_polar_coords_output)
+    def polar2image(self, data, dataq = None):
+        return polar2image(data, self.image_shape, dataq, self.centre,
+                           self.get_polar_coords_output)
+
 def normalize_4D(data4D, mask4D = None):
     """
         Note::
             make sure you have set mask4D[data4D == 0] = 0 when dealing with
             Poisson.
     """
     data4D = data4D.copy()
@@ -205,8 +219,25 @@
     dset_std = dset_std**0.5
     dset_std_tile = np.tile(np.array([dset_std]).swapaxes(0,1), (1, n_r * n_c))
     data4D[dset_std_tile>0] /= dset_std_tile[dset_std_tile>0]
     
     data4D = data4D.reshape(n_x, n_y, n_r* n_c)
     data4D = data4D.reshape(n_x, n_y, n_r, n_c)
     
-    return data4D
+    return data4D
+
+def data4D_to_multichannel(data4D):
+    """data4D to multichannel
+    
+        Given the input numpy array of shape n_x x n_y x n_r x n_c the output
+        would simply be n_r x n_c x n_x*n_y.
+        
+        The definition of channel is according to RGB of matplotlib. As such 
+        this can be easily given to functions that take multichannel in lognflow
+    
+    """
+    n_x, n_y, n_r, n_c = data4D.shape
+    data4D_multich = data4D.reshape(n_x*n_y, n_r, n_c)
+    return data4D_multich.swapaxes(0, 1).swapaxes(1, 2)
+    
+    
+
```

### Comparing `mcemtools-0.8.4/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.8.5/mcemtools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.8.4
+Version: 0.8.5
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -120,7 +120,11 @@
 0.8.3 (2023-07-28)
 ------------------
 * critical bug was fixed in viewer_4D
 
 0.8.4 (2023-07-28)
 ------------------
 * critical bug was fixed in viewer_4D
+
+0.8.5 (2023-08-03)
+------------------
+* bug fixed in image_by_windows
```

### Comparing `mcemtools-0.8.4/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.8.5/mcemtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/setup.py` & `mcemtools-0.8.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #!/usr/bin/env python
 
-__version__ = '0.8.4'
+__version__ = '0.8.5'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = ['numpy', 'matplotlib', 'scipy', 
-                'scikit-learn', 'scikit-image',
-                'lognflow', 'RobustGaussianFittingLibrary']
+                'scikit-learn', 'scikit-image', 'lognflow']
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Alireza Sadri",
     author_email='Alireza.Sadri@monash.edu',
     python_requires='>=3.7',
```

### Comparing `mcemtools-0.8.4/tests/test_analysis.py` & `mcemtools-0.8.5/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/tests/test_masking.py` & `mcemtools-0.8.5/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/tests/test_mcemtools.py` & `mcemtools-0.8.5/tests/test_mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/tests/test_tensor_svd.py` & `mcemtools-0.8.5/tests/test_tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.4/tests/test_transforms.py` & `mcemtools-0.8.5/tests/test_transforms.py`

 * *Files identical despite different names*

