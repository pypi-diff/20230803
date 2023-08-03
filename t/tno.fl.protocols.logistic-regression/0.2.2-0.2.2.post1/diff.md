# Comparing `tmp/tno.fl.protocols.logistic_regression-0.2.2.tar.gz` & `tmp/tno.fl.protocols.logistic_regression-0.2.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tno.fl.protocols.logistic_regression-0.2.2.tar", last modified: Thu Aug  3 10:35:38 2023, max compression
+gzip compressed data, was "tno.fl.protocols.logistic_regression-0.2.2.post1.tar", last modified: Thu Aug  3 11:59:39 2023, max compression
```

## Comparing `tno.fl.protocols.logistic_regression-0.2.2.tar` & `tno.fl.protocols.logistic_regression-0.2.2.post1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 10:35:38.907544 tno.fl.protocols.logistic_regression-0.2.2/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      716 2023-08-03 10:35:00.000000 tno.fl.protocols.logistic_regression-0.2.2/CITATION.cff
--rw-r--r--   0 thomas    (1000) thomas    (1000)    10986 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2/LICENSE
--rw-r--r--   0 thomas    (1000) thomas    (1000)    11168 2023-08-03 10:35:38.897544 tno.fl.protocols.logistic_regression-0.2.2/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)    10157 2023-08-01 13:45:55.000000 tno.fl.protocols.logistic_regression-0.2.2/README.md
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1484 2023-08-01 13:40:30.000000 tno.fl.protocols.logistic_regression-0.2.2/pyproject.toml
--rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2023-08-03 10:35:38.907544 tno.fl.protocols.logistic_regression-0.2.2/setup.cfg
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 10:35:38.897544 tno.fl.protocols.logistic_regression-0.2.2/src/
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 10:35:38.897544 tno.fl.protocols.logistic_regression-0.2.2/src/tno/
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 10:35:38.897544 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 10:35:38.897544 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 10:35:38.897544 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       58 2023-08-01 13:28:42.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5633 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/client.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     8642 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/config.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      191 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/msg_ids.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/py.typed
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5057 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/server.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 10:35:38.897544 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/test/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/test/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1881 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/test/test_config.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2060 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/test/test_protocol.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 10:35:38.897544 tno.fl.protocols.logistic_regression-0.2.2/src/tno.fl.protocols.logistic_regression.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    11168 2023-08-03 10:35:38.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno.fl.protocols.logistic_regression.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)      854 2023-08-03 10:35:38.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno.fl.protocols.logistic_regression.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-08-03 10:35:38.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno.fl.protocols.logistic_regression.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       90 2023-08-03 10:35:38.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno.fl.protocols.logistic_regression.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        4 2023-08-03 10:35:38.000000 tno.fl.protocols.logistic_regression-0.2.2/src/tno.fl.protocols.logistic_regression.egg-info/top_level.txt
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 11:59:39.417544 tno.fl.protocols.logistic_regression-0.2.2.post1/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      716 2023-08-03 10:35:00.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/CITATION.cff
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    10986 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/LICENSE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    11189 2023-08-03 11:59:39.407544 tno.fl.protocols.logistic_regression-0.2.2.post1/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    10172 2023-08-03 11:57:29.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/README.md
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1484 2023-08-01 13:40:30.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/pyproject.toml
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       38 2023-08-03 11:59:39.417544 tno.fl.protocols.logistic_regression-0.2.2.post1/setup.cfg
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 11:59:39.407544 tno.fl.protocols.logistic_regression-0.2.2.post1/src/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 11:59:39.407544 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 11:59:39.407544 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 11:59:39.407544 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 11:59:39.407544 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       64 2023-08-03 11:59:17.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5633 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/client.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     8642 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/config.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      191 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/msg_ids.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/py.typed
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5057 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/server.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 11:59:39.407544 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/test/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/test/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1881 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/test/test_config.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2060 2023-08-01 12:23:35.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/test/test_protocol.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-08-03 11:59:39.407544 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno.fl.protocols.logistic_regression.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    11189 2023-08-03 11:59:39.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno.fl.protocols.logistic_regression.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      854 2023-08-03 11:59:39.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno.fl.protocols.logistic_regression.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-08-03 11:59:39.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno.fl.protocols.logistic_regression.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       90 2023-08-03 11:59:39.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno.fl.protocols.logistic_regression.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        4 2023-08-03 11:59:39.000000 tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno.fl.protocols.logistic_regression.egg-info/top_level.txt
```

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/CITATION.cff` & `tno.fl.protocols.logistic_regression-0.2.2.post1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/LICENSE` & `tno.fl.protocols.logistic_regression-0.2.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/PKG-INFO` & `tno.fl.protocols.logistic_regression-0.2.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tno.fl.protocols.logistic_regression
-Version: 0.2.2
+Version: 0.2.2.post1
 Summary: Generic utilities for implementing encryption schemes
 Author-email: TNO PET Lab <petlab@tno.nl>
 Maintainer-email: TNO PET Lab <petlab@tno.nl>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://pet.tno.nl/
 Project-URL: Documentation, https://docs.pet.tno.nl/fl/protocols/logistic_regression/0.2.2
 Project-URL: Source, https://github.com/TNO-FL/protocols.logistic_regression
@@ -50,15 +50,15 @@
 _Limitations in (end-)use: the content of this software package may solely be
 used for applications that comply with international export control laws.  
 This implementation of cryptographic software has not been audited. Use at your
 own risk._
 
 ## Documentation
 
-Documentation of the tno.mpc.communication package can be found
+Documentation of the tno.fl.protocols.logistic_regression package can be found
 [here](https://docs.pet.tno.nl/fl/protocols/logistic_regression/0.2.2).
 
 ## Install
 
 Easily install the tno.fl.protocols.logistic_regression package using pip:
 
 ```console
```

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/README.md` & `tno.fl.protocols.logistic_regression-0.2.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 _Limitations in (end-)use: the content of this software package may solely be
 used for applications that comply with international export control laws.  
 This implementation of cryptographic software has not been audited. Use at your
 own risk._
 
 ## Documentation
 
-Documentation of the tno.mpc.communication package can be found
+Documentation of the tno.fl.protocols.logistic_regression package can be found
 [here](https://docs.pet.tno.nl/fl/protocols/logistic_regression/0.2.2).
 
 ## Install
 
 Easily install the tno.fl.protocols.logistic_regression package using pip:
 
 ```console
```

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/pyproject.toml` & `tno.fl.protocols.logistic_regression-0.2.2.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/client.py` & `tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/client.py`

 * *Files identical despite different names*

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/config.py` & `tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/config.py`

 * *Files identical despite different names*

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/server.py` & `tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/server.py`

 * *Files identical despite different names*

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/test/test_config.py` & `tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/test/test_config.py`

 * *Files identical despite different names*

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/src/tno/fl/protocols/logistic_regression/test/test_protocol.py` & `tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno/fl/protocols/logistic_regression/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/src/tno.fl.protocols.logistic_regression.egg-info/PKG-INFO` & `tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno.fl.protocols.logistic_regression.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tno.fl.protocols.logistic-regression
-Version: 0.2.2
+Version: 0.2.2.post1
 Summary: Generic utilities for implementing encryption schemes
 Author-email: TNO PET Lab <petlab@tno.nl>
 Maintainer-email: TNO PET Lab <petlab@tno.nl>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://pet.tno.nl/
 Project-URL: Documentation, https://docs.pet.tno.nl/fl/protocols/logistic_regression/0.2.2
 Project-URL: Source, https://github.com/TNO-FL/protocols.logistic_regression
@@ -50,15 +50,15 @@
 _Limitations in (end-)use: the content of this software package may solely be
 used for applications that comply with international export control laws.  
 This implementation of cryptographic software has not been audited. Use at your
 own risk._
 
 ## Documentation
 
-Documentation of the tno.mpc.communication package can be found
+Documentation of the tno.fl.protocols.logistic_regression package can be found
 [here](https://docs.pet.tno.nl/fl/protocols/logistic_regression/0.2.2).
 
 ## Install
 
 Easily install the tno.fl.protocols.logistic_regression package using pip:
 
 ```console
```

### Comparing `tno.fl.protocols.logistic_regression-0.2.2/src/tno.fl.protocols.logistic_regression.egg-info/SOURCES.txt` & `tno.fl.protocols.logistic_regression-0.2.2.post1/src/tno.fl.protocols.logistic_regression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

