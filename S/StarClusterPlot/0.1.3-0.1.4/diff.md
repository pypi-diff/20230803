# Comparing `tmp/StarClusterPlot-0.1.3.tar.gz` & `tmp/StarClusterPlot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StarClusterPlot-0.1.3.tar", last modified: Thu Aug  3 04:12:01 2023, max compression
+gzip compressed data, was "StarClusterPlot-0.1.4.tar", last modified: Thu Aug  3 04:28:40 2023, max compression
```

## Comparing `StarClusterPlot-0.1.3.tar` & `StarClusterPlot-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 04:12:01.135468 StarClusterPlot-0.1.3/
--rw-rw-rw-   0        0        0      329 2023-08-03 04:11:45.000000 StarClusterPlot-0.1.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.3/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1173 2023-08-03 04:12:01.134466 StarClusterPlot-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-08-03 04:10:17.000000 StarClusterPlot-0.1.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 04:12:01.096108 StarClusterPlot-0.1.3/StarClusterPlot/
--rw-rw-rw-   0        0        0     4064 2023-08-03 04:08:38.000000 StarClusterPlot-0.1.3/StarClusterPlot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 04:12:01.132441 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/
--rw-rw-rw-   0        0        0     1173 2023-08-03 04:12:00.000000 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-03 04:12:00.000000 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 04:12:00.000000 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-08-03 04:12:00.000000 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-03 04:12:00.000000 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 04:12:01.135468 StarClusterPlot-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-08-03 04:11:05.000000 StarClusterPlot-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 04:28:40.061937 StarClusterPlot-0.1.4/
+-rw-rw-rw-   0        0        0      399 2023-08-03 04:26:54.000000 StarClusterPlot-0.1.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1271 2023-08-03 04:28:40.061937 StarClusterPlot-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-08-03 04:10:17.000000 StarClusterPlot-0.1.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 04:28:40.044476 StarClusterPlot-0.1.4/StarClusterPlot/
+-rw-rw-rw-   0        0        0     4062 2023-08-03 04:27:25.000000 StarClusterPlot-0.1.4/StarClusterPlot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 04:28:40.060939 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/
+-rw-rw-rw-   0        0        0     1271 2023-08-03 04:28:40.000000 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-03 04:28:40.000000 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 04:28:40.000000 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 04:28:40.000000 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-03 04:28:40.000000 StarClusterPlot-0.1.4/StarClusterPlot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 04:28:40.061937 StarClusterPlot-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-08-03 04:27:10.000000 StarClusterPlot-0.1.4/setup.py
```

### Comparing `StarClusterPlot-0.1.3/LICENCE.txt` & `StarClusterPlot-0.1.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `StarClusterPlot-0.1.3/StarClusterPlot/__init__.py` & `StarClusterPlot-0.1.4/StarClusterPlot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
   plt.rcParams['axes.facecolor'] = '#252525'
   plt.scatter(RA,DEC, s=0.05, marker='o', c=RGB)
 
 
 
 
 
-def HRDiagram(data, left_bound = -40, right_bound = 40, lower_bound = -40, upper_bound = 40, x_scale = 12, y_scale = 6.75):
+def HRDiagram(data, left_bound = -3, right_bound = 4, lower_bound = -10, upper_bound = 25, x_scale = 12, y_scale = 6.75):
 
   g = data['g']
   r = data['r']
 
   data['B'] = g + 0.3130*(g-r) + 0.2271
   data['V'] = g - 0.5784*(g-r) - 0.0038
```

### Comparing `StarClusterPlot-0.1.3/setup.py` & `StarClusterPlot-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='StarClusterPlot',
-    version='0.1.3',
+    version='0.1.4',
     description='Python package for visualizing star clusters and their Hertzsprung-Russell diagrams',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Teerat Chanromyen',
     author_email='teerat.nahm@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

