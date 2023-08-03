# Comparing `tmp/dosmaster-1.7.2.tar.gz` & `tmp/dosmaster-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.7.2.tar", last modified: Thu Aug  3 06:01:12 2023, max compression
+gzip compressed data, was "dist/dosmaster-1.7.3.tar", last modified: Thu Aug  3 06:08:10 2023, max compression
```

## Comparing `dosmaster-1.7.2.tar` & `dosmaster-1.7.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:01:12.000000 dosmaster-1.7.2/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 05:54:29.000000 dosmaster-1.7.2/README.md
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/base/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2023-08-02 06:02:15.000000 dosmaster-1.7.2/base/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3359 2023-08-03 05:06:09.000000 dosmaster-1.7.2/base/data_generation.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4424 2023-08-03 05:46:08.000000 dosmaster-1.7.2/base/printer.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      809 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/SOURCES.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/dependency_links.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       50 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/entry_points.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/requires.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       53 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/top_level.txt
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/features/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2023-08-02 06:01:36.000000 dosmaster-1.7.2/features/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2502 2023-08-02 17:22:25.000000 dosmaster-1.7.2/features/a_add_atom_dos.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     8593 2023-08-02 17:23:25.000000 dosmaster-1.7.2/features/b_dos_projection.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1403 2023-08-03 05:49:40.000000 dosmaster-1.7.2/features/c_dos_sum.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2012 2023-08-03 05:47:51.000000 dosmaster-1.7.2/features/d_avergae_dos.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1304 2023-08-02 17:22:33.000000 dosmaster-1.7.2/features/e_remove_dos.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2023-08-03 05:44:18.000000 dosmaster-1.7.2/features/f_change_sign.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9843 2023-08-03 05:41:11.000000 dosmaster-1.7.2/features/g_graph_editor.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5927 2023-08-03 05:43:37.000000 dosmaster-1.7.2/features/h_axis_optimization.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/fileparser/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2023-08-02 06:06:47.000000 dosmaster-1.7.2/fileparser/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4062 2023-08-02 05:45:07.000000 dosmaster-1.7.2/fileparser/doscar_split.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2023-08-02 05:43:24.000000 dosmaster-1.7.2/fileparser/procar_parser.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2023-08-03 05:52:11.000000 dosmaster-1.7.2/fileparser/structure_parser.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/main/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2023-08-03 01:18:13.000000 dosmaster-1.7.2/main/__init__.py
--rwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)     6526 2023-08-03 05:45:54.000000 dosmaster-1.7.2/main/dosmaster.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/mainplotter/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2023-08-02 06:02:44.000000 dosmaster-1.7.2/mainplotter/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9823 2023-08-03 05:06:26.000000 dosmaster-1.7.2/mainplotter/dosplot.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 06:01:12.000000 dosmaster-1.7.2/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1267 2023-08-03 05:59:58.000000 dosmaster-1.7.2/setup.py
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/subplotter/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-02 06:03:49.000000 dosmaster-1.7.2/subplotter/__init__.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2023-08-02 05:45:15.000000 dosmaster-1.7.2/subplotter/colortable.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6330 2023-08-02 17:30:13.000000 dosmaster-1.7.2/subplotter/dosplot_manager.py
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2023-08-03 05:49:02.000000 dosmaster-1.7.2/subplotter/make_color_list.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:08:10.000000 dosmaster-1.7.3/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 06:07:44.000000 dosmaster-1.7.3/README.md
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/base/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2023-08-02 06:02:15.000000 dosmaster-1.7.3/base/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3359 2023-08-03 05:06:09.000000 dosmaster-1.7.3/base/data_generation.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4424 2023-08-03 05:46:08.000000 dosmaster-1.7.3/base/printer.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      809 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       50 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/entry_points.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/requires.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       53 2023-08-03 06:08:10.000000 dosmaster-1.7.3/dosmaster.egg-info/top_level.txt
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/features/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2023-08-02 06:01:36.000000 dosmaster-1.7.3/features/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2502 2023-08-02 17:22:25.000000 dosmaster-1.7.3/features/a_add_atom_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     8593 2023-08-02 17:23:25.000000 dosmaster-1.7.3/features/b_dos_projection.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1403 2023-08-03 05:49:40.000000 dosmaster-1.7.3/features/c_dos_sum.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2012 2023-08-03 05:47:51.000000 dosmaster-1.7.3/features/d_avergae_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1304 2023-08-02 17:22:33.000000 dosmaster-1.7.3/features/e_remove_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2023-08-03 05:44:18.000000 dosmaster-1.7.3/features/f_change_sign.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9843 2023-08-03 05:41:11.000000 dosmaster-1.7.3/features/g_graph_editor.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5927 2023-08-03 05:43:37.000000 dosmaster-1.7.3/features/h_axis_optimization.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/fileparser/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2023-08-02 06:06:47.000000 dosmaster-1.7.3/fileparser/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4062 2023-08-02 05:45:07.000000 dosmaster-1.7.3/fileparser/doscar_split.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2023-08-02 05:43:24.000000 dosmaster-1.7.3/fileparser/procar_parser.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2023-08-03 05:52:11.000000 dosmaster-1.7.3/fileparser/structure_parser.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/main/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2023-08-03 06:06:36.000000 dosmaster-1.7.3/main/__init__.py
+-rwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)     6221 2023-08-03 06:07:13.000000 dosmaster-1.7.3/main/dosmaster.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/mainplotter/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2023-08-02 06:02:44.000000 dosmaster-1.7.3/mainplotter/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9823 2023-08-03 05:06:26.000000 dosmaster-1.7.3/mainplotter/dosplot.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 06:08:10.000000 dosmaster-1.7.3/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1267 2023-08-03 05:59:58.000000 dosmaster-1.7.3/setup.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:08:10.000000 dosmaster-1.7.3/subplotter/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-02 06:03:49.000000 dosmaster-1.7.3/subplotter/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2023-08-02 05:45:15.000000 dosmaster-1.7.3/subplotter/colortable.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6330 2023-08-02 17:30:13.000000 dosmaster-1.7.3/subplotter/dosplot_manager.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2023-08-03 05:49:02.000000 dosmaster-1.7.3/subplotter/make_color_list.py
```

### Comparing `dosmaster-1.7.2/PKG-INFO` & `dosmaster-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.7.2
+Version: 1.7.3
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.7.2/README.md` & `dosmaster-1.7.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ver.1.2 : 최종 data 파일 저장 기능 추가
 
 ver.1.3 : 버그 수정
 
 ver.1.4.2 : PyPI에 올릴 수 있도록 수정
 
-ver 1.7.2 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
+ver 1.7.3 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
 
 
 ## Features
 1) Add Atom DOS
 2) DOS Projection
 3) Sum DOS
 4) Average DOS
```

### Comparing `dosmaster-1.7.2/base/data_generation.py` & `dosmaster-1.7.3/base/data_generation.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/base/printer.py` & `dosmaster-1.7.3/base/printer.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/dosmaster.egg-info/PKG-INFO` & `dosmaster-1.7.3/dosmaster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.7.2
+Version: 1.7.3
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.7.2/dosmaster.egg-info/SOURCES.txt` & `dosmaster-1.7.3/dosmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/features/a_add_atom_dos.py` & `dosmaster-1.7.3/features/a_add_atom_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/features/b_dos_projection.py` & `dosmaster-1.7.3/features/b_dos_projection.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/features/c_dos_sum.py` & `dosmaster-1.7.3/features/c_dos_sum.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/features/d_avergae_dos.py` & `dosmaster-1.7.3/features/d_avergae_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/features/e_remove_dos.py` & `dosmaster-1.7.3/features/e_remove_dos.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/features/f_change_sign.py` & `dosmaster-1.7.3/features/f_change_sign.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/features/g_graph_editor.py` & `dosmaster-1.7.3/features/g_graph_editor.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/features/h_axis_optimization.py` & `dosmaster-1.7.3/features/h_axis_optimization.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/fileparser/doscar_split.py` & `dosmaster-1.7.3/fileparser/doscar_split.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/fileparser/structure_parser.py` & `dosmaster-1.7.3/fileparser/structure_parser.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/main/dosmaster.py` & `dosmaster-1.7.3/main/dosmaster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #======================================================================================================
-#Script Name : dosmaster Program(ver.1.7.2)
+#Script Name : dosmaster Program(ver.1.7.3)
 #Made by Youngjun Park (yjpark29@postech.ac.kr)
 #Inspired by Jaesun Kim
 #Edit Date : 23/08/02
 #======================================================================================================
 #Description : DOS Plot Smartly in Terminal Environment
 #======================================================================================================
 #: 1) Add Atom DOS
@@ -80,65 +80,58 @@
                     'save_filename' : 'DOS',
                     'save_format' : 'pdf',
                     'save_dpi' : 200,
                     'dos_color' : {list_to_string_name(data_dict['DOS_list'][0]) : {'color':'gray', 'User_Edit':None}},
                     'ylim_optimization' : False,
                     }
         
-    try:
-        StartMessage()
+    StartMessage()
             
-        while True:
-            # Main Loop
-            print_current_DOS(data_dict['DOS_list'], data_dict['Labellist'], graph_config)
-            print('What would you like to do? (Exit : q or qq)')
-            print('==================================================================================================================')
-            print('1 : Add Atom DOS')
-            print('2 : Project DOS')
-            print('3 : Sum DOS')
-            print('4 : Average DOS')
-            print('5 : Remove specific DOS')
-            print('6 : Show only positive/negative part')
-            print('7 : Edit graph style')
-            print('8 : ylim optimization')
-            print('==================================================================================================================')
-            Input_Work=input('Choice : ')
-            print('-'*80)
-
-            # User Selection
-            if Input_Work == 'q':
-                user_is_save=input('o you want to save the currently drawn DOS? (1 : yes / 2 : no(default) : ')
-                if user_is_save == '1':
-                    data_dict['is_save'] = True
-                else:
-                    data_dict['is_save'] = False
-                DOSplot(data_dict, graph_config)
-                break
-            elif Input_Work == '1':
-                data_dict['DOS_list'], graph_config = Add_Atom_DOS(data_dict, graph_config)
-            elif Input_Work == '2':
-                data_dict['DOS_list'], graph_config = Projected_DOS(data_dict, graph_config)
-            elif Input_Work == '3':
-                data_dict['DOS_list'], graph_config = DOS_Sum(data_dict, graph_config)
-            elif Input_Work == '4':
-                data_dict['DOS_list'], graph_config = Average_DOS(data_dict, graph_config)
-            elif Input_Work == '5':
-                data_dict['DOS_list'], graph_config = Remove_DOS(data_dict, graph_config)
-            elif Input_Work == '6':
-                graph_config = Change_Sign(data_dict, graph_config)
-            elif Input_Work == '7':
-                graph_config = Graph_Editor(data_dict, graph_config)
-            elif Input_Work == '8':
-                graph_config = Axis_Optimization(data_dict, graph_config)
-            
-            # Modified DOS Plot
-            graph_config = Dos_Color_Update(data_dict, graph_config)
-            graph_config = DOSplot(data_dict, graph_config)
-    
-    except:
-        print('DOSMaster Error Occured!')
+    while True:
+        # Main Loop
+        print_current_DOS(data_dict['DOS_list'], data_dict['Labellist'], graph_config)
+        print('What would you like to do? (Exit : q or qq)')
+        print('==================================================================================================================')
+        print('1 : Add Atom DOS')
+        print('2 : Project DOS')
+        print('3 : Sum DOS')
+        print('4 : Average DOS')
+        print('5 : Remove specific DOS')
+        print('6 : Show only positive/negative part')
+        print('7 : Edit graph style')
+        print('8 : ylim optimization')
+        print('==================================================================================================================')
+        Input_Work=input('Choice : ')
+        print('-'*80)
+
+        # User Selection
+        if Input_Work == 'q':
+            user_is_save=input('o you want to save the currently drawn DOS? (1 : yes / 2 : no(default) : ')
+            if user_is_save == '1':
+                data_dict['is_save'] = True
+            else:
+                data_dict['is_save'] = False
+            DOSplot(data_dict, graph_config)
+            break
+        elif Input_Work == '1':
+            data_dict['DOS_list'], graph_config = Add_Atom_DOS(data_dict, graph_config)
+        elif Input_Work == '2':
+            data_dict['DOS_list'], graph_config = Projected_DOS(data_dict, graph_config)
+        elif Input_Work == '3':
+            data_dict['DOS_list'], graph_config = DOS_Sum(data_dict, graph_config)
+        elif Input_Work == '4':
+            data_dict['DOS_list'], graph_config = Average_DOS(data_dict, graph_config)
+        elif Input_Work == '5':
+            data_dict['DOS_list'], graph_config = Remove_DOS(data_dict, graph_config)
+        elif Input_Work == '6':
+            graph_config = Change_Sign(data_dict, graph_config)
+        elif Input_Work == '7':
+            graph_config = Graph_Editor(data_dict, graph_config)
+        elif Input_Work == '8':
+            graph_config = Axis_Optimization(data_dict, graph_config)
         
-    finally:
-        print(Style.RESET_ALL)
+        # Modified DOS Plot
+        graph_config = Dos_Color_Update(data_dict, graph_config)
+        graph_config = DOSplot(data_dict, graph_config)
 
 if __name__ == "__main__":
     main()
```

### Comparing `dosmaster-1.7.2/mainplotter/dosplot.py` & `dosmaster-1.7.3/mainplotter/dosplot.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/setup.py` & `dosmaster-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/subplotter/colortable.py` & `dosmaster-1.7.3/subplotter/colortable.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/subplotter/dosplot_manager.py` & `dosmaster-1.7.3/subplotter/dosplot_manager.py`

 * *Files identical despite different names*

### Comparing `dosmaster-1.7.2/subplotter/make_color_list.py` & `dosmaster-1.7.3/subplotter/make_color_list.py`

 * *Files identical despite different names*

