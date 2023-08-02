# Comparing `tmp/loveread-0.2.6.tar.gz` & `tmp/loveread-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loveread-0.2.6.tar", last modified: Wed Aug  2 22:16:26 2023, max compression
+gzip compressed data, was "loveread-0.2.7.tar", last modified: Wed Aug  2 22:21:30 2023, max compression
```

## Comparing `loveread-0.2.6.tar` & `loveread-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:16:26.236889 loveread-0.2.6/
--rw-r--r--   0 shinsheel   (501) staff       (20)        7 2023-08-02 19:55:40.000000 loveread-0.2.6/LICENSE
--rw-r--r--   0 shinsheel   (501) staff       (20)      779 2023-08-02 22:16:26.236700 loveread-0.2.6/PKG-INFO
--rw-r--r--   0 shinsheel   (501) staff       (20)      315 2023-08-02 22:16:01.000000 loveread-0.2.6/README.md
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:16:26.235745 loveread-0.2.6/loveread/
--rw-r--r--   0 shinsheel   (501) staff       (20)       23 2023-08-02 22:13:40.000000 loveread-0.2.6/loveread/__init__.py
--rw-r--r--   0 shinsheel   (501) staff       (20)      272 2023-08-02 22:14:01.000000 loveread-0.2.6/loveread/__main__.py
--rw-r--r--   0 shinsheel   (501) staff       (20)     1247 2023-08-02 19:48:30.000000 loveread-0.2.6/loveread/loveread.py
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:16:26.236436 loveread-0.2.6/loveread.egg-info/
--rw-r--r--   0 shinsheel   (501) staff       (20)      779 2023-08-02 22:16:26.000000 loveread-0.2.6/loveread.egg-info/PKG-INFO
--rw-r--r--   0 shinsheel   (501) staff       (20)      217 2023-08-02 22:16:26.000000 loveread-0.2.6/loveread.egg-info/SOURCES.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)        1 2023-08-02 22:16:26.000000 loveread-0.2.6/loveread.egg-info/dependency_links.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)        9 2023-08-02 22:16:26.000000 loveread-0.2.6/loveread.egg-info/top_level.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)       38 2023-08-02 22:16:26.236939 loveread-0.2.6/setup.cfg
--rw-r--r--   0 shinsheel   (501) staff       (20)      596 2023-08-02 22:16:11.000000 loveread-0.2.6/setup.py
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:21:30.595475 loveread-0.2.7/
+-rw-r--r--   0 shinsheel   (501) staff       (20)        7 2023-08-02 19:55:40.000000 loveread-0.2.7/LICENSE
+-rw-r--r--   0 shinsheel   (501) staff       (20)      779 2023-08-02 22:21:30.595151 loveread-0.2.7/PKG-INFO
+-rw-r--r--   0 shinsheel   (501) staff       (20)      315 2023-08-02 22:16:01.000000 loveread-0.2.7/README.md
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:21:30.592402 loveread-0.2.7/loveread/
+-rw-r--r--   0 shinsheel   (501) staff       (20)       23 2023-08-02 22:13:40.000000 loveread-0.2.7/loveread/__init__.py
+-rw-r--r--   0 shinsheel   (501) staff       (20)      272 2023-08-02 22:14:01.000000 loveread-0.2.7/loveread/__main__.py
+-rw-r--r--   0 shinsheel   (501) staff       (20)     1247 2023-08-02 19:48:30.000000 loveread-0.2.7/loveread/loveread.py
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:21:30.594875 loveread-0.2.7/loveread.egg-info/
+-rw-r--r--   0 shinsheel   (501) staff       (20)      779 2023-08-02 22:21:30.000000 loveread-0.2.7/loveread.egg-info/PKG-INFO
+-rw-r--r--   0 shinsheel   (501) staff       (20)      248 2023-08-02 22:21:30.000000 loveread-0.2.7/loveread.egg-info/SOURCES.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        1 2023-08-02 22:21:30.000000 loveread-0.2.7/loveread.egg-info/dependency_links.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        4 2023-08-02 22:21:30.000000 loveread-0.2.7/loveread.egg-info/requires.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        9 2023-08-02 22:21:30.000000 loveread-0.2.7/loveread.egg-info/top_level.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)       38 2023-08-02 22:21:30.595542 loveread-0.2.7/setup.cfg
+-rw-r--r--   0 shinsheel   (501) staff       (20)      626 2023-08-02 22:21:25.000000 loveread-0.2.7/setup.py
```

### Comparing `loveread-0.2.6/PKG-INFO` & `loveread-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loveread
-Version: 0.2.6
+Version: 0.2.7
 Summary: A brief description of your package
 Home-page: https://gitlab.com/wladgavrilov/loveread
 Author: Vlad Havrylov
 Author-email: wladgavrilov@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `loveread-0.2.6/loveread/loveread.py` & `loveread-0.2.7/loveread/loveread.py`

 * *Files identical despite different names*

### Comparing `loveread-0.2.6/loveread.egg-info/PKG-INFO` & `loveread-0.2.7/loveread.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loveread
-Version: 0.2.6
+Version: 0.2.7
 Summary: A brief description of your package
 Home-page: https://gitlab.com/wladgavrilov/loveread
 Author: Vlad Havrylov
 Author-email: wladgavrilov@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `loveread-0.2.6/setup.py` & `loveread-0.2.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup
 
 setup(
     name="loveread",
-    version="0.2.6",
+    version="0.2.7",
     author="Vlad Havrylov",
     author_email="wladgavrilov@gmail.com",
     description="A brief description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://gitlab.com/wladgavrilov/loveread",
     packages=['loveread'],
+    install_requires=["bs4"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
     ],
 )
```

