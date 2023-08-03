# Comparing `tmp/DdlGeneratorTool-1.0.6.tar.gz` & `tmp/DdlGeneratorTool-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DdlGeneratorTool-1.0.6.tar", last modified: Thu Aug  3 03:04:08 2023, max compression
+gzip compressed data, was "DdlGeneratorTool-1.0.7.tar", last modified: Thu Aug  3 03:28:10 2023, max compression
```

## Comparing `DdlGeneratorTool-1.0.6.tar` & `DdlGeneratorTool-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:04:08.641763 DdlGeneratorTool-1.0.6/
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:04:08.636035 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/
--rw-r--r--   0 caowenpeng   (501) staff       (20)      881 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/PKG-INFO
--rw-r--r--   0 caowenpeng   (501) staff       (20)      318 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/SOURCES.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/dependency_links.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)       57 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/entry_points.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/requires.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-08-03 03:04:08.000000 DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/top_level.txt
--rw-r--r--   0 caowenpeng   (501) staff       (20)    11558 2023-03-30 09:08:05.000000 DdlGeneratorTool-1.0.6/LICENSE
--rw-r--r--   0 caowenpeng   (501) staff       (20)      881 2023-08-03 03:04:08.641124 DdlGeneratorTool-1.0.6/PKG-INFO
-drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:04:08.639433 DdlGeneratorTool-1.0.6/ddl2pojo/
--rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-29 13:41:10.000000 DdlGeneratorTool-1.0.6/ddl2pojo/__init__.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)      197 2023-07-29 10:27:59.000000 DdlGeneratorTool-1.0.6/ddl2pojo/ddl2pojo.tpl
--rw-r--r--   0 caowenpeng   (501) staff       (20)     3128 2023-08-03 02:52:33.000000 DdlGeneratorTool-1.0.6/ddl2pojo/main.py
--rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-08-03 03:04:08.642024 DdlGeneratorTool-1.0.6/setup.cfg
--rw-r--r--   0 caowenpeng   (501) staff       (20)      842 2023-08-03 03:03:54.000000 DdlGeneratorTool-1.0.6/setup.py
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:28:10.779919 DdlGeneratorTool-1.0.7/
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:28:10.772459 DdlGeneratorTool-1.0.7/DdlGeneratorTool.egg-info/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      881 2023-08-03 03:28:10.000000 DdlGeneratorTool-1.0.7/DdlGeneratorTool.egg-info/PKG-INFO
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      318 2023-08-03 03:28:10.000000 DdlGeneratorTool-1.0.7/DdlGeneratorTool.egg-info/SOURCES.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        1 2023-08-03 03:28:10.000000 DdlGeneratorTool-1.0.7/DdlGeneratorTool.egg-info/dependency_links.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       57 2023-08-03 03:28:10.000000 DdlGeneratorTool-1.0.7/DdlGeneratorTool.egg-info/entry_points.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       29 2023-08-03 03:28:10.000000 DdlGeneratorTool-1.0.7/DdlGeneratorTool.egg-info/requires.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        9 2023-08-03 03:28:10.000000 DdlGeneratorTool-1.0.7/DdlGeneratorTool.egg-info/top_level.txt
+-rw-r--r--   0 caowenpeng   (501) staff       (20)    11558 2023-03-30 09:08:05.000000 DdlGeneratorTool-1.0.7/LICENSE
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      881 2023-08-03 03:28:10.779428 DdlGeneratorTool-1.0.7/PKG-INFO
+drwxr-xr-x   0 caowenpeng   (501) staff       (20)        0 2023-08-03 03:28:10.776019 DdlGeneratorTool-1.0.7/ddl2pojo/
+-rw-r--r--   0 caowenpeng   (501) staff       (20)        0 2023-07-29 13:41:10.000000 DdlGeneratorTool-1.0.7/ddl2pojo/__init__.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      197 2023-07-29 10:27:59.000000 DdlGeneratorTool-1.0.7/ddl2pojo/ddl2pojo.tpl
+-rw-r--r--   0 caowenpeng   (501) staff       (20)     3128 2023-08-03 02:52:33.000000 DdlGeneratorTool-1.0.7/ddl2pojo/main.py
+-rw-r--r--   0 caowenpeng   (501) staff       (20)       38 2023-08-03 03:28:10.780100 DdlGeneratorTool-1.0.7/setup.cfg
+-rw-r--r--   0 caowenpeng   (501) staff       (20)      866 2023-08-03 03:27:16.000000 DdlGeneratorTool-1.0.7/setup.py
```

### Comparing `DdlGeneratorTool-1.0.6/DdlGeneratorTool.egg-info/PKG-INFO` & `DdlGeneratorTool-1.0.7/DdlGeneratorTool.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DdlGeneratorTool
-Version: 1.0.6
+Version: 1.0.7
 Summary: DDL文件解析程序
 Home-page: https://gitee.com/visonforcoding/code-template-tools
 Author: visonforcoding
 Author-email: visonforcoding@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `DdlGeneratorTool-1.0.6/LICENSE` & `DdlGeneratorTool-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `DdlGeneratorTool-1.0.6/PKG-INFO` & `DdlGeneratorTool-1.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DdlGeneratorTool
-Version: 1.0.6
+Version: 1.0.7
 Summary: DDL文件解析程序
 Home-page: https://gitee.com/visonforcoding/code-template-tools
 Author: visonforcoding
 Author-email: visonforcoding@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `DdlGeneratorTool-1.0.6/ddl2pojo/main.py` & `DdlGeneratorTool-1.0.7/ddl2pojo/main.py`

 * *Files identical despite different names*

### Comparing `DdlGeneratorTool-1.0.6/setup.py` & `DdlGeneratorTool-1.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 readmepath = 'README.md'
 setup(
     name='DdlGeneratorTool',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'DdlGeneratorTool = ddl2pojo.main:main'
         ]
     },
     install_requires=[
-        'argparse'
+        'argparse','string_utils','jinja2'
     ],
     author='visonforcoding',
     author_email='visonforcoding@gmail.com',
     description='DDL文件解析程序',
     long_description=open(readmepath, encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://gitee.com/visonforcoding/code-template-tools',
```

