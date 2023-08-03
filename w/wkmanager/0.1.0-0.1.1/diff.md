# Comparing `tmp/wkmanager-0.1.0.tar.gz` & `tmp/wkmanager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkmanager-0.1.0.tar", max compression
+gzip compressed data, was "wkmanager-0.1.1.tar", max compression
```

## Comparing `wkmanager-0.1.0.tar` & `wkmanager-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      485 2023-07-27 14:20:12.256096 wkmanager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2251 2023-07-26 22:51:17.840863 wkmanager-0.1.0/README.md
--rw-r--r--   0        0        0      254 2023-07-26 17:13:36.388380 wkmanager-0.1.0/resources/windows_versions.json
--rw-r--r--   0        0        0     8636 2023-07-26 22:08:37.463366 wkmanager-0.1.0/wkmanager/main.py
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 wkmanager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      442 2023-08-03 15:16:14.222613 wkmanager-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2251 2023-07-26 22:51:17.840863 wkmanager-0.1.1/README.md
+-rw-r--r--   0        0        0       51 2023-08-03 15:03:29.408115 wkmanager-0.1.1/wkmanager/__init__.py
+-rw-r--r--   0        0        0     8629 2023-07-27 14:30:37.231949 wkmanager-0.1.1/wkmanager/main.py
+-rw-r--r--   0        0        0      254 2023-07-26 17:13:36.388380 wkmanager-0.1.1/wkmanager/resources/windows_versions.json
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 wkmanager-0.1.1/PKG-INFO
```

### Comparing `wkmanager-0.1.0/README.md` & `wkmanager-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wkmanager-0.1.0/wkmanager/main.py` & `wkmanager-0.1.1/wkmanager/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests
 import zipfile
 import json
 import re
 import os
 
 
-class WkManager:
+class Wk:
     def __init__(self, sys: str = None, support: str = None, arch: str = None, extension: str = None):
         self.__df = self.__get_df_from_wkorg()
         self.sys = self.__sys_validator(sys)
         self.support = self.__support_validator(support)
         self.arch = self.__arch_validator(arch)
         self.extension = self.__extension_validator(extension)
```

### Comparing `wkmanager-0.1.0/PKG-INFO` & `wkmanager-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkmanager
-Version: 0.1.0
+Version: 0.1.1
 Summary: Lib to download wkhtmltopdf/wkhtmltoimage (wkhtmltox) based on OS.
 License: MIT
 Author: Ricardo Castro
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

