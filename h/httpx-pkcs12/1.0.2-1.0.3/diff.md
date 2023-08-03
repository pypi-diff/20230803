# Comparing `tmp/httpx_pkcs12-1.0.2.tar.gz` & `tmp/httpx_pkcs12-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx_pkcs12-1.0.2.tar", max compression
+gzip compressed data, was "httpx_pkcs12-1.0.3.tar", max compression
```

## Comparing `httpx_pkcs12-1.0.2.tar` & `httpx_pkcs12-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1073 2022-04-22 19:36:44.174591 httpx_pkcs12-1.0.2/LICENSE
--rw-r--r--   0        0        0      421 2022-04-22 19:36:44.174591 httpx_pkcs12-1.0.2/README.md
--rw-r--r--   0        0        0     1817 2022-04-22 19:36:44.174591 httpx_pkcs12-1.0.2/httpx_pkcs12/__init__.py
--rw-r--r--   0        0        0      396 2022-04-22 19:36:44.174591 httpx_pkcs12-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1107 2022-04-22 19:38:53.518350 httpx_pkcs12-1.0.2/setup.py
--rw-r--r--   0        0        0      991 2022-04-22 19:38:53.518607 httpx_pkcs12-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-03 10:04:51.028545 httpx_pkcs12-1.0.3/LICENSE
+-rw-r--r--   0        0        0      421 2023-08-03 10:04:51.028545 httpx_pkcs12-1.0.3/README.md
+-rw-r--r--   0        0        0     1817 2023-08-03 10:04:51.028545 httpx_pkcs12-1.0.3/httpx_pkcs12/__init__.py
+-rw-r--r--   0        0        0      397 2023-08-03 10:05:07.985229 httpx_pkcs12-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 httpx_pkcs12-1.0.3/PKG-INFO
```

### Comparing `httpx_pkcs12-1.0.2/LICENSE` & `httpx_pkcs12-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx_pkcs12-1.0.2/httpx_pkcs12/__init__.py` & `httpx_pkcs12-1.0.3/httpx_pkcs12/__init__.py`

 * *Files identical despite different names*

### Comparing `httpx_pkcs12-1.0.2/PKG-INFO` & `httpx_pkcs12-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: httpx-pkcs12
-Version: 1.0.2
+Version: 1.0.3
 Summary: Addon which activates PKCS12 certificates usage with HTTPX client.
 License: MIT
 Author: Shagit Ziganshin
 Author-email: theLastOfCats@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: cryptography (>=3.4.7,<37.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cryptography (>=3.4.7,<42.0.0)
 Description-Content-Type: text/markdown
 
 ## httpx-pkcs12
 
 Addon which activates PKCS12 certificates usage with HTTPX client.
 
 ## Usage
```

