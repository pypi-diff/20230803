# Comparing `tmp/FedxD-0.6.tar.gz` & `tmp/FedxD-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FedxD-0.6.tar", last modified: Wed Aug  2 15:48:06 2023, max compression
+gzip compressed data, was "FedxD-0.7.tar", last modified: Thu Aug  3 18:33:57 2023, max compression
```

## Comparing `FedxD-0.6.tar` & `FedxD-0.7.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 15:48:06.052286 FedxD-0.6/
-drwxrwxrwx   0        0        0        0 2023-08-02 15:48:06.025302 FedxD-0.6/FedxD/
--rw-rw-rw-   0        0        0    40746 2023-08-02 15:26:35.000000 FedxD-0.6/FedxD/Lists.py
--rw-rw-rw-   0        0        0       79 2023-08-02 14:51:40.000000 FedxD-0.6/FedxD/__init__.py
--rw-rw-rw-   0        0        0     2250 2023-08-02 15:26:35.000000 FedxD-0.6/FedxD/color.py
--rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.6/FedxD/converters.py
--rw-rw-rw-   0        0        0      565 2023-08-02 15:45:59.000000 FedxD-0.6/FedxD/random.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:48:06.045290 FedxD-0.6/FedxD.egg-info/
--rw-rw-rw-   0        0        0     2025 2023-08-02 15:48:05.000000 FedxD-0.6/FedxD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-08-02 15:48:05.000000 FedxD-0.6/FedxD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 15:48:05.000000 FedxD-0.6/FedxD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-02 15:48:05.000000 FedxD-0.6/FedxD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.6/License.txt
--rw-rw-rw-   0        0        0     2025 2023-08-02 15:48:06.048287 FedxD-0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-02 15:48:06.052286 FedxD-0.6/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-08-02 15:47:52.000000 FedxD-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:33:57.003008 FedxD-0.7/
+drwxrwxrwx   0        0        0        0 2023-08-03 18:33:56.966030 FedxD-0.7/FedxD/
+-rw-rw-rw-   0        0        0    40746 2023-08-02 15:26:35.000000 FedxD-0.7/FedxD/Lists.py
+-rw-rw-rw-   0        0        0      211 2023-08-03 18:06:39.000000 FedxD-0.7/FedxD/__init__.py
+-rw-rw-rw-   0        0        0     2250 2023-08-02 15:26:35.000000 FedxD-0.7/FedxD/color.py
+-rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.7/FedxD/converters.py
+-rw-rw-rw-   0        0        0      225 2023-08-03 18:01:13.000000 FedxD-0.7/FedxD/discord.py
+-rw-rw-rw-   0        0        0      776 2023-08-03 17:55:09.000000 FedxD-0.7/FedxD/excel.py
+-rw-rw-rw-   0        0        0      769 2023-08-03 18:33:36.000000 FedxD-0.7/FedxD/pygame.py
+-rw-rw-rw-   0        0        0      565 2023-08-02 15:45:59.000000 FedxD-0.7/FedxD/random.py
+drwxrwxrwx   0        0        0        0 2023-08-03 18:33:56.998011 FedxD-0.7/FedxD.egg-info/
+-rw-rw-rw-   0        0        0     3601 2023-08-03 18:33:55.000000 FedxD-0.7/FedxD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-08-03 18:33:55.000000 FedxD-0.7/FedxD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 18:33:55.000000 FedxD-0.7/FedxD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-03 18:33:55.000000 FedxD-0.7/FedxD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.7/License.txt
+-rw-rw-rw-   0        0        0     3601 2023-08-03 18:33:57.001008 FedxD-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-03 18:33:57.003008 FedxD-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-08-03 18:33:36.000000 FedxD-0.7/setup.py
```

### Comparing `FedxD-0.6/FedxD/Lists.py` & `FedxD-0.7/FedxD/Lists.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.6/FedxD/color.py` & `FedxD-0.7/FedxD/color.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.6/FedxD/converters.py` & `FedxD-0.7/FedxD/converters.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.6/FedxD/random.py` & `FedxD-0.7/FedxD/random.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.6/License.txt` & `FedxD-0.7/License.txt`

 * *Files identical despite different names*

### Comparing `FedxD-0.6/setup.py` & `FedxD-0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import twine
 from setuptools import setup , find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(name='FedxD',
-    version='0.6',
+    version='0.7',
     packages=['FedxD'],
     author='FedxD',
     author_email='abbaskazim135@gmail.com',
     description='This Package is for Quality of life stuff that you will need in your project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/FedxD',
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     pyton_requires='>=3.10',
+    requires=['openpyxl','discord','pygame'],
 
 )
```

