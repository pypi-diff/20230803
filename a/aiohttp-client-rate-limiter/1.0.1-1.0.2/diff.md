# Comparing `tmp/aiohttp_client_rate_limiter-1.0.1.tar.gz` & `tmp/aiohttp_client_rate_limiter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_client_rate_limiter-1.0.1.tar", last modified: Thu Aug  3 00:53:15 2023, max compression
+gzip compressed data, was "aiohttp_client_rate_limiter-1.0.2.tar", last modified: Thu Aug  3 00:56:37 2023, max compression
```

## Comparing `aiohttp_client_rate_limiter-1.0.1.tar` & `aiohttp_client_rate_limiter-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:53:15.989146 aiohttp_client_rate_limiter-1.0.1/
--rw-r--r--   0 peterbigmac   (501) staff       (20)    11357 2023-07-31 07:45:41.000000 aiohttp_client_rate_limiter-1.0.1/LICENSE
--rw-r--r--   0 peterbigmac   (501) staff       (20)      539 2023-08-03 00:53:15.988783 aiohttp_client_rate_limiter-1.0.1/PKG-INFO
--rw-r--r--   0 peterbigmac   (501) staff       (20)       54 2023-07-31 07:45:41.000000 aiohttp_client_rate_limiter-1.0.1/README.md
-drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:53:15.985128 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter/
--rw-r--r--   0 peterbigmac   (501) staff       (20)     2842 2023-08-03 00:32:26.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter/ClientSession.py
--rw-r--r--   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:31:52.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter/__init__.py
-drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:53:15.987945 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/
--rw-r--r--   0 peterbigmac   (501) staff       (20)      539 2023-08-03 00:53:15.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/PKG-INFO
--rw-r--r--   0 peterbigmac   (501) staff       (20)      365 2023-08-03 00:53:15.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)        1 2023-08-03 00:53:15.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)      150 2023-08-03 00:53:15.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/requires.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)       28 2023-08-03 00:53:15.000000 aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/top_level.txt
--rw-r--r--   0 peterbigmac   (501) staff       (20)       38 2023-08-03 00:53:15.989264 aiohttp_client_rate_limiter-1.0.1/setup.cfg
--rw-r--r--   0 peterbigmac   (501) staff       (20)     1051 2023-08-03 00:47:25.000000 aiohttp_client_rate_limiter-1.0.1/setup.py
+drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:56:37.248962 aiohttp_client_rate_limiter-1.0.2/
+-rw-r--r--   0 peterbigmac   (501) staff       (20)    11357 2023-07-31 07:45:41.000000 aiohttp_client_rate_limiter-1.0.2/LICENSE
+-rw-r--r--   0 peterbigmac   (501) staff       (20)      543 2023-08-03 00:56:37.248290 aiohttp_client_rate_limiter-1.0.2/PKG-INFO
+-rw-r--r--   0 peterbigmac   (501) staff       (20)       54 2023-07-31 07:45:41.000000 aiohttp_client_rate_limiter-1.0.2/README.md
+drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:56:37.242601 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter/
+-rw-r--r--   0 peterbigmac   (501) staff       (20)     2842 2023-08-03 00:32:26.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter/ClientSession.py
+-rw-r--r--   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:31:52.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter/__init__.py
+drwxr-xr-x   0 peterbigmac   (501) staff       (20)        0 2023-08-03 00:56:37.246920 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/
+-rw-r--r--   0 peterbigmac   (501) staff       (20)      543 2023-08-03 00:56:37.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 peterbigmac   (501) staff       (20)      365 2023-08-03 00:56:37.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbigmac   (501) staff       (20)        1 2023-08-03 00:56:37.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbigmac   (501) staff       (20)      150 2023-08-03 00:56:37.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/requires.txt
+-rw-r--r--   0 peterbigmac   (501) staff       (20)       28 2023-08-03 00:56:37.000000 aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/top_level.txt
+-rw-r--r--   0 peterbigmac   (501) staff       (20)       38 2023-08-03 00:56:37.249171 aiohttp_client_rate_limiter-1.0.2/setup.cfg
+-rw-r--r--   0 peterbigmac   (501) staff       (20)     1055 2023-08-03 00:56:33.000000 aiohttp_client_rate_limiter-1.0.2/setup.py
```

### Comparing `aiohttp_client_rate_limiter-1.0.1/LICENSE` & `aiohttp_client_rate_limiter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_client_rate_limiter-1.0.1/PKG-INFO` & `aiohttp_client_rate_limiter-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aiohttp_client_rate_limiter
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is a mini tool that overwrite aiohttp session to provide rate limit function within a same session.
-Home-page: https://github.com/PeterBunBun/aiohttp_rate_limiter
+Home-page: https://github.com/peteropensource/aiohttp_rate_limiter
 Author: Peter Lee
 Author-email: info@peterlee.space
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 This is a mini tool that overwrite aiohttp session to provide rate limit function within a same session.
```

### Comparing `aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter/ClientSession.py` & `aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter/ClientSession.py`

 * *Files identical despite different names*

### Comparing `aiohttp_client_rate_limiter-1.0.1/aiohttp_client_rate_limiter.egg-info/PKG-INFO` & `aiohttp_client_rate_limiter-1.0.2/aiohttp_client_rate_limiter.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aiohttp-client-rate-limiter
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is a mini tool that overwrite aiohttp session to provide rate limit function within a same session.
-Home-page: https://github.com/PeterBunBun/aiohttp_rate_limiter
+Home-page: https://github.com/peteropensource/aiohttp_rate_limiter
 Author: Peter Lee
 Author-email: info@peterlee.space
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 This is a mini tool that overwrite aiohttp session to provide rate limit function within a same session.
```

### Comparing `aiohttp_client_rate_limiter-1.0.1/setup.py` & `aiohttp_client_rate_limiter-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 setup(
     name='aiohttp_client_rate_limiter',
-    version='1.0.1',
+    version='1.0.2',
     description='This is a mini tool that overwrite aiohttp session to provide rate limit function within a same session.',
     long_description='This is a mini tool that overwrite aiohttp session to provide rate limit function within a same session.',
     author='Peter Lee',
     author_email='info@peterlee.space',
-    url='https://github.com/PeterBunBun/aiohttp_rate_limiter',
+    url='https://github.com/peteropensource/aiohttp_rate_limiter',
     packages=['aiohttp_client_rate_limiter'],
     install_requires=[
         # List any dependencies required by your package
         "aiohttp>=3.8.5",
         "aiosignal>=1.3.1",
         "async-timeout==4.0.2",
         "attrs==23.1.0",
```

