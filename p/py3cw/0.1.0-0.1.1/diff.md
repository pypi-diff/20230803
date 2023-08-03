# Comparing `tmp/py3cw-0.1.0.tar.gz` & `tmp/py3cw-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3cw-0.1.0.tar", last modified: Fri Jul 21 07:50:41 2023, max compression
+gzip compressed data, was "py3cw-0.1.1.tar", last modified: Thu Aug  3 11:53:26 2023, max compression
```

## Comparing `py3cw-0.1.0.tar` & `py3cw-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:50:41.608322 py3cw-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-21 07:50:31.000000 py3cw-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:50:41.608322 py3cw-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-21 07:50:31.000000 py3cw-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:50:41.604322 py3cw-0.1.0/py3cw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:50:31.000000 py3cw-0.1.0/py3cw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-21 07:50:31.000000 py3cw-0.1.0/py3cw/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-21 07:50:31.000000 py3cw-0.1.0/py3cw/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-21 07:50:31.000000 py3cw-0.1.0/py3cw/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-21 07:50:31.000000 py3cw-0.1.0/py3cw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:50:41.604322 py3cw-0.1.0/py3cw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:50:41.000000 py3cw-0.1.0/py3cw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-21 07:50:41.000000 py3cw-0.1.0/py3cw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:50:41.000000 py3cw-0.1.0/py3cw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 07:50:41.000000 py3cw-0.1.0/py3cw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 07:50:41.000000 py3cw-0.1.0/py3cw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:50:41.608322 py3cw-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-21 07:50:31.000000 py3cw-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:26.006237 py3cw-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-03 11:53:09.000000 py3cw-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-03 11:53:26.006237 py3cw-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-08-03 11:53:09.000000 py3cw-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:26.002237 py3cw-0.1.1/py3cw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:09.000000 py3cw-0.1.1/py3cw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-08-03 11:53:09.000000 py3cw-0.1.1/py3cw/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-08-03 11:53:09.000000 py3cw-0.1.1/py3cw/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-03 11:53:09.000000 py3cw-0.1.1/py3cw/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-03 11:53:09.000000 py3cw-0.1.1/py3cw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:53:26.002237 py3cw-0.1.1/py3cw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-03 11:53:25.000000 py3cw-0.1.1/py3cw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-03 11:53:25.000000 py3cw-0.1.1/py3cw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:53:25.000000 py3cw-0.1.1/py3cw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 11:53:25.000000 py3cw-0.1.1/py3cw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 11:53:25.000000 py3cw-0.1.1/py3cw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:53:26.006237 py3cw-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-03 11:53:09.000000 py3cw-0.1.1/setup.py
```

### Comparing `py3cw-0.1.0/LICENSE` & `py3cw-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py3cw-0.1.0/README.md` & `py3cw-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py3cw-0.1.0/py3cw/config.py` & `py3cw-0.1.1/py3cw/config.py`

 * *Files identical despite different names*

### Comparing `py3cw-0.1.0/py3cw/request.py` & `py3cw-0.1.1/py3cw/request.py`

 * *Files identical despite different names*

### Comparing `py3cw-0.1.0/py3cw/test_request.py` & `py3cw-0.1.1/py3cw/test_request.py`

 * *Files identical despite different names*

### Comparing `py3cw-0.1.0/py3cw/utils.py` & `py3cw-0.1.1/py3cw/utils.py`

 * *Files identical despite different names*

### Comparing `py3cw-0.1.0/setup.py` & `py3cw-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='py3cw',
-    version='0.1.0',
+    version='0.1.1',
 
     description='3commas Python wrapper',
 
     url='https://github.com/bogdanteodoru/py3cw',
 
     author='Bogdan Teodoru',
     author_email='me@bogdanteodoru.com',
@@ -19,9 +19,10 @@
 
     keywords='api 3commas trading crypto bitcoin altcoin',
 
     packages=find_packages(exclude=['tests']),
 
     install_requires=[
         'requests',
+        'pycryptodome',
     ],
 )
```

