# Comparing `tmp/dosmaster-1.7.4.tar.gz` & `tmp/dosmaster-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dosmaster-1.7.4.tar", last modified: Thu Aug  3 06:43:31 2023, max compression
+gzip compressed data, was "dist/dosmaster-1.7.5.tar", last modified: Thu Aug  3 06:48:36 2023, max compression
```

## Comparing `dosmaster-1.7.4.tar` & `dosmaster-1.7.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:43:31.000000 dosmaster-1.7.4/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:43:31.000000 dosmaster-1.7.4/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 06:38:30.000000 dosmaster-1.7.4/README.md
-drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/PKG-INFO
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      218 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/SOURCES.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/dependency_links.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/entry_points.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/requires.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:43:31.000000 dosmaster-1.7.4/dosmaster.egg-info/top_level.txt
--rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 06:43:31.000000 dosmaster-1.7.4/setup.cfg
--rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1318 2023-08-03 06:43:29.000000 dosmaster-1.7.4/setup.py
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:48:36.000000 dosmaster-1.7.5/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:48:36.000000 dosmaster-1.7.5/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)     1590 2023-08-03 06:47:15.000000 dosmaster-1.7.5/README.md
+drwxr-xr-x   0 parkyj6767  (1016) parkyj6767  (1017)        0 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      639 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/PKG-INFO
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)      218 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       60 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/entry_points.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       59 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/requires.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)        1 2023-08-03 06:48:36.000000 dosmaster-1.7.5/dosmaster.egg-info/top_level.txt
+-rw-r--r--   0 parkyj6767  (1016) parkyj6767  (1017)       38 2023-08-03 06:48:36.000000 dosmaster-1.7.5/setup.cfg
+-rw-rw-r--   0 parkyj6767  (1016) parkyj6767  (1017)     1318 2023-08-03 06:46:51.000000 dosmaster-1.7.5/setup.py
```

### Comparing `dosmaster-1.7.4/PKG-INFO` & `dosmaster-1.7.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.7.4
+Version: 1.7.5
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.7.4/README.md` & `dosmaster-1.7.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ver.1.2 : 최종 data 파일 저장 기능 추가
 
 ver.1.3 : 버그 수정
 
 ver.1.4.2 : PyPI에 올릴 수 있도록 수정
 
-ver 1.7.4 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
+ver 1.7.5 : Packaging 진행, DOS_Sum, Average_DOS, Axis_Optimization 추가 및 각종 성능 향상
 
 
 ## Features
 1) Add Atom DOS
 2) DOS Projection
 3) Sum DOS
 4) Average DOS
```

### Comparing `dosmaster-1.7.4/dosmaster.egg-info/PKG-INFO` & `dosmaster-1.7.5/dosmaster.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosmaster
-Version: 1.7.4
+Version: 1.7.5
 Summary: DOS(Density Of States) Plot Smartly in Terminal
 Home-page: https://github.com/pyj6767/DOSMaster
 Author: Youngjun Park, Jaeson Kim
 Author-email: yjpark29@postech.ac.kr
 License: CNMD
 Keywords: vasp dos
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dosmaster-1.7.4/setup.py` & `dosmaster-1.7.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,14 @@
         "colorama>=0.4.6",
     ],
     package_data={
         "dosmaster": [
             "subplotter/colors.csv",
         ]
     },
-    inclued_package_data=True,
+    include_package_data=True,
     entry_points={
         "console_scripts": [
             "dosmaster = dosmaster.main.dosmaster:main",
         ]
     },
 )
```

