# Comparing `tmp/google-cloud-confidentialcomputing-0.1.1.tar.gz` & `tmp/google-cloud-confidentialcomputing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-confidentialcomputing-0.1.1.tar", last modified: Wed Jul  5 15:51:32 2023, max compression
+gzip compressed data, was "google-cloud-confidentialcomputing-0.2.0.tar", last modified: Thu Aug  3 19:06:35 2023, max compression
```

## Comparing `google-cloud-confidentialcomputing-0.1.1.tar` & `google-cloud-confidentialcomputing-0.2.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4822 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3886 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.548206 google-cloud-confidentialcomputing-0.1.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.548206 google-cloud-confidentialcomputing-0.1.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.548206 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/
--rw-rw-r--   0 root         (0)     1003     1446 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.548206 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/
--rw-rw-r--   0 root         (0)     1003     1269 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1480 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.548206 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/
--rw-rw-r--   0 root         (0)     1003      797 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/__init__.py
--rw-rw-r--   0 root         (0)     1003    22618 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/async_client.py
--rw-rw-r--   0 root         (0)     1003    31103 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7821 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14797 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15031 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    25103 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/types/
--rw-rw-r--   0 root         (0)     1003      940 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     8300 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/
--rw-r--r--   0 root         (0)     1003     4822 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1877 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:51:32.000000 google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:51:32.556207 google-cloud-confidentialcomputing-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2974 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:32.552207 google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/confidentialcomputing_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/confidentialcomputing_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   103349 2023-07-05 15:46:58.000000 google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/confidentialcomputing_v1/test_confidential_computing.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.202925 google-cloud-confidentialcomputing-0.2.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4941 2023-08-03 19:06:35.202925 google-cloud-confidentialcomputing-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4005 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.194924 google-cloud-confidentialcomputing-0.2.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.194924 google-cloud-confidentialcomputing-0.2.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.198924 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing/
+-rw-rw-r--   0 root         (0)     1003     1684 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.198924 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/
+-rw-rw-r--   0 root         (0)     1003     1507 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1480 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.198924 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.198924 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/
+-rw-rw-r--   0 root         (0)     1003      797 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22618 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/async_client.py
+-rw-rw-r--   0 root         (0)     1003    31103 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.198924 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7821 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14797 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15031 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    25103 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.202925 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1178 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13366 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.202925 google-cloud-confidentialcomputing-0.2.0/google_cloud_confidentialcomputing.egg-info/
+-rw-r--r--   0 root         (0)     1003     4941 2023-08-03 19:06:35.000000 google-cloud-confidentialcomputing-0.2.0/google_cloud_confidentialcomputing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1877 2023-08-03 19:06:35.000000 google-cloud-confidentialcomputing-0.2.0/google_cloud_confidentialcomputing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:35.000000 google-cloud-confidentialcomputing-0.2.0/google_cloud_confidentialcomputing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 19:06:35.000000 google-cloud-confidentialcomputing-0.2.0/google_cloud_confidentialcomputing.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:35.000000 google-cloud-confidentialcomputing-0.2.0/google_cloud_confidentialcomputing.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-08-03 19:06:35.000000 google-cloud-confidentialcomputing-0.2.0/google_cloud_confidentialcomputing.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 19:06:35.000000 google-cloud-confidentialcomputing-0.2.0/google_cloud_confidentialcomputing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-08-03 19:06:35.202925 google-cloud-confidentialcomputing-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2974 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.202925 google-cloud-confidentialcomputing-0.2.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.202925 google-cloud-confidentialcomputing-0.2.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.202925 google-cloud-confidentialcomputing-0.2.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:35.202925 google-cloud-confidentialcomputing-0.2.0/tests/unit/gapic/confidentialcomputing_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/tests/unit/gapic/confidentialcomputing_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   103349 2023-08-03 19:03:10.000000 google-cloud-confidentialcomputing-0.2.0/tests/unit/gapic/confidentialcomputing_v1/test_confidential_computing.py
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/LICENSE` & `google-cloud-confidentialcomputing-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.1/MANIFEST.in` & `google-cloud-confidentialcomputing-0.2.0/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2020 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/PKG-INFO` & `google-cloud-confidentialcomputing-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-confidentialcomputing
-Version: 0.1.1
+Version: 0.2.0
 Summary: Google Cloud Confidentialcomputing API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Confidential Computing API.:  https://cloud.google.com/confidential-computing
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
-Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
+creates isolated Python environments. These isolated environments can have separate
+versions of Python packages, which allows you to isolate one project's dependencies
+from the dependencies of other projects.
 
-With `virtualenv`_, it's possible to install this library without needing system
+With `venv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
-.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+.. _`venv`: https://docs.python.org/3/library/venv.html
 
 
 Code samples and snippets
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Code samples and snippets live in the `samples/` folder.
+Code samples and snippets live in the `samples/`_ folder.
+
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-confidentialcomputing/samples
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
 Python.
 
@@ -97,29 +100,27 @@
 .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
+    python3 -m venv <your-env>
     source <your-env>/bin/activate
-    <your-env>/bin/pip install google-cloud-confidentialcomputing
+    pip install google-cloud-confidentialcomputing
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-confidentialcomputing
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-confidentialcomputing
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Confidential Computing API
    to see other available methods on the client.
 -  Read the `Confidential Computing API Product documentation`_ to learn
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/README.rst` & `google-cloud-confidentialcomputing-0.2.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Confidential Computing API.:  https://cloud.google.com/confidential-computing
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
-Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
+creates isolated Python environments. These isolated environments can have separate
+versions of Python packages, which allows you to isolate one project's dependencies
+from the dependencies of other projects.
 
-With `virtualenv`_, it's possible to install this library without needing system
+With `venv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
-.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+.. _`venv`: https://docs.python.org/3/library/venv.html
 
 
 Code samples and snippets
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Code samples and snippets live in the `samples/` folder.
+Code samples and snippets live in the `samples/`_ folder.
+
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-confidentialcomputing/samples
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
 Python.
 
@@ -73,29 +76,27 @@
 .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
+    python3 -m venv <your-env>
     source <your-env>/bin/activate
-    <your-env>/bin/pip install google-cloud-confidentialcomputing
+    pip install google-cloud-confidentialcomputing
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-confidentialcomputing
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-confidentialcomputing
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Confidential Computing API
    to see other available methods on the client.
 -  Read the `Confidential Computing API Product documentation`_ to learn
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/__init__.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,24 +22,34 @@
     ConfidentialComputingAsyncClient,
 )
 from google.cloud.confidentialcomputing_v1.services.confidential_computing.client import (
     ConfidentialComputingClient,
 )
 from google.cloud.confidentialcomputing_v1.types.service import (
     Challenge,
+    ConfidentialSpaceInfo,
+    ContainerImageSignature,
     CreateChallengeRequest,
     GcpCredentials,
+    SignedEntity,
+    SigningAlgorithm,
+    TokenOptions,
     TpmAttestation,
     VerifyAttestationRequest,
     VerifyAttestationResponse,
 )
 
 __all__ = (
     "ConfidentialComputingClient",
     "ConfidentialComputingAsyncClient",
     "Challenge",
+    "ConfidentialSpaceInfo",
+    "ContainerImageSignature",
     "CreateChallengeRequest",
     "GcpCredentials",
+    "SignedEntity",
+    "TokenOptions",
     "TpmAttestation",
     "VerifyAttestationRequest",
     "VerifyAttestationResponse",
+    "SigningAlgorithm",
 )
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing/gapic_version.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/__init__.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,24 +20,34 @@
 
 from .services.confidential_computing import (
     ConfidentialComputingAsyncClient,
     ConfidentialComputingClient,
 )
 from .types.service import (
     Challenge,
+    ConfidentialSpaceInfo,
+    ContainerImageSignature,
     CreateChallengeRequest,
     GcpCredentials,
+    SignedEntity,
+    SigningAlgorithm,
+    TokenOptions,
     TpmAttestation,
     VerifyAttestationRequest,
     VerifyAttestationResponse,
 )
 
 __all__ = (
     "ConfidentialComputingAsyncClient",
     "Challenge",
     "ConfidentialComputingClient",
+    "ConfidentialSpaceInfo",
+    "ContainerImageSignature",
     "CreateChallengeRequest",
     "GcpCredentials",
+    "SignedEntity",
+    "SigningAlgorithm",
+    "TokenOptions",
     "TpmAttestation",
     "VerifyAttestationRequest",
     "VerifyAttestationResponse",
 )
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/gapic_metadata.json` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/gapic_version.py` & `google-cloud-confidentialcomputing-0.2.0/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/__init__.py` & `google-cloud-confidentialcomputing-0.2.0/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/__init__.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/async_client.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/client.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/__init__.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/base.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc_asyncio.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/rest.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/services/confidential_computing/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google/cloud/confidentialcomputing_v1/types/__init__.py` & `google-cloud-confidentialcomputing-0.2.0/google/cloud/confidentialcomputing_v1/types/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,22 +11,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from .service import (
     Challenge,
+    ConfidentialSpaceInfo,
+    ContainerImageSignature,
     CreateChallengeRequest,
     GcpCredentials,
+    SignedEntity,
+    SigningAlgorithm,
+    TokenOptions,
     TpmAttestation,
     VerifyAttestationRequest,
     VerifyAttestationResponse,
 )
 
 __all__ = (
     "Challenge",
+    "ConfidentialSpaceInfo",
+    "ContainerImageSignature",
     "CreateChallengeRequest",
     "GcpCredentials",
+    "SignedEntity",
+    "TokenOptions",
     "TpmAttestation",
     "VerifyAttestationRequest",
     "VerifyAttestationResponse",
+    "SigningAlgorithm",
 )
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/PKG-INFO` & `google-cloud-confidentialcomputing-0.2.0/google_cloud_confidentialcomputing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-confidentialcomputing
-Version: 0.1.1
+Version: 0.2.0
 Summary: Google Cloud Confidentialcomputing API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Confidential Computing API.:  https://cloud.google.com/confidential-computing
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
-Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
+creates isolated Python environments. These isolated environments can have separate
+versions of Python packages, which allows you to isolate one project's dependencies
+from the dependencies of other projects.
 
-With `virtualenv`_, it's possible to install this library without needing system
+With `venv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
-.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+.. _`venv`: https://docs.python.org/3/library/venv.html
 
 
 Code samples and snippets
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Code samples and snippets live in the `samples/` folder.
+Code samples and snippets live in the `samples/`_ folder.
+
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-confidentialcomputing/samples
 
 
 Supported Python Versions
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
 Python.
 
@@ -97,29 +100,27 @@
 .. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
 
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
+    python3 -m venv <your-env>
     source <your-env>/bin/activate
-    <your-env>/bin/pip install google-cloud-confidentialcomputing
+    pip install google-cloud-confidentialcomputing
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-confidentialcomputing
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-confidentialcomputing
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Confidential Computing API
    to see other available methods on the client.
 -  Read the `Confidential Computing API Product documentation`_ to learn
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/google_cloud_confidentialcomputing.egg-info/SOURCES.txt` & `google-cloud-confidentialcomputing-0.2.0/google_cloud_confidentialcomputing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-confidentialcomputing-0.1.1/setup.py` & `google-cloud-confidentialcomputing-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/tests/__init__.py` & `google-cloud-confidentialcomputing-0.2.0/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/tests/unit/__init__.py` & `google-cloud-confidentialcomputing-0.2.0/tests/unit/gapic/confidentialcomputing_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-confidentialcomputing-0.1.1/tests/unit/gapic/confidentialcomputing_v1/test_confidential_computing.py` & `google-cloud-confidentialcomputing-0.2.0/tests/unit/gapic/confidentialcomputing_v1/test_confidential_computing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

