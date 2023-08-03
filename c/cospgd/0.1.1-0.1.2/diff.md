# Comparing `tmp/cospgd-0.1.1.tar.gz` & `tmp/cospgd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cospgd-0.1.1.tar", last modified: Thu Aug  3 19:45:19 2023, max compression
+gzip compressed data, was "cospgd-0.1.2.tar", last modified: Thu Aug  3 19:50:21 2023, max compression
```

## Comparing `cospgd-0.1.1.tar` & `cospgd-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:45:19.718332 cospgd-0.1.1/
--rw-rw-r--   0 shashank  (1000) shashank  (1000)     1114 2023-08-03 16:40:23.000000 cospgd-0.1.1/LICENSE.md
--rw-rw-r--   0 shashank  (1000) shashank  (1000)     1010 2023-08-03 19:45:19.718332 cospgd-0.1.1/PKG-INFO
--rw-rw-r--   0 shashank  (1000) shashank  (1000)     1813 2023-08-03 16:23:45.000000 cospgd-0.1.1/README.md
-drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:45:19.718332 cospgd-0.1.1/cospgd/
--rw-rw-r--   0 shashank  (1000) shashank  (1000)      470 2023-08-03 17:23:15.000000 cospgd-0.1.1/cospgd/__init__.py
--rw-rw-r--   0 shashank  (1000) shashank  (1000)    11624 2023-08-03 19:37:49.000000 cospgd-0.1.1/cospgd/attack_implementations.py
-drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:45:19.718332 cospgd-0.1.1/cospgd.egg-info/
--rw-rw-r--   0 shashank  (1000) shashank  (1000)     1010 2023-08-03 19:45:19.000000 cospgd-0.1.1/cospgd.egg-info/PKG-INFO
--rw-rw-r--   0 shashank  (1000) shashank  (1000)      230 2023-08-03 19:45:19.000000 cospgd-0.1.1/cospgd.egg-info/SOURCES.txt
--rw-rw-r--   0 shashank  (1000) shashank  (1000)        1 2023-08-03 19:45:19.000000 cospgd-0.1.1/cospgd.egg-info/dependency_links.txt
--rw-rw-r--   0 shashank  (1000) shashank  (1000)       17 2023-08-03 19:45:19.000000 cospgd-0.1.1/cospgd.egg-info/requires.txt
--rw-rw-r--   0 shashank  (1000) shashank  (1000)        7 2023-08-03 19:45:19.000000 cospgd-0.1.1/cospgd.egg-info/top_level.txt
--rw-rw-r--   0 shashank  (1000) shashank  (1000)       38 2023-08-03 19:45:19.718332 cospgd-0.1.1/setup.cfg
--rw-rw-r--   0 shashank  (1000) shashank  (1000)     1207 2023-08-03 19:44:17.000000 cospgd-0.1.1/setup.py
+drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:50:21.027300 cospgd-0.1.2/
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)     1114 2023-08-03 16:40:23.000000 cospgd-0.1.2/LICENSE.md
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)     2865 2023-08-03 19:50:21.027300 cospgd-0.1.2/PKG-INFO
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)     1813 2023-08-03 16:23:45.000000 cospgd-0.1.2/README.md
+drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:50:21.027300 cospgd-0.1.2/cospgd/
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)      470 2023-08-03 17:23:15.000000 cospgd-0.1.2/cospgd/__init__.py
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)    11624 2023-08-03 19:37:49.000000 cospgd-0.1.2/cospgd/attack_implementations.py
+drwxrwxr-x   0 shashank  (1000) shashank  (1000)        0 2023-08-03 19:50:21.027300 cospgd-0.1.2/cospgd.egg-info/
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)     2865 2023-08-03 19:50:21.000000 cospgd-0.1.2/cospgd.egg-info/PKG-INFO
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)      230 2023-08-03 19:50:21.000000 cospgd-0.1.2/cospgd.egg-info/SOURCES.txt
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)        1 2023-08-03 19:50:21.000000 cospgd-0.1.2/cospgd.egg-info/dependency_links.txt
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)       17 2023-08-03 19:50:21.000000 cospgd-0.1.2/cospgd.egg-info/requires.txt
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)        7 2023-08-03 19:50:21.000000 cospgd-0.1.2/cospgd.egg-info/top_level.txt
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)       38 2023-08-03 19:50:21.027300 cospgd-0.1.2/setup.cfg
+-rw-rw-r--   0 shashank  (1000) shashank  (1000)     1423 2023-08-03 19:50:07.000000 cospgd-0.1.2/setup.py
```

### Comparing `cospgd-0.1.1/LICENSE.md` & `cospgd-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cospgd-0.1.1/README.md` & `cospgd-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cospgd-0.1.1/cospgd/attack_implementations.py` & `cospgd-0.1.2/cospgd/attack_implementations.py`

 * *Files identical despite different names*

### Comparing `cospgd-0.1.1/setup.py` & `cospgd-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from setuptools import setup
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cospgd',
-    version='0.1.1',    
+    version='0.1.2',    
     description='A tool for benchmarking adversarial robustness of pixel-wise prediction tasks.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     url='https://github.com/shashankskagnihotri/cospgd',
     author='Shashank Agnihotri, Steffen Jung, Prof. Dr. Margret Keuper',
     author_email='shashanksagnihotri@gmail.com',
     license='MIT',
     packages=['cospgd'],
     install_requires=['torch>=1.7',
                       'numpy',
```

