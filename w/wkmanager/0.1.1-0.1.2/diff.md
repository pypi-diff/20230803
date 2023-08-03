# Comparing `tmp/wkmanager-0.1.1.tar.gz` & `tmp/wkmanager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wkmanager-0.1.1.tar", max compression
+gzip compressed data, was "wkmanager-0.1.2.tar", max compression
```

## Comparing `wkmanager-0.1.1.tar` & `wkmanager-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      442 2023-08-03 15:16:14.222613 wkmanager-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2251 2023-07-26 22:51:17.840863 wkmanager-0.1.1/README.md
--rw-r--r--   0        0        0       51 2023-08-03 15:03:29.408115 wkmanager-0.1.1/wkmanager/__init__.py
--rw-r--r--   0        0        0     8629 2023-07-27 14:30:37.231949 wkmanager-0.1.1/wkmanager/main.py
--rw-r--r--   0        0        0      254 2023-07-26 17:13:36.388380 wkmanager-0.1.1/wkmanager/resources/windows_versions.json
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 wkmanager-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      442 2023-08-03 15:28:34.513754 wkmanager-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2251 2023-07-26 22:51:17.840863 wkmanager-0.1.2/README.md
+-rw-r--r--   0        0        0       51 2023-08-03 15:03:29.408115 wkmanager-0.1.2/wkmanager/__init__.py
+-rw-r--r--   0        0        0     8696 2023-08-03 15:27:46.622207 wkmanager-0.1.2/wkmanager/main.py
+-rw-r--r--   0        0        0      254 2023-07-26 17:13:36.388380 wkmanager-0.1.2/wkmanager/resources/windows_versions.json
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 wkmanager-0.1.2/PKG-INFO
```

### Comparing `wkmanager-0.1.1/README.md` & `wkmanager-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wkmanager-0.1.1/wkmanager/main.py` & `wkmanager-0.1.2/wkmanager/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pkg_resources
 import pandas as pd
 import subprocess
 import platform
 import requests
 import zipfile
 import json
 import re
@@ -71,15 +72,16 @@
 
     def __support_validator(self, support: str) -> str:
         if not support:
             support = platform.release()
 
         if self.sys in ["Windows", "macOS"]:
             if self.sys == "Windows":
-                with open("resources/windows_versions.json", "r") as file:
+
+                with open(pkg_resources.resource_filename(__name__, "resources/windows_versions.json"), "r") as file:
                     windows_versions = json.load(file)
 
                 if support in windows_versions:
                     version_number = windows_versions[support]
                 elif re.match(r'^[-+]?\d*\.?\d+(?:[eE][-+]?\d+)?$', support):
                     version_number = float(support)
                 else:
```

### Comparing `wkmanager-0.1.1/PKG-INFO` & `wkmanager-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wkmanager
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lib to download wkhtmltopdf/wkhtmltoimage (wkhtmltox) based on OS.
 License: MIT
 Author: Ricardo Castro
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

