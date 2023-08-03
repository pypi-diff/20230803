# Comparing `tmp/dosmaster-1.4.2.tar.gz` & `tmp/dosmaster-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.4.2.tar", last modified: Tue Aug  1 20:44:55 2023, max compression
+gzip compressed data, was "dist/dosmaster-1.7.2.tar", last modified: Thu Aug  3 06:01:12 2023, max compression
```

## Comparing `dosmaster-1.4.2.tar` & `dosmaster-1.7.2.tar`

### file list

```diff
@@ -1,15 +1,42 @@
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-01 20:44:55.000000 dosmaster-1.4.2/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      627 2023-08-01 20:44:55.000000 dosmaster-1.4.2/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1433 2023-08-01 20:39:31.000000 dosmaster-1.4.2/README.md
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-01 20:44:55.000000 dosmaster-1.4.2/dosmaster.egg-info/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      627 2023-08-01 20:44:55.000000 dosmaster-1.4.2/dosmaster.egg-info/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      253 2023-08-01 20:44:55.000000 dosmaster-1.4.2/dosmaster.egg-info/SOURCES.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-01 20:44:55.000000 dosmaster-1.4.2/dosmaster.egg-info/dependency_links.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       50 2023-08-01 20:44:55.000000 dosmaster-1.4.2/dosmaster.egg-info/entry_points.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       43 2023-08-01 20:44:55.000000 dosmaster-1.4.2/dosmaster.egg-info/requires.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        5 2023-08-01 20:44:55.000000 dosmaster-1.4.2/dosmaster.egg-info/top_level.txt
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-01 20:44:55.000000 dosmaster-1.4.2/main/
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2023-08-01 20:39:24.000000 dosmaster-1.4.2/main/__init__.py
--rwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)    52897 2023-08-01 20:44:38.000000 dosmaster-1.4.2/main/dosmaster.py
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-01 20:44:55.000000 dosmaster-1.4.2/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1703 2023-08-01 20:39:02.000000 dosmaster-1.4.2/setup.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:01:12.000000 dosmaster-1.7.2/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 05:54:29.000000 dosmaster-1.7.2/README.md
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/base/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       39 2023-08-02 06:02:15.000000 dosmaster-1.7.2/base/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3359 2023-08-03 05:06:09.000000 dosmaster-1.7.2/base/data_generation.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4424 2023-08-03 05:46:08.000000 dosmaster-1.7.2/base/printer.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      809 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       50 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/entry_points.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/requires.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       53 2023-08-03 06:01:12.000000 dosmaster-1.7.2/dosmaster.egg-info/top_level.txt
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/features/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       55 2023-08-02 06:01:36.000000 dosmaster-1.7.2/features/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2502 2023-08-02 17:22:25.000000 dosmaster-1.7.2/features/a_add_atom_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     8593 2023-08-02 17:23:25.000000 dosmaster-1.7.2/features/b_dos_projection.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1403 2023-08-03 05:49:40.000000 dosmaster-1.7.2/features/c_dos_sum.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     2012 2023-08-03 05:47:51.000000 dosmaster-1.7.2/features/d_avergae_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1304 2023-08-02 17:22:33.000000 dosmaster-1.7.2/features/e_remove_dos.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1350 2023-08-03 05:44:18.000000 dosmaster-1.7.2/features/f_change_sign.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9843 2023-08-03 05:41:11.000000 dosmaster-1.7.2/features/g_graph_editor.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     5927 2023-08-03 05:43:37.000000 dosmaster-1.7.2/features/h_axis_optimization.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/fileparser/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       61 2023-08-02 06:06:47.000000 dosmaster-1.7.2/fileparser/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     4062 2023-08-02 05:45:07.000000 dosmaster-1.7.2/fileparser/doscar_split.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      221 2023-08-02 05:43:24.000000 dosmaster-1.7.2/fileparser/procar_parser.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6742 2023-08-03 05:52:11.000000 dosmaster-1.7.2/fileparser/structure_parser.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/main/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)      153 2023-08-03 01:18:13.000000 dosmaster-1.7.2/main/__init__.py
+-rwxrwxr-x   0 parkyj6767  (1016) parkyj6767  (1017)     6526 2023-08-03 05:45:54.000000 dosmaster-1.7.2/main/dosmaster.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/mainplotter/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       36 2023-08-02 06:02:44.000000 dosmaster-1.7.2/mainplotter/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     9823 2023-08-03 05:06:26.000000 dosmaster-1.7.2/mainplotter/dosplot.py
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 06:01:12.000000 dosmaster-1.7.2/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1267 2023-08-03 05:59:58.000000 dosmaster-1.7.2/setup.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:01:12.000000 dosmaster-1.7.2/subplotter/
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)       40 2023-08-02 06:03:49.000000 dosmaster-1.7.2/subplotter/__init__.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     3361 2023-08-02 05:45:15.000000 dosmaster-1.7.2/subplotter/colortable.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     6330 2023-08-02 17:30:13.000000 dosmaster-1.7.2/subplotter/dosplot_manager.py
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1947 2023-08-03 05:49:02.000000 dosmaster-1.7.2/subplotter/make_color_list.py
```

### Comparing `dosmaster-1.4.2/PKG-INFO` & `dosmaster-1.7.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.4.2
-Summary: DOS(Density Of States) Plot Smartly
+Version: 1.7.2
+Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dosmaster-1.4.2/dosmaster.egg-info/PKG-INFO` & `dosmaster-1.7.2/dosmaster.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.4.2
-Summary: DOS(Density Of States) Plot Smartly
+Version: 1.7.2
+Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dosmaster-1.4.2/setup.py` & `dosmaster-1.7.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
 from main import __version__
 
-# with open("README.rst") as file:
-#     long_description = file.read()
+#with open("README.md") as file:
+#    long_description = file.read()
 
 setup(
     name="dosmaster",
     version=__version__,
-    description="DOS(Density Of States) Plot Smartly",
+    description="DOS(Density Of States) Plot Smartly in Terminal",
     url="https://github.com/pyj6767/DOSMaster",
     author="Youngjun Park, Jaeson Kim",
     author_email="yjpark29@postech.ac.kr",
     #long_description=long_description,
     license="CNMD",
     classifiers=[
         "Development Status :: 4 - Beta",
@@ -27,26 +27,20 @@
     packages=find_packages(),
     python_requires=">=3.7.13",
     install_requires=[
         "numpy",
         "matplotlib",
         "pandas>=1.3.5",
         "ase>=3.22.1",
+        "colorama>=0.4.6",
     ],
-    # package_data={ #python 파일이 아닌 다른 파일들을 포함시키는 옵션
-    #     "dosmaster": [
-    #         "symmetry/bradcrack.json",
-    #         "plotting/orbital_colours.conf",
-    #         "plotting/sumo_base.mplstyle",
-    #         "plotting/sumo_bs.mplstyle",
-    #         "plotting/sumo_dos.mplstyle",
-    #         "plotting/sumo_optics.mplstyle",
-    #         "plotting/sumo_phonon.mplstyle",
-    #     ]
-    # },
-    #data_files=["examples/orbital_colours.conf", "LICENSE"],
+    package_data={
+        "dosmaster": [
+            "subplotter/colors.csv",
+        ]
+    },
     entry_points={
         "console_scripts": [
-            "dosmaster = main.dosmaster:main", #main : 폴더, dosmaster : python 파일, main : 함수
+            "dosmaster = main.dosmaster:main",
         ]
     },
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

