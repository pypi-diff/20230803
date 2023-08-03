# Comparing `tmp/StarClusterPlot-0.1.5.tar.gz` & `tmp/StarClusterPlot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StarClusterPlot-0.1.5.tar", last modified: Thu Aug  3 07:00:28 2023, max compression
+gzip compressed data, was "StarClusterPlot-0.1.6.tar", last modified: Thu Aug  3 07:11:57 2023, max compression
```

## Comparing `StarClusterPlot-0.1.5.tar` & `StarClusterPlot-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:00:28.665394 StarClusterPlot-0.1.5/
--rw-rw-rw-   0        0        0      492 2023-08-03 06:55:54.000000 StarClusterPlot-0.1.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.5/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1364 2023-08-03 07:00:28.664390 StarClusterPlot-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-08-03 04:10:17.000000 StarClusterPlot-0.1.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 07:00:28.635197 StarClusterPlot-0.1.5/StarClusterPlot/
--rw-rw-rw-   0        0        0     4125 2023-08-03 06:59:35.000000 StarClusterPlot-0.1.5/StarClusterPlot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:00:28.663396 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/
--rw-rw-rw-   0        0        0     1364 2023-08-03 07:00:28.000000 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-03 07:00:28.000000 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:00:28.000000 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-08-03 07:00:28.000000 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-03 07:00:28.000000 StarClusterPlot-0.1.5/StarClusterPlot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 07:00:28.665394 StarClusterPlot-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-08-03 06:56:31.000000 StarClusterPlot-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:11:57.284500 StarClusterPlot-0.1.6/
+-rw-rw-rw-   0        0        0      572 2023-08-03 07:11:10.000000 StarClusterPlot-0.1.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1416 2023-08-03 07:11:57.283498 StarClusterPlot-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-08-03 04:10:17.000000 StarClusterPlot-0.1.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 07:11:57.261498 StarClusterPlot-0.1.6/StarClusterPlot/
+-rw-rw-rw-   0        0        0     4085 2023-08-03 07:10:32.000000 StarClusterPlot-0.1.6/StarClusterPlot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:11:57.282500 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/
+-rw-rw-rw-   0        0        0     1416 2023-08-03 07:11:57.000000 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-03 07:11:57.000000 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:11:57.000000 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 07:11:57.000000 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-03 07:11:57.000000 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:11:57.284500 StarClusterPlot-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-08-03 07:11:20.000000 StarClusterPlot-0.1.6/setup.py
```

### Comparing `StarClusterPlot-0.1.5/LICENCE.txt` & `StarClusterPlot-0.1.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `StarClusterPlot-0.1.5/PKG-INFO` & `StarClusterPlot-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: StarClusterPlot
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for visualizing star clusters and their Hertzsprung-Russell diagrams
-Home-page: UNKNOWN
+Home-page: 
 Author: Teerat Chanromyen
 Author-email: teerat.nahm@gmail.com
 License: MIT
 Keywords: Astronomy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
 License-File: LICENCE.txt
@@ -19,14 +18,18 @@
 This is a Python library for visualizing star clusters and their Hertzsprung-Russell diagrams. 
 All stars colors shown in this program are derived from their calculated temperatures.
 The package includes two functions: ClusterVis() and HRDiagram().
 
 Change Log
 ==========
 
+0.1.6 (3/08/2023)
+-----------------
+- Edit return value for Streamlit plot
+
 0.1.5 (3/08/2023)
 -----------------
 - Change plotting method to subplots, Return figure
 
 0.1.4 (3/08/2023)
 -----------------
 - Update optional parameters
@@ -42,8 +45,7 @@
 0.1.1 (2/08/2023)
 -----------------
 - Fix the out-of-bound RGB value error
 
 0.1.0 (2/08/2023)
 -----------------
 - Initial Release
-
```

### Comparing `StarClusterPlot-0.1.5/StarClusterPlot/__init__.py` & `StarClusterPlot-0.1.6/StarClusterPlot/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,17 +56,15 @@
 
   RGB = data['RGB']
 
   fig, ax = plt.subplots(figsize=(x_scale, y_scale))
   ax.set_facecolor('#252525')
   ax.scatter(RA,DEC, s=0.05, marker='o', c=RGB)
 
-  plt.show(fig)
-
-  return fig
+  return ax
 
 
 
 
 
 def HRDiagram(data, left_bound = -3, right_bound = 4, lower_bound = -10, upper_bound = 25, x_scale = 12, y_scale = 6.75):
 
@@ -127,10 +125,8 @@
   y_axis = r
   y_axis = y_axis.where(y_axis <= upper_bound).where(y_axis >= lower_bound)
 
   fig, ax = plt.subplots(figsize=(x_scale, y_scale))
   ax.set_facecolor('#252525')
   ax.scatter(x_axis, y_axis, s=0.05, marker='o', c=RGB)
 
-  plt.show(fig)
-
-  return fig
+  return ax
```

### Comparing `StarClusterPlot-0.1.5/StarClusterPlot.egg-info/PKG-INFO` & `StarClusterPlot-0.1.6/StarClusterPlot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: StarClusterPlot
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for visualizing star clusters and their Hertzsprung-Russell diagrams
-Home-page: UNKNOWN
+Home-page: 
 Author: Teerat Chanromyen
 Author-email: teerat.nahm@gmail.com
 License: MIT
 Keywords: Astronomy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
 License-File: LICENCE.txt
@@ -19,14 +18,18 @@
 This is a Python library for visualizing star clusters and their Hertzsprung-Russell diagrams. 
 All stars colors shown in this program are derived from their calculated temperatures.
 The package includes two functions: ClusterVis() and HRDiagram().
 
 Change Log
 ==========
 
+0.1.6 (3/08/2023)
+-----------------
+- Edit return value for Streamlit plot
+
 0.1.5 (3/08/2023)
 -----------------
 - Change plotting method to subplots, Return figure
 
 0.1.4 (3/08/2023)
 -----------------
 - Update optional parameters
@@ -42,8 +45,7 @@
 0.1.1 (2/08/2023)
 -----------------
 - Fix the out-of-bound RGB value error
 
 0.1.0 (2/08/2023)
 -----------------
 - Initial Release
-
```

### Comparing `StarClusterPlot-0.1.5/setup.py` & `StarClusterPlot-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='StarClusterPlot',
-    version='0.1.5',
+    version='0.1.6',
     description='Python package for visualizing star clusters and their Hertzsprung-Russell diagrams',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Teerat Chanromyen',
     author_email='teerat.nahm@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

