# Comparing `tmp/pycasatunes-0.1.3.tar.gz` & `tmp/pycasatunes-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycasatunes-0.1.3.tar", max compression
+gzip compressed data, was "pycasatunes-0.1.4.tar", max compression
```

## Comparing `pycasatunes-0.1.3.tar` & `pycasatunes-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      722 2023-05-09 12:08:10.310945 pycasatunes-0.1.3/README.md
--rw-r--r--   0        0        0     8123 2023-07-27 19:17:54.326603 pycasatunes-0.1.3/pycasatunes/__init__.py
--rw-r--r--   0        0        0     1678 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/client.py
--rw-r--r--   0        0        0       43 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/const.py
--rw-r--r--   0        0        0      106 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/exceptions.py
--rw-r--r--   0        0        0       25 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/__init__.py
--rw-r--r--   0        0        0      462 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/base.py
--rw-r--r--   0        0        0     3242 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/media.py
--rw-r--r--   0        0        0     7608 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/nowplaying.py
--rw-r--r--   0        0        0     1000 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/source.py
--rw-r--r--   0        0        0     3530 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/system.py
--rw-r--r--   0        0        0     4915 2023-05-09 12:08:10.314278 pycasatunes-0.1.3/pycasatunes/objects/zone.py
--rw-r--r--   0        0        0      735 2023-07-27 19:19:11.106600 pycasatunes-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 pycasatunes-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      722 2023-05-09 12:08:10.310945 pycasatunes-0.1.4/README.md
+-rw-r--r--   0        0        0    10215 2023-08-03 16:55:44.654452 pycasatunes-0.1.4/pycasatunes/__init__.py
+-rw-r--r--   0        0        0     1678 2023-05-09 12:08:10.314278 pycasatunes-0.1.4/pycasatunes/client.py
+-rw-r--r--   0        0        0       43 2023-05-09 12:08:10.314278 pycasatunes-0.1.4/pycasatunes/const.py
+-rw-r--r--   0        0        0      106 2023-05-09 12:08:10.314278 pycasatunes-0.1.4/pycasatunes/exceptions.py
+-rw-r--r--   0        0        0       25 2023-05-09 12:08:10.314278 pycasatunes-0.1.4/pycasatunes/objects/__init__.py
+-rw-r--r--   0        0        0      462 2023-05-09 12:08:10.314278 pycasatunes-0.1.4/pycasatunes/objects/base.py
+-rw-r--r--   0        0        0     3242 2023-05-09 12:08:10.314278 pycasatunes-0.1.4/pycasatunes/objects/media.py
+-rw-r--r--   0        0        0     7608 2023-05-09 12:08:10.314278 pycasatunes-0.1.4/pycasatunes/objects/nowplaying.py
+-rw-r--r--   0        0        0     1000 2023-05-09 12:08:10.314278 pycasatunes-0.1.4/pycasatunes/objects/source.py
+-rw-r--r--   0        0        0     3530 2023-05-09 12:08:10.314278 pycasatunes-0.1.4/pycasatunes/objects/system.py
+-rw-r--r--   0        0        0     4915 2023-05-09 12:08:10.314278 pycasatunes-0.1.4/pycasatunes/objects/zone.py
+-rw-r--r--   0        0        0      735 2023-08-03 16:55:22.071119 pycasatunes-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 pycasatunes-0.1.4/PKG-INFO
```

### Comparing `pycasatunes-0.1.3/README.md` & `pycasatunes-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.3/pycasatunes/client.py` & `pycasatunes-0.1.4/pycasatunes/client.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.3/pycasatunes/objects/media.py` & `pycasatunes-0.1.4/pycasatunes/objects/media.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.3/pycasatunes/objects/nowplaying.py` & `pycasatunes-0.1.4/pycasatunes/objects/nowplaying.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.3/pycasatunes/objects/source.py` & `pycasatunes-0.1.4/pycasatunes/objects/source.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.3/pycasatunes/objects/system.py` & `pycasatunes-0.1.4/pycasatunes/objects/system.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.3/pycasatunes/objects/zone.py` & `pycasatunes-0.1.4/pycasatunes/objects/zone.py`

 * *Files identical despite different names*

### Comparing `pycasatunes-0.1.3/pyproject.toml` & `pycasatunes-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycasatunes"
-version = "0.1.3"
+version = "0.1.4"
 description = "Asynchronous python client for CasaTunes."
 authors = ["Jon Kristian Nilsen <hello@jonkristian.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jonkristian/pycasatunes"
 repository = "https://github.com/jonkristian/pycasatunes"
 documentation = "https://github.com/jonkristian/pycasatunes"
```

### Comparing `pycasatunes-0.1.3/PKG-INFO` & `pycasatunes-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycasatunes
-Version: 0.1.3
+Version: 0.1.4
 Summary: Asynchronous python client for CasaTunes.
 Home-page: https://github.com/jonkristian/pycasatunes
 License: MIT
 Keywords: casatunes,multiroom,api,async,client
 Author: Jon Kristian Nilsen
 Author-email: hello@jonkristian.no
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycasatunes Version: 0.1.3 Summary: Asynchronous
+Metadata-Version: 2.1 Name: pycasatunes Version: 0.1.4 Summary: Asynchronous
 python client for CasaTunes. Home-page: https://github.com/jonkristian/
 pycasatunes License: MIT Keywords: casatunes,multiroom,api,async,client Author:
 Jon Kristian Nilsen Author-email: hello@jonkristian.no Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

