# Comparing `tmp/dosmaster-1.7.3.tar.gz` & `tmp/dosmaster-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.7.3.tar", last modified: Thu Aug  3 06:08:10 2023, max compression
+gzip compressed data, was "dist/dosmaster-1.7.4.tar", last modified: Thu Aug  3 06:43:31 2023, max compression
```

## Comparing `dosmaster-1.7.3.tar` & `dosmaster-1.7.4.tar`

### file list

```diff
@@ -1,42 +1,12 @@
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:08:10.000000 dosmaster-1.7.3/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 06:07:44.000000 dosmaster-1.7.3/README.md
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/base/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2023-08-02 06:02:15.000000 dosmaster-1.7.3/base/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3359 2023-08-03 05:06:09.000000 dosmaster-1.7.3/base/data_generation.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4424 2023-08-03 05:46:08.000000 dosmaster-1.7.3/base/printer.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      809 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/SOURCES.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/dependency_links.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       50 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/entry_points.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/requires.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       53 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/top_level.txt
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/features/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2023-08-02 06:01:36.000000 dosmaster-1.7.3/features/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2502 2023-08-02 17:22:25.000000 dosmaster-1.7.3/features/a_add_atom_dos.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     8593 2023-08-02 17:23:25.000000 dosmaster-1.7.3/features/b_dos_projection.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1403 2023-08-03 05:49:40.000000 dosmaster-1.7.3/features/c_dos_sum.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2012 2023-08-03 05:47:51.000000 dosmaster-1.7.3/features/d_avergae_dos.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1304 2023-08-02 17:22:33.000000 dosmaster-1.7.3/features/e_remove_dos.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2023-08-03 05:44:18.000000 dosmaster-1.7.3/features/f_change_sign.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9843 2023-08-03 05:41:11.000000 dosmaster-1.7.3/features/g_graph_editor.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5927 2023-08-03 05:43:37.000000 dosmaster-1.7.3/features/h_axis_optimization.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/fileparser/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2023-08-02 06:06:47.000000 dosmaster-1.7.3/fileparser/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4062 2023-08-02 05:45:07.000000 dosmaster-1.7.3/fileparser/doscar_split.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2023-08-02 05:43:24.000000 dosmaster-1.7.3/fileparser/procar_parser.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2023-08-03 05:52:11.000000 dosmaster-1.7.3/fileparser/structure_parser.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/main/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2023-08-03 06:06:36.000000 dosmaster-1.7.3/main/__init__.py
--rwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)     6221 2023-08-03 06:07:13.000000 dosmaster-1.7.3/main/dosmaster.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/mainplotter/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2023-08-02 06:02:44.000000 dosmaster-1.7.3/mainplotter/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9823 2023-08-03 05:06:26.000000 dosmaster-1.7.3/mainplotter/dosplot.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 06:08:10.000000 dosmaster-1.7.3/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1267 2023-08-03 05:59:58.000000 dosmaster-1.7.3/setup.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/subplotter/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-02 06:03:49.000000 dosmaster-1.7.3/subplotter/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2023-08-02 05:45:15.000000 dosmaster-1.7.3/subplotter/colortable.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6330 2023-08-02 17:30:13.000000 dosmaster-1.7.3/subplotter/dosplot_manager.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2023-08-03 05:49:02.000000 dosmaster-1.7.3/subplotter/make_color_list.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:43:31.000000 dosmaster-1.7.4/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:43:31.000000 dosmaster-1.7.4/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 06:38:30.000000 dosmaster-1.7.4/README.md
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      218 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/entry_points.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/requires.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/top_level.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 06:43:31.000000 dosmaster-1.7.4/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1318 2023-08-03 06:43:29.000000 dosmaster-1.7.4/setup.py
```

### Comparing `dosmaster-1.7.3/PKG-INFO` & `dosmaster-1.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.7.3
+Version: 1.7.4
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.7.3/README.md` & `dosmaster-1.7.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ver.1.2 : 최종 data 파일 저장 기능 추가
 
 ver.1.3 : 버그 수정
 
 ver.1.4.2 : PyPI에 올릴 수 있도록 수정
 
-ver 1.7.3 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
+ver 1.7.4 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
 
 
 ## Features
 1) Add Atom DOS
 2) DOS Projection
 3) Sum DOS
 4) Average DOS
```

### Comparing `dosmaster-1.7.3/dosmaster.egg-info/PKG-INFO` & `dosmaster-1.7.4/dosmaster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.7.3
+Version: 1.7.4
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.7.3/setup.py` & `dosmaster-1.7.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-from main import __version__
+from dosmaster.main import __version__
 
 #with open("README.md") as file:
 #    long_description = file.read()
 
 setup(
     name="dosmaster",
     version=__version__,
@@ -34,13 +34,14 @@
         "colorama>=0.4.6",
     ],
     package_data={
         "dosmaster": [
             "subplotter/colors.csv",
         ]
     },
+    inclued_package_data=True,
     entry_points={
         "console_scripts": [
-            "dosmaster = main.dosmaster:main",
+            "dosmaster = dosmaster.main.dosmaster:main",
         ]
     },
 )
```

