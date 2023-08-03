# Comparing `tmp/StarClusterPlot-0.1.2.tar.gz` & `tmp/StarClusterPlot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StarClusterPlot-0.1.2.tar", last modified: Thu Aug  3 04:01:30 2023, max compression
+gzip compressed data, was "StarClusterPlot-0.1.3.tar", last modified: Thu Aug  3 04:12:01 2023, max compression
```

## Comparing `StarClusterPlot-0.1.2.tar` & `StarClusterPlot-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 04:01:30.804077 StarClusterPlot-0.1.2/
--rw-rw-rw-   0        0        0      259 2023-08-03 04:00:37.000000 StarClusterPlot-0.1.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1306 2023-08-03 04:01:30.804077 StarClusterPlot-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-08-03 03:51:38.000000 StarClusterPlot-0.1.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 04:01:30.765823 StarClusterPlot-0.1.2/StarClusterPlot/
--rw-rw-rw-   0        0        0     4064 2023-08-03 03:59:57.000000 StarClusterPlot-0.1.2/StarClusterPlot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 04:01:30.802179 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/
--rw-rw-rw-   0        0        0     1306 2023-08-03 04:01:30.000000 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-03 04:01:30.000000 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 04:01:30.000000 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-08-03 04:01:30.000000 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-03 04:01:30.000000 StarClusterPlot-0.1.2/StarClusterPlot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 04:01:30.805079 StarClusterPlot-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-08-03 03:51:51.000000 StarClusterPlot-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 04:12:01.135468 StarClusterPlot-0.1.3/
+-rw-rw-rw-   0        0        0      329 2023-08-03 04:11:45.000000 StarClusterPlot-0.1.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1070 2023-08-02 08:41:25.000000 StarClusterPlot-0.1.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-08-02 08:41:23.000000 StarClusterPlot-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1173 2023-08-03 04:12:01.134466 StarClusterPlot-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-08-03 04:10:17.000000 StarClusterPlot-0.1.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 04:12:01.096108 StarClusterPlot-0.1.3/StarClusterPlot/
+-rw-rw-rw-   0        0        0     4064 2023-08-03 04:08:38.000000 StarClusterPlot-0.1.3/StarClusterPlot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 04:12:01.132441 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/
+-rw-rw-rw-   0        0        0     1173 2023-08-03 04:12:00.000000 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-03 04:12:00.000000 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 04:12:00.000000 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-03 04:12:00.000000 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-03 04:12:00.000000 StarClusterPlot-0.1.3/StarClusterPlot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 04:12:01.135468 StarClusterPlot-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-08-03 04:11:05.000000 StarClusterPlot-0.1.3/setup.py
```

### Comparing `StarClusterPlot-0.1.2/LICENCE.txt` & `StarClusterPlot-0.1.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `StarClusterPlot-0.1.2/StarClusterPlot/__init__.py` & `StarClusterPlot-0.1.3/StarClusterPlot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
   plt.rcParams['axes.facecolor'] = '#252525'
   plt.scatter(RA,DEC, s=0.05, marker='o', c=RGB)
 
 
 
 
 
-def HRDiagram(data, left_bound = -40, right_bound = 40, lower_bound = -40, upper_bound = 40, x_scale = 6.75, y_scale = 12):
+def HRDiagram(data, left_bound = -40, right_bound = 40, lower_bound = -40, upper_bound = 40, x_scale = 12, y_scale = 6.75):
 
   g = data['g']
   r = data['r']
 
   data['B'] = g + 0.3130*(g-r) + 0.2271
   data['V'] = g - 0.5784*(g-r) - 0.0038
```

### Comparing `StarClusterPlot-0.1.2/setup.py` & `StarClusterPlot-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='StarClusterPlot',
-    version='0.1.2',
+    version='0.1.3',
     description='Python package for visualizing star clusters and their Hertzsprung-Russell diagrams',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Teerat Chanromyen',
     author_email='teerat.nahm@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

