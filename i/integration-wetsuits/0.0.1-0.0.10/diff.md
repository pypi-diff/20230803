# Comparing `tmp/integration-wetsuits-0.0.1.tar.gz` & `tmp/integration-wetsuits-0.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integration-wetsuits-0.0.1.tar", last modified: Wed Aug  2 10:04:19 2023, max compression
+gzip compressed data, was "integration-wetsuits-0.0.10.tar", last modified: Thu Aug  3 08:02:55 2023, max compression
```

## Comparing `integration-wetsuits-0.0.1.tar` & `integration-wetsuits-0.0.10.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:04:19.038341 integration-wetsuits-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 10:04:19.038341 integration-wetsuits-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-02 10:03:55.000000 integration-wetsuits-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 10:04:19.038341 integration-wetsuits-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:04:19.038341 integration-wetsuits-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 10:03:55.000000 integration-wetsuits-0.0.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-02 10:03:55.000000 integration-wetsuits-0.0.1/src/edi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:04:19.038341 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 10:04:19.000000 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-08-02 10:04:19.000000 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 10:04:19.000000 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 10:04:19.000000 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 10:04:19.000000 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-02 10:03:55.000000 integration-wetsuits-0.0.1/src/itsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:02:55.277799 integration-wetsuits-0.0.10/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-03 08:02:55.277799 integration-wetsuits-0.0.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-03 08:02:27.000000 integration-wetsuits-0.0.10/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:02:55.277799 integration-wetsuits-0.0.10/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:02:55.273799 integration-wetsuits-0.0.10/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:02:55.273799 integration-wetsuits-0.0.10/src/integration_wetsuits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:02:27.000000 integration-wetsuits-0.0.10/src/integration_wetsuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-03 08:02:27.000000 integration-wetsuits-0.0.10/src/integration_wetsuits/edi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-03 08:02:27.000000 integration-wetsuits-0.0.10/src/integration_wetsuits/itsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:02:55.273799 integration-wetsuits-0.0.10/src/integration_wetsuits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-03 08:02:55.000000 integration-wetsuits-0.0.10/src/integration_wetsuits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-03 08:02:55.000000 integration-wetsuits-0.0.10/src/integration_wetsuits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:02:55.000000 integration-wetsuits-0.0.10/src/integration_wetsuits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-03 08:02:55.000000 integration-wetsuits-0.0.10/src/integration_wetsuits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-03 08:02:55.000000 integration-wetsuits-0.0.10/src/integration_wetsuits.egg-info/top_level.txt
```

### Comparing `integration-wetsuits-0.0.1/pyproject.toml` & `integration-wetsuits-0.0.10/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "integration-wetsuits"
-version = "0.0.1"
+version = "0.0.10"
 authors= [
     { name="Name", email="info@wetsuits.com" }
 ]
+
 description = "integration"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 1 - Planning",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests==2.31.0",
-    "pandas==1.5.2"
+    "pandas==2.0.3"
 ]
 
 [project.urls]
 
 [tool.black]
 line-length = 88
 target-version = ['py310']
```

### Comparing `integration-wetsuits-0.0.1/src/edi.py` & `integration-wetsuits-0.0.10/src/integration_wetsuits/edi.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,50 +2,40 @@
 import clappform
 import clappform.dataclasses as cldc
 import pandas as pd
 
 class Edi:
 
     edifact_order_header_regexes =  {
-        
-    #header
-    "messagenumber": "BGM\+\d+\+([\d:]+)\+",
-    "messagedate": "DTM\+137:([^:]+)",
-    "buyerid":"(?<=NAD\+BY\+)([^:]+)",
-    "buyerreference":"(?<=NAD\+SU\+)([^:]+)",
-    "deliveryaddressID":"(?<=NAD\+DP\+)([^:]+)",
-    #"deliverypartyname":"(?<=NAD\+DP\+\d{13}::\d+\+\+)[^+]+",
-    "deliverypartyaddress":"NAD\+DP\+\d{13}::\d+\+\+\+[^+]+", # not working
-        
-    #rows
-        
+        "messagenumber": "BGM\+\d+\+([\d:]+)\+",
+        "messagedate": "DTM\+137:([^:]+)",
+        "buyerid":"(?<=NAD\+BY\+)([^:]+)",
+        "buyerreference":"(?<=NAD\+SU\+)([^:]+)",
+        "deliveryaddressID":"(?<=NAD\+DP\+)([^:]+)",
+        #"deliverypartyname":"(?<=NAD\+DP\+\d{13}::\d+\+\+)[^+]+",
+        "deliverypartyaddress":"NAD\+DP\+\d{13}::\d+\+\+\+[^+]+", # not working
     }
-    
 
     edifact_order_lines_regexes = {
-        #row
         "currency":"CUX\+2:([A-Z]{3}):",
         "lineitemnr":"LIN\+(\d+)\+\+",
         "barcode":"LIN.[a-z0-9]*\+\+([0-9]*)",
         "fedas":"PIA.[a-z0-9]*\+(\d+).GD",
         "quantity":"PIA.[a-z0-9]*\+(\d+).ST",
         "itemNr":"PIA.[a-z0-9]*\+(\d+).SA",
         "itemcolor":"(?<=IMD\+C\+35\+)\d+",
         "itemsize":"(?<=IMD\+C\+98\+).[a-z0-9]*",
         "deliverydate":"(?<=DTM\+2:)\d{8}",
         "grossprice":"(?<=PRI\+AAB:)(\d*.\d*)?",
         "netprice": "(?<=PRI\+NTP:)(\d*.\d*)?"
     }
-    
 
     id=None
 
     def __init__(self, message):
         self.message = message
 
-    
-
     def parser(self):
         for reg in self.edifact_order_lines_regexes.items():
             print(reg)
-        
-    
+
+
```

