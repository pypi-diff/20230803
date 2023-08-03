# Comparing `tmp/google-cloud-advisorynotifications-0.2.1.tar.gz` & `tmp/google-cloud-advisorynotifications-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-advisorynotifications-0.2.1.tar", last modified: Wed Jul  5 15:49:52 2023, max compression
+gzip compressed data, was "google-cloud-advisorynotifications-0.3.0.tar", last modified: Thu Aug  3 19:06:04 2023, max compression
```

## Comparing `google-cloud-advisorynotifications-0.2.1.tar` & `google-cloud-advisorynotifications-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4917 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3981 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.960839 google-cloud-advisorynotifications-0.2.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.960839 google-cloud-advisorynotifications-0.2.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.960839 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/
--rw-rw-r--   0 root         (0)     1003     1684 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/
--rw-rw-r--   0 root         (0)     1003     1499 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1508 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/
--rw-rw-r--   0 root         (0)     1003      825 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    19615 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28106 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py
--rw-rw-r--   0 root         (0)     1003     5956 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/
--rw-rw-r--   0 root         (0)     1003     1617 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7257 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13030 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13277 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17467 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/types/
--rw-rw-r--   0 root         (0)     1003     1134 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12969 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.964840 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/
--rw-r--r--   0 root         (0)     1003     4917 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2037 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:49:52.000000 google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2974 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:49:52.968840 google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/advisorynotifications_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/advisorynotifications_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   103948 2023-07-05 15:46:58.000000 google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.621470 google-cloud-advisorynotifications-0.3.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5036 2023-08-03 19:06:04.621470 google-cloud-advisorynotifications-0.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4100 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.613469 google-cloud-advisorynotifications-0.3.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.613469 google-cloud-advisorynotifications-0.3.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.617469 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications/
+-rw-rw-r--   0 root         (0)     1003     1684 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.617469 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/
+-rw-rw-r--   0 root         (0)     1003     1499 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1508 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.617469 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.617469 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/
+-rw-rw-r--   0 root         (0)     1003      825 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19616 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28107 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5956 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.617469 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1617 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7257 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13030 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13277 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17467 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.621470 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1134 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13217 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.621470 google-cloud-advisorynotifications-0.3.0/google_cloud_advisorynotifications.egg-info/
+-rw-r--r--   0 root         (0)     1003     5036 2023-08-03 19:06:04.000000 google-cloud-advisorynotifications-0.3.0/google_cloud_advisorynotifications.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2037 2023-08-03 19:06:04.000000 google-cloud-advisorynotifications-0.3.0/google_cloud_advisorynotifications.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:04.000000 google-cloud-advisorynotifications-0.3.0/google_cloud_advisorynotifications.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 19:06:04.000000 google-cloud-advisorynotifications-0.3.0/google_cloud_advisorynotifications.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:04.000000 google-cloud-advisorynotifications-0.3.0/google_cloud_advisorynotifications.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-08-03 19:06:04.000000 google-cloud-advisorynotifications-0.3.0/google_cloud_advisorynotifications.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 19:06:04.000000 google-cloud-advisorynotifications-0.3.0/google_cloud_advisorynotifications.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-08-03 19:06:04.621470 google-cloud-advisorynotifications-0.3.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2974 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.621470 google-cloud-advisorynotifications-0.3.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.621470 google-cloud-advisorynotifications-0.3.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.621470 google-cloud-advisorynotifications-0.3.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:04.621470 google-cloud-advisorynotifications-0.3.0/tests/unit/gapic/advisorynotifications_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/tests/unit/gapic/advisorynotifications_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   103948 2023-08-03 19:03:09.000000 google-cloud-advisorynotifications-0.3.0/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py
```

### Comparing `google-cloud-advisorynotifications-0.2.1/LICENSE` & `google-cloud-advisorynotifications-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.1/MANIFEST.in` & `google-cloud-advisorynotifications-0.3.0/MANIFEST.in`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/PKG-INFO` & `google-cloud-advisorynotifications-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-advisorynotifications
-Version: 0.2.1
+Version: 0.3.0
 Summary: Google Cloud Advisorynotifications API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Advisory Notifications.:  https://cloud.google.com/advisory-notifications/
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-advisorynotifications/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-advisorynotifications
+    pip install google-cloud-advisorynotifications
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-advisorynotifications
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-advisorynotifications
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Advisory Notifications
    to see other available methods on the client.
 -  Read the `Advisory Notifications Product documentation`_ to learn
```

### Comparing `google-cloud-advisorynotifications-0.2.1/README.rst` & `google-cloud-advisorynotifications-0.3.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Advisory Notifications.:  https://cloud.google.com/advisory-notifications/
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-advisorynotifications/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-advisorynotifications
+    pip install google-cloud-advisorynotifications
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-advisorynotifications
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-advisorynotifications
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Advisory Notifications
    to see other available methods on the client.
 -  Read the `Advisory Notifications Product documentation`_ to learn
```

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/__init__.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications/__init__.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications/gapic_version.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
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
-__version__ = "0.2.1"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/__init__.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/__init__.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/gapic_metadata.json` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/gapic_version.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
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
-__version__ = "0.2.1"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/__init__.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/__init__.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py`

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
@@ -394,14 +394,15 @@
 
         Args:
             request (Optional[Union[google.cloud.advisorynotifications_v1.types.GetNotificationRequest, dict]]):
                 The request object. Request for fetching a notification.
             name (:class:`str`):
                 Required. A name of the notification
                 to retrieve. Format:
+
                 organizations/{organization}/locations/{location}/notifications/{notification}.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py`

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
@@ -607,14 +607,15 @@
 
         Args:
             request (Union[google.cloud.advisorynotifications_v1.types.GetNotificationRequest, dict]):
                 The request object. Request for fetching a notification.
             name (str):
                 Required. A name of the notification
                 to retrieve. Format:
+
                 organizations/{organization}/locations/{location}/notifications/{notification}.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
```

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/types/__init__.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/types/__init__.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/google/cloud/advisorynotifications_v1/types/service.py` & `google-cloud-advisorynotifications-0.3.0/google/cloud/advisorynotifications_v1/types/service.py`

 * *Files 2% similar despite different names*

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
@@ -64,20 +64,21 @@
 
     Values:
         LOCALIZATION_STATE_UNSPECIFIED (0):
             Not used.
         LOCALIZATION_STATE_NOT_APPLICABLE (1):
             Localization is not applicable for requested
             language. This can happen when:
+
             - The requested language was not supported by
-            Advisory Notifications at the time of
-            localization (including notifications created
-            before the localization feature was launched).
+              Advisory Notifications at the time of
+              localization (including notifications created
+              before the localization feature was launched).
             - The requested language is English, so only the
-            English text is returned.
+              English text is returned.
         LOCALIZATION_STATE_PENDING (2):
             Localization for requested language is in
             progress, and not ready yet.
         LOCALIZATION_STATE_COMPLETED (3):
             Localization for requested language is
             completed.
     """
@@ -93,28 +94,35 @@
     Values:
         NOTIFICATION_TYPE_UNSPECIFIED (0):
             Default type
         NOTIFICATION_TYPE_SECURITY_PRIVACY_ADVISORY (1):
             Security and privacy advisory notifications
         NOTIFICATION_TYPE_SENSITIVE_ACTIONS (2):
             Sensitive action notifications
+        NOTIFICATION_TYPE_SECURITY_MSA (3):
+            General security MSA
+        NOTIFICATION_TYPE_THREAT_HORIZONS (4):
+            Threat horizons MSA
     """
     NOTIFICATION_TYPE_UNSPECIFIED = 0
     NOTIFICATION_TYPE_SECURITY_PRIVACY_ADVISORY = 1
     NOTIFICATION_TYPE_SENSITIVE_ACTIONS = 2
+    NOTIFICATION_TYPE_SECURITY_MSA = 3
+    NOTIFICATION_TYPE_THREAT_HORIZONS = 4
 
 
 class Notification(proto.Message):
     r"""A notification object for notifying customers about security
     and privacy issues.
 
     Attributes:
         name (str):
             The resource name of the notification.
             Format:
+
             organizations/{organization}/locations/{location}/notifications/{notification}.
         subject (google.cloud.advisorynotifications_v1.types.Subject):
             The subject line of the notification.
         messages (MutableSequence[google.cloud.advisorynotifications_v1.types.Message]):
             A list of messages in the notification.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time the notification was
@@ -401,14 +409,15 @@
 class GetNotificationRequest(proto.Message):
     r"""Request for fetching a notification.
 
     Attributes:
         name (str):
             Required. A name of the notification to
             retrieve. Format:
+
             organizations/{organization}/locations/{location}/notifications/{notification}.
         language_code (str):
             ISO code for requested localization language.
             If unset, will be interpereted as "en". If the
             requested language is valid, but not supported
             for this notification, English will be returned
             with an "Not applicable" LocalizationState. If
```

### Comparing `google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/PKG-INFO` & `google-cloud-advisorynotifications-0.3.0/google_cloud_advisorynotifications.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-advisorynotifications
-Version: 0.2.1
+Version: 0.3.0
 Summary: Google Cloud Advisorynotifications API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Advisory Notifications.:  https://cloud.google.com/advisory-notifications/
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-advisorynotifications/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-advisorynotifications
+    pip install google-cloud-advisorynotifications
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-advisorynotifications
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-advisorynotifications
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Advisory Notifications
    to see other available methods on the client.
 -  Read the `Advisory Notifications Product documentation`_ to learn
```

### Comparing `google-cloud-advisorynotifications-0.2.1/google_cloud_advisorynotifications.egg-info/SOURCES.txt` & `google-cloud-advisorynotifications-0.3.0/google_cloud_advisorynotifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.2.1/setup.py` & `google-cloud-advisorynotifications-0.3.0/setup.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/tests/__init__.py` & `google-cloud-advisorynotifications-0.3.0/tests/__init__.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/tests/unit/__init__.py` & `google-cloud-advisorynotifications-0.3.0/tests/unit/__init__.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/__init__.py` & `google-cloud-advisorynotifications-0.3.0/tests/unit/gapic/__init__.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/advisorynotifications_v1/__init__.py` & `google-cloud-advisorynotifications-0.3.0/tests/unit/gapic/advisorynotifications_v1/__init__.py`

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

### Comparing `google-cloud-advisorynotifications-0.2.1/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py` & `google-cloud-advisorynotifications-0.3.0/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py`

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

