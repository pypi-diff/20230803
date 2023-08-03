# Comparing `tmp/HallmasterAPI-0.1.1.tar.gz` & `tmp/HallmasterAPI-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HallmasterAPI-0.1.1.tar", last modified: Thu Aug  3 14:43:47 2023, max compression
+gzip compressed data, was "HallmasterAPI-0.1.2.tar", last modified: Thu Aug  3 15:04:19 2023, max compression
```

## Comparing `HallmasterAPI-0.1.1.tar` & `HallmasterAPI-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 14:43:47.695236 HallmasterAPI-0.1.1/
--rw-rw-rw-   0        0        0    35823 2023-08-03 12:27:09.000000 HallmasterAPI-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      592 2023-08-03 14:43:47.695236 HallmasterAPI-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-08-03 12:27:09.000000 HallmasterAPI-0.1.1/README.md
--rw-rw-rw-   0        0        0      619 2023-08-03 14:42:50.000000 HallmasterAPI-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-03 14:43:47.703273 HallmasterAPI-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-03 14:43:47.600815 HallmasterAPI-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 14:43:47.686829 HallmasterAPI-0.1.1/src/HallmasterAPI.egg-info/
--rw-rw-rw-   0        0        0      592 2023-08-03 14:43:47.000000 HallmasterAPI-0.1.1/src/HallmasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-08-03 14:43:47.000000 HallmasterAPI-0.1.1/src/HallmasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 14:43:47.000000 HallmasterAPI-0.1.1/src/HallmasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-03 14:43:47.000000 HallmasterAPI-0.1.1/src/HallmasterAPI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-03 14:43:47.686829 HallmasterAPI-0.1.1/src/hallmasterapi/
--rw-rw-rw-   0        0        0       29 2023-08-03 14:10:16.000000 HallmasterAPI-0.1.1/src/hallmasterapi/__init__.py
--rw-rw-rw-   0        0        0     5889 2023-08-03 14:02:09.000000 HallmasterAPI-0.1.1/src/hallmasterapi/hallmasterapi.py
+drwxrwxrwx   0        0        0        0 2023-08-03 15:04:19.206750 HallmasterAPI-0.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-08-03 12:27:09.000000 HallmasterAPI-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      592 2023-08-03 15:04:19.205750 HallmasterAPI-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-08-03 12:27:09.000000 HallmasterAPI-0.1.2/README.md
+-rw-rw-rw-   0        0        0      680 2023-08-03 15:01:51.000000 HallmasterAPI-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-03 15:04:19.207751 HallmasterAPI-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-03 15:04:19.162749 HallmasterAPI-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-03 15:04:19.195750 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/
+-rw-rw-rw-   0        0        0      592 2023-08-03 15:04:19.000000 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-08-03 15:04:19.000000 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 15:04:19.000000 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-08-03 15:04:19.000000 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-03 15:04:19.000000 HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 15:04:19.202751 HallmasterAPI-0.1.2/src/hallmasterapi/
+-rw-rw-rw-   0        0        0       29 2023-08-03 14:10:16.000000 HallmasterAPI-0.1.2/src/hallmasterapi/__init__.py
+-rw-rw-rw-   0        0        0     5889 2023-08-03 15:01:51.000000 HallmasterAPI-0.1.2/src/hallmasterapi/hallmasterapi.py
```

### Comparing `HallmasterAPI-0.1.1/LICENSE` & `HallmasterAPI-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HallmasterAPI-0.1.1/PKG-INFO` & `HallmasterAPI-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HallmasterAPI
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper for the Hallmaster API
 Author: Matthew Larby
 Project-URL: Homepage, https://github.com/mattl1598/HallmasterAPI
 Project-URL: Bug Tracker, https://github.com/mattl1598/HallmasterAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `HallmasterAPI-0.1.1/src/HallmasterAPI.egg-info/PKG-INFO` & `HallmasterAPI-0.1.2/src/HallmasterAPI.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HallmasterAPI
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python wrapper for the Hallmaster API
 Author: Matthew Larby
 Project-URL: Homepage, https://github.com/mattl1598/HallmasterAPI
 Project-URL: Bug Tracker, https://github.com/mattl1598/HallmasterAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `HallmasterAPI-0.1.1/src/hallmasterapi/hallmasterapi.py` & `HallmasterAPI-0.1.2/src/hallmasterapi/hallmasterapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 	message = "Venue ID does not exist."
 
 	def __init__(self):
 		super().__init__(self.message)
 
 
 class HallmasterAPI:
-	version = '0.1.1'
+	version = '0.1.2'
 
 	api_subdomain = "https://v2.hallmaster.co.uk"
 	api_time_format = "%Y-%m-%dT%H:%M:%S+00:00"  # note: tz addon as %z not currently working for datetime.now(), assume UTC
 	api_user_agent = f"Hallmaster Python API v{version}"
 
 	def __init__(self, venue_id: int):
 		self.hall_id = venue_id
```

