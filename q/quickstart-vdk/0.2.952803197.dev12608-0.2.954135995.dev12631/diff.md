# Comparing `tmp/quickstart-vdk-0.2.952803197.dev12608.tar.gz` & `tmp/quickstart-vdk-0.2.954135995.dev12631.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.952803197.dev12608.tar", last modified: Wed Aug  2 04:24:04 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.954135995.dev12631.tar", last modified: Thu Aug  3 04:24:07 2023, max compression
```

## Comparing `quickstart-vdk-0.2.952803197.dev12608.tar` & `quickstart-vdk-0.2.954135995.dev12631.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 04:24:04.198743 quickstart-vdk-0.2.952803197.dev12608/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-08-02 04:24:04.194743 quickstart-vdk-0.2.952803197.dev12608/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-08-02 04:21:15.000000 quickstart-vdk-0.2.952803197.dev12608/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 04:24:04.194743 quickstart-vdk-0.2.952803197.dev12608/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-08-02 04:24:04.000000 quickstart-vdk-0.2.952803197.dev12608/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-08-02 04:24:04.000000 quickstart-vdk-0.2.952803197.dev12608/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 04:24:04.000000 quickstart-vdk-0.2.952803197.dev12608/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-08-02 04:24:04.000000 quickstart-vdk-0.2.952803197.dev12608/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-02 04:24:04.000000 quickstart-vdk-0.2.952803197.dev12608/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 04:24:04.198743 quickstart-vdk-0.2.952803197.dev12608/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-08-02 04:23:51.000000 quickstart-vdk-0.2.952803197.dev12608/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 04:24:04.194743 quickstart-vdk-0.2.952803197.dev12608/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-08-02 04:21:15.000000 quickstart-vdk-0.2.952803197.dev12608/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 04:24:07.214194 quickstart-vdk-0.2.954135995.dev12631/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-08-03 04:24:07.214194 quickstart-vdk-0.2.954135995.dev12631/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-08-03 04:21:17.000000 quickstart-vdk-0.2.954135995.dev12631/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 04:24:07.214194 quickstart-vdk-0.2.954135995.dev12631/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-08-03 04:24:07.000000 quickstart-vdk-0.2.954135995.dev12631/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-08-03 04:24:07.000000 quickstart-vdk-0.2.954135995.dev12631/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 04:24:07.000000 quickstart-vdk-0.2.954135995.dev12631/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-08-03 04:24:07.000000 quickstart-vdk-0.2.954135995.dev12631/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-03 04:24:07.000000 quickstart-vdk-0.2.954135995.dev12631/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-03 04:24:07.214194 quickstart-vdk-0.2.954135995.dev12631/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-08-03 04:23:55.000000 quickstart-vdk-0.2.954135995.dev12631/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 04:24:07.214194 quickstart-vdk-0.2.954135995.dev12631/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-08-03 04:21:17.000000 quickstart-vdk-0.2.954135995.dev12631/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.952803197.dev12608/PKG-INFO` & `quickstart-vdk-0.2.954135995.dev12631/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.952803197.dev12608
+Version: 0.2.954135995.dev12631
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.952803197.dev12608/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.954135995.dev12631/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.952803197.dev12608
+Version: 0.2.954135995.dev12631
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.952803197.dev12608/setup.py` & `quickstart-vdk-0.2.954135995.dev12631/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.952803197.dev12608"
+__version__ = "0.2.954135995.dev12631"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

