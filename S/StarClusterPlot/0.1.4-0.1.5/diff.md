# Comparing `tmp/StarClusterPlot-0.1.4.tar.gz` & `tmp/StarClusterPlot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StarClusterPlot-0.1.4.tar", last modified: Thu Aug  3 04:28:40 2023, max compression
+gzip compressed data, was "StarClusterPlot-0.1.5.tar", last modified: Thu Aug  3 07:00:28 2023, max compression
```

## Comparing `StarClusterPlot-0.1.4.tar` & `StarClusterPlot-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 04:28:40.061937 StarClusterPlot-0.1.4/
--rw-rw-rw-   0        0        0      399 2023-08-03 04:26:54.000000 StarClusterPlot-0.1.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.4/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1271 2023-08-03 04:28:40.061937 StarClusterPlot-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-08-03 04:10:17.000000 StarClusterPlot-0.1.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 04:28:40.044476 StarClusterPlot-0.1.4/StarClusterPlot/
--rw-rw-rw-   0        0        0     4062 2023-08-03 04:27:25.000000 StarClusterPlot-0.1.4/StarClusterPlot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 04:28:40.060939 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/
--rw-rw-rw-   0        0        0     1271 2023-08-03 04:28:40.000000 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-03 04:28:40.000000 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 04:28:40.000000 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-08-03 04:28:40.000000 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-03 04:28:40.000000 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 04:28:40.061937 StarClusterPlot-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-08-03 04:27:10.000000 StarClusterPlot-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:00:28.665394 StarClusterPlot-0.1.5/
+-rw-rw-rw-   0        0        0      492 2023-08-03 06:55:54.000000 StarClusterPlot-0.1.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.5/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1364 2023-08-03 07:00:28.664390 StarClusterPlot-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-08-03 04:10:17.000000 StarClusterPlot-0.1.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 07:00:28.635197 StarClusterPlot-0.1.5/StarClusterPlot/
+-rw-rw-rw-   0        0        0     4125 2023-08-03 06:59:35.000000 StarClusterPlot-0.1.5/StarClusterPlot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:00:28.663396 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/
+-rw-rw-rw-   0        0        0     1364 2023-08-03 07:00:28.000000 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-03 07:00:28.000000 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:00:28.000000 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 07:00:28.000000 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-03 07:00:28.000000 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:00:28.665394 StarClusterPlot-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-08-03 06:56:31.000000 StarClusterPlot-0.1.5/setup.py
```

### Comparing `StarClusterPlot-0.1.4/LICENCE.txt` & `StarClusterPlot-0.1.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `StarClusterPlot-0.1.4/PKG-INFO` & `StarClusterPlot-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StarClusterPlot
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package for visualizing star clusters and their Hertzsprung-Russell diagrams
 Home-page: UNKNOWN
 Author: Teerat Chanromyen
 Author-email: teerat.nahm@gmail.com
 License: MIT
 Keywords: Astronomy
 Platform: UNKNOWN
@@ -19,21 +19,25 @@
 This is a Python library for visualizing star clusters and their Hertzsprung-Russell diagrams. 
 All stars colors shown in this program are derived from their calculated temperatures.
 The package includes two functions: ClusterVis() and HRDiagram().
 
 Change Log
 ==========
 
+0.1.5 (3/08/2023)
+-----------------
+- Change plotting method to subplots, Return figure
+
 0.1.4 (3/08/2023)
 -----------------
-- update optional parameters
+- Update optional parameters
 
 0.1.3 (3/08/2023)
 -----------------
-- update optional parameters
+- Update optional parameters
 
 0.1.2 (3/08/2023)
 -----------------
 - Add six optional parameters for the HRDiagram function
 
 0.1.1 (2/08/2023)
 -----------------
```

### Comparing `StarClusterPlot-0.1.4/StarClusterPlot/__init__.py` & `StarClusterPlot-0.1.5/StarClusterPlot/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,17 +52,21 @@
     RGB = XYZ_to_RGB(XYZ[0], XYZ[1], XYZ[2])
     return RGB
 
   data['RGB'] = data['temperature'].apply(Kelvin_to_RGB)
 
   RGB = data['RGB']
 
-  plt.figure(figsize=(x_scale, y_scale))
-  plt.rcParams['axes.facecolor'] = '#252525'
-  plt.scatter(RA,DEC, s=0.05, marker='o', c=RGB)
+  fig, ax = plt.subplots(figsize=(x_scale, y_scale))
+  ax.set_facecolor('#252525')
+  ax.scatter(RA,DEC, s=0.05, marker='o', c=RGB)
+
+  plt.show(fig)
+
+  return fig
 
 
 
 
 
 def HRDiagram(data, left_bound = -3, right_bound = 4, lower_bound = -10, upper_bound = 25, x_scale = 12, y_scale = 6.75):
 
@@ -119,10 +123,14 @@
   RGB = data['RGB']
 
   x_axis = g-r
   x_axis = x_axis.where(x_axis <= right_bound).where(x_axis >= left_bound)
   y_axis = r
   y_axis = y_axis.where(y_axis <= upper_bound).where(y_axis >= lower_bound)
 
-  plt.figure(figsize=(x_scale,y_scale))
-  plt.rcParams['axes.facecolor'] = '#252525'
-  plt.scatter(x_axis, y_axis, s=0.05, marker='o', c=RGB)
+  fig, ax = plt.subplots(figsize=(x_scale, y_scale))
+  ax.set_facecolor('#252525')
+  ax.scatter(x_axis, y_axis, s=0.05, marker='o', c=RGB)
+
+  plt.show(fig)
+
+  return fig
```

### Comparing `StarClusterPlot-0.1.4/StarClusterPlot.egg-info/PKG-INFO` & `StarClusterPlot-0.1.5/StarClusterPlot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StarClusterPlot
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package for visualizing star clusters and their Hertzsprung-Russell diagrams
 Home-page: UNKNOWN
 Author: Teerat Chanromyen
 Author-email: teerat.nahm@gmail.com
 License: MIT
 Keywords: Astronomy
 Platform: UNKNOWN
@@ -19,21 +19,25 @@
 This is a Python library for visualizing star clusters and their Hertzsprung-Russell diagrams. 
 All stars colors shown in this program are derived from their calculated temperatures.
 The package includes two functions: ClusterVis() and HRDiagram().
 
 Change Log
 ==========
 
+0.1.5 (3/08/2023)
+-----------------
+- Change plotting method to subplots, Return figure
+
 0.1.4 (3/08/2023)
 -----------------
-- update optional parameters
+- Update optional parameters
 
 0.1.3 (3/08/2023)
 -----------------
-- update optional parameters
+- Update optional parameters
 
 0.1.2 (3/08/2023)
 -----------------
 - Add six optional parameters for the HRDiagram function
 
 0.1.1 (2/08/2023)
 -----------------
```

### Comparing `StarClusterPlot-0.1.4/setup.py` & `StarClusterPlot-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='StarClusterPlot',
-    version='0.1.4',
+    version='0.1.5',
     description='Python package for visualizing star clusters and their Hertzsprung-Russell diagrams',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Teerat Chanromyen',
     author_email='teerat.nahm@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

