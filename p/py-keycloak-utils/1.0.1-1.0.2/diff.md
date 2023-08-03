# Comparing `tmp/py-keycloak-utils-1.0.1.tar.gz` & `tmp/py-keycloak-utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-keycloak-utils-1.0.1.tar", last modified: Thu Aug  3 09:40:31 2023, max compression
+gzip compressed data, was "py-keycloak-utils-1.0.2.tar", last modified: Thu Aug  3 09:51:00 2023, max compression
```

## Comparing `py-keycloak-utils-1.0.1.tar` & `py-keycloak-utils-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-03 09:40:31.138481 py-keycloak-utils-1.0.1/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      431 2023-08-03 09:40:31.138481 py-keycloak-utils-1.0.1/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     6386 2023-08-03 07:43:36.000000 py-keycloak-utils-1.0.1/README.md
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-03 09:40:31.138481 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      431 2023-08-03 09:40:30.000000 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/PKG-INFO
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      281 2023-08-03 09:40:30.000000 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/SOURCES.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-03 09:40:30.000000 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/dependency_links.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       44 2023-08-03 09:40:30.000000 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/requires.txt
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       16 2023-08-03 09:40:30.000000 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/top_level.txt
-drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-03 09:40:31.138481 py-keycloak-utils-1.0.1/pykeycloakutils/
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       82 2023-08-03 09:24:50.000000 py-keycloak-utils-1.0.1/pykeycloakutils/__init__.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3105 2023-08-03 09:34:25.000000 py-keycloak-utils-1.0.1/pykeycloakutils/_decorators.py
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-03 09:40:31.138481 py-keycloak-utils-1.0.1/setup.cfg
--rw-r--r--   0 vgurin    (1000) vgurin    (1000)      761 2023-08-03 09:24:50.000000 py-keycloak-utils-1.0.1/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-03 09:51:00.228482 py-keycloak-utils-1.0.2/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      431 2023-08-03 09:51:00.228482 py-keycloak-utils-1.0.2/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     6386 2023-08-03 07:43:36.000000 py-keycloak-utils-1.0.2/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-03 09:51:00.228482 py-keycloak-utils-1.0.2/py_keycloak_utils.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      431 2023-08-03 09:50:59.000000 py-keycloak-utils-1.0.2/py_keycloak_utils.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      281 2023-08-03 09:50:59.000000 py-keycloak-utils-1.0.2/py_keycloak_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-03 09:50:59.000000 py-keycloak-utils-1.0.2/py_keycloak_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       44 2023-08-03 09:50:59.000000 py-keycloak-utils-1.0.2/py_keycloak_utils.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       16 2023-08-03 09:50:59.000000 py-keycloak-utils-1.0.2/py_keycloak_utils.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-03 09:51:00.228482 py-keycloak-utils-1.0.2/pykeycloakutils/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       82 2023-08-03 09:24:50.000000 py-keycloak-utils-1.0.2/pykeycloakutils/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3141 2023-08-03 09:50:20.000000 py-keycloak-utils-1.0.2/pykeycloakutils/_decorators.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-03 09:51:00.228482 py-keycloak-utils-1.0.2/setup.cfg
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      761 2023-08-03 09:50:39.000000 py-keycloak-utils-1.0.2/setup.py
```

### Comparing `py-keycloak-utils-1.0.1/README.md` & `py-keycloak-utils-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py-keycloak-utils-1.0.1/pykeycloakutils/_decorators.py` & `py-keycloak-utils-1.0.2/pykeycloakutils/_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import logging
-from flask import make_response, request
 from functools import wraps
+
+import requests
+from flask import request
 from keycloak import KeycloakOpenID
 from keycloak.exceptions import KeycloakError
+from requests import HTTPError
 
 
 def flask_keycloak_authenticate(server_url, client_id, client_secret_key):
     """
     Method to be used as decorator, which accepts instance of KeycloakOpenID
     :param server_url: the URL of keycloak.
     :param client_id: The client_id of keycloak.
```

### Comparing `py-keycloak-utils-1.0.1/setup.py` & `py-keycloak-utils-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "Utilities with Keycloak"
 
 # Setting up
 setup(
     name="py-keycloak-utils",
     version=VERSION,
     author="KE",
```

