# Comparing `tmp/efpy-0.1.6.tar.gz` & `tmp/efpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efpy-0.1.6.tar", last modified: Fri Jul 28 04:36:27 2023, max compression
+gzip compressed data, was "efpy-0.1.7.tar", last modified: Thu Aug  3 14:06:54 2023, max compression
```

## Comparing `efpy-0.1.6.tar` & `efpy-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 04:36:27.564125 efpy-0.1.6/
--rw-rw-rw-   0        0        0      255 2023-07-28 04:36:27.563152 efpy-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 04:36:27.555149 efpy-0.1.6/efpy/
--rw-rw-rw-   0        0        0      868 2023-07-28 04:22:45.000000 efpy-0.1.6/efpy/__init__.py
--rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.6/efpy/env.py
--rw-rw-rw-   0        0        0     3021 2023-07-28 04:11:00.000000 efpy-0.1.6/efpy/expHelper.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:36:27.562157 efpy-0.1.6/efpy.egg-info/
--rw-rw-rw-   0        0        0      255 2023-07-28 04:36:27.000000 efpy-0.1.6/efpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-07-28 04:36:27.000000 efpy-0.1.6/efpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 04:36:27.000000 efpy-0.1.6/efpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 04:36:27.000000 efpy-0.1.6/efpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 04:36:27.000000 efpy-0.1.6/efpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 04:36:27.564125 efpy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-07-28 04:25:27.000000 efpy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:06:54.763632 efpy-0.1.7/
+-rw-rw-rw-   0        0        0      255 2023-08-03 14:06:54.763632 efpy-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-03 14:06:54.754687 efpy-0.1.7/efpy/
+-rw-rw-rw-   0        0        0      868 2023-07-28 04:22:45.000000 efpy-0.1.7/efpy/__init__.py
+-rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.7/efpy/env.py
+-rw-rw-rw-   0        0        0     5068 2023-08-03 14:05:43.000000 efpy-0.1.7/efpy/expHelper.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:06:54.761638 efpy-0.1.7/efpy.egg-info/
+-rw-rw-rw-   0        0        0      255 2023-08-03 14:06:54.000000 efpy-0.1.7/efpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-08-03 14:06:54.000000 efpy-0.1.7/efpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 14:06:54.000000 efpy-0.1.7/efpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-03 14:06:54.000000 efpy-0.1.7/efpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-03 14:06:54.000000 efpy-0.1.7/efpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-03 14:06:54.763632 efpy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      831 2023-08-03 14:06:48.000000 efpy-0.1.7/setup.py
```

### Comparing `efpy-0.1.6/efpy/__init__.py` & `efpy-0.1.7/efpy/__init__.py`

 * *Files identical despite different names*

### Comparing `efpy-0.1.6/efpy/env.py` & `efpy-0.1.7/efpy/env.py`

 * *Files identical despite different names*

### Comparing `efpy-0.1.6/setup.py` & `efpy-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Created Time:  2023-4-29 07:13:42
 #############################################
 
 
 from setuptools import setup, find_packages
 #主要变量
 name="efpy"
-version = "0.1.6"
+version = "0.1.7"
 install_requires = ['PyYAML']
 
 setup(
     name = name,
     version = version,
     keywords = ("experience","environment"),
     description = "experience",
```

