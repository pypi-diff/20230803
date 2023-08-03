# Comparing `tmp/dosmaster-1.7.5.tar.gz` & `tmp/dosmaster-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.7.5.tar", last modified: Thu Aug  3 06:48:36 2023, max compression
+gzip compressed data, was "dist/dosmaster-1.7.6.tar", last modified: Thu Aug  3 06:52:52 2023, max compression
```

## Comparing `dosmaster-1.7.5.tar` & `dosmaster-1.7.6.tar`

### file list

```diff
@@ -1,12 +1,45 @@
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:48:36.000000 dosmaster-1.7.5/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:48:36.000000 dosmaster-1.7.5/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 06:47:15.000000 dosmaster-1.7.5/README.md
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      218 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/SOURCES.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/dependency_links.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/entry_points.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/requires.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/top_level.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 06:48:36.000000 dosmaster-1.7.5/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1318 2023-08-03 06:46:51.000000 dosmaster-1.7.5/setup.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:52:52.000000 dosmaster-1.7.6/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:52:52.000000 dosmaster-1.7.6/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 06:52:44.000000 dosmaster-1.7.6/README.md
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2023-08-03 06:52:13.000000 dosmaster-1.7.6/dosmaster/__init__.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster/base/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2023-08-02 06:02:15.000000 dosmaster-1.7.6/dosmaster/base/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3389 2023-08-03 06:40:27.000000 dosmaster-1.7.6/dosmaster/base/data_generation.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4455 2023-08-03 06:40:41.000000 dosmaster-1.7.6/dosmaster/base/printer.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster/features/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2023-08-02 06:01:36.000000 dosmaster-1.7.6/dosmaster/features/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2512 2023-08-03 06:40:48.000000 dosmaster-1.7.6/dosmaster/features/a_add_atom_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     8603 2023-08-03 06:40:51.000000 dosmaster-1.7.6/dosmaster/features/b_dos_projection.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1413 2023-08-03 06:40:54.000000 dosmaster-1.7.6/dosmaster/features/c_dos_sum.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2032 2023-08-03 06:40:57.000000 dosmaster-1.7.6/dosmaster/features/d_avergae_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1314 2023-08-03 06:41:00.000000 dosmaster-1.7.6/dosmaster/features/e_remove_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2023-08-03 05:44:18.000000 dosmaster-1.7.6/dosmaster/features/f_change_sign.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9873 2023-08-03 06:41:09.000000 dosmaster-1.7.6/dosmaster/features/g_graph_editor.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5937 2023-08-03 06:41:12.000000 dosmaster-1.7.6/dosmaster/features/h_axis_optimization.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster/fileparser/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2023-08-02 06:06:47.000000 dosmaster-1.7.6/dosmaster/fileparser/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4062 2023-08-02 05:45:07.000000 dosmaster-1.7.6/dosmaster/fileparser/doscar_split.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2023-08-02 05:43:24.000000 dosmaster-1.7.6/dosmaster/fileparser/procar_parser.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2023-08-03 05:52:11.000000 dosmaster-1.7.6/dosmaster/fileparser/structure_parser.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster/main/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2023-08-03 06:52:25.000000 dosmaster-1.7.6/dosmaster/main/__init__.py
+-rwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)     6371 2023-08-03 06:52:36.000000 dosmaster-1.7.6/dosmaster/main/dosmaster.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster/mainplotter/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2023-08-02 06:02:44.000000 dosmaster-1.7.6/dosmaster/mainplotter/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9843 2023-08-03 06:41:53.000000 dosmaster-1.7.6/dosmaster/mainplotter/dosplot.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster/subplotter/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-02 06:03:49.000000 dosmaster-1.7.6/dosmaster/subplotter/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2023-08-02 07:17:13.000000 dosmaster-1.7.6/dosmaster/subplotter/colors.csv
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2023-08-02 05:45:15.000000 dosmaster-1.7.6/dosmaster/subplotter/colortable.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6330 2023-08-02 17:30:13.000000 dosmaster-1.7.6/dosmaster/subplotter/dosplot_manager.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2023-08-03 06:42:01.000000 dosmaster-1.7.6/dosmaster/subplotter/make_color_list.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster.egg-info/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster.egg-info/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1103 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster.egg-info/entry_points.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster.egg-info/requires.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2023-08-03 06:52:52.000000 dosmaster-1.7.6/dosmaster.egg-info/top_level.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 06:52:52.000000 dosmaster-1.7.6/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1318 2023-08-03 06:46:51.000000 dosmaster-1.7.6/setup.py
```

### Comparing `dosmaster-1.7.5/PKG-INFO` & `dosmaster-1.7.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.7.5
+Version: 1.7.6
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.7.5/README.md` & `dosmaster-1.7.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ver.1.2 : 최종 data 파일 저장 기능 추가
 
 ver.1.3 : 버그 수정
 
 ver.1.4.2 : PyPI에 올릴 수 있도록 수정
 
-ver 1.7.5 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
+ver 1.7.6 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
 
 
 ## Features
 1) Add Atom DOS
 2) DOS Projection
 3) Sum DOS
 4) Average DOS
```

### Comparing `dosmaster-1.7.5/dosmaster.egg-info/PKG-INFO` & `dosmaster-1.7.6/dosmaster.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.7.5
+Version: 1.7.6
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.7.5/setup.py` & `dosmaster-1.7.6/setup.py`

 * *Files identical despite different names*

