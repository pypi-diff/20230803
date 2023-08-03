# Comparing `tmp/RWAPIMicroservicePython-3.0.0b2.tar.gz` & `tmp/RWAPIMicroservicePython-3.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RWAPIMicroservicePython-3.0.0b2.tar", last modified: Wed Aug  2 08:02:51 2023, max compression
+gzip compressed data, was "RWAPIMicroservicePython-3.0.0b3.tar", last modified: Thu Aug  3 08:42:41 2023, max compression
```

## Comparing `RWAPIMicroservicePython-3.0.0b2.tar` & `RWAPIMicroservicePython-3.0.0b3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-02 08:02:51.166221 RWAPIMicroservicePython-3.0.0b2/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-3.0.0b2/LICENSE
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      276 2023-08-02 08:02:51.166221 RWAPIMicroservicePython-3.0.0b2/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2318 2023-07-31 11:34:02.000000 RWAPIMicroservicePython-3.0.0b2/README.md
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-02 08:02:51.166221 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      223 2023-08-01 11:02:35.000000 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython/__init__.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     3111 2023-08-01 12:50:17.000000 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython/cloudwatch.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      409 2023-07-31 16:10:42.000000 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython/errors.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     6590 2023-08-01 14:44:13.000000 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython/main.py
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-02 08:02:51.166221 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython.egg-info/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      276 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython.egg-info/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      446 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython.egg-info/SOURCES.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython.egg-info/dependency_links.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython.egg-info/not-zip-safe
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      171 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython.egg-info/requires.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython.egg-info/top_level.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-08-02 08:02:51.166221 RWAPIMicroservicePython-3.0.0b2/setup.cfg
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      766 2023-08-02 08:00:56.000000 RWAPIMicroservicePython-3.0.0b2/setup.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 08:42:41.738542 RWAPIMicroservicePython-3.0.0b3/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-3.0.0b3/LICENSE
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      364 2023-08-03 08:42:41.735209 RWAPIMicroservicePython-3.0.0b3/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2318 2023-07-31 11:34:02.000000 RWAPIMicroservicePython-3.0.0b3/README.md
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 08:42:41.735209 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      295 2023-08-03 08:22:35.000000 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython/__init__.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     3111 2023-08-01 12:50:17.000000 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython/cloudwatch.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      409 2023-07-31 16:10:42.000000 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython/errors.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     6590 2023-08-01 14:44:13.000000 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython/main.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 08:42:41.735209 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython.egg-info/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      364 2023-08-03 08:42:41.000000 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython.egg-info/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      446 2023-08-03 08:42:41.000000 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython.egg-info/SOURCES.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-03 08:42:41.000000 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython.egg-info/dependency_links.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython.egg-info/not-zip-safe
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      171 2023-08-03 08:42:41.000000 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython.egg-info/requires.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-08-03 08:42:41.000000 RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython.egg-info/top_level.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-08-03 08:42:41.738542 RWAPIMicroservicePython-3.0.0b3/setup.cfg
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      888 2023-08-03 08:42:38.000000 RWAPIMicroservicePython-3.0.0b3/setup.py
```

### Comparing `RWAPIMicroservicePython-3.0.0b2/LICENSE` & `RWAPIMicroservicePython-3.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b2/README.md` & `RWAPIMicroservicePython-3.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython/cloudwatch.py` & `RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b2/RWAPIMicroservicePython/main.py` & `RWAPIMicroservicePython-3.0.0b3/RWAPIMicroservicePython/main.py`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b2/setup.py` & `RWAPIMicroservicePython-3.0.0b3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from setuptools import setup
 
 setup(name='RWAPIMicroservicePython',
-      version='3.0.0-beta.2',
+      version='3.0.0-beta.3',
+      long_description='Python integration library for the RW API microservices',
       description='Python integration library for the RW API microservices',
+      long_description_content_type='text',
       author='Vizzuality',
       author_email='info@vizzuality.com',
       url='https://vizzuality.com',
       license='MIT',
       packages=['RWAPIMicroservicePython'],
       install_requires=[
+        'boto3==1.28.16',
         'Flask<=2.3.2',
         'requests<=2.31',
       ],
       extras_require={
         'dev': [
-            'boto3==1.28.16',
             'codecov==2.1.13',
             'Flask==2.3.2',
             'moto[logs]==4.1.4',
             'pytest==7.4.0',
             'pytest-cov==4.1.0',
             'pytest-mock==3.11.1',
             'requests_mock==1.11.0',
```

