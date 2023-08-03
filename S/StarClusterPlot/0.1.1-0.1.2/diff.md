# Comparing `tmp/StarClusterPlot-0.1.1.tar.gz` & `tmp/StarClusterPlot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StarClusterPlot-0.1.1.tar", last modified: Wed Aug  2 16:45:40 2023, max compression
+gzip compressed data, was "StarClusterPlot-0.1.2.tar", last modified: Thu Aug  3 04:01:30 2023, max compression
```

## Comparing `StarClusterPlot-0.1.1.tar` & `StarClusterPlot-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:45:40.867017 StarClusterPlot-0.1.1/
--rw-rw-rw-   0        0        0      119 2023-08-02 16:41:17.000000 StarClusterPlot-0.1.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1169 2023-08-02 16:45:40.865848 StarClusterPlot-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-08-02 11:27:34.000000 StarClusterPlot-0.1.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 16:45:40.834741 StarClusterPlot-0.1.1/StarClusterPlot/
--rw-rw-rw-   0        0        0     3920 2023-08-02 16:37:46.000000 StarClusterPlot-0.1.1/StarClusterPlot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:45:40.863504 StarClusterPlot-0.1.1/StarClusterPlot.egg-info/
--rw-rw-rw-   0        0        0     1169 2023-08-02 16:45:40.000000 StarClusterPlot-0.1.1/StarClusterPlot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-02 16:45:40.000000 StarClusterPlot-0.1.1/StarClusterPlot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:45:40.000000 StarClusterPlot-0.1.1/StarClusterPlot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-08-02 16:45:40.000000 StarClusterPlot-0.1.1/StarClusterPlot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-02 16:45:40.000000 StarClusterPlot-0.1.1/StarClusterPlot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 16:45:40.868025 StarClusterPlot-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-08-02 16:38:38.000000 StarClusterPlot-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 04:01:30.804077 StarClusterPlot-0.1.2/
+-rw-rw-rw-   0        0        0      259 2023-08-03 04:00:37.000000 StarClusterPlot-0.1.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1306 2023-08-03 04:01:30.804077 StarClusterPlot-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-08-03 03:51:38.000000 StarClusterPlot-0.1.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 04:01:30.765823 StarClusterPlot-0.1.2/StarClusterPlot/
+-rw-rw-rw-   0        0        0     4064 2023-08-03 03:59:57.000000 StarClusterPlot-0.1.2/StarClusterPlot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 04:01:30.802179 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/
+-rw-rw-rw-   0        0        0     1306 2023-08-03 04:01:30.000000 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-03 04:01:30.000000 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 04:01:30.000000 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 04:01:30.000000 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-03 04:01:30.000000 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 04:01:30.805079 StarClusterPlot-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-08-03 03:51:51.000000 StarClusterPlot-0.1.2/setup.py
```

### Comparing `StarClusterPlot-0.1.1/LICENCE.txt` & `StarClusterPlot-0.1.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `StarClusterPlot-0.1.1/PKG-INFO` & `StarClusterPlot-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StarClusterPlot
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for visualizing star clusters and their Hertzsprung-Russell diagrams
 Home-page: UNKNOWN
 Author: Teerat Chanromyen
 Author-email: teerat.nahm@gmail.com
 License: MIT
 Keywords: Astronomy
 Platform: UNKNOWN
@@ -15,19 +15,24 @@
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
 License-File: LICENCE.txt
 
 This is a Python library for visualizing star clusters and their Hertzsprung-Russell diagrams. 
 All stars colors shown in this program are derived from their calculated temperatures.
 The package includes two functions: ClusterVis() and HRDiagram(). 
-The former takes one dataframe as a required input along withÂ two optional parameters to set the x and y scale of the plot. The latter simply requires one dataframe input. 
+The former takes one dataframe as a required input along with two optional parameters to set the x and y scale of the plot. The latter simply requires one dataframe input. 
 
 Change Log
 ==========
 
-0.1.0 (2/08/2023)
+0.1.2 (3/08/2023)
 -----------------
-Initial Release
+- Add six optional parameters for the HRDiagram function
 
 0.1.1 (3/08/2023)
 -----------------
+- Fix the out-of-bound RGB value error
+
+0.1.0 (2/08/2023)
+-----------------
+- Initial Release
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `StarClusterPlot-0.1.1/StarClusterPlot/__init__.py` & `StarClusterPlot-0.1.2/StarClusterPlot/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from matplotlib import pyplot as plt
 
-def ClusterVis(data, x_ratio = 6.75, y_ratio = 12):
+def ClusterVis(data, x_scale = 6.75, y_scale = 12):
 
   RA = data['ra']
   DEC = data['dec']
   g = data['g']
   r = data['r']
 
   data['B'] = g + 0.3130*(g-r) + 0.2271
@@ -52,23 +52,23 @@
     RGB = XYZ_to_RGB(XYZ[0], XYZ[1], XYZ[2])
     return RGB
 
   data['RGB'] = data['temperature'].apply(Kelvin_to_RGB)
 
   RGB = data['RGB']
 
-  plt.figure(figsize=(x_ratio, y_ratio))
+  plt.figure(figsize=(x_scale, y_scale))
   plt.rcParams['axes.facecolor'] = '#252525'
   plt.scatter(RA,DEC, s=0.05, marker='o', c=RGB)
 
 
 
 
 
-def HRDiagram(data):
+def HRDiagram(data, left_bound = -40, right_bound = 40, lower_bound = -40, upper_bound = 40, x_scale = 6.75, y_scale = 12):
 
   g = data['g']
   r = data['r']
 
   data['B'] = g + 0.3130*(g-r) + 0.2271
   data['V'] = g - 0.5784*(g-r) - 0.0038
 
@@ -115,14 +115,14 @@
     return RGB
 
   data['RGB'] = data['temperature'].apply(Kelvin_to_RGB)
 
   RGB = data['RGB']
 
   x_axis = g-r
-  x_axis = x_axis.where(x_axis <= 40).where(x_axis >= -40)
+  x_axis = x_axis.where(x_axis <= right_bound).where(x_axis >= left_bound)
   y_axis = r
-  y_axis = y_axis.where(y_axis <= 40).where(x_axis >= -40)
+  y_axis = y_axis.where(y_axis <= upper_bound).where(y_axis >= lower_bound)
 
-  plt.figure(figsize=(12,6.75))
+  plt.figure(figsize=(x_scale,y_scale))
   plt.rcParams['axes.facecolor'] = '#252525'
   plt.scatter(x_axis, y_axis, s=0.05, marker='o', c=RGB)
```

### Comparing `StarClusterPlot-0.1.1/StarClusterPlot.egg-info/PKG-INFO` & `StarClusterPlot-0.1.2/StarClusterPlot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StarClusterPlot
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for visualizing star clusters and their Hertzsprung-Russell diagrams
 Home-page: UNKNOWN
 Author: Teerat Chanromyen
 Author-email: teerat.nahm@gmail.com
 License: MIT
 Keywords: Astronomy
 Platform: UNKNOWN
@@ -15,19 +15,24 @@
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
 License-File: LICENCE.txt
 
 This is a Python library for visualizing star clusters and their Hertzsprung-Russell diagrams. 
 All stars colors shown in this program are derived from their calculated temperatures.
 The package includes two functions: ClusterVis() and HRDiagram(). 
-The former takes one dataframe as a required input along withÂ two optional parameters to set the x and y scale of the plot. The latter simply requires one dataframe input. 
+The former takes one dataframe as a required input along with two optional parameters to set the x and y scale of the plot. The latter simply requires one dataframe input. 
 
 Change Log
 ==========
 
-0.1.0 (2/08/2023)
+0.1.2 (3/08/2023)
 -----------------
-Initial Release
+- Add six optional parameters for the HRDiagram function
 
 0.1.1 (3/08/2023)
 -----------------
+- Fix the out-of-bound RGB value error
+
+0.1.0 (2/08/2023)
+-----------------
+- Initial Release
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `StarClusterPlot-0.1.1/setup.py` & `StarClusterPlot-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='StarClusterPlot',
-    version='0.1.1',
+    version='0.1.2',
     description='Python package for visualizing star clusters and their Hertzsprung-Russell diagrams',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Teerat Chanromyen',
     author_email='teerat.nahm@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

