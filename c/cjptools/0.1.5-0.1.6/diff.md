# Comparing `tmp/cjptools-0.1.5.tar.gz` & `tmp/cjptools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjptools-0.1.5.tar", last modified: Thu Aug  3 07:35:13 2023, max compression
+gzip compressed data, was "cjptools-0.1.6.tar", last modified: Thu Aug  3 07:48:00 2023, max compression
```

## Comparing `cjptools-0.1.5.tar` & `cjptools-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 07:35:13.688538 cjptools-0.1.5/
--rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 cjptools-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      276 2023-08-03 07:35:13.687541 cjptools-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 07:35:13.661628 cjptools-0.1.5/cjptools/
--rw-rw-rw-   0        0        0       69 2023-07-28 04:04:26.000000 cjptools-0.1.5/cjptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:35:13.669599 cjptools-0.1.5/cjptools/dptools/
--rw-rw-rw-   0        0        0       25 2023-07-31 13:36:57.000000 cjptools-0.1.5/cjptools/dptools/__init__.py
--rw-rw-rw-   0        0        0     3603 2023-07-31 13:36:34.000000 cjptools-0.1.5/cjptools/dptools/rdpAccount.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:35:13.675213 cjptools-0.1.5/cjptools/printModules/
--rw-rw-rw-   0        0        0      125 2022-10-13 16:20:01.000000 cjptools-0.1.5/cjptools/printModules/__init__.py
--rw-rw-rw-   0        0        0      103 2022-10-13 16:20:01.000000 cjptools-0.1.5/cjptools/printModules/absPrinter.py
--rw-rw-rw-   0        0        0      317 2022-10-13 16:20:01.000000 cjptools-0.1.5/cjptools/printModules/printerCompose.py
--rw-rw-rw-   0        0        0      643 2023-08-02 13:22:06.000000 cjptools-0.1.5/cjptools/printModules/printers.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:35:13.686545 cjptools-0.1.5/cjptools/utils/
--rw-rw-rw-   0        0        0      207 2023-08-03 07:34:59.000000 cjptools-0.1.5/cjptools/utils/__init__.py
--rw-rw-rw-   0        0        0      103 2023-07-28 03:39:04.000000 cjptools-0.1.5/cjptools/utils/check.py
--rw-rw-rw-   0        0        0     4490 2023-07-28 03:39:27.000000 cjptools-0.1.5/cjptools/utils/gpu_mem_track.py
--rw-rw-rw-   0        0        0     1382 2023-07-28 03:39:31.000000 cjptools-0.1.5/cjptools/utils/modelsize_estimate.py
--rw-rw-rw-   0        0        0      541 2023-07-28 07:17:31.000000 cjptools-0.1.5/cjptools/utils/path.py
--rw-rw-rw-   0        0        0      511 2023-08-03 07:33:23.000000 cjptools-0.1.5/cjptools/utils/reflect.py
--rw-rw-rw-   0        0        0      741 2023-07-31 13:33:07.000000 cjptools-0.1.5/cjptools/utils/rnd.py
--rw-rw-rw-   0        0        0      330 2023-07-28 03:39:53.000000 cjptools-0.1.5/cjptools/utils/timer.py
-drwxrwxrwx   0        0        0        0 2023-08-03 07:35:13.666608 cjptools-0.1.5/cjptools.egg-info/
--rw-rw-rw-   0        0        0      276 2023-08-03 07:35:13.000000 cjptools-0.1.5/cjptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-08-03 07:35:13.000000 cjptools-0.1.5/cjptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 07:35:13.000000 cjptools-0.1.5/cjptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 07:35:13.000000 cjptools-0.1.5/cjptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 07:35:13.688538 cjptools-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-08-03 07:35:08.000000 cjptools-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.256385 cjptools-0.1.6/
+-rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 cjptools-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-08-03 07:48:00.255387 cjptools-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.221532 cjptools-0.1.6/cjptools/
+-rw-rw-rw-   0        0        0       69 2023-07-28 04:04:26.000000 cjptools-0.1.6/cjptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.232505 cjptools-0.1.6/cjptools/dptools/
+-rw-rw-rw-   0        0        0       25 2023-07-31 13:36:57.000000 cjptools-0.1.6/cjptools/dptools/__init__.py
+-rw-rw-rw-   0        0        0     3603 2023-07-31 13:36:34.000000 cjptools-0.1.6/cjptools/dptools/rdpAccount.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.240480 cjptools-0.1.6/cjptools/printModules/
+-rw-rw-rw-   0        0        0      125 2022-10-13 16:20:01.000000 cjptools-0.1.6/cjptools/printModules/__init__.py
+-rw-rw-rw-   0        0        0      103 2022-10-13 16:20:01.000000 cjptools-0.1.6/cjptools/printModules/absPrinter.py
+-rw-rw-rw-   0        0        0      317 2022-10-13 16:20:01.000000 cjptools-0.1.6/cjptools/printModules/printerCompose.py
+-rw-rw-rw-   0        0        0      643 2023-08-02 13:22:06.000000 cjptools-0.1.6/cjptools/printModules/printers.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.253393 cjptools-0.1.6/cjptools/utils/
+-rw-rw-rw-   0        0        0      207 2023-08-03 07:34:59.000000 cjptools-0.1.6/cjptools/utils/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-07-28 03:39:04.000000 cjptools-0.1.6/cjptools/utils/check.py
+-rw-rw-rw-   0        0        0     4490 2023-07-28 03:39:27.000000 cjptools-0.1.6/cjptools/utils/gpu_mem_track.py
+-rw-rw-rw-   0        0        0     1382 2023-07-28 03:39:31.000000 cjptools-0.1.6/cjptools/utils/modelsize_estimate.py
+-rw-rw-rw-   0        0        0      541 2023-07-28 07:17:31.000000 cjptools-0.1.6/cjptools/utils/path.py
+-rw-rw-rw-   0        0        0      336 2023-08-03 07:47:46.000000 cjptools-0.1.6/cjptools/utils/reflect.py
+-rw-rw-rw-   0        0        0      741 2023-07-31 13:33:07.000000 cjptools-0.1.6/cjptools/utils/rnd.py
+-rw-rw-rw-   0        0        0      330 2023-07-28 03:39:53.000000 cjptools-0.1.6/cjptools/utils/timer.py
+drwxrwxrwx   0        0        0        0 2023-08-03 07:48:00.227515 cjptools-0.1.6/cjptools.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-08-03 07:48:00.000000 cjptools-0.1.6/cjptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-08-03 07:48:00.000000 cjptools-0.1.6/cjptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 07:48:00.000000 cjptools-0.1.6/cjptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 07:48:00.000000 cjptools-0.1.6/cjptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 07:48:00.256385 cjptools-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-08-03 07:47:55.000000 cjptools-0.1.6/setup.py
```

### Comparing `cjptools-0.1.5/LICENSE` & `cjptools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.5/cjptools/dptools/rdpAccount.py` & `cjptools-0.1.6/cjptools/dptools/rdpAccount.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.5/cjptools/printModules/printers.py` & `cjptools-0.1.6/cjptools/printModules/printers.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.5/cjptools/utils/gpu_mem_track.py` & `cjptools-0.1.6/cjptools/utils/gpu_mem_track.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.5/cjptools/utils/modelsize_estimate.py` & `cjptools-0.1.6/cjptools/utils/modelsize_estimate.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.5/cjptools/utils/path.py` & `cjptools-0.1.6/cjptools/utils/path.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.5/cjptools/utils/rnd.py` & `cjptools-0.1.6/cjptools/utils/rnd.py`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.5/cjptools.egg-info/SOURCES.txt` & `cjptools-0.1.6/cjptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cjptools-0.1.5/setup.py` & `cjptools-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="cjptools",
-    version="0.1.5",
+    version="0.1.6",
     keywords=("database", "localServer"),
     description="My Personal Toolkit",
     long_description="My Personal Toolkit",
     license="MIT Licence",
     author="Cai Jianping",
     author_email="jpingcai@163.com",
```

