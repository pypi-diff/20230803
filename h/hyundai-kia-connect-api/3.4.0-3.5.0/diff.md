# Comparing `tmp/hyundai_kia_connect_api-3.4.0.tar.gz` & `tmp/hyundai_kia_connect_api-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyundai_kia_connect_api-3.4.0.tar", last modified: Sat Jul 29 15:54:43 2023, max compression
+gzip compressed data, was "hyundai_kia_connect_api-3.5.0.tar", last modified: Thu Aug  3 20:32:44 2023, max compression
```

## Comparing `hyundai_kia_connect_api-3.4.0.tar` & `hyundai_kia_connect_api-3.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:54:43.381278 hyundai_kia_connect_api-3.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/ApiImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    29985 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiCA.py
--rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiCN.py
--rw-r--r--   0 runner    (1001) docker     (123)    54198 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiEU.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/Vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/VehicleManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 15:54:43.000000 hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-29 15:54:29.000000 hyundai_kia_connect_api-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 15:54:43.385278 hyundai_kia_connect_api-3.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/tests/ca_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/tests/eu_check_response_for_errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-29 15:53:58.000000 hyundai_kia_connect_api-3.4.0/tests/eu_login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:32:44.119226 hyundai_kia_connect_api-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-08-03 20:32:44.119226 hyundai_kia_connect_api-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:32:44.115226 hyundai_kia_connect_api-3.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:32:44.119226 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/ApiImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30103 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/KiaUvoApiCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/KiaUvoApiCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54198 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/KiaUvoApiEU.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/Vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/VehicleManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:32:44.119226 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-08-03 20:32:44.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-03 20:32:44.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:32:44.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:32:43.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 20:32:44.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 20:32:44.000000 hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-03 20:32:44.119226 hyundai_kia_connect_api-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-03 20:32:32.000000 hyundai_kia_connect_api-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:32:44.119226 hyundai_kia_connect_api-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/tests/ca_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/tests/eu_check_response_for_errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-03 20:32:09.000000 hyundai_kia_connect_api-3.5.0/tests/eu_login_test.py
```

### Comparing `hyundai_kia_connect_api-3.4.0/CONTRIBUTING.rst` & `hyundai_kia_connect_api-3.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/LICENSE` & `hyundai_kia_connect_api-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/PKG-INFO` & `hyundai_kia_connect_api-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai_kia_connect_api
-Version: 3.4.0
+Version: 3.5.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,15 +16,15 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 
 Introduction
 ============
 
-This is a Kia UVO and Hyundai Bluelink written in python.  It is primary consumed by home assistant.  If you are looking for a home assistant Kia / Hyundai implementation please look here: https://github.com/fuatakgun/kia_uvo.  Much of this base code came from reading bluelinky and contributions to the kia_uvo home assistant project.
+This is a Kia UVO, Hyundai Bluelink, Genesis Connect(Canada Only) written in python.  It is primary consumed by home assistant.  If you are looking for a home assistant Kia / Hyundai implementation please look here: https://github.com/fuatakgun/kia_uvo.  Much of this base code came from reading bluelinky and contributions to the kia_uvo home assistant project.
 
 
 Usage
 =====
 
 This package is designed to simplify the complexity of using multiple regions.  It attempts to standardize the usage regardless of what brand or region the car is in.  That isn't always possible though, in particular some features differ from one to the next.
 
@@ -35,15 +35,15 @@
     username: str
     password: str
     pin: str (required for CA, and potentially USA, otherwise pass a blank string)
 
 Key values for the int exist in the constant(https://github.com/fuatakgun/hyundai_kia_connect_api/blob/master/hyundai_kia_connect_api/const.py) file as::
 
     REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
-    BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI}
+    BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI, 3: BRAND_GENESIS}
 
 Once this is done you can now make the following calls against the vehicle manager::
 
  #Checks the token is still valid and updates it if not.  Should be called before anything else if the code has been running for any length of time.
  check_and_refresh_token(self)
 
  #Ideal refresh command. Checks if the car has been updated since the time in seconds provided.  If so does a cached update. If not force calls the car.
```

### Comparing `hyundai_kia_connect_api-3.4.0/README.rst` & `hyundai_kia_connect_api-3.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 Introduction
 ============
 
-This is a Kia UVO and Hyundai Bluelink written in python.  It is primary consumed by home assistant.  If you are looking for a home assistant Kia / Hyundai implementation please look here: https://github.com/fuatakgun/kia_uvo.  Much of this base code came from reading bluelinky and contributions to the kia_uvo home assistant project.
+This is a Kia UVO, Hyundai Bluelink, Genesis Connect(Canada Only) written in python.  It is primary consumed by home assistant.  If you are looking for a home assistant Kia / Hyundai implementation please look here: https://github.com/fuatakgun/kia_uvo.  Much of this base code came from reading bluelinky and contributions to the kia_uvo home assistant project.
 
 
 Usage
 =====
 
 This package is designed to simplify the complexity of using multiple regions.  It attempts to standardize the usage regardless of what brand or region the car is in.  That isn't always possible though, in particular some features differ from one to the next.
 
@@ -17,15 +17,15 @@
     username: str
     password: str
     pin: str (required for CA, and potentially USA, otherwise pass a blank string)
 
 Key values for the int exist in the constant(https://github.com/fuatakgun/hyundai_kia_connect_api/blob/master/hyundai_kia_connect_api/const.py) file as::
 
     REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
-    BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI}
+    BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI, 3: BRAND_GENESIS}
 
 Once this is done you can now make the following calls against the vehicle manager::
 
  #Checks the token is still valid and updates it if not.  Should be called before anything else if the code has been running for any length of time.
  check_and_refresh_token(self)
 
  #Ideal refresh command. Checks if the car has been updated since the time in seconds provided.  If so does a cached update. If not force calls the car.
```

### Comparing `hyundai_kia_connect_api-3.4.0/docs/Makefile` & `hyundai_kia_connect_api-3.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/docs/conf.py` & `hyundai_kia_connect_api-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/docs/installation.rst` & `hyundai_kia_connect_api-3.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/docs/make.bat` & `hyundai_kia_connect_api-3.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/ApiImpl.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/ApiImpl.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/KiaUvoAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiCA.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/KiaUvoApiCA.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from .ApiImpl import ApiImpl, ClimateRequestOptions
 from .Token import Token
 from .Vehicle import Vehicle
 from .const import (
     BRAND_HYUNDAI,
     BRAND_KIA,
+    BRAND_GENESIS,
     BRANDS,
     DOMAIN,
     DISTANCE_UNITS,
     TEMPERATURE_UNITS,
     SEAT_STATUS,
     ENGINE_TYPES,
     VEHICLE_LOCK_ACTION,
@@ -66,14 +67,17 @@
     def __init__(self, region: int, brand: int, language: str) -> None:
         self.vehicle_timezone = self.data_timezone
         self.LANGUAGE: str = language
         if BRANDS[brand] == BRAND_KIA:
             self.BASE_URL: str = "kiaconnect.ca"
         elif BRANDS[brand] == BRAND_HYUNDAI:
             self.BASE_URL: str = "mybluelink.ca"
+        elif BRANDS[brand] == BRAND_GENESIS:
+            self.BASE_URL: str = "genesisconnect.ca"
+
         self.old_vehicle_status = {}
         self.API_URL: str = "https://" + self.BASE_URL + "/tods/api/"
         self.API_HEADERS = {
             "content-type": "application/json;charset=UTF-8",
             "accept": "application/json, text/plain, */*",
             "accept-encoding": "gzip, deflate, br",
             "accept-language": "en-US,en;q=0.9",
```

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiCN.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/KiaUvoApiCN.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/KiaUvoApiEU.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/KiaUvoApiEU.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/Vehicle.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/Vehicle.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/VehicleManager.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/VehicleManager.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/const.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from enum import Enum
 
 DOMAIN: str = "hyundai_kia_connect_api"
 
 BRAND_KIA = "Kia"
 BRAND_HYUNDAI = "Hyundai"
-BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI}
+BRAND_GENESIS = "Genesis"
+BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI, 3: BRAND_GENESIS}
 
 REGION_EUROPE = "Europe"
 REGION_CANADA = "Canada"
 REGION_USA = "USA"
 REGION_CHINA = "China"
 REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
```

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/exceptions.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api/utils.py` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api/utils.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/PKG-INFO` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai-kia-connect-api
-Version: 3.4.0
+Version: 3.5.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,15 +16,15 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 
 Introduction
 ============
 
-This is a Kia UVO and Hyundai Bluelink written in python.  It is primary consumed by home assistant.  If you are looking for a home assistant Kia / Hyundai implementation please look here: https://github.com/fuatakgun/kia_uvo.  Much of this base code came from reading bluelinky and contributions to the kia_uvo home assistant project.
+This is a Kia UVO, Hyundai Bluelink, Genesis Connect(Canada Only) written in python.  It is primary consumed by home assistant.  If you are looking for a home assistant Kia / Hyundai implementation please look here: https://github.com/fuatakgun/kia_uvo.  Much of this base code came from reading bluelinky and contributions to the kia_uvo home assistant project.
 
 
 Usage
 =====
 
 This package is designed to simplify the complexity of using multiple regions.  It attempts to standardize the usage regardless of what brand or region the car is in.  That isn't always possible though, in particular some features differ from one to the next.
 
@@ -35,15 +35,15 @@
     username: str
     password: str
     pin: str (required for CA, and potentially USA, otherwise pass a blank string)
 
 Key values for the int exist in the constant(https://github.com/fuatakgun/hyundai_kia_connect_api/blob/master/hyundai_kia_connect_api/const.py) file as::
 
     REGIONS = {1: REGION_EUROPE, 2: REGION_CANADA, 3: REGION_USA, 4: REGION_CHINA}
-    BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI}
+    BRANDS = {1: BRAND_KIA, 2: BRAND_HYUNDAI, 3: BRAND_GENESIS}
 
 Once this is done you can now make the following calls against the vehicle manager::
 
  #Checks the token is still valid and updates it if not.  Should be called before anything else if the code has been running for any length of time.
  check_and_refresh_token(self)
 
  #Ideal refresh command. Checks if the car has been updated since the time in seconds provided.  If so does a cached update. If not force calls the car.
```

### Comparing `hyundai_kia_connect_api-3.4.0/hyundai_kia_connect_api.egg-info/SOURCES.txt` & `hyundai_kia_connect_api-3.5.0/hyundai_kia_connect_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/setup.py` & `hyundai_kia_connect_api-3.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     name="hyundai_kia_connect_api",
     packages=find_packages(
         include=["hyundai_kia_connect_api", "hyundai_kia_connect_api.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/fuatakgun/hyundai_kia_connect_api",
-    version="3.4.0",
+    version="3.5.0",
     zip_safe=False,
 )
```

### Comparing `hyundai_kia_connect_api-3.4.0/tests/ca_login_test.py` & `hyundai_kia_connect_api-3.5.0/tests/ca_login_test.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.4.0/tests/eu_check_response_for_errors_test.py` & `hyundai_kia_connect_api-3.5.0/tests/eu_check_response_for_errors_test.py`

 * *Files identical despite different names*

