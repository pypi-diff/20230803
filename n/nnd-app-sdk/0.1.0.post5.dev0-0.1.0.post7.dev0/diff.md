# Comparing `tmp/nnd_app_sdk-0.1.0.post5.dev0.tar.gz` & `tmp/nnd_app_sdk-0.1.0.post7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnd_app_sdk-0.1.0.post5.dev0.tar", max compression
+gzip compressed data, was "nnd_app_sdk-0.1.0.post7.dev0.tar", max compression
```

## Comparing `nnd_app_sdk-0.1.0.post5.dev0.tar` & `nnd_app_sdk-0.1.0.post7.dev0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      658 2023-07-31 20:24:39.063396 nnd_app_sdk-0.1.0.post5.dev0/LICENSE
--rw-r--r--   0        0        0       88 2023-07-31 20:24:39.063396 nnd_app_sdk-0.1.0.post5.dev0/README.md
--rw-r--r--   0        0        0        0 2023-07-31 20:24:39.088395 nnd_app_sdk-0.1.0.post5.dev0/nnd_app_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 20:24:39.088395 nnd_app_sdk-0.1.0.post5.dev0/nnd_app_sdk/signin/__init__.py
--rw-r--r--   0        0        0     4541 2023-07-31 20:24:39.064396 nnd_app_sdk-0.1.0.post5.dev0/nnd_app_sdk/signin/base.py
--rw-r--r--   0        0        0        0 2023-07-31 20:24:39.088395 nnd_app_sdk-0.1.0.post5.dev0/nnd_app_sdk/signin/signins/__init__.py
--rw-r--r--   0        0        0     1028 2023-07-31 20:24:39.064396 nnd_app_sdk-0.1.0.post5.dev0/nnd_app_sdk/signin/signins/bonfire.py
--rw-r--r--   0        0        0     1162 2023-07-31 20:24:51.741177 nnd_app_sdk-0.1.0.post5.dev0/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 nnd_app_sdk-0.1.0.post5.dev0/PKG-INFO
+-rw-r--r--   0        0        0      658 2023-08-01 13:39:46.853078 nnd_app_sdk-0.1.0.post7.dev0/LICENSE
+-rw-r--r--   0        0        0       88 2023-08-01 13:39:46.853078 nnd_app_sdk-0.1.0.post7.dev0/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 13:39:46.876078 nnd_app_sdk-0.1.0.post7.dev0/nnd_app_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:39:46.876078 nnd_app_sdk-0.1.0.post7.dev0/nnd_app_sdk/signin/__init__.py
+-rw-r--r--   0        0        0     4541 2023-08-01 13:39:46.854078 nnd_app_sdk-0.1.0.post7.dev0/nnd_app_sdk/signin/base.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:39:46.876078 nnd_app_sdk-0.1.0.post7.dev0/nnd_app_sdk/signin/signins/__init__.py
+-rw-r--r--   0        0        0     1028 2023-08-01 13:39:46.854078 nnd_app_sdk-0.1.0.post7.dev0/nnd_app_sdk/signin/signins/bonfire.py
+-rw-r--r--   0        0        0     1162 2023-08-01 13:39:58.565962 nnd_app_sdk-0.1.0.post7.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 nnd_app_sdk-0.1.0.post7.dev0/PKG-INFO
```

### Comparing `nnd_app_sdk-0.1.0.post5.dev0/LICENSE` & `nnd_app_sdk-0.1.0.post7.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `nnd_app_sdk-0.1.0.post5.dev0/nnd_app_sdk/signin/base.py` & `nnd_app_sdk-0.1.0.post7.dev0/nnd_app_sdk/signin/base.py`

 * *Files identical despite different names*

### Comparing `nnd_app_sdk-0.1.0.post5.dev0/nnd_app_sdk/signin/signins/bonfire.py` & `nnd_app_sdk-0.1.0.post7.dev0/nnd_app_sdk/signin/signins/bonfire.py`

 * *Files identical despite different names*

### Comparing `nnd_app_sdk-0.1.0.post5.dev0/pyproject.toml` & `nnd_app_sdk-0.1.0.post7.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nnd-app-sdk"
-version = "0.1.0.post5.dev0"
+version = "0.1.0.post7.dev0"
 repository = "https://gitlab.com/nomnomdata/tools/nnd-app-sdk"
 authors = ["Nom Nom Data Inc <info@nomnomdata.com>"]
 description = "Package containing common functions for developing Nom Nom Data Apps."
 license = "LGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `nnd_app_sdk-0.1.0.post5.dev0/PKG-INFO` & `nnd_app_sdk-0.1.0.post7.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnd-app-sdk
-Version: 0.1.0.post5.dev0
+Version: 0.1.0.post7.dev0
 Summary: Package containing common functions for developing Nom Nom Data Apps.
 Home-page: https://gitlab.com/nomnomdata/tools/nnd-app-sdk
 License: LGPL-3.0-only
 Author: Nom Nom Data Inc
 Author-email: info@nomnomdata.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

