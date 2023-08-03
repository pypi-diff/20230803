# Comparing `tmp/HallmasterAPI-0.1.2.tar.gz` & `tmp/HallmasterAPI-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HallmasterAPI-0.1.2.tar", last modified: Thu Aug  3 15:04:19 2023, max compression
+gzip compressed data, was "HallmasterAPI-0.1.3.tar", last modified: Thu Aug  3 15:26:56 2023, max compression
```

## Comparing `HallmasterAPI-0.1.2.tar` & `HallmasterAPI-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 15:04:19.206750 HallmasterAPI-0.1.2/
--rw-rw-rw-   0        0        0    35823 2023-08-03 12:27:09.000000 HallmasterAPI-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      592 2023-08-03 15:04:19.205750 HallmasterAPI-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-08-03 12:27:09.000000 HallmasterAPI-0.1.2/README.md
--rw-rw-rw-   0        0        0      680 2023-08-03 15:01:51.000000 HallmasterAPI-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 15:04:19.207751 HallmasterAPI-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-03 15:04:19.162749 HallmasterAPI-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 15:04:19.195750 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/
--rw-rw-rw-   0        0        0      592 2023-08-03 15:04:19.000000 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-08-03 15:04:19.000000 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 15:04:19.000000 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-08-03 15:04:19.000000 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-03 15:04:19.000000 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 15:04:19.202751 HallmasterAPI-0.1.2/src/hallmasterapi/
--rw-rw-rw-   0        0        0       29 2023-08-03 14:10:16.000000 HallmasterAPI-0.1.2/src/hallmasterapi/__init__.py
--rw-rw-rw-   0        0        0     5889 2023-08-03 15:01:51.000000 HallmasterAPI-0.1.2/src/hallmasterapi/hallmasterapi.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:26:56.276946 HallmasterAPI-0.1.3/
+-rw-rw-rw-   0        0        0    35823 2023-08-03 12:27:09.000000 HallmasterAPI-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      593 2023-08-03 15:26:56.275946 HallmasterAPI-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-08-03 12:27:09.000000 HallmasterAPI-0.1.3/README.md
+-rw-rw-rw-   0        0        0      681 2023-08-03 15:24:23.000000 HallmasterAPI-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 15:26:56.277946 HallmasterAPI-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 15:26:56.245949 HallmasterAPI-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 15:26:56.267946 HallmasterAPI-0.1.3/src/HallmasterAPI.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-08-03 15:26:56.000000 HallmasterAPI-0.1.3/src/HallmasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-08-03 15:26:56.000000 HallmasterAPI-0.1.3/src/HallmasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 15:26:56.000000 HallmasterAPI-0.1.3/src/HallmasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-08-03 15:26:56.000000 HallmasterAPI-0.1.3/src/HallmasterAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-03 15:26:56.000000 HallmasterAPI-0.1.3/src/HallmasterAPI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 15:26:56.272953 HallmasterAPI-0.1.3/src/hallmasterapi/
+-rw-rw-rw-   0        0        0      246 2023-08-03 15:23:48.000000 HallmasterAPI-0.1.3/src/hallmasterapi/__init__.py
+-rw-rw-rw-   0        0        0     5836 2023-08-03 15:24:23.000000 HallmasterAPI-0.1.3/src/hallmasterapi/hallmasterapi.py
```

### Comparing `HallmasterAPI-0.1.2/LICENSE` & `HallmasterAPI-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HallmasterAPI-0.1.2/PKG-INFO` & `HallmasterAPI-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: HallmasterAPI
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper for the Hallmaster API
 Author: Matthew Larby
 Project-URL: Homepage, https://github.com/mattl1598/HallmasterAPI
 Project-URL: Bug Tracker, https://github.com/mattl1598/HallmasterAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HallmasterAPI
 Python wrapper for Hallmaster API
```

### Comparing `HallmasterAPI-0.1.2/pyproject.toml` & `HallmasterAPI-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HallmasterAPI"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Matthew Larby" },
 ]
 description = "Python wrapper for the Hallmaster API"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dependencies = [
     "requests",
     "beautifulsoup4",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/PKG-INFO` & `HallmasterAPI-0.1.3/src/HallmasterAPI.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: HallmasterAPI
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python wrapper for the Hallmaster API
 Author: Matthew Larby
 Project-URL: Homepage, https://github.com/mattl1598/HallmasterAPI
 Project-URL: Bug Tracker, https://github.com/mattl1598/HallmasterAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HallmasterAPI
 Python wrapper for Hallmaster API
```

### Comparing `HallmasterAPI-0.1.2/src/hallmasterapi/hallmasterapi.py` & `HallmasterAPI-0.1.3/src/hallmasterapi/hallmasterapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import re
-from pprint import pprint
-from typing import Any
-
 import requests
 import json
 from datetime import datetime, timedelta
 from bs4 import BeautifulSoup
 
 
 class Booking:
@@ -47,15 +44,15 @@
 	message = "Venue ID does not exist."
 
 	def __init__(self):
 		super().__init__(self.message)
 
 
 class HallmasterAPI:
-	version = '0.1.2'
+	version = '0.1.3'
 
 	api_subdomain = "https://v2.hallmaster.co.uk"
 	api_time_format = "%Y-%m-%dT%H:%M:%S+00:00"  # note: tz addon as %z not currently working for datetime.now(), assume UTC
 	api_user_agent = f"Hallmaster Python API v{version}"
 
 	def __init__(self, venue_id: int):
 		self.hall_id = venue_id
```

