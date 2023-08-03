# Comparing `tmp/dosmaster-1.7.7.tar.gz` & `tmp/dosmaster-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.7.7.tar", last modified: Thu Aug  3 07:01:47 2023, max compression
+gzip compressed data, was "dist/dosmaster-1.7.8.tar", last modified: Thu Aug  3 07:04:52 2023, max compression
```

## Comparing `dosmaster-1.7.7.tar` & `dosmaster-1.7.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:01:47.000000 dosmaster-1.7.7/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-03 06:58:46.000000 dosmaster-1.7.7/MANIFEST.in
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 07:01:47.000000 dosmaster-1.7.7/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 07:01:13.000000 dosmaster-1.7.7/README.md
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2023-08-03 06:52:13.000000 dosmaster-1.7.7/dosmaster/__init__.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster/base/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2023-08-02 06:02:15.000000 dosmaster-1.7.7/dosmaster/base/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3389 2023-08-03 06:40:27.000000 dosmaster-1.7.7/dosmaster/base/data_generation.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4455 2023-08-03 06:40:41.000000 dosmaster-1.7.7/dosmaster/base/printer.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster/features/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2023-08-02 06:01:36.000000 dosmaster-1.7.7/dosmaster/features/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2512 2023-08-03 06:40:48.000000 dosmaster-1.7.7/dosmaster/features/a_add_atom_dos.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     8603 2023-08-03 06:40:51.000000 dosmaster-1.7.7/dosmaster/features/b_dos_projection.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1413 2023-08-03 06:40:54.000000 dosmaster-1.7.7/dosmaster/features/c_dos_sum.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2032 2023-08-03 06:40:57.000000 dosmaster-1.7.7/dosmaster/features/d_avergae_dos.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1314 2023-08-03 06:41:00.000000 dosmaster-1.7.7/dosmaster/features/e_remove_dos.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2023-08-03 05:44:18.000000 dosmaster-1.7.7/dosmaster/features/f_change_sign.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9873 2023-08-03 06:41:09.000000 dosmaster-1.7.7/dosmaster/features/g_graph_editor.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5937 2023-08-03 06:41:12.000000 dosmaster-1.7.7/dosmaster/features/h_axis_optimization.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster/fileparser/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2023-08-02 06:06:47.000000 dosmaster-1.7.7/dosmaster/fileparser/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4062 2023-08-02 05:45:07.000000 dosmaster-1.7.7/dosmaster/fileparser/doscar_split.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2023-08-02 05:43:24.000000 dosmaster-1.7.7/dosmaster/fileparser/procar_parser.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2023-08-03 05:52:11.000000 dosmaster-1.7.7/dosmaster/fileparser/structure_parser.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster/main/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2023-08-03 07:01:23.000000 dosmaster-1.7.7/dosmaster/main/__init__.py
--rwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)     6371 2023-08-03 07:01:32.000000 dosmaster-1.7.7/dosmaster/main/dosmaster.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster/mainplotter/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2023-08-02 06:02:44.000000 dosmaster-1.7.7/dosmaster/mainplotter/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9843 2023-08-03 06:41:53.000000 dosmaster-1.7.7/dosmaster/mainplotter/dosplot.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster/subplotter/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-02 06:03:49.000000 dosmaster-1.7.7/dosmaster/subplotter/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2023-08-02 07:17:13.000000 dosmaster-1.7.7/dosmaster/subplotter/colors.csv
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2023-08-02 05:45:15.000000 dosmaster-1.7.7/dosmaster/subplotter/colortable.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6330 2023-08-02 17:30:13.000000 dosmaster-1.7.7/dosmaster/subplotter/dosplot_manager.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2023-08-03 06:42:01.000000 dosmaster-1.7.7/dosmaster/subplotter/make_color_list.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster.egg-info/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster.egg-info/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1115 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster.egg-info/SOURCES.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster.egg-info/dependency_links.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster.egg-info/entry_points.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster.egg-info/requires.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2023-08-03 07:01:47.000000 dosmaster-1.7.7/dosmaster.egg-info/top_level.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 07:01:47.000000 dosmaster-1.7.7/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1328 2023-08-03 07:00:57.000000 dosmaster-1.7.7/setup.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:04:52.000000 dosmaster-1.7.8/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-03 06:58:46.000000 dosmaster-1.7.8/MANIFEST.in
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 07:04:52.000000 dosmaster-1.7.8/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 07:04:17.000000 dosmaster-1.7.8/README.md
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      130 2023-08-03 06:52:13.000000 dosmaster-1.7.8/dosmaster/__init__.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster/base/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2023-08-02 06:02:15.000000 dosmaster-1.7.8/dosmaster/base/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3400 2023-08-03 07:04:07.000000 dosmaster-1.7.8/dosmaster/base/data_generation.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4455 2023-08-03 06:40:41.000000 dosmaster-1.7.8/dosmaster/base/printer.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster/features/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2023-08-02 06:01:36.000000 dosmaster-1.7.8/dosmaster/features/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2512 2023-08-03 06:40:48.000000 dosmaster-1.7.8/dosmaster/features/a_add_atom_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     8603 2023-08-03 06:40:51.000000 dosmaster-1.7.8/dosmaster/features/b_dos_projection.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1413 2023-08-03 06:40:54.000000 dosmaster-1.7.8/dosmaster/features/c_dos_sum.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2032 2023-08-03 06:40:57.000000 dosmaster-1.7.8/dosmaster/features/d_avergae_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1314 2023-08-03 06:41:00.000000 dosmaster-1.7.8/dosmaster/features/e_remove_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2023-08-03 05:44:18.000000 dosmaster-1.7.8/dosmaster/features/f_change_sign.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9873 2023-08-03 06:41:09.000000 dosmaster-1.7.8/dosmaster/features/g_graph_editor.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5937 2023-08-03 06:41:12.000000 dosmaster-1.7.8/dosmaster/features/h_axis_optimization.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster/fileparser/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2023-08-02 06:06:47.000000 dosmaster-1.7.8/dosmaster/fileparser/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4062 2023-08-02 05:45:07.000000 dosmaster-1.7.8/dosmaster/fileparser/doscar_split.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2023-08-02 05:43:24.000000 dosmaster-1.7.8/dosmaster/fileparser/procar_parser.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2023-08-03 05:52:11.000000 dosmaster-1.7.8/dosmaster/fileparser/structure_parser.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster/main/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2023-08-03 07:04:31.000000 dosmaster-1.7.8/dosmaster/main/__init__.py
+-rwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)     6371 2023-08-03 07:04:38.000000 dosmaster-1.7.8/dosmaster/main/dosmaster.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster/mainplotter/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2023-08-02 06:02:44.000000 dosmaster-1.7.8/dosmaster/mainplotter/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9843 2023-08-03 06:41:53.000000 dosmaster-1.7.8/dosmaster/mainplotter/dosplot.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster/subplotter/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-02 06:03:49.000000 dosmaster-1.7.8/dosmaster/subplotter/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1180 2023-08-02 07:17:13.000000 dosmaster-1.7.8/dosmaster/subplotter/colors.csv
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2023-08-02 05:45:15.000000 dosmaster-1.7.8/dosmaster/subplotter/colortable.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6330 2023-08-02 17:30:13.000000 dosmaster-1.7.8/dosmaster/subplotter/dosplot_manager.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2023-08-03 06:42:01.000000 dosmaster-1.7.8/dosmaster/subplotter/make_color_list.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster.egg-info/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster.egg-info/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1115 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster.egg-info/entry_points.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster.egg-info/requires.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       10 2023-08-03 07:04:52.000000 dosmaster-1.7.8/dosmaster.egg-info/top_level.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 07:04:52.000000 dosmaster-1.7.8/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1328 2023-08-03 07:00:57.000000 dosmaster-1.7.8/setup.py
```

### Comparing `dosmaster-1.7.7/PKG-INFO` & `dosmaster-1.7.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.7.7
+Version: 1.7.8
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.7.7/README.md` & `dosmaster-1.7.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ver.1.2 : 최종 data 파일 저장 기능 추가
 
 ver.1.3 : 버그 수정
 
 ver.1.4.2 : PyPI에 올릴 수 있도록 수정
 
-ver 1.7.7 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
+ver 1.7.8 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
 
 
 ## Features
 1) Add Atom DOS
 2) DOS Projection
 3) Sum DOS
 4) Average DOS
```

### Comparing `dosmaster-1.7.7/dosmaster/base/data_generation.py` & `dosmaster-1.7.8/dosmaster/base/data_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         return dos_element
     else:
         return ' and '.join(dos_element)
     
 def Dos_Color_Update(data_dict, graph_config):
     DOS_list = data_dict['DOS_list']
     
-    with open('subplotter/colors.csv', 'r') as f:
+    with open('dosmaster/subplotter/colors.csv', 'r') as f:
         reader = csv.reader(f)
         Color_list = list(reader)[0]
 
     old_dos_color_list = [graph_config['dos_color'][dos_name]['color'] for dos_name in graph_config['dos_color']]
     
     # Add the dos_name that is not in graph_config['dos_color']
     data_dict_dos_name_list = [list_to_string_name(dos) for dos in DOS_list]
@@ -72,8 +72,8 @@
             pass
         
     # Remove the dos_name that is not in DOS_list 
     remove_index = [i for i, item in enumerate(old_graph_dos_name_list) if item not in data_dict_dos_name_list]
     for index in sorted(remove_index, reverse=True):
         del graph_config['dos_color'][old_graph_dos_name_list[index]]
             
-    return graph_config
+    return graph_config
```

### Comparing `dosmaster-1.7.7/dosmaster/base/printer.py` & `dosmaster-1.7.8/dosmaster/base/printer.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/features/a_add_atom_dos.py` & `dosmaster-1.7.8/dosmaster/features/a_add_atom_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/features/b_dos_projection.py` & `dosmaster-1.7.8/dosmaster/features/b_dos_projection.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/features/c_dos_sum.py` & `dosmaster-1.7.8/dosmaster/features/c_dos_sum.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/features/d_avergae_dos.py` & `dosmaster-1.7.8/dosmaster/features/d_avergae_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/features/e_remove_dos.py` & `dosmaster-1.7.8/dosmaster/features/e_remove_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/features/f_change_sign.py` & `dosmaster-1.7.8/dosmaster/features/f_change_sign.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/features/g_graph_editor.py` & `dosmaster-1.7.8/dosmaster/features/g_graph_editor.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/features/h_axis_optimization.py` & `dosmaster-1.7.8/dosmaster/features/h_axis_optimization.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/fileparser/doscar_split.py` & `dosmaster-1.7.8/dosmaster/fileparser/doscar_split.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/fileparser/structure_parser.py` & `dosmaster-1.7.8/dosmaster/fileparser/structure_parser.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/main/dosmaster.py` & `dosmaster-1.7.8/dosmaster/main/dosmaster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #======================================================================================================
-#Script Name : dosmaster Program(ver.1.7.7)
+#Script Name : dosmaster Program(ver.1.7.8)
 #Made by Youngjun Park (yjpark29@postech.ac.kr)
 #Inspired by Jaesun Kim
 #Edit Date : 23/08/02
 #======================================================================================================
 #Description : DOS Plot Smartly in Terminal Environment
 #======================================================================================================
 #: 1) Add Atom DOS
```

### Comparing `dosmaster-1.7.7/dosmaster/mainplotter/dosplot.py` & `dosmaster-1.7.8/dosmaster/mainplotter/dosplot.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/subplotter/colors.csv` & `dosmaster-1.7.8/dosmaster/subplotter/colors.csv`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/subplotter/colortable.py` & `dosmaster-1.7.8/dosmaster/subplotter/colortable.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/subplotter/dosplot_manager.py` & `dosmaster-1.7.8/dosmaster/subplotter/dosplot_manager.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster/subplotter/make_color_list.py` & `dosmaster-1.7.8/dosmaster/subplotter/make_color_list.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/dosmaster.egg-info/PKG-INFO` & `dosmaster-1.7.8/dosmaster.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.7.7
+Version: 1.7.8
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.7.7/dosmaster.egg-info/SOURCES.txt` & `dosmaster-1.7.8/dosmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.7/setup.py` & `dosmaster-1.7.8/setup.py`

 * *Files identical despite different names*

