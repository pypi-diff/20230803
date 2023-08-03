# Comparing `tmp/RWAPIMicroservicePython-2.0.0.tar.gz` & `tmp/RWAPIMicroservicePython-3.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RWAPIMicroservicePython-2.0.0.tar", last modified: Thu Jan 19 05:58:54 2023, max compression
+gzip compressed data, was "RWAPIMicroservicePython-3.0.0b4.tar", last modified: Thu Aug  3 09:32:18 2023, max compression
```

## Comparing `RWAPIMicroservicePython-2.0.0.tar` & `RWAPIMicroservicePython-3.0.0b4.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-01-19 05:58:54.518782 RWAPIMicroservicePython-2.0.0/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-2.0.0/LICENSE
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      274 2023-01-19 05:58:54.518782 RWAPIMicroservicePython-2.0.0/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2321 2021-06-24 15:27:40.000000 RWAPIMicroservicePython-2.0.0/README.md
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-01-19 05:58:54.518782 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2554 2021-06-15 15:48:01.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython/__init__.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      243 2019-10-28 16:32:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython/errors.py
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-01-19 05:58:54.518782 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      274 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      376 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/SOURCES.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/dependency_links.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/not-zip-safe
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      206 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/requires.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-01-19 05:58:54.000000 RWAPIMicroservicePython-2.0.0/RWAPIMicroservicePython.egg-info/top_level.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-01-19 05:58:54.518782 RWAPIMicroservicePython-2.0.0/setup.cfg
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      844 2023-01-19 05:30:39.000000 RWAPIMicroservicePython-2.0.0/setup.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 09:32:18.140776 RWAPIMicroservicePython-3.0.0b4/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-3.0.0b4/LICENSE
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      364 2023-08-03 09:32:18.140776 RWAPIMicroservicePython-3.0.0b4/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2318 2023-07-31 11:34:02.000000 RWAPIMicroservicePython-3.0.0b4/README.md
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 09:32:18.140776 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      294 2023-08-03 09:29:42.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/__init__.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     3111 2023-08-01 12:50:17.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/cloudwatch.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      409 2023-07-31 16:10:42.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/errors.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     6590 2023-08-01 14:44:13.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/main.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1943 2023-08-03 09:21:00.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/test_utils.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 09:32:18.140776 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      364 2023-08-03 09:32:18.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      484 2023-08-03 09:32:18.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/SOURCES.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-03 09:32:18.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/dependency_links.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/not-zip-safe
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      171 2023-08-03 09:32:18.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/requires.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-08-03 09:32:18.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/top_level.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-08-03 09:32:18.140776 RWAPIMicroservicePython-3.0.0b4/setup.cfg
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      888 2023-08-03 09:31:54.000000 RWAPIMicroservicePython-3.0.0b4/setup.py
```

### Comparing `RWAPIMicroservicePython-2.0.0/LICENSE` & `RWAPIMicroservicePython-3.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-2.0.0/README.md` & `RWAPIMicroservicePython-3.0.0b4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 Library to register and integrate microservices in the [RW API](https://api.resourcewatch.org/).
 
 
 ## Requirements
 
 This library is tested to work with following Python versions:
-- 3.6+
-- 2.7 (legacy)
+- 3.11.4
+- 3.10.12
 
 Additionally, it requires the following Python libraries: 
 - Flask (tested with v1.1.1)
 - Requests
 
 ## Install
```

