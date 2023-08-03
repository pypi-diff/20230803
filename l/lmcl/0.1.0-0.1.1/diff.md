# Comparing `tmp/lmcl-0.1.0.tar.gz` & `tmp/lmcl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmcl-0.1.0.tar", last modified: Thu Aug  3 15:53:17 2023, max compression
+gzip compressed data, was "lmcl-0.1.1.tar", last modified: Thu Aug  3 17:47:48 2023, max compression
```

## Comparing `lmcl-0.1.0.tar` & `lmcl-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 15:53:17.163989 lmcl-0.1.0/
--rw-rw-rw-   0        0        0      190 2023-08-03 15:53:17.162439 lmcl-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 15:53:17.130649 lmcl-0.1.0/lmcl/
--rw-rw-rw-   0        0        0       21 2023-08-03 15:15:57.000000 lmcl-0.1.0/lmcl/__init__.py
--rw-rw-rw-   0        0        0     5186 2023-08-03 15:14:16.000000 lmcl-0.1.0/lmcl/lmcl.py
-drwxrwxrwx   0        0        0        0 2023-08-03 15:53:17.155757 lmcl-0.1.0/lmcl.egg-info/
--rw-rw-rw-   0        0        0      190 2023-08-03 15:53:17.000000 lmcl-0.1.0/lmcl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-08-03 15:53:17.000000 lmcl-0.1.0/lmcl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 15:53:17.000000 lmcl-0.1.0/lmcl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-03 15:53:17.000000 lmcl-0.1.0/lmcl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-03 15:53:17.000000 lmcl-0.1.0/lmcl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 15:53:17.163989 lmcl-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-08-03 15:52:34.000000 lmcl-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:47:48.565390 lmcl-0.1.1/
+-rw-rw-rw-   0        0        0      190 2023-08-03 17:47:48.565390 lmcl-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 17:47:48.541386 lmcl-0.1.1/lmcl/
+-rw-rw-rw-   0        0        0     5229 2023-08-03 17:47:05.000000 lmcl-0.1.1/lmcl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 17:47:48.565390 lmcl-0.1.1/lmcl.egg-info/
+-rw-rw-rw-   0        0        0      190 2023-08-03 17:47:48.000000 lmcl-0.1.1/lmcl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2023-08-03 17:47:48.000000 lmcl-0.1.1/lmcl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 17:47:48.000000 lmcl-0.1.1/lmcl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 17:47:48.000000 lmcl-0.1.1/lmcl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-03 17:47:48.000000 lmcl-0.1.1/lmcl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 17:47:48.565390 lmcl-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-08-03 17:47:06.000000 lmcl-0.1.1/setup.py
```

### Comparing `lmcl-0.1.0/lmcl/lmcl.py` & `lmcl-0.1.1/lmcl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#VERSION
+__version__ = '0.1.1'
+#PROGRAM
 import openai
 class result:
     def __init__(self):
         self.result = ""
         self.variables = {}
     def assignResult(self,result):
         self.result = result
```

