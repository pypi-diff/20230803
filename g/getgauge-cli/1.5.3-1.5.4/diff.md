# Comparing `tmp/getgauge-cli-1.5.3.tar.gz` & `tmp/getgauge-cli-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getgauge-cli-1.5.3.tar", last modified: Fri Jul 28 12:18:55 2023, max compression
+gzip compressed data, was "getgauge-cli-1.5.4.tar", last modified: Thu Aug  3 08:23:21 2023, max compression
```

## Comparing `getgauge-cli-1.5.3.tar` & `getgauge-cli-1.5.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:18:55.735874 getgauge-cli-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 12:18:38.000000 getgauge-cli-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-28 12:18:55.735874 getgauge-cli-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-28 12:18:38.000000 getgauge-cli-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:18:55.735874 getgauge-cli-1.5.3/getgauge_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-28 12:18:55.000000 getgauge-cli-1.5.3/getgauge_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-28 12:18:55.000000 getgauge-cli-1.5.3/getgauge_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:18:55.000000 getgauge-cli-1.5.3/getgauge_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 12:18:55.000000 getgauge-cli-1.5.3/getgauge_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:18:55.000000 getgauge-cli-1.5.3/getgauge_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 12:18:55.735874 getgauge-cli-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-28 12:18:54.000000 getgauge-cli-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:23:21.900016 getgauge-cli-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 08:23:06.000000 getgauge-cli-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-03 08:23:21.900016 getgauge-cli-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-08-03 08:23:06.000000 getgauge-cli-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:23:21.900016 getgauge-cli-1.5.4/getgauge_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-03 08:23:21.000000 getgauge-cli-1.5.4/getgauge_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-03 08:23:21.000000 getgauge-cli-1.5.4/getgauge_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:23:21.000000 getgauge-cli-1.5.4/getgauge_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 08:23:21.000000 getgauge-cli-1.5.4/getgauge_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:23:21.000000 getgauge-cli-1.5.4/getgauge_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:23:21.900016 getgauge-cli-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-08-03 08:23:20.000000 getgauge-cli-1.5.4/setup.py
```

### Comparing `getgauge-cli-1.5.3/PKG-INFO` & `getgauge-cli-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getgauge-cli
-Version: 1.5.3
+Version: 1.5.4
 Home-page: https://github.com/getgauge/gauge
 Author: getgauge
 Author-email: getgauge@googlegroups.com
 Maintainer: getgauge
 License: Apache-2.0
 Platform: Windows
 Platform: Linux
```

### Comparing `getgauge-cli-1.5.3/README.md` & `getgauge-cli-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `getgauge-cli-1.5.3/getgauge_cli.egg-info/PKG-INFO` & `getgauge-cli-1.5.4/getgauge_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getgauge-cli
-Version: 1.5.3
+Version: 1.5.4
 Home-page: https://github.com/getgauge/gauge
 Author: getgauge
 Author-email: getgauge@googlegroups.com
 Maintainer: getgauge
 License: Apache-2.0
 Platform: Windows
 Platform: Linux
```

### Comparing `getgauge-cli-1.5.3/setup.py` & `getgauge-cli-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import platform
 import zipfile
 import os
 import sys
 
 
-_version = "1.5.3"
+_version = "1.5.4"
 _latest_version = ""
 
 
 class CustomInstallCommand(install):
     """Customized setuptools install command to download and setup."""
 
     _base_url = 'https://api.github.com/repos/getgauge/gauge/releases'
```

