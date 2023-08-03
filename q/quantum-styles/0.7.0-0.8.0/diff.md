# Comparing `tmp/quantum-styles-0.7.0.tar.gz` & `tmp/quantum-styles-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/quantum-styles-0.7.0.tar", last modified: Fri Feb 17 20:00:24 2023, max compression
+gzip compressed data, was "quantum-styles-0.8.0.tar", last modified: Thu Aug  3 15:48:45 2023, max compression
```

## Comparing `quantum-styles-0.7.0.tar` & `quantum-styles-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-02-17 20:00:24.000000 quantum-styles-0.7.0/
--rw-r--r--   0 paul       (501) staff       (20)       90 2022-10-25 00:55:38.000000 quantum-styles-0.7.0/MANIFEST.in
--rw-r--r--   0 paul       (501) staff       (20)      735 2023-02-17 20:00:24.000000 quantum-styles-0.7.0/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)       38 2022-10-24 18:24:45.000000 quantum-styles-0.7.0/README.md
--rw-r--r--   0 paul       (501) staff       (20)       76 2022-11-03 20:37:19.000000 quantum-styles-0.7.0/pyproject.toml
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-02-17 20:00:24.000000 quantum-styles-0.7.0/quantum_styles.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)      735 2023-02-17 20:00:23.000000 quantum-styles-0.7.0/quantum_styles.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      559 2023-02-17 20:00:23.000000 quantum-styles-0.7.0/quantum_styles.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-02-17 20:00:23.000000 quantum-styles-0.7.0/quantum_styles.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-02-17 20:00:23.000000 quantum-styles-0.7.0/quantum_styles.egg-info/not-zip-safe
--rw-r--r--   0 paul       (501) staff       (20)       16 2023-02-17 20:00:23.000000 quantum-styles-0.7.0/quantum_styles.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-02-17 20:00:23.000000 quantum-styles-0.7.0/quantum_styles.egg-info/top_level.txt
--rw-r--r--   0 paul       (501) staff       (20)       16 2022-10-24 18:43:06.000000 quantum-styles-0.7.0/requirements.txt
--rw-r--r--   0 paul       (501) staff       (20)       38 2023-02-17 20:00:24.000000 quantum-styles-0.7.0/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)     3274 2023-02-17 19:38:34.000000 quantum-styles-0.7.0/setup.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-02-17 20:00:24.000000 quantum-styles-0.7.0/styles/
--rw-r--r--   0 paul       (501) staff       (20)     6148 2023-02-17 19:38:22.000000 quantum-styles-0.7.0/styles/.DS_Store
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-02-17 20:00:24.000000 quantum-styles-0.7.0/styles/mpl_styles/
--rw-r--r--   0 paul       (501) staff       (20)     6148 2022-10-24 18:03:57.000000 quantum-styles-0.7.0/styles/mpl_styles/.DS_Store
--rw-r--r--   0 paul       (501) staff       (20)     1190 2023-02-17 19:38:01.000000 quantum-styles-0.7.0/styles/mpl_styles/quantum-dark.mplstyle
--rw-r--r--   0 paul       (501) staff       (20)     1171 2023-02-17 19:38:14.000000 quantum-styles-0.7.0/styles/mpl_styles/quantum-light.mplstyle
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-02-17 20:00:24.000000 quantum-styles-0.7.0/styles/qiskit_styles/
--rw-r--r--   0 paul       (501) staff       (20)     6148 2022-10-24 18:03:57.000000 quantum-styles-0.7.0/styles/qiskit_styles/.DS_Store
--rw-r--r--   0 paul       (501) staff       (20)     3879 2022-10-25 00:51:00.000000 quantum-styles-0.7.0/styles/qiskit_styles/quantum-dark.json
--rw-r--r--   0 paul       (501) staff       (20)     3874 2022-09-07 22:25:03.000000 quantum-styles-0.7.0/styles/qiskit_styles/quantum-light.json
--rw-r--r--   0 paul       (501) staff       (20)       79 2022-10-26 13:51:40.000000 quantum-styles-0.7.0/styles/qiskit_styles/settings.conf
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 15:48:45.904211 quantum-styles-0.8.0/
+-rw-r--r--   0 paul       (501) staff       (20)    11357 2023-06-20 19:27:17.000000 quantum-styles-0.8.0/LICENSE
+-rw-r--r--   0 paul       (501) staff       (20)       90 2023-06-20 19:27:17.000000 quantum-styles-0.8.0/MANIFEST.in
+-rw-r--r--   0 paul       (501) staff       (20)      711 2023-08-03 15:48:45.904040 quantum-styles-0.8.0/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-06-20 19:27:17.000000 quantum-styles-0.8.0/README.md
+-rw-r--r--   0 paul       (501) staff       (20)       76 2023-06-20 19:27:17.000000 quantum-styles-0.8.0/pyproject.toml
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 15:48:45.902264 quantum-styles-0.8.0/quantum_styles.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)      711 2023-08-03 15:48:45.000000 quantum-styles-0.8.0/quantum_styles.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      508 2023-08-03 15:48:45.000000 quantum-styles-0.8.0/quantum_styles.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-08-03 15:48:45.000000 quantum-styles-0.8.0/quantum_styles.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-08-03 15:48:45.000000 quantum-styles-0.8.0/quantum_styles.egg-info/not-zip-safe
+-rw-r--r--   0 paul       (501) staff       (20)       16 2023-08-03 15:48:45.000000 quantum-styles-0.8.0/quantum_styles.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)        7 2023-08-03 15:48:45.000000 quantum-styles-0.8.0/quantum_styles.egg-info/top_level.txt
+-rw-r--r--   0 paul       (501) staff       (20)       16 2023-06-20 19:27:17.000000 quantum-styles-0.8.0/requirements.txt
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-08-03 15:48:45.904265 quantum-styles-0.8.0/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)     3274 2023-08-03 15:47:18.000000 quantum-styles-0.8.0/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 15:48:45.902465 quantum-styles-0.8.0/styles/
+-rw-r--r--   0 paul       (501) staff       (20)     6148 2023-08-03 15:35:48.000000 quantum-styles-0.8.0/styles/.DS_Store
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 15:48:45.903017 quantum-styles-0.8.0/styles/mpl_styles/
+-rw-r--r--   0 paul       (501) staff       (20)     1173 2023-08-03 15:46:52.000000 quantum-styles-0.8.0/styles/mpl_styles/quantum-dark.mplstyle
+-rw-r--r--   0 paul       (501) staff       (20)     1155 2023-08-03 15:46:52.000000 quantum-styles-0.8.0/styles/mpl_styles/quantum-light.mplstyle
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-03 15:48:45.903622 quantum-styles-0.8.0/styles/qiskit_styles/
+-rw-r--r--   0 paul       (501) staff       (20)     4027 2023-08-03 15:46:52.000000 quantum-styles-0.8.0/styles/qiskit_styles/quantum-dark.json
+-rw-r--r--   0 paul       (501) staff       (20)     4022 2023-08-03 15:46:52.000000 quantum-styles-0.8.0/styles/qiskit_styles/quantum-light.json
+-rw-r--r--   0 paul       (501) staff       (20)       79 2023-06-20 19:27:17.000000 quantum-styles-0.8.0/styles/qiskit_styles/settings.conf
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `quantum-styles-0.7.0/PKG-INFO` & `quantum-styles-0.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: quantum-styles
-Version: 0.7.0
+Version: 0.8.0
 Summary: Quantum-styles
-Home-page: UNKNOWN
+Home-page: 
 Author: Paul Nation
 Author-email: paul.nation@ibm.com
 License: Apache 2.0
-Description: Quantum styles for Matplotlib
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
+License-File: LICENSE
+
+Quantum styles for Matplotlib
```

### Comparing `quantum-styles-0.7.0/quantum_styles.egg-info/PKG-INFO` & `quantum-styles-0.8.0/quantum_styles.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: quantum-styles
-Version: 0.7.0
+Version: 0.8.0
 Summary: Quantum-styles
-Home-page: UNKNOWN
+Home-page: 
 Author: Paul Nation
 Author-email: paul.nation@ibm.com
 License: Apache 2.0
-Description: Quantum styles for Matplotlib
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
+License-File: LICENSE
+
+Quantum styles for Matplotlib
```

### Comparing `quantum-styles-0.7.0/setup.py` & `quantum-styles-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import matplotlib
 
 from setuptools import setup
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 
 MAJOR = 0
-MINOR = 7
+MINOR = 8
 MICRO = 0
 
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 REQUIREMENTS = ['matplotlib>=3.3',
                ]
```

### Comparing `quantum-styles-0.7.0/styles/mpl_styles/quantum-dark.mplstyle` & `quantum-styles-0.8.0/styles/mpl_styles/quantum-dark.mplstyle`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 ytick.color: white
 
 figure.subplot.left: 0.08
 figure.subplot.right: 0.95
 figure.subplot.bottom: 0.07
 figure.facecolor: 161616
 figure.figsize: 8, 6
-figure.dpi: 300 
 
 ### Boxplots
 boxplot.boxprops.color: white
 boxplot.capprops.color: white
 boxplot.flierprops.color: white
 boxplot.flierprops.markeredgecolor: white
 boxplot.whiskerprops.color: white
```

### Comparing `quantum-styles-0.7.0/styles/mpl_styles/quantum-light.mplstyle` & `quantum-styles-0.8.0/styles/mpl_styles/quantum-light.mplstyle`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 ytick.color: black
 
 figure.subplot.left: 0.08
 figure.subplot.right: 0.95
 figure.subplot.bottom: 0.07
 figure.facecolor: f2f0ed
 figure.figsize: 8, 6
-figure.dpi: 300
 
 ### Boxplots
 boxplot.boxprops.color: black
 boxplot.capprops.color: black
 boxplot.flierprops.color: black
 boxplot.flierprops.markeredgecolor: black
 boxplot.whiskerprops.color: black
```

### Comparing `quantum-styles-0.7.0/styles/qiskit_styles/quantum-dark.json` & `quantum-styles-0.8.0/styles/qiskit_styles/quantum-dark.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987163029525032%*

 * *Differences: {"'displaycolor'": "{'ecr': ['#f4a67a', '#000000'], 'delay': ['#FFFFFF', '#000000']}"}*

```diff
@@ -36,14 +36,22 @@
             "#0099e6",
             "#FFFFFF"
         ],
         "dcx": [
             "#f4a67a",
             "#FFFFFF"
         ],
+        "delay": [
+            "#FFFFFF",
+            "#000000"
+        ],
+        "ecr": [
+            "#f4a67a",
+            "#000000"
+        ],
         "h": [
             "#925cdd",
             "#FFFFFF"
         ],
         "id": [
             "#f4a67a",
             "#000000"
```

### Comparing `quantum-styles-0.7.0/styles/qiskit_styles/quantum-light.json` & `quantum-styles-0.8.0/styles/qiskit_styles/quantum-light.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987163029525032%*

 * *Differences: {"'displaycolor'": "{'ecr': ['#EE7733', '#FFFFFF'], 'delay': ['#000000', '#FFFFFF']}"}*

```diff
@@ -36,14 +36,22 @@
             "#0075C3",
             "#FFFFFF"
         ],
         "dcx": [
             "#EE7733",
             "#FFFFFF"
         ],
+        "delay": [
+            "#000000",
+            "#FFFFFF"
+        ],
+        "ecr": [
+            "#EE7733",
+            "#FFFFFF"
+        ],
         "h": [
             "#925cdd",
             "#FFFFFF"
         ],
         "id": [
             "#EE7733",
             "#ffffff"
```

