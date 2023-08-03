# Comparing `tmp/DdlGeneratorTool-1.0.5.tar.gz` & `tmp/DdlGeneratorTool-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DdlGeneratorTool-1.0.5.tar", last modified: Thu Aug  3 03:00:22 2023, max compression
+gzip compressed data, was "DdlGeneratorTool-1.0.6.tar", last modified: Thu Aug  3 03:04:08 2023, max compression
```

## Comparing `DdlGeneratorTool-1.0.5.tar` & `DdlGeneratorTool-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:00:22.624483 DdlGeneratorTool-1.0.5/
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:00:22.618170 DdlGeneratorTool-1.0.5/DdlGeneratorTool.egg-info/
--rw-r--r--   0 caowenpeng   (501) staff       (20)      869 2023-08-03 03:00:22.000000 DdlGeneratorTool-1.0.5/DdlGeneratorTool.egg-info/PKG-INFO
--rw-r--r--   0 caowenpeng   (501) staff       (20)      318 2023-08-03 03:00:22.000000 DdlGeneratorTool-1.0.5/DdlGeneratorTool.egg-info/SOURCES.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-03 03:00:22.000000 DdlGeneratorTool-1.0.5/DdlGeneratorTool.egg-info/dependency_links.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       57 2023-08-03 03:00:22.000000 DdlGeneratorTool-1.0.5/DdlGeneratorTool.egg-info/entry_points.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-08-03 03:00:22.000000 DdlGeneratorTool-1.0.5/DdlGeneratorTool.egg-info/requires.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-08-03 03:00:22.000000 DdlGeneratorTool-1.0.5/DdlGeneratorTool.egg-info/top_level.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)    11558 2023-03-30 09:08:05.000000 DdlGeneratorTool-1.0.5/LICENSE
--rw-r--r--   0 caowenpeng   (501) staff       (20)      869 2023-08-03 03:00:22.623888 DdlGeneratorTool-1.0.5/PKG-INFO
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:00:22.621644 DdlGeneratorTool-1.0.5/ddl2pojo/
--rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-29 13:41:10.000000 DdlGeneratorTool-1.0.5/ddl2pojo/__init__.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)      197 2023-07-29 10:27:59.000000 DdlGeneratorTool-1.0.5/ddl2pojo/ddl2pojo.tpl
--rw-r--r--   0 caowenpeng   (501) staff       (20)     3128 2023-08-03 02:52:33.000000 DdlGeneratorTool-1.0.5/ddl2pojo/main.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-08-03 03:00:22.624681 DdlGeneratorTool-1.0.5/setup.cfg
--rw-r--r--   0 caowenpeng   (501) staff       (20)      842 2023-08-03 03:00:10.000000 DdlGeneratorTool-1.0.5/setup.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:04:08.641763 DdlGeneratorTool-1.0.6/
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:04:08.636035 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      881 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/PKG-INFO
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      318 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/SOURCES.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/dependency_links.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       57 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/entry_points.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/requires.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/top_level.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)    11558 2023-03-30 09:08:05.000000 DdlGeneratorTool-1.0.6/LICENSE
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      881 2023-08-03 03:04:08.641124 DdlGeneratorTool-1.0.6/PKG-INFO
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:04:08.639433 DdlGeneratorTool-1.0.6/ddl2pojo/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-29 13:41:10.000000 DdlGeneratorTool-1.0.6/ddl2pojo/__init__.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      197 2023-07-29 10:27:59.000000 DdlGeneratorTool-1.0.6/ddl2pojo/ddl2pojo.tpl
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     3128 2023-08-03 02:52:33.000000 DdlGeneratorTool-1.0.6/ddl2pojo/main.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-08-03 03:04:08.642024 DdlGeneratorTool-1.0.6/setup.cfg
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      842 2023-08-03 03:03:54.000000 DdlGeneratorTool-1.0.6/setup.py
```

### Comparing `DdlGeneratorTool-1.0.5/DdlGeneratorTool.egg-info/PKG-INFO` & `DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DdlGeneratorTool
-Version: 1.0.5
+Version: 1.0.6
 Summary: DDL文件解析程序
 Home-page: https://gitee.com/visonforcoding/code-template-tools
 Author: visonforcoding
 Author-email: visonforcoding@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,21 +16,21 @@
 # ddl code generation tool
 
 Currently, only supports generating Java objects.
 
 ## Installation
 
 ```
-pip install DdlGeneric
+pip install DdlGeneratorTool
 ```
 
 ## ddl2Pojo Usage
 
 ```
-DdlGeneric kaquan_user_dicount.sql
+DdlGeneratorTool kaquan_user_dicount.sql
 ```
 
 - By default, the result will be printed to the current terminal window.
 - If you want to save it to a file, you can use the `--ddl_file` parameter.
 
 ## Future Plans
```

### Comparing `DdlGeneratorTool-1.0.5/LICENSE` & `DdlGeneratorTool-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `DdlGeneratorTool-1.0.5/PKG-INFO` & `DdlGeneratorTool-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DdlGeneratorTool
-Version: 1.0.5
+Version: 1.0.6
 Summary: DDL文件解析程序
 Home-page: https://gitee.com/visonforcoding/code-template-tools
 Author: visonforcoding
 Author-email: visonforcoding@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,21 +16,21 @@
 # ddl code generation tool
 
 Currently, only supports generating Java objects.
 
 ## Installation
 
 ```
-pip install DdlGeneric
+pip install DdlGeneratorTool
 ```
 
 ## ddl2Pojo Usage
 
 ```
-DdlGeneric kaquan_user_dicount.sql
+DdlGeneratorTool kaquan_user_dicount.sql
 ```
 
 - By default, the result will be printed to the current terminal window.
 - If you want to save it to a file, you can use the `--ddl_file` parameter.
 
 ## Future Plans
```

### Comparing `DdlGeneratorTool-1.0.5/ddl2pojo/main.py` & `DdlGeneratorTool-1.0.6/ddl2pojo/main.py`

 * *Files identical despite different names*

### Comparing `DdlGeneratorTool-1.0.5/setup.py` & `DdlGeneratorTool-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 readmepath = 'README.md'
 setup(
     name='DdlGeneratorTool',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'DdlGeneratorTool = ddl2pojo.main:main'
         ]
     },
     install_requires=[
```

