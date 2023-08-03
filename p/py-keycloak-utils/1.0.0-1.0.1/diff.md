# Comparing `tmp/py-keycloak-utils-1.0.0.tar.gz` & `tmp/py-keycloak-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-keycloak-utils-1.0.0.tar", last modified: Thu Jul 20 13:35:17 2023, max compression
+gzip compressed data, was "py-keycloak-utils-1.0.1.tar", last modified: Thu Aug  3 09:40:31 2023, max compression
```

## Comparing `py-keycloak-utils-1.0.0.tar` & `py-keycloak-utils-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-07-20 13:35:17.081884 py-keycloak-utils-1.0.0/
--rw-r--r--   0 erne      (1000) erne      (1000)      431 2023-07-20 13:35:17.081884 py-keycloak-utils-1.0.0/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)     6386 2023-07-20 13:12:23.000000 py-keycloak-utils-1.0.0/README.md
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-07-20 13:35:17.081884 py-keycloak-utils-1.0.0/py_keycloak_utils.egg-info/
--rw-r--r--   0 erne      (1000) erne      (1000)      431 2023-07-20 13:35:16.000000 py-keycloak-utils-1.0.0/py_keycloak_utils.egg-info/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)      281 2023-07-20 13:35:16.000000 py-keycloak-utils-1.0.0/py_keycloak_utils.egg-info/SOURCES.txt
--rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-07-20 13:35:16.000000 py-keycloak-utils-1.0.0/py_keycloak_utils.egg-info/dependency_links.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       44 2023-07-20 13:35:16.000000 py-keycloak-utils-1.0.0/py_keycloak_utils.egg-info/requires.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       16 2023-07-20 13:35:16.000000 py-keycloak-utils-1.0.0/py_keycloak_utils.egg-info/top_level.txt
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-07-20 13:35:17.081884 py-keycloak-utils-1.0.0/pykeycloakutils/
--rw-r--r--   0 erne      (1000) erne      (1000)       54 2023-07-20 13:19:46.000000 py-keycloak-utils-1.0.0/pykeycloakutils/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     1160 2023-07-20 13:23:33.000000 py-keycloak-utils-1.0.0/pykeycloakutils/_decorators.py
--rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-07-20 13:35:17.081884 py-keycloak-utils-1.0.0/setup.cfg
--rw-r--r--   0 erne      (1000) erne      (1000)      761 2023-07-20 13:30:11.000000 py-keycloak-utils-1.0.0/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-03 09:40:31.138481 py-keycloak-utils-1.0.1/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      431 2023-08-03 09:40:31.138481 py-keycloak-utils-1.0.1/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     6386 2023-08-03 07:43:36.000000 py-keycloak-utils-1.0.1/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-03 09:40:31.138481 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      431 2023-08-03 09:40:30.000000 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      281 2023-08-03 09:40:30.000000 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-03 09:40:30.000000 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       44 2023-08-03 09:40:30.000000 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       16 2023-08-03 09:40:30.000000 py-keycloak-utils-1.0.1/py_keycloak_utils.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-03 09:40:31.138481 py-keycloak-utils-1.0.1/pykeycloakutils/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       82 2023-08-03 09:24:50.000000 py-keycloak-utils-1.0.1/pykeycloakutils/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3105 2023-08-03 09:34:25.000000 py-keycloak-utils-1.0.1/pykeycloakutils/_decorators.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-03 09:40:31.138481 py-keycloak-utils-1.0.1/setup.cfg
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      761 2023-08-03 09:24:50.000000 py-keycloak-utils-1.0.1/setup.py
```

### Comparing `py-keycloak-utils-1.0.0/README.md` & `py-keycloak-utils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `py-keycloak-utils-1.0.0/setup.py` & `py-keycloak-utils-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = "Utilities with Keycloak"
 
 # Setting up
 setup(
     name="py-keycloak-utils",
     version=VERSION,
     author="KE",
```

