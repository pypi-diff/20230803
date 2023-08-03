# Comparing `tmp/disruptive-1.5.6.tar.gz` & `tmp/disruptive-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disruptive-1.5.6.tar", last modified: Wed Aug  2 11:14:38 2023, max compression
+gzip compressed data, was "disruptive-1.6.0.tar", last modified: Thu Aug  3 12:12:47 2023, max compression
```

## Comparing `disruptive-1.5.6.tar` & `disruptive-1.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:38.829436 disruptive-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 11:14:21.000000 disruptive-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-08-02 11:14:38.829436 disruptive-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-08-02 11:14:21.000000 disruptive-1.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:38.817436 disruptive-1.5.6/disruptive/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:38.817436 disruptive-1.5.6/disruptive/events/
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61763 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:38.829436 disruptive-1.5.6/disruptive/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/eventhistory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:38.817436 disruptive-1.5.6/disruptive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-08-02 11:14:38.000000 disruptive-1.5.6/disruptive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-02 11:14:38.000000 disruptive-1.5.6/disruptive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:14:38.000000 disruptive-1.5.6/disruptive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 11:14:38.000000 disruptive-1.5.6/disruptive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 11:14:38.000000 disruptive-1.5.6/disruptive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 11:14:21.000000 disruptive-1.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-02 11:14:38.829436 disruptive-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-02 11:14:21.000000 disruptive-1.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:12:47.701202 disruptive-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 12:12:38.000000 disruptive-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-08-03 12:12:47.701202 disruptive-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-03 12:12:38.000000 disruptive-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:12:47.701202 disruptive-1.6.0/disruptive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:12:47.701202 disruptive-1.6.0/disruptive/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61763 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:12:47.701202 disruptive-1.6.0/disruptive/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/eventhistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/resources/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-03 12:12:38.000000 disruptive-1.6.0/disruptive/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:12:47.701202 disruptive-1.6.0/disruptive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-08-03 12:12:47.000000 disruptive-1.6.0/disruptive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 12:12:47.000000 disruptive-1.6.0/disruptive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:12:47.000000 disruptive-1.6.0/disruptive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-03 12:12:47.000000 disruptive-1.6.0/disruptive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 12:12:47.000000 disruptive-1.6.0/disruptive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-03 12:12:38.000000 disruptive-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-03 12:12:47.701202 disruptive-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-03 12:12:38.000000 disruptive-1.6.0/setup.py
```

### Comparing `disruptive-1.5.6/LICENSE` & `disruptive-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/PKG-INFO` & `disruptive-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: disruptive
-Version: 1.5.6
+Version: 1.6.0
 Summary: Disruptive Technologies Python API.
 Home-page: https://github.com/disruptive-technologies/disruptive-python
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
 Project-URL: Documentation, https://developer.disruptive-technologies.com/api/libraries/python/
 Project-URL: Developers Page, https://developer.disruptive-technologies.com/docs/
 Keywords: disruptive,technologies,dt,rest,api
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: extra
 License-File: LICENSE
 
 # Disruptive Technologies Python Client
 
@@ -47,15 +45,15 @@
 
 ```sh
 pip install .
 ```
 
 ### Requirements
 
-- Python 3.7, 3.8, 3.9, 3.10, and 3.11
+- Python 3.8, 3.9, 3.10, and 3.11
 
 ## Authentication
 
 The package is authenticated by providing [Service Account](https://developer.disruptive-technologies.com/docs/service-accounts/introduction-to-service-accounts) credentials in either of the following ways.
 
 - By setting the following environment variables:
 ```bash
```

### Comparing `disruptive-1.5.6/README.md` & `disruptive-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 ```sh
 pip install .
 ```
 
 ### Requirements
 
-- Python 3.7, 3.8, 3.9, 3.10, and 3.11
+- Python 3.8, 3.9, 3.10, and 3.11
 
 ## Authentication
 
 The package is authenticated by providing [Service Account](https://developer.disruptive-technologies.com/docs/service-accounts/introduction-to-service-accounts) credentials in either of the following ways.
 
 - By setting the following environment variables:
 ```bash
```

### Comparing `disruptive-1.5.6/disruptive/__init__.py` & `disruptive-1.6.0/disruptive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Metadata
-__version__ = '1.5.6'
+__version__ = '1.6.0'
 
 # If set, logs of chosen level and higher are printed to console.
 # Default value None results in no logs at any level.
 log_level = None
 
 # REST API base URLs of which all endpoints are an expansion.
 base_url = 'https://api.disruptive-technologies.com/v2'
```

### Comparing `disruptive-1.5.6/disruptive/authentication.py` & `disruptive-1.6.0/disruptive/authentication.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/errors.py` & `disruptive-1.6.0/disruptive/errors.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/events/__init__.py` & `disruptive-1.6.0/disruptive/events/__init__.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/events/events.py` & `disruptive-1.6.0/disruptive/events/events.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/logging.py` & `disruptive-1.6.0/disruptive/logging.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/outputs.py` & `disruptive-1.6.0/disruptive/outputs.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/requests.py` & `disruptive-1.6.0/disruptive/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 import requests
 
 import disruptive as dt
 import disruptive.logging as dtlog
 import disruptive.errors as dterrors
 
 
-USER_AGENT = f'DisruptivePythonAPI/{dt.__version__}'
+USER_AGENT = 'DisruptivePythonAPI/{} Python/{}'.format(
+    dt.__version__,
+    f'{sys.version_info.major}.{sys.version_info.minor}',
+)
 
 
 class DTRequest():
 
     def __init__(self, method: str, url: str, **kwargs: Any):
         # Set attributes from parameters.
         self.method = method
```

### Comparing `disruptive-1.5.6/disruptive/resources/claim.py` & `disruptive-1.6.0/disruptive/resources/claim.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/resources/data_connector.py` & `disruptive-1.6.0/disruptive/resources/data_connector.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/resources/device.py` & `disruptive-1.6.0/disruptive/resources/device.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/resources/emulator.py` & `disruptive-1.6.0/disruptive/resources/emulator.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/resources/eventhistory.py` & `disruptive-1.6.0/disruptive/resources/eventhistory.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/resources/organization.py` & `disruptive-1.6.0/disruptive/resources/organization.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/resources/project.py` & `disruptive-1.6.0/disruptive/resources/project.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/resources/role.py` & `disruptive-1.6.0/disruptive/resources/role.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/resources/service_account.py` & `disruptive-1.6.0/disruptive/resources/service_account.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/resources/stream.py` & `disruptive-1.6.0/disruptive/resources/stream.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive/transforms.py` & `disruptive-1.6.0/disruptive/transforms.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/disruptive.egg-info/PKG-INFO` & `disruptive-1.6.0/disruptive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: disruptive
-Version: 1.5.6
+Version: 1.6.0
 Summary: Disruptive Technologies Python API.
 Home-page: https://github.com/disruptive-technologies/disruptive-python
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
 Project-URL: Documentation, https://developer.disruptive-technologies.com/api/libraries/python/
 Project-URL: Developers Page, https://developer.disruptive-technologies.com/docs/
 Keywords: disruptive,technologies,dt,rest,api
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: extra
 License-File: LICENSE
 
 # Disruptive Technologies Python Client
 
@@ -47,15 +45,15 @@
 
 ```sh
 pip install .
 ```
 
 ### Requirements
 
-- Python 3.7, 3.8, 3.9, 3.10, and 3.11
+- Python 3.8, 3.9, 3.10, and 3.11
 
 ## Authentication
 
 The package is authenticated by providing [Service Account](https://developer.disruptive-technologies.com/docs/service-accounts/introduction-to-service-accounts) credentials in either of the following ways.
 
 - By setting the following environment variables:
 ```bash
```

### Comparing `disruptive-1.5.6/disruptive.egg-info/SOURCES.txt` & `disruptive-1.6.0/disruptive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.6/setup.cfg` & `disruptive-1.6.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -18,24 +18,22 @@
 	api
 license_file = LICENSE
 classifiers = 
 	Natural Language :: English
 	License :: OSI Approved :: MIT License
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	requests >= 2.19.0, < 3.0.0
 	pyjwt >= 2.0.0, < 3.0.0
 include-package-data = True
 packages = find:
 
 [options.package_data]
@@ -52,13 +50,13 @@
 	wheel>=0.36.2
 	pytest>=6.2.2
 	pytest-mock>=3.5.1
 	pytest-cov>=2.11.1
 	mypy>=0.812
 	flake8>=3.9.0
 extra = 
-	pandas >= 1.3.5, < 2.0.0
+	pandas >= 2.0.0, < 3.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

