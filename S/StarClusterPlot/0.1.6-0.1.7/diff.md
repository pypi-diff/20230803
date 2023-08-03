# Comparing `tmp/StarClusterPlot-0.1.6.tar.gz` & `tmp/StarClusterPlot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StarClusterPlot-0.1.6.tar", last modified: Thu Aug  3 07:11:57 2023, max compression
+gzip compressed data, was "StarClusterPlot-0.1.7.tar", last modified: Thu Aug  3 07:37:31 2023, max compression
```

## Comparing `StarClusterPlot-0.1.6.tar` & `StarClusterPlot-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:11:57.284500 StarClusterPlot-0.1.6/
--rw-rw-rw-   0        0        0      572 2023-08-03 07:11:10.000000 StarClusterPlot-0.1.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.6/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1416 2023-08-03 07:11:57.283498 StarClusterPlot-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-08-03 04:10:17.000000 StarClusterPlot-0.1.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 07:11:57.261498 StarClusterPlot-0.1.6/StarClusterPlot/
--rw-rw-rw-   0        0        0     4085 2023-08-03 07:10:32.000000 StarClusterPlot-0.1.6/StarClusterPlot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:11:57.282500 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/
--rw-rw-rw-   0        0        0     1416 2023-08-03 07:11:57.000000 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-03 07:11:57.000000 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:11:57.000000 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-08-03 07:11:57.000000 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-03 07:11:57.000000 StarClusterPlot-0.1.6/StarClusterPlot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 07:11:57.284500 StarClusterPlot-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-08-03 07:11:20.000000 StarClusterPlot-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:37:31.137177 StarClusterPlot-0.1.7/
+-rw-rw-rw-   0        0        0      652 2023-08-03 07:36:34.000000 StarClusterPlot-0.1.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1524 2023-08-03 07:37:31.136167 StarClusterPlot-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-08-03 04:10:17.000000 StarClusterPlot-0.1.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 07:37:31.107166 StarClusterPlot-0.1.7/StarClusterPlot/
+-rw-rw-rw-   0        0        0     4087 2023-08-03 07:36:57.000000 StarClusterPlot-0.1.7/StarClusterPlot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:37:31.134169 StarClusterPlot-0.1.7/StarClusterPlot.egg-info/
+-rw-rw-rw-   0        0        0     1524 2023-08-03 07:37:31.000000 StarClusterPlot-0.1.7/StarClusterPlot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-03 07:37:31.000000 StarClusterPlot-0.1.7/StarClusterPlot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:37:31.000000 StarClusterPlot-0.1.7/StarClusterPlot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 07:37:31.000000 StarClusterPlot-0.1.7/StarClusterPlot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-03 07:37:31.000000 StarClusterPlot-0.1.7/StarClusterPlot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:37:31.137177 StarClusterPlot-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-08-03 07:36:00.000000 StarClusterPlot-0.1.7/setup.py
```

### Comparing `StarClusterPlot-0.1.6/LICENCE.txt` & `StarClusterPlot-0.1.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `StarClusterPlot-0.1.6/PKG-INFO` & `StarClusterPlot-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: StarClusterPlot
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for visualizing star clusters and their Hertzsprung-Russell diagrams
-Home-page: 
+Home-page: UNKNOWN
 Author: Teerat Chanromyen
 Author-email: teerat.nahm@gmail.com
 License: MIT
 Keywords: Astronomy
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
 License-File: LICENCE.txt
@@ -18,14 +19,18 @@
 This is a Python library for visualizing star clusters and their Hertzsprung-Russell diagrams. 
 All stars colors shown in this program are derived from their calculated temperatures.
 The package includes two functions: ClusterVis() and HRDiagram().
 
 Change Log
 ==========
 
+0.1.7 (3/08/2023)
+-----------------
+- Dedicated version for Streamlit plot
+
 0.1.6 (3/08/2023)
 -----------------
 - Edit return value for Streamlit plot
 
 0.1.5 (3/08/2023)
 -----------------
 - Change plotting method to subplots, Return figure
@@ -45,7 +50,8 @@
 0.1.1 (2/08/2023)
 -----------------
 - Fix the out-of-bound RGB value error
 
 0.1.0 (2/08/2023)
 -----------------
 - Initial Release
+
```

### Comparing `StarClusterPlot-0.1.6/StarClusterPlot/__init__.py` & `StarClusterPlot-0.1.7/StarClusterPlot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
   RGB = data['RGB']
 
   fig, ax = plt.subplots(figsize=(x_scale, y_scale))
   ax.set_facecolor('#252525')
   ax.scatter(RA,DEC, s=0.05, marker='o', c=RGB)
 
-  return ax
+  return fig
 
 
 
 
 
 def HRDiagram(data, left_bound = -3, right_bound = 4, lower_bound = -10, upper_bound = 25, x_scale = 12, y_scale = 6.75):
 
@@ -125,8 +125,8 @@
   y_axis = r
   y_axis = y_axis.where(y_axis <= upper_bound).where(y_axis >= lower_bound)
 
   fig, ax = plt.subplots(figsize=(x_scale, y_scale))
   ax.set_facecolor('#252525')
   ax.scatter(x_axis, y_axis, s=0.05, marker='o', c=RGB)
 
-  return ax
+  return fig
```

### Comparing `StarClusterPlot-0.1.6/StarClusterPlot.egg-info/PKG-INFO` & `StarClusterPlot-0.1.7/StarClusterPlot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: StarClusterPlot
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for visualizing star clusters and their Hertzsprung-Russell diagrams
-Home-page: 
+Home-page: UNKNOWN
 Author: Teerat Chanromyen
 Author-email: teerat.nahm@gmail.com
 License: MIT
 Keywords: Astronomy
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
 License-File: LICENCE.txt
@@ -18,14 +19,18 @@
 This is a Python library for visualizing star clusters and their Hertzsprung-Russell diagrams. 
 All stars colors shown in this program are derived from their calculated temperatures.
 The package includes two functions: ClusterVis() and HRDiagram().
 
 Change Log
 ==========
 
+0.1.7 (3/08/2023)
+-----------------
+- Dedicated version for Streamlit plot
+
 0.1.6 (3/08/2023)
 -----------------
 - Edit return value for Streamlit plot
 
 0.1.5 (3/08/2023)
 -----------------
 - Change plotting method to subplots, Return figure
@@ -45,7 +50,8 @@
 0.1.1 (2/08/2023)
 -----------------
 - Fix the out-of-bound RGB value error
 
 0.1.0 (2/08/2023)
 -----------------
 - Initial Release
+
```

### Comparing `StarClusterPlot-0.1.6/setup.py` & `StarClusterPlot-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='StarClusterPlot',
-    version='0.1.6',
+    version='0.1.7',
     description='Python package for visualizing star clusters and their Hertzsprung-Russell diagrams',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Teerat Chanromyen',
     author_email='teerat.nahm@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

