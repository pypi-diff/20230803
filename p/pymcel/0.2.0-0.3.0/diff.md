# Comparing `tmp/pymcel-0.2.0.tar.gz` & `tmp/pymcel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymcel-0.2.0.tar", last modified: Thu Mar 23 14:08:22 2023, max compression
+gzip compressed data, was "pymcel-0.3.0.tar", last modified: Thu Aug  3 16:06:46 2023, max compression
```

## Comparing `pymcel-0.2.0.tar` & `pymcel-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-03-23 14:08:22.877369 pymcel-0.2.0/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1073 2023-02-08 18:16:21.000000 pymcel-0.2.0/LICENSE
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2236 2023-03-23 14:08:22.877245 pymcel-0.2.0/PKG-INFO
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1781 2023-02-08 18:20:22.000000 pymcel-0.2.0/README.md
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1269 2023-03-17 13:15:03.000000 pymcel-0.2.0/pyproject.toml
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       38 2023-03-23 14:08:22.877407 pymcel-0.2.0/setup.cfg
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     3361 2023-03-23 14:08:09.000000 pymcel-0.2.0/setup.py
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-03-23 14:08:22.874631 pymcel-0.2.0/src/
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-03-23 14:08:22.876060 pymcel-0.2.0/src/pymcel/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)    42023 2023-03-17 13:12:21.000000 pymcel-0.2.0/src/pymcel/__init__.py
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-03-23 14:08:22.876938 pymcel-0.2.0/src/pymcel/data/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      526 2023-02-08 19:46:43.000000 pymcel-0.2.0/src/pymcel/data/kernels
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       16 2023-03-23 14:08:09.000000 pymcel-0.2.0/src/pymcel/version.py
-drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-03-23 14:08:22.876810 pymcel-0.2.0/src/pymcel.egg-info/
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2236 2023-03-23 14:08:22.000000 pymcel-0.2.0/src/pymcel.egg-info/PKG-INFO
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      316 2023-03-23 14:08:22.000000 pymcel-0.2.0/src/pymcel.egg-info/SOURCES.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        1 2023-03-23 14:08:22.000000 pymcel-0.2.0/src/pymcel.egg-info/dependency_links.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       48 2023-03-23 14:08:22.000000 pymcel-0.2.0/src/pymcel.egg-info/entry_points.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       50 2023-03-23 14:08:22.000000 pymcel-0.2.0/src/pymcel.egg-info/requires.txt
--rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        7 2023-03-23 14:08:22.000000 pymcel-0.2.0/src/pymcel.egg-info/top_level.txt
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-08-03 16:06:46.346047 pymcel-0.3.0/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1073 2023-02-08 18:16:21.000000 pymcel-0.3.0/LICENSE
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2236 2023-08-03 16:06:46.345921 pymcel-0.3.0/PKG-INFO
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1781 2023-02-08 18:20:22.000000 pymcel-0.3.0/README.md
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     1269 2023-03-17 13:15:03.000000 pymcel-0.3.0/pyproject.toml
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       38 2023-08-03 16:06:46.346085 pymcel-0.3.0/setup.cfg
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     3361 2023-08-03 16:06:33.000000 pymcel-0.3.0/setup.py
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-08-03 16:06:46.340626 pymcel-0.3.0/src/
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-08-03 16:06:46.343659 pymcel-0.3.0/src/pymcel/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)    42023 2023-03-17 13:12:21.000000 pymcel-0.3.0/src/pymcel/__init__.py
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-08-03 16:06:46.345598 pymcel-0.3.0/src/pymcel/data/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      526 2023-02-08 19:46:43.000000 pymcel-0.3.0/src/pymcel/data/kernels
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       16 2023-08-03 16:06:33.000000 pymcel-0.3.0/src/pymcel/version.py
+drwxr-xr-x   0 jorgezuluagacallejas   (501) staff       (20)        0 2023-08-03 16:06:46.345445 pymcel-0.3.0/src/pymcel.egg-info/
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)     2236 2023-08-03 16:06:46.000000 pymcel-0.3.0/src/pymcel.egg-info/PKG-INFO
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)      316 2023-08-03 16:06:46.000000 pymcel-0.3.0/src/pymcel.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        1 2023-08-03 16:06:46.000000 pymcel-0.3.0/src/pymcel.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       48 2023-08-03 16:06:46.000000 pymcel-0.3.0/src/pymcel.egg-info/entry_points.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)       50 2023-08-03 16:06:46.000000 pymcel-0.3.0/src/pymcel.egg-info/requires.txt
+-rw-r--r--   0 jorgezuluagacallejas   (501) staff       (20)        7 2023-08-03 16:06:46.000000 pymcel-0.3.0/src/pymcel.egg-info/top_level.txt
```

### Comparing `pymcel-0.2.0/LICENSE` & `pymcel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymcel-0.2.0/PKG-INFO` & `pymcel-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcel
-Version: 0.2.0
+Version: 0.3.0
 Summary: Utilidades de Mecánica Celeste
 Home-page: https://pypi.org/project/pymcel
 Author: Jorge I. Zuluaga
 Author-email: jorge.zuluaga@udea.edu.co
 License: MIT
 Keywords: astronomy astrodynamics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymcel-0.2.0/README.md` & `pymcel-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pymcel-0.2.0/pyproject.toml` & `pymcel-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymcel-0.2.0/setup.py` & `pymcel-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         ],
-    version='0.2.0',
+    version='0.3.0',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `pymcel-0.2.0/src/pymcel/__init__.py` & `pymcel-0.3.0/src/pymcel/__init__.py`

 * *Files identical despite different names*

### Comparing `pymcel-0.2.0/src/pymcel/data/kernels` & `pymcel-0.3.0/src/pymcel/data/kernels`

 * *Files identical despite different names*

### Comparing `pymcel-0.2.0/src/pymcel.egg-info/PKG-INFO` & `pymcel-0.3.0/src/pymcel.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymcel
-Version: 0.2.0
+Version: 0.3.0
 Summary: Utilidades de Mecánica Celeste
 Home-page: https://pypi.org/project/pymcel
 Author: Jorge I. Zuluaga
 Author-email: jorge.zuluaga@udea.edu.co
 License: MIT
 Keywords: astronomy astrodynamics
 Classifier: Programming Language :: Python :: 3
```

