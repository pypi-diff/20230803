# Comparing `tmp/retakesearch-0.1.26.tar.gz` & `tmp/retakesearch-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.1.26.tar", max compression
+gzip compressed data, was "retakesearch-0.1.27.tar", max compression
```

## Comparing `retakesearch-0.1.26.tar` & `retakesearch-0.1.27.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-08-02 06:35:04.001745 retakesearch-0.1.26/README.md
--rw-r--r--   0        0        0      429 2023-08-02 06:35:25.190951 retakesearch-0.1.26/pyproject.toml
--rw-r--r--   0        0        0      174 2023-08-02 06:35:04.001745 retakesearch-0.1.26/retakesearch/__init__.py
--rw-r--r--   0        0        0     1818 2023-08-02 06:35:04.001745 retakesearch-0.1.26/retakesearch/client.py
--rw-r--r--   0        0        0     3687 2023-08-02 06:35:04.001745 retakesearch-0.1.26/retakesearch/index.py
--rw-r--r--   0        0        0      159 2023-08-02 06:35:04.001745 retakesearch-0.1.26/retakesearch/search.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 retakesearch-0.1.26/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 04:48:37.874287 retakesearch-0.1.27/README.md
+-rw-r--r--   0        0        0      429 2023-08-03 04:49:02.458485 retakesearch-0.1.27/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-08-03 04:48:37.874287 retakesearch-0.1.27/retakesearch/__init__.py
+-rw-r--r--   0        0        0     1818 2023-08-03 04:48:37.874287 retakesearch-0.1.27/retakesearch/client.py
+-rw-r--r--   0        0        0     4523 2023-08-03 04:48:37.874287 retakesearch-0.1.27/retakesearch/index.py
+-rw-r--r--   0        0        0      159 2023-08-03 04:48:37.874287 retakesearch-0.1.27/retakesearch/search.py
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 retakesearch-0.1.27/PKG-INFO
```

### Comparing `retakesearch-0.1.26/retakesearch/client.py` & `retakesearch-0.1.27/retakesearch/client.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.1.26/PKG-INFO` & `retakesearch-0.1.27/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.1.26
+Version: 0.1.27
 Summary: Python client for Retake: universal search infra for developers
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

