# Comparing `tmp/nemusicapi-0.0.3a1.tar.gz` & `tmp/nemusicapi-0.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.0.3a1.tar", max compression
+gzip compressed data, was "nemusicapi-0.0.3a2.tar", max compression
```

## Comparing `nemusicapi-0.0.3a1.tar` & `nemusicapi-0.0.3a2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.3a1/LICENSE
--rw-r--r--   0        0        0       71 2023-08-03 05:56:14.055185 nemusicapi-0.0.3a1/NEmusicApi/__init__.py
--rw-r--r--   0        0        0     4750 2023-08-03 05:41:17.034038 nemusicapi-0.0.3a1/NEmusicApi/api.py
--rw-r--r--   0        0        0      466 2023-08-03 05:56:30.073117 nemusicapi-0.0.3a1/pyproject.toml
--rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.3a1/README.md
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.3a1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.3a2/LICENSE
+-rw-r--r--   0        0        0       82 2023-08-03 06:16:56.349661 nemusicapi-0.0.3a2/NEmusicApi/__init__.py
+-rw-r--r--   0        0        0     4750 2023-08-03 05:41:17.034038 nemusicapi-0.0.3a2/NEmusicApi/api.py
+-rw-r--r--   0        0        0      466 2023-08-03 06:15:59.534577 nemusicapi-0.0.3a2/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.3a2/README.md
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.3a2/PKG-INFO
```

### Comparing `nemusicapi-0.0.3a1/LICENSE` & `nemusicapi-0.0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.3a1/NEmusicApi/api.py` & `nemusicapi-0.0.3a2/NEmusicApi/api.py`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.3a1/PKG-INFO` & `nemusicapi-0.0.3a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.0.3a1
+Version: 0.0.3a2
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

