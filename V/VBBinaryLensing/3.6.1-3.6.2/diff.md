# Comparing `tmp/VBBinaryLensing-3.6.1.tar.gz` & `tmp/VBBinaryLensing-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VBBinaryLensing-3.6.1.tar", last modified: Wed Aug  2 23:15:32 2023, max compression
+gzip compressed data, was "VBBinaryLensing-3.6.2.tar", last modified: Wed Aug  2 23:57:39 2023, max compression
```

## Comparing `VBBinaryLensing-3.6.1.tar` & `VBBinaryLensing-3.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     7651 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/LICENSE
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       59 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/MANIFEST.in
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     6162 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/PKG-INFO
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     5143 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/README.md
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.060952 VBBinaryLensing-3.6.1/VBBinaryLensing/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       45 2023-08-02 23:09:57.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/__init__.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/VBBinaryLensing/data/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)   488032 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/data/ESPL.tbl
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       18 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/data/OB151212coords.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/data/__init__.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)   110290 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/data/satellite1.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)   112560 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/data/satellite2.txt
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/VBBinaryLensing/lib/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)   145042 2023-07-30 22:24:42.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    11092 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/lib/VBBinaryLensingLibrary.h
--rw-rw-r--   0 etienne   (1000) etienne   (1000)    30353 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/lib/python_bindings.cpp
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/VBBinaryLensing/tests/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1995 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/tests/test_all.py
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     7279 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.1/VBBinaryLensing/tests/test_magnification.py
-drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:15:32.064952 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     6162 2023-08-02 23:15:32.000000 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/PKG-INFO
--rw-rw-r--   0 etienne   (1000) etienne   (1000)      670 2023-08-02 23:15:32.000000 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/SOURCES.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2023-08-02 23:15:32.000000 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/dependency_links.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       28 2023-08-02 23:15:32.000000 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/requires.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)       45 2023-08-02 23:15:32.000000 VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/top_level.txt
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     1322 2023-08-02 23:09:57.000000 VBBinaryLensing-3.6.1/pyproject.toml
--rw-rw-r--   0 etienne   (1000) etienne   (1000)      875 2023-08-02 23:15:32.068952 VBBinaryLensing-3.6.1/setup.cfg
--rw-rw-r--   0 etienne   (1000) etienne   (1000)     2685 2023-08-02 23:09:57.000000 VBBinaryLensing-3.6.1/setup.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:57:39.708504 VBBinaryLensing-3.6.2/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     7651 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/LICENSE
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       59 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/MANIFEST.in
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     6162 2023-08-02 23:57:39.708504 VBBinaryLensing-3.6.2/PKG-INFO
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     5143 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/README.md
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:57:39.708504 VBBinaryLensing-3.6.2/VBBinaryLensing/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       45 2023-08-02 23:09:57.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/__init__.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:57:39.708504 VBBinaryLensing-3.6.2/VBBinaryLensing/data/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)   488032 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/data/ESPL.tbl
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       18 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/data/OB151212coords.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        0 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/data/__init__.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)   110290 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/data/satellite1.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)   112560 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/data/satellite2.txt
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:57:39.708504 VBBinaryLensing-3.6.2/VBBinaryLensing/lib/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)   145042 2023-07-30 22:24:42.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    11092 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/lib/VBBinaryLensingLibrary.h
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)    30353 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/lib/python_bindings.cpp
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:57:39.708504 VBBinaryLensing-3.6.2/VBBinaryLensing/tests/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1995 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/tests/test_all.py
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     7279 2023-07-30 22:23:55.000000 VBBinaryLensing-3.6.2/VBBinaryLensing/tests/test_magnification.py
+drwxrwxr-x   0 etienne   (1000) etienne   (1000)        0 2023-08-02 23:57:39.708504 VBBinaryLensing-3.6.2/VBBinaryLensing.egg-info/
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     6162 2023-08-02 23:57:39.000000 VBBinaryLensing-3.6.2/VBBinaryLensing.egg-info/PKG-INFO
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      670 2023-08-02 23:57:39.000000 VBBinaryLensing-3.6.2/VBBinaryLensing.egg-info/SOURCES.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)        1 2023-08-02 23:57:39.000000 VBBinaryLensing-3.6.2/VBBinaryLensing.egg-info/dependency_links.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       28 2023-08-02 23:57:39.000000 VBBinaryLensing-3.6.2/VBBinaryLensing.egg-info/requires.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)       45 2023-08-02 23:57:39.000000 VBBinaryLensing-3.6.2/VBBinaryLensing.egg-info/top_level.txt
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     1322 2023-08-02 23:55:47.000000 VBBinaryLensing-3.6.2/pyproject.toml
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)      875 2023-08-02 23:57:39.708504 VBBinaryLensing-3.6.2/setup.cfg
+-rw-rw-r--   0 etienne   (1000) etienne   (1000)     2685 2023-08-02 23:09:57.000000 VBBinaryLensing-3.6.2/setup.py
```

### Comparing `VBBinaryLensing-3.6.1/LICENSE` & `VBBinaryLensing-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/PKG-INFO` & `VBBinaryLensing-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VBBinaryLensing
-Version: 3.6.1
+Version: 3.6.2
 Summary: VBBinaryLensing is a tool for efficient computation in gravitational microlensing events using the advanced contour integration method, supporting single and binary lenses.
 Home-page: http://astropy.org
 Author: fran
 Author-email: Valerio Bozza <valboz@sa.infn.it>, Fran Bartolić <fb90@st-andrews.ac.uk>, Etienne Bachelet <etibachelet@gmail.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/valboz/VBBinaryLensing
 Project-URL: Documentation, https://www.fisica.unisa.it/gravitationastrophysics/VBBinaryLensing.htm
```

### Comparing `VBBinaryLensing-3.6.1/README.md` & `VBBinaryLensing-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/VBBinaryLensing/data/ESPL.tbl` & `VBBinaryLensing-3.6.2/VBBinaryLensing/data/ESPL.tbl`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/VBBinaryLensing/data/satellite1.txt` & `VBBinaryLensing-3.6.2/VBBinaryLensing/data/satellite1.txt`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/VBBinaryLensing/data/satellite2.txt` & `VBBinaryLensing-3.6.2/VBBinaryLensing/data/satellite2.txt`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp` & `VBBinaryLensing-3.6.2/VBBinaryLensing/lib/VBBinaryLensingLibrary.cpp`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/VBBinaryLensing/lib/VBBinaryLensingLibrary.h` & `VBBinaryLensing-3.6.2/VBBinaryLensing/lib/VBBinaryLensingLibrary.h`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/VBBinaryLensing/lib/python_bindings.cpp` & `VBBinaryLensing-3.6.2/VBBinaryLensing/lib/python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/VBBinaryLensing/tests/test_all.py` & `VBBinaryLensing-3.6.2/VBBinaryLensing/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/VBBinaryLensing/tests/test_magnification.py` & `VBBinaryLensing-3.6.2/VBBinaryLensing/tests/test_magnification.py`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/PKG-INFO` & `VBBinaryLensing-3.6.2/VBBinaryLensing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VBBinaryLensing
-Version: 3.6.1
+Version: 3.6.2
 Summary: VBBinaryLensing is a tool for efficient computation in gravitational microlensing events using the advanced contour integration method, supporting single and binary lenses.
 Home-page: http://astropy.org
 Author: fran
 Author-email: Valerio Bozza <valboz@sa.infn.it>, Fran Bartolić <fb90@st-andrews.ac.uk>, Etienne Bachelet <etibachelet@gmail.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/valboz/VBBinaryLensing
 Project-URL: Documentation, https://www.fisica.unisa.it/gravitationastrophysics/VBBinaryLensing.htm
```

### Comparing `VBBinaryLensing-3.6.1/VBBinaryLensing.egg-info/SOURCES.txt` & `VBBinaryLensing-3.6.2/VBBinaryLensing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/pyproject.toml` & `VBBinaryLensing-3.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["setuptools>=42", "wheel", "pybind11~=2.6.1"]
+requires = ["setuptools>=42", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "VBBinaryLensing"
 description = "VBBinaryLensing is a tool for efficient computation in gravitational microlensing events using the advanced contour integration method, supporting single and binary lenses."
-version = "3.6.1"
+version = "3.6.2"
 keywords = ['Microlsening magnification and astrometry']
 authors = [
     { name = "Valerio Bozza", email = "valboz@sa.infn.it" },
     { name = "Fran Bartolić", email = "fb90@st-andrews.ac.uk" },
     { name = "Etienne Bachelet", email = "etibachelet@gmail.com" },
 ]
 license = { text = "GPL-3.0" }
```

### Comparing `VBBinaryLensing-3.6.1/setup.cfg` & `VBBinaryLensing-3.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `VBBinaryLensing-3.6.1/setup.py` & `VBBinaryLensing-3.6.2/setup.py`

 * *Files identical despite different names*

