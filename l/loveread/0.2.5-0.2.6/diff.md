# Comparing `tmp/loveread-0.2.5.tar.gz` & `tmp/loveread-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loveread-0.2.5.tar", last modified: Wed Aug  2 22:14:24 2023, max compression
+gzip compressed data, was "loveread-0.2.6.tar", last modified: Wed Aug  2 22:16:26 2023, max compression
```

## Comparing `loveread-0.2.5.tar` & `loveread-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:14:24.656806 loveread-0.2.5/
--rw-r--r--   0 shinsheel   (501) staff       (20)        7 2023-08-02 19:55:40.000000 loveread-0.2.5/LICENSE
--rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 22:14:24.656593 loveread-0.2.5/PKG-INFO
--rw-r--r--   0 shinsheel   (501) staff       (20)      313 2023-08-02 20:04:30.000000 loveread-0.2.5/README.md
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:14:24.655460 loveread-0.2.5/loveread/
--rw-r--r--   0 shinsheel   (501) staff       (20)       23 2023-08-02 22:13:40.000000 loveread-0.2.5/loveread/__init__.py
--rw-r--r--   0 shinsheel   (501) staff       (20)      272 2023-08-02 22:14:01.000000 loveread-0.2.5/loveread/__main__.py
--rw-r--r--   0 shinsheel   (501) staff       (20)     1247 2023-08-02 19:48:30.000000 loveread-0.2.5/loveread/loveread.py
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:14:24.656337 loveread-0.2.5/loveread.egg-info/
--rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 22:14:24.000000 loveread-0.2.5/loveread.egg-info/PKG-INFO
--rw-r--r--   0 shinsheel   (501) staff       (20)      217 2023-08-02 22:14:24.000000 loveread-0.2.5/loveread.egg-info/SOURCES.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)        1 2023-08-02 22:14:24.000000 loveread-0.2.5/loveread.egg-info/dependency_links.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)        9 2023-08-02 22:14:24.000000 loveread-0.2.5/loveread.egg-info/top_level.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)       38 2023-08-02 22:14:24.656856 loveread-0.2.5/setup.cfg
--rw-r--r--   0 shinsheel   (501) staff       (20)      596 2023-08-02 22:14:12.000000 loveread-0.2.5/setup.py
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:16:26.236889 loveread-0.2.6/
+-rw-r--r--   0 shinsheel   (501) staff       (20)        7 2023-08-02 19:55:40.000000 loveread-0.2.6/LICENSE
+-rw-r--r--   0 shinsheel   (501) staff       (20)      779 2023-08-02 22:16:26.236700 loveread-0.2.6/PKG-INFO
+-rw-r--r--   0 shinsheel   (501) staff       (20)      315 2023-08-02 22:16:01.000000 loveread-0.2.6/README.md
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:16:26.235745 loveread-0.2.6/loveread/
+-rw-r--r--   0 shinsheel   (501) staff       (20)       23 2023-08-02 22:13:40.000000 loveread-0.2.6/loveread/__init__.py
+-rw-r--r--   0 shinsheel   (501) staff       (20)      272 2023-08-02 22:14:01.000000 loveread-0.2.6/loveread/__main__.py
+-rw-r--r--   0 shinsheel   (501) staff       (20)     1247 2023-08-02 19:48:30.000000 loveread-0.2.6/loveread/loveread.py
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 22:16:26.236436 loveread-0.2.6/loveread.egg-info/
+-rw-r--r--   0 shinsheel   (501) staff       (20)      779 2023-08-02 22:16:26.000000 loveread-0.2.6/loveread.egg-info/PKG-INFO
+-rw-r--r--   0 shinsheel   (501) staff       (20)      217 2023-08-02 22:16:26.000000 loveread-0.2.6/loveread.egg-info/SOURCES.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        1 2023-08-02 22:16:26.000000 loveread-0.2.6/loveread.egg-info/dependency_links.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        9 2023-08-02 22:16:26.000000 loveread-0.2.6/loveread.egg-info/top_level.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)       38 2023-08-02 22:16:26.236939 loveread-0.2.6/setup.cfg
+-rw-r--r--   0 shinsheel   (501) staff       (20)      596 2023-08-02 22:16:11.000000 loveread-0.2.6/setup.py
```

### Comparing `loveread-0.2.5/PKG-INFO` & `loveread-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: loveread
-Version: 0.2.5
+Version: 0.2.6
 Summary: A brief description of your package
 Home-page: https://gitlab.com/wladgavrilov/loveread
 Author: Vlad Havrylov
 Author-email: wladgavrilov@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 * Install
 `pip3 install loveread`
 - Use through terminal
-`python3 -m loveread http://loveread.ec/read_book.php?id=PUT_BOOK_ID`
+`python3 -m loveread "http://loveread.ec/read_book.php?id=PUT_BOOK_ID"`
 * Through code
 `import loveread`
 `url = "http://loveread.ec/read_book.php?id={PUT_BOOK_ID}`
 `loveread.download(url)`
 
 * In both cases the book would appear as txt file in the same folder
```

### Comparing `loveread-0.2.5/loveread/loveread.py` & `loveread-0.2.6/loveread/loveread.py`

 * *Files identical despite different names*

### Comparing `loveread-0.2.5/loveread.egg-info/PKG-INFO` & `loveread-0.2.6/loveread.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: loveread
-Version: 0.2.5
+Version: 0.2.6
 Summary: A brief description of your package
 Home-page: https://gitlab.com/wladgavrilov/loveread
 Author: Vlad Havrylov
 Author-email: wladgavrilov@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 * Install
 `pip3 install loveread`
 - Use through terminal
-`python3 -m loveread http://loveread.ec/read_book.php?id=PUT_BOOK_ID`
+`python3 -m loveread "http://loveread.ec/read_book.php?id=PUT_BOOK_ID"`
 * Through code
 `import loveread`
 `url = "http://loveread.ec/read_book.php?id={PUT_BOOK_ID}`
 `loveread.download(url)`
 
 * In both cases the book would appear as txt file in the same folder
```

### Comparing `loveread-0.2.5/setup.py` & `loveread-0.2.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="loveread",
-    version="0.2.5",
+    version="0.2.6",
     author="Vlad Havrylov",
     author_email="wladgavrilov@gmail.com",
     description="A brief description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://gitlab.com/wladgavrilov/loveread",
     packages=['loveread'],
```

