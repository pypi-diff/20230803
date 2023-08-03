# Comparing `tmp/ekea-1.2.1.tar.gz` & `tmp/ekea-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ekea-1.2.1.tar", last modified: Thu Aug  3 14:54:20 2023, max compression
+gzip compressed data, was "dist/ekea-1.2.2.tar", last modified: Thu Aug  3 18:00:25 2023, max compression
```

## Comparing `ekea-1.2.1.tar` & `ekea-1.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:54:20.000000 ekea-1.2.1/
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     1070 2022-09-10 16:48:49.000000 ekea-1.2.1/LICENSE
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)       19 2022-09-10 17:37:23.000000 ekea-1.2.1/MANIFEST.in
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      877 2023-08-03 14:54:20.000000 ekea-1.2.1/PKG-INFO
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     2832 2022-10-03 02:29:10.000000 ekea-1.2.1/README.rst
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:54:20.000000 ekea-1.2.1/ekea/
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)       71 2022-09-10 17:37:23.000000 ekea-1.2.1/ekea/__init__.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)      178 2022-09-10 17:43:26.000000 ekea-1.2.1/ekea/__main__.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     8896 2022-10-04 18:52:35.000000 ekea-1.2.1/ekea/e3smapp.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)      558 2022-09-30 15:02:50.000000 ekea-1.2.1/ekea/eam.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)      294 2022-09-10 16:48:49.000000 ekea-1.2.1/ekea/exclude_e3sm_cam.ini
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)      297 2022-10-04 18:52:35.000000 ekea-1.2.1/ekea/exclude_e3sm_eam.ini
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)      798 2022-10-04 18:52:35.000000 ekea-1.2.1/ekea/exclude_e3sm_mpas.ini
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)       53 2022-09-10 16:48:49.000000 ekea-1.2.1/ekea/exclude_e3sm_varlist.ini
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)      695 2023-08-03 14:40:04.000000 ekea-1.2.1/ekea/main.py
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1397 2023-08-03 14:38:31.000000 ekea-1.2.1/ekea/mpasocn.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     9976 2022-10-01 14:55:42.000000 ekea-1.2.1/ekea/timing.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)      237 2022-09-10 16:48:49.000000 ekea-1.2.1/ekea/utils.py
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     3967 2022-10-01 14:56:14.000000 ekea-1.2.1/ekea/varwhere.py
-drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 14:54:20.000000 ekea-1.2.1/ekea.egg-info/
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)      877 2023-08-03 14:54:20.000000 ekea-1.2.1/ekea.egg-info/PKG-INFO
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)      455 2023-08-03 14:54:20.000000 ekea-1.2.1/ekea.egg-info/SOURCES.txt
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)        1 2023-08-03 14:54:20.000000 ekea-1.2.1/ekea.egg-info/dependency_links.txt
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)       78 2023-08-03 14:54:20.000000 ekea-1.2.1/ekea.egg-info/entry_points.txt
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)       15 2023-08-03 14:54:20.000000 ekea-1.2.1/ekea.egg-info/requires.txt
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)        5 2023-08-03 14:54:20.000000 ekea-1.2.1/ekea.egg-info/top_level.txt
--rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       38 2023-08-03 14:54:20.000000 ekea-1.2.1/setup.cfg
--rw-r--r--   0 grnydawn (10270) grnydawn (19448)     1491 2023-08-03 14:45:27.000000 ekea-1.2.1/setup.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 18:00:25.000000 ekea-1.2.2/
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     1070 2022-09-10 16:48:49.000000 ekea-1.2.2/LICENSE
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)       19 2022-09-10 17:37:23.000000 ekea-1.2.2/MANIFEST.in
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)      877 2023-08-03 18:00:25.000000 ekea-1.2.2/PKG-INFO
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     2832 2022-10-03 02:29:10.000000 ekea-1.2.2/README.rst
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 18:00:25.000000 ekea-1.2.2/ekea/
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)       71 2022-09-10 17:37:23.000000 ekea-1.2.2/ekea/__init__.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)      178 2022-09-10 17:43:26.000000 ekea-1.2.2/ekea/__main__.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     8896 2022-10-04 18:52:35.000000 ekea-1.2.2/ekea/e3smapp.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)      558 2022-09-30 15:02:50.000000 ekea-1.2.2/ekea/eam.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)      294 2022-09-10 16:48:49.000000 ekea-1.2.2/ekea/exclude_e3sm_cam.ini
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)      297 2022-10-04 18:52:35.000000 ekea-1.2.2/ekea/exclude_e3sm_eam.ini
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)      798 2022-10-04 18:52:35.000000 ekea-1.2.2/ekea/exclude_e3sm_mpas.ini
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)       53 2022-09-10 16:48:49.000000 ekea-1.2.2/ekea/exclude_e3sm_varlist.ini
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)      695 2023-08-03 17:59:34.000000 ekea-1.2.2/ekea/main.py
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)     1397 2023-08-03 14:38:31.000000 ekea-1.2.2/ekea/mpasocn.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     9976 2022-10-01 14:55:42.000000 ekea-1.2.2/ekea/timing.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)      237 2022-09-10 16:48:49.000000 ekea-1.2.2/ekea/utils.py
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     3967 2022-10-01 14:56:14.000000 ekea-1.2.2/ekea/varwhere.py
+drwxrwxr-x   0 grnydawn (10270) grnydawn (19448)        0 2023-08-03 18:00:25.000000 ekea-1.2.2/ekea.egg-info/
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)      877 2023-08-03 18:00:24.000000 ekea-1.2.2/ekea.egg-info/PKG-INFO
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)      455 2023-08-03 18:00:24.000000 ekea-1.2.2/ekea.egg-info/SOURCES.txt
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)        1 2023-08-03 18:00:24.000000 ekea-1.2.2/ekea.egg-info/dependency_links.txt
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)       78 2023-08-03 18:00:24.000000 ekea-1.2.2/ekea.egg-info/entry_points.txt
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)       15 2023-08-03 18:00:24.000000 ekea-1.2.2/ekea.egg-info/requires.txt
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)        5 2023-08-03 18:00:24.000000 ekea-1.2.2/ekea.egg-info/top_level.txt
+-rw-rw-r--   0 grnydawn (10270) grnydawn (19448)       38 2023-08-03 18:00:25.000000 ekea-1.2.2/setup.cfg
+-rw-r--r--   0 grnydawn (10270) grnydawn (19448)     1491 2023-08-03 17:51:06.000000 ekea-1.2.2/setup.py
```

### Comparing `ekea-1.2.1/LICENSE` & `ekea-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ekea-1.2.1/PKG-INFO` & `ekea-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ekea
-Version: 1.2.1
+Version: 1.2.2
 Summary: E3SM Fortran Kernel Extraction and Analysis
 Home-page: UNKNOWN
 Author: Youngsung Kim
 Author-email: youngsung.kim.act2@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/grnydawn/ekea/issues
 Project-URL: Source, https://github.com/grnydawn/ekea
```

### Comparing `ekea-1.2.1/README.rst` & `ekea-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `ekea-1.2.1/ekea/e3smapp.py` & `ekea-1.2.2/ekea/e3smapp.py`

 * *Files identical despite different names*

### Comparing `ekea-1.2.1/ekea/eam.py` & `ekea-1.2.2/ekea/eam.py`

 * *Files identical despite different names*

### Comparing `ekea-1.2.1/ekea/exclude_e3sm_mpas.ini` & `ekea-1.2.2/ekea/exclude_e3sm_mpas.ini`

 * *Files identical despite different names*

### Comparing `ekea-1.2.1/ekea/main.py` & `ekea-1.2.2/ekea/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ekea.eam import EAMKernel
 from ekea.timing import KernelTimeGenerator, KernelTimeViewer
 from ekea.varwhere import VariableList
 
 class EKEA(Fortlab):
 
     _name_ = "ekea"
-    _version_ = "1.2.1"
+    _version_ = "1.2.2"
     _description_ = "E3SM Fortran Kernel Extraction and Analysis"
     _long_description_ = "E3SM Fortran Kernel Extraction and Analysis"
     _author_ = "Youngsung Kim"
     _author_email_ = "youngsung.kim.act2@gmail.com"
     _url_ = "https://github.com/grnydawn/ekea"
     _builtin_apps_ = [MPASOcnKernel, EAMKernel, KernelTimeGenerator,
                       KernelTimeViewer, VariableList]
```

### Comparing `ekea-1.2.1/ekea/mpasocn.py` & `ekea-1.2.2/ekea/mpasocn.py`

 * *Files identical despite different names*

### Comparing `ekea-1.2.1/ekea/timing.py` & `ekea-1.2.2/ekea/timing.py`

 * *Files identical despite different names*

### Comparing `ekea-1.2.1/ekea/varwhere.py` & `ekea-1.2.2/ekea/varwhere.py`

 * *Files identical despite different names*

### Comparing `ekea-1.2.1/ekea.egg-info/PKG-INFO` & `ekea-1.2.2/ekea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ekea
-Version: 1.2.1
+Version: 1.2.2
 Summary: E3SM Fortran Kernel Extraction and Analysis
 Home-page: UNKNOWN
 Author: Youngsung Kim
 Author-email: youngsung.kim.act2@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/grnydawn/ekea/issues
 Project-URL: Source, https://github.com/grnydawn/ekea
```

### Comparing `ekea-1.2.1/setup.py` & `ekea-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def main():
 
     from setuptools import setup, find_packages
     from ekea.main import EKEA
 
     console_scripts = ["ekea=ekea.__main__:main"]
-    install_requires = ["fortlab>=1.1.2"]
+    install_requires = ["fortlab>=1.1.3"]
 
     setup(
         name=EKEA._name_,
         version=EKEA._version_,
         description=EKEA._description_,
         long_description=EKEA._long_description_,
         author=EKEA._author_,
```

