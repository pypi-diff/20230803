# Comparing `tmp/aiohttp_client_rate_limiter-1.0.0.tar.gz` & `tmp/aiohttp_client_rate_limiter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_client_rate_limiter-1.0.0.tar", last modified: Thu Aug  3 00:43:42 2023, max compression
+gzip compressed data, was "aiohttp_client_rate_limiter-1.0.1.tar", last modified: Thu Aug  3 00:53:15 2023, max compression
```

## Comparing `aiohttp_client_rate_limiter-1.0.0.tar` & `aiohttp_client_rate_limiter-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:43:42.321232 aiohttp_client_rate_limiter-1.0.0/
--rw-r--r--   0 peterbigmac   (501) staff       (20)    11357 2023-07-31 07:45:41.000000 aiohttp_client_rate_limiter-1.0.0/LICENSE
--rw-r--r--   0 peterbigmac   (501) staff       (20)      539 2023-08-03 00:43:42.320832 aiohttp_client_rate_limiter-1.0.0/PKG-INFO
--rw-r--r--   0 peterbigmac   (501) staff       (20)       54 2023-07-31 07:45:41.000000 aiohttp_client_rate_limiter-1.0.0/README.md
-drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:43:42.318617 aiohttp_client_rate_limiter-1.0.0/aiohttp_client_rate_limiter.egg-info/
--rw-r--r--   0 peterbigmac   (501) staff       (20)      539 2023-08-03 00:43:42.000000 aiohttp_client_rate_limiter-1.0.0/aiohttp_client_rate_limiter.egg-info/PKG-INFO
--rw-r--r--   0 peterbigmac   (501) staff       (20)      351 2023-08-03 00:43:42.000000 aiohttp_client_rate_limiter-1.0.0/aiohttp_client_rate_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)        1 2023-08-03 00:43:42.000000 aiohttp_client_rate_limiter-1.0.0/aiohttp_client_rate_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)      150 2023-08-03 00:43:42.000000 aiohttp_client_rate_limiter-1.0.0/aiohttp_client_rate_limiter.egg-info/requires.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)       21 2023-08-03 00:43:42.000000 aiohttp_client_rate_limiter-1.0.0/aiohttp_client_rate_limiter.egg-info/top_level.txt
-drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:43:42.320081 aiohttp_client_rate_limiter-1.0.0/aiohttp_rate_limiter/
--rw-r--r--   0 peterbigmac   (501) staff       (20)     2842 2023-08-03 00:32:26.000000 aiohttp_client_rate_limiter-1.0.0/aiohttp_rate_limiter/ClientSession.py
--rw-r--r--   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:31:52.000000 aiohttp_client_rate_limiter-1.0.0/aiohttp_rate_limiter/__init__.py
--rw-r--r--   0 peterbigmac   (501) staff       (20)       38 2023-08-03 00:43:42.321385 aiohttp_client_rate_limiter-1.0.0/setup.cfg
--rw-r--r--   0 peterbigmac   (501) staff       (20)     1044 2023-08-03 00:43:31.000000 aiohttp_client_rate_limiter-1.0.0/setup.py
+drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:53:15.989146 aiohttp_client_rate_limiter-1.0.1/
+-rw-r--r--   0 peterbigmac   (501) staff       (20)    11357 2023-07-31 07:45:41.000000 aiohttp_client_rate_limiter-1.0.1/LICENSE
+-rw-r--r--   0 peterbigmac   (501) staff       (20)      539 2023-08-03 00:53:15.988783 aiohttp_client_rate_limiter-1.0.1/PKG-INFO
+-rw-r--r--   0 peterbigmac   (501) staff       (20)       54 2023-07-31 07:45:41.000000 aiohttp_client_rate_limiter-1.0.1/README.md
+drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:53:15.985128 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter/
+-rw-r--r--   0 peterbigmac   (501) staff       (20)     2842 2023-08-03 00:32:26.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter/ClientSession.py
+-rw-r--r--   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:31:52.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter/__init__.py
+drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:53:15.987945 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/
+-rw-r--r--   0 peterbigmac   (501) staff       (20)      539 2023-08-03 00:53:15.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 peterbigmac   (501) staff       (20)      365 2023-08-03 00:53:15.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbigmac   (501) staff       (20)        1 2023-08-03 00:53:15.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbigmac   (501) staff       (20)      150 2023-08-03 00:53:15.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/requires.txt
+-rw-r--r--   0 peterbigmac   (501) staff       (20)       28 2023-08-03 00:53:15.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/top_level.txt
+-rw-r--r--   0 peterbigmac   (501) staff       (20)       38 2023-08-03 00:53:15.989264 aiohttp_client_rate_limiter-1.0.1/setup.cfg
+-rw-r--r--   0 peterbigmac   (501) staff       (20)     1051 2023-08-03 00:47:25.000000 aiohttp_client_rate_limiter-1.0.1/setup.py
```

### Comparing `aiohttp_client_rate_limiter-1.0.0/LICENSE` & `aiohttp_client_rate_limiter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_client_rate_limiter-1.0.0/PKG-INFO` & `aiohttp_client_rate_limiter-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp_client_rate_limiter
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is a mini tool that overwrite aiohttp session to provide rate limit function within a same session.
 Home-page: https://github.com/PeterBunBun/aiohttp_rate_limiter
 Author: Peter Lee
 Author-email: info@peterlee.space
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `aiohttp_client_rate_limiter-1.0.0/aiohttp_client_rate_limiter.egg-info/PKG-INFO` & `aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-client-rate-limiter
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is a mini tool that overwrite aiohttp session to provide rate limit function within a same session.
 Home-page: https://github.com/PeterBunBun/aiohttp_rate_limiter
 Author: Peter Lee
 Author-email: info@peterlee.space
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `aiohttp_client_rate_limiter-1.0.0/aiohttp_rate_limiter/ClientSession.py` & `aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter/ClientSession.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_rate_limiter-1.0.0/setup.py` & `aiohttp_client_rate_limiter-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 setup(
     name='aiohttp_client_rate_limiter',
-    version='1.0.0',
+    version='1.0.1',
     description='This is a mini tool that overwrite aiohttp session to provide rate limit function within a same session.',
     long_description='This is a mini tool that overwrite aiohttp session to provide rate limit function within a same session.',
     author='Peter Lee',
     author_email='info@peterlee.space',
     url='https://github.com/PeterBunBun/aiohttp_rate_limiter',
-    packages=['aiohttp_rate_limiter'],
+    packages=['aiohttp_client_rate_limiter'],
     install_requires=[
         # List any dependencies required by your package
         "aiohttp>=3.8.5",
         "aiosignal>=1.3.1",
         "async-timeout==4.0.2",
         "attrs==23.1.0",
         "charset-normalizer==3.2.0",
```

