# Comparing `tmp/sqlup-0.0.1.tar.gz` & `tmp/sqlup-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlup-0.0.1.tar", last modified: Thu Aug  3 07:02:07 2023, max compression
+gzip compressed data, was "sqlup-0.0.2.tar", last modified: Thu Aug  3 07:22:06 2023, max compression
```

## Comparing `sqlup-0.0.1.tar` & `sqlup-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:02:07.244380 sqlup-0.0.1/
--rw-rw-rw-   0        0        0      399 2023-08-03 07:02:07.243380 sqlup-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        3 2023-08-03 06:24:53.000000 sqlup-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-03 07:02:07.244380 sqlup-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      654 2023-08-03 07:01:40.000000 sqlup-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:02:07.233378 sqlup-0.0.1/sqls/
--rw-rw-rw-   0        0        0       22 2023-08-03 06:47:30.000000 sqlup-0.0.1/sqls/__init__.py
--rw-rw-rw-   0        0        0      389 2023-08-03 06:47:32.000000 sqlup-0.0.1/sqls/sqls.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:02:07.242381 sqlup-0.0.1/sqlup.egg-info/
--rw-rw-rw-   0        0        0      399 2023-08-03 07:02:06.000000 sqlup-0.0.1/sqlup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-08-03 07:02:07.000000 sqlup-0.0.1/sqlup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:02:06.000000 sqlup-0.0.1/sqlup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-03 07:02:06.000000 sqlup-0.0.1/sqlup.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-08-03 07:02:06.000000 sqlup-0.0.1/sqlup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-03 07:02:06.000000 sqlup-0.0.1/sqlup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 07:22:06.647145 sqlup-0.0.2/
+-rw-rw-rw-   0        0        0      399 2023-08-03 07:22:06.647145 sqlup-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        3 2023-08-03 06:24:53.000000 sqlup-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:22:06.648146 sqlup-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      654 2023-08-03 07:21:51.000000 sqlup-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:22:06.637143 sqlup-0.0.2/sqls/
+-rw-rw-rw-   0        0        0       22 2023-08-03 06:47:30.000000 sqlup-0.0.2/sqls/__init__.py
+-rw-rw-rw-   0        0        0      384 2023-08-03 07:20:50.000000 sqlup-0.0.2/sqls/sqls.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:22:06.645146 sqlup-0.0.2/sqlup.egg-info/
+-rw-rw-rw-   0        0        0      399 2023-08-03 07:22:06.000000 sqlup-0.0.2/sqlup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-08-03 07:22:06.000000 sqlup-0.0.2/sqlup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:22:06.000000 sqlup-0.0.2/sqlup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-03 07:22:06.000000 sqlup-0.0.2/sqlup.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-08-03 07:22:06.000000 sqlup-0.0.2/sqlup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-03 07:22:06.000000 sqlup-0.0.2/sqlup.egg-info/top_level.txt
```

### Comparing `sqlup-0.0.1/setup.py` & `sqlup-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿# setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='sqlup',
-    version='0.0.1',
+    version='0.0.2',
     description='mysql_laod',
     author='sang',
     author_email='dnl6098@gamil.com',
     url='https://github.com/wisangyun/MyProject',
     packages=find_packages(exclude=[]),
     python_requires='>=3.6',
     package_data={},
```

