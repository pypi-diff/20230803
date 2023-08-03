# Comparing `tmp/lazymedia-0.0.2.tar.gz` & `tmp/lazymedia-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazymedia-0.0.2.tar", last modified: Tue Mar  7 15:54:40 2023, max compression
+gzip compressed data, was "lazymedia-0.0.3.tar", last modified: Thu Aug  3 02:41:43 2023, max compression
```

## Comparing `lazymedia-0.0.2.tar` & `lazymedia-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-03-07 15:54:40.973805 lazymedia-0.0.2/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      254 2023-03-07 15:54:40.973697 lazymedia-0.0.2/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      908 2023-03-07 14:18:50.000000 lazymedia-0.0.2/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-03-07 15:54:40.972780 lazymedia-0.0.2/lazymedia/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      226 2023-03-07 15:53:30.000000 lazymedia-0.0.2/lazymedia/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1219 2023-03-07 14:18:50.000000 lazymedia-0.0.2/lazymedia/ixigua.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4500 2023-03-07 15:53:30.000000 lazymedia-0.0.2/lazymedia/youtube.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-03-07 15:54:40.973520 lazymedia-0.0.2/lazymedia.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      254 2023-03-07 15:54:40.000000 lazymedia-0.0.2/lazymedia.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      245 2023-03-07 15:54:40.000000 lazymedia-0.0.2/lazymedia.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-03-07 15:54:40.000000 lazymedia-0.0.2/lazymedia.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-03-07 15:54:40.000000 lazymedia-0.0.2/lazymedia.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-03-07 15:54:40.000000 lazymedia-0.0.2/lazymedia.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-03-07 15:54:40.973875 lazymedia-0.0.2/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      849 2023-03-07 15:53:30.000000 lazymedia-0.0.2/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-03 02:41:43.392636 lazymedia-0.0.3/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      254 2023-08-03 02:41:43.392522 lazymedia-0.0.3/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      908 2023-03-07 14:18:50.000000 lazymedia-0.0.3/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-03 02:41:43.391691 lazymedia-0.0.3/lazymedia/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      226 2023-03-07 15:53:30.000000 lazymedia-0.0.3/lazymedia/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      827 2023-03-15 05:10:08.000000 lazymedia-0.0.3/lazymedia/castbox.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1219 2023-03-07 14:18:50.000000 lazymedia-0.0.3/lazymedia/ixigua.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5944 2023-08-03 02:40:55.000000 lazymedia-0.0.3/lazymedia/youtube.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-08-03 02:41:43.392352 lazymedia-0.0.3/lazymedia.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      254 2023-08-03 02:41:43.000000 lazymedia-0.0.3/lazymedia.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      266 2023-08-03 02:41:43.000000 lazymedia-0.0.3/lazymedia.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-08-03 02:41:43.000000 lazymedia-0.0.3/lazymedia.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-08-03 02:41:43.000000 lazymedia-0.0.3/lazymedia.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-08-03 02:41:43.000000 lazymedia-0.0.3/lazymedia.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-08-03 02:41:43.392687 lazymedia-0.0.3/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      849 2023-08-03 02:41:22.000000 lazymedia-0.0.3/setup.py
```

### Comparing `lazymedia-0.0.2/README.md` & `lazymedia-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lazymedia-0.0.2/lazymedia/ixigua.py` & `lazymedia-0.0.3/lazymedia/ixigua.py`

 * *Files identical despite different names*

### Comparing `lazymedia-0.0.2/setup.py` & `lazymedia-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazymedia",
-    version="0.0.2",
+    version="0.0.3",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/lazymedia",
     packages=setuptools.find_packages(),
```

