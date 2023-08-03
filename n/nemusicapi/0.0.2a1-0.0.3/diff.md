# Comparing `tmp/nemusicapi-0.0.2a1.tar.gz` & `tmp/nemusicapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemusicapi-0.0.2a1.tar", max compression
+gzip compressed data, was "nemusicapi-0.0.3.tar", max compression
```

## Comparing `nemusicapi-0.0.2a1.tar` & `nemusicapi-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.2a1/LICENSE
--rw-r--r--   0        0        0     3351 2023-08-01 07:33:42.704150 nemusicapi-0.0.2a1/NEmusicApi/api.py
--rw-r--r--   0        0        0      466 2023-08-01 09:17:47.191205 nemusicapi-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.2a1/README.md
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 nemusicapi-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-08-01 07:21:02.527622 nemusicapi-0.0.3/LICENSE
+-rw-r--r--   0        0        0       27 2023-08-03 05:37:07.632198 nemusicapi-0.0.3/NEmusicApi/__init__.py
+-rw-r--r--   0        0        0     4750 2023-08-03 05:41:17.034038 nemusicapi-0.0.3/NEmusicApi/api.py
+-rw-r--r--   0        0        0      464 2023-08-03 05:42:17.769101 nemusicapi-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-08-01 07:21:02.528622 nemusicapi-0.0.3/README.md
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 nemusicapi-0.0.3/PKG-INFO
```

### Comparing `nemusicapi-0.0.2a1/LICENSE` & `nemusicapi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nemusicapi-0.0.2a1/PKG-INFO` & `nemusicapi-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemusicapi
-Version: 0.0.2a1
+Version: 0.0.3
 Summary: A Netsase music api
 Home-page: https://github.com/yuyi2439/NeteaseMusicApi
 License: Apache-2.0
 Author: yuyi2439
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

