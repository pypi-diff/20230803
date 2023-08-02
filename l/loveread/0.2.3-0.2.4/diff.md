# Comparing `tmp/loveread-0.2.3.tar.gz` & `tmp/loveread-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loveread-0.2.3.tar", last modified: Wed Aug  2 20:16:31 2023, max compression
+gzip compressed data, was "loveread-0.2.4.tar", last modified: Wed Aug  2 22:08:36 2023, max compression
```

## Comparing `loveread-0.2.3.tar` & `loveread-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:16:31.458116 loveread-0.2.3/
--rw-r--r--   0 shinsheel   (501) staff       (20)        7 2023-08-02 19:55:40.000000 loveread-0.2.3/LICENSE
--rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 20:16:31.457946 loveread-0.2.3/PKG-INFO
--rw-r--r--   0 shinsheel   (501) staff       (20)      313 2023-08-02 20:04:30.000000 loveread-0.2.3/README.md
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:16:31.456969 loveread-0.2.3/loveread/
--rw-r--r--   0 shinsheel   (501) staff       (20)       17 2023-08-02 20:15:08.000000 loveread-0.2.3/loveread/__init__.py
--rw-r--r--   0 shinsheel   (501) staff       (20)      266 2023-08-02 20:15:05.000000 loveread-0.2.3/loveread/__main__.py
--rw-r--r--   0 shinsheel   (501) staff       (20)     1247 2023-08-02 19:48:30.000000 loveread-0.2.3/loveread/lib.py
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:16:31.457725 loveread-0.2.3/loveread.egg-info/
--rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 20:16:31.000000 loveread-0.2.3/loveread.egg-info/PKG-INFO
--rw-r--r--   0 shinsheel   (501) staff       (20)      212 2023-08-02 20:16:31.000000 loveread-0.2.3/loveread.egg-info/SOURCES.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)        1 2023-08-02 20:16:31.000000 loveread-0.2.3/loveread.egg-info/dependency_links.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)        9 2023-08-02 20:16:31.000000 loveread-0.2.3/loveread.egg-info/top_level.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)       38 2023-08-02 20:16:31.458175 loveread-0.2.3/setup.cfg
--rw-r--r--   0 shinsheel   (501) staff       (20)      596 2023-08-02 20:16:25.000000 loveread-0.2.3/setup.py
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:08:36.033490 loveread-0.2.4/
+-rw-r--r--   0 shinsheel   (501) staff       (20)        7 2023-08-02 19:55:40.000000 loveread-0.2.4/LICENSE
+-rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 22:08:36.033299 loveread-0.2.4/PKG-INFO
+-rw-r--r--   0 shinsheel   (501) staff       (20)      313 2023-08-02 20:04:30.000000 loveread-0.2.4/README.md
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:08:36.032285 loveread-0.2.4/loveread/
+-rw-r--r--   0 shinsheel   (501) staff       (20)      271 2023-08-02 22:08:27.000000 loveread-0.2.4/loveread/__init__.py
+-rw-r--r--   0 shinsheel   (501) staff       (20)     1247 2023-08-02 19:48:30.000000 loveread-0.2.4/loveread/loveread.py
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:08:36.033047 loveread-0.2.4/loveread.egg-info/
+-rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 22:08:35.000000 loveread-0.2.4/loveread.egg-info/PKG-INFO
+-rw-r--r--   0 shinsheel   (501) staff       (20)      196 2023-08-02 22:08:35.000000 loveread-0.2.4/loveread.egg-info/SOURCES.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        1 2023-08-02 22:08:35.000000 loveread-0.2.4/loveread.egg-info/dependency_links.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        9 2023-08-02 22:08:35.000000 loveread-0.2.4/loveread.egg-info/top_level.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)       38 2023-08-02 22:08:36.033541 loveread-0.2.4/setup.cfg
+-rw-r--r--   0 shinsheel   (501) staff       (20)      596 2023-08-02 22:08:32.000000 loveread-0.2.4/setup.py
```

### Comparing `loveread-0.2.3/PKG-INFO` & `loveread-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loveread
-Version: 0.2.3
+Version: 0.2.4
 Summary: A brief description of your package
 Home-page: https://gitlab.com/wladgavrilov/loveread
 Author: Vlad Havrylov
 Author-email: wladgavrilov@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `loveread-0.2.3/loveread/lib.py` & `loveread-0.2.4/loveread/loveread.py`

 * *Files identical despite different names*

### Comparing `loveread-0.2.3/loveread.egg-info/PKG-INFO` & `loveread-0.2.4/loveread.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loveread
-Version: 0.2.3
+Version: 0.2.4
 Summary: A brief description of your package
 Home-page: https://gitlab.com/wladgavrilov/loveread
 Author: Vlad Havrylov
 Author-email: wladgavrilov@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `loveread-0.2.3/setup.py` & `loveread-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="loveread",
-    version="0.2.3",
+    version="0.2.4",
     author="Vlad Havrylov",
     author_email="wladgavrilov@gmail.com",
     description="A brief description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://gitlab.com/wladgavrilov/loveread",
     packages=['loveread'],
```

