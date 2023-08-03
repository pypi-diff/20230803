# Comparing `tmp/nemusicapi-0.0.5a1.tar.gz` & `tmp/nemusicapi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.0.5a1.tar", max compression
+gzip compressed data, was "nemusicapi-0.1.0.tar", max compression
```

## Comparing `nemusicapi-0.0.5a1.tar` & `nemusicapi-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.5a1/LICENSE
--rw-r--r--   0        0        0      289 2023-08-03 08:47:05.141775 nemusicapi-0.0.5a1/nemusicapi/__init__.py
--rw-r--r--   0        0        0     4829 2023-08-03 08:15:45.913944 nemusicapi-0.0.5a1/nemusicapi/api.py
--rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.0.5a1/nemusicapi/exception.py
--rw-r--r--   0        0        0      338 2023-08-03 08:13:25.809448 nemusicapi-0.0.5a1/nemusicapi/type.py
--rw-r--r--   0        0        0      466 2023-08-03 08:48:05.839823 nemusicapi-0.0.5a1/pyproject.toml
--rw-r--r--   0        0        0     1285 2023-08-03 08:27:02.179801 nemusicapi-0.0.5a1/README.md
--rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 nemusicapi-0.0.5a1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.1.0/LICENSE
+-rw-r--r--   0        0        0      311 2023-08-03 09:11:40.318932 nemusicapi-0.1.0/nemusicapi/__init__.py
+-rw-r--r--   0        0        0     4829 2023-08-03 09:08:35.550244 nemusicapi-0.1.0/nemusicapi/api.py
+-rw-r--r--   0        0        0      113 2023-08-03 06:48:17.625541 nemusicapi-0.1.0/nemusicapi/exception.py
+-rw-r--r--   0        0        0      338 2023-08-03 08:13:25.809448 nemusicapi-0.1.0/nemusicapi/type.py
+-rw-r--r--   0        0        0      464 2023-08-03 09:11:50.295603 nemusicapi-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1285 2023-08-03 08:27:02.179801 nemusicapi-0.1.0/README.md
+-rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 nemusicapi-0.1.0/PKG-INFO
```

### Comparing `nemusicapi-0.0.5a1/LICENSE` & `nemusicapi-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.5a1/nemusicapi/api.py` & `nemusicapi-0.1.0/nemusicapi/api.py`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.5a1/README.md` & `nemusicapi-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.5a1/PKG-INFO` & `nemusicapi-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.0.5a1
+Version: 0.1.0
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

