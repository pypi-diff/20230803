# Comparing `tmp/google-cloud-bigquery-data-exchange-0.5.4.tar.gz` & `tmp/google-cloud-bigquery-data-exchange-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-data-exchange-0.5.4.tar", last modified: Wed Jul  5 15:51:01 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-data-exchange-0.5.5.tar", last modified: Thu Aug  3 19:06:22 2023, max compression
```

## Comparing `google-cloud-bigquery-data-exchange-0.5.4.tar` & `google-cloud-bigquery-data-exchange-0.5.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.902845 google-cloud-bigquery-data-exchange-0.5.4/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4906 2023-07-05 15:51:01.902845 google-cloud-bigquery-data-exchange-0.5.4/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3968 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.890844 google-cloud-bigquery-data-exchange-0.5.4/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.890844 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.894844 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/
--rw-rw-r--   0 root         (0)     1003     2366 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       96 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.894844 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2177 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4399 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       96 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.894844 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.894844 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    86200 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    97979 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py
--rw-rw-r--   0 root         (0)     1003    16537 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    13308 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    30551 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    31129 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1851 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    26457 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/
--rw-r--r--   0 root         (0)     1003     4906 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1986 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:51:01.000000 google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:51:01.902845 google-cloud-bigquery-data-exchange-0.5.4/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3024 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:01.898845 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/bigquery_data_exchange_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   217456 2023-07-05 15:46:58.000000 google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.062454 google-cloud-bigquery-data-exchange-0.5.5/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5026 2023-08-03 19:06:22.062454 google-cloud-bigquery-data-exchange-0.5.5/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4088 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.054454 google-cloud-bigquery-data-exchange-0.5.5/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.054454 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.054454 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange/
+-rw-rw-r--   0 root         (0)     1003     2366 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       96 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.058454 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2177 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4399 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       96 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.058454 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.058454 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    85460 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    97239 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16537 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.058454 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13308 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30551 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    31129 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.058454 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1851 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26457 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.058454 google-cloud-bigquery-data-exchange-0.5.5/google_cloud_bigquery_data_exchange.egg-info/
+-rw-r--r--   0 root         (0)     1003     5026 2023-08-03 19:06:21.000000 google-cloud-bigquery-data-exchange-0.5.5/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1986 2023-08-03 19:06:22.000000 google-cloud-bigquery-data-exchange-0.5.5/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:21.000000 google-cloud-bigquery-data-exchange-0.5.5/google_cloud_bigquery_data_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 19:06:21.000000 google-cloud-bigquery-data-exchange-0.5.5/google_cloud_bigquery_data_exchange.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:21.000000 google-cloud-bigquery-data-exchange-0.5.5/google_cloud_bigquery_data_exchange.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-08-03 19:06:21.000000 google-cloud-bigquery-data-exchange-0.5.5/google_cloud_bigquery_data_exchange.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 19:06:21.000000 google-cloud-bigquery-data-exchange-0.5.5/google_cloud_bigquery_data_exchange.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-08-03 19:06:22.062454 google-cloud-bigquery-data-exchange-0.5.5/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3024 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.058454 google-cloud-bigquery-data-exchange-0.5.5/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.062454 google-cloud-bigquery-data-exchange-0.5.5/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.062454 google-cloud-bigquery-data-exchange-0.5.5/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:22.062454 google-cloud-bigquery-data-exchange-0.5.5/tests/unit/gapic/bigquery_data_exchange_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   217456 2023-08-03 19:03:10.000000 google-cloud-bigquery-data-exchange-0.5.5/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/LICENSE` & `google-cloud-bigquery-data-exchange-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/MANIFEST.in` & `google-cloud-bigquery-data-exchange-0.5.5/MANIFEST.in`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/PKG-INFO` & `google-cloud-bigquery-data-exchange-0.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-data-exchange
-Version: 0.5.4
+Version: 0.5.5
 Summary: Google Cloud Bigquery Data Exchange API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the BigQuery Analytics Hub.:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-data-exchange/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-bigquery-data-exchange
+    pip install google-cloud-bigquery-data-exchange
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-bigquery-data-exchange
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-bigquery-data-exchange
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for BigQuery Analytics Hub
    to see other available methods on the client.
 -  Read the `BigQuery Analytics Hub Product documentation`_ to learn
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/README.rst` & `google-cloud-bigquery-data-exchange-0.5.5/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the BigQuery Analytics Hub.:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-data-exchange/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-bigquery-data-exchange
+    pip install google-cloud-bigquery-data-exchange
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-bigquery-data-exchange
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-bigquery-data-exchange
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for BigQuery Analytics Hub
    to see other available methods on the client.
 -  Read the `BigQuery Analytics Hub Product documentation`_ to learn
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange/__init__.py`

 * *Files 4% similar despite different names*

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange/gapic_version.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange/gapic_version.py`

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
-__version__ = "0.5.4"  # {x-release-please-version}
+__version__ = "0.5.5"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/__init__.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/gapic_version.py`

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
-__version__ = "0.5.4"  # {x-release-please-version}
+__version__ = "0.5.5"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/__init__.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/__init__.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/async_client.py`

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
@@ -1631,50 +1631,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
@@ -1773,50 +1742,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/client.py`

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
@@ -1892,50 +1892,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
@@ -2033,50 +2002,19 @@
                    constraints based on attributes of the request, the
                    resource, or both. To learn which resources support
                    conditions in their IAM policies, see the [IAM
                    documentation](\ https://cloud.google.com/iam/help/conditions/resource-policies).
 
                    **JSON example:**
 
-                      {
-                         "bindings": [
-                            {
-                               "role":
-                               "roles/resourcemanager.organizationAdmin",
-                               "members": [ "user:mike@example.com",
-                               "group:admins@example.com",
-                               "domain:google.com",
-                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                               ]
-
-                            }, { "role":
-                            "roles/resourcemanager.organizationViewer",
-                            "members": [ "user:eve@example.com" ],
-                            "condition": { "title": "expirable access",
-                            "description": "Does not grant access after
-                            Sep 2020", "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')", } }
-
-                         ], "etag": "BwWWja0YfJA=", "version": 3
-
-                      }
+                   :literal:`\`     {       "bindings": [         {           "role": "roles/resourcemanager.organizationAdmin",           "members": [             "user:mike@example.com",             "group:admins@example.com",             "domain:google.com",             "serviceAccount:my-project-id@appspot.gserviceaccount.com"           ]         },         {           "role": "roles/resourcemanager.organizationViewer",           "members": [             "user:eve@example.com"           ],           "condition": {             "title": "expirable access",             "description": "Does not grant access after Sep 2020",             "expression": "request.time <             timestamp('2020-10-01T00:00:00.000Z')",           }         }       ],       "etag": "BwWWja0YfJA=",       "version": 3     }`\ \`
 
                    **YAML example:**
 
-                      bindings: - members: - user:\ mike@example.com -
-                      group:\ admins@example.com - domain:google.com -
-                      serviceAccount:\ my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin -
-                      members: - user:\ eve@example.com role:
-                      roles/resourcemanager.organizationViewer
-                      condition: title: expirable access description:
-                      Does not grant access after Sep 2020 expression:
-                      request.time <
-                      timestamp('2020-10-01T00:00:00.000Z') etag:
-                      BwWWja0YfJA= version: 3
+                   :literal:`\`     bindings:     - members:       - user:mike@example.com       - group:admins@example.com       - domain:google.com       - serviceAccount:my-project-id@appspot.gserviceaccount.com       role: roles/resourcemanager.organizationAdmin     - members:       - user:eve@example.com       role: roles/resourcemanager.organizationViewer       condition:         title: expirable access         description: Does not grant access after Sep 2020         expression: request.time < timestamp('2020-10-01T00:00:00.000Z')     etag: BwWWja0YfJA=     version: 3`\ \`
 
                    For a description of IAM and its features, see the
                    [IAM
                    documentation](\ https://cloud.google.com/iam/docs/).
 
         """
         # Create or coerce a protobuf request object.
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/pagers.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/__init__.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/base.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/services/analytics_hub_service/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/types/__init__.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py` & `google-cloud-bigquery-data-exchange-0.5.5/google/cloud/bigquery_data_exchange_v1beta1/types/dataexchange.py`

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
@@ -81,19 +81,19 @@
             Optional. Documentation describing the data
             exchange.
         listing_count (int):
             Output only. Number of listings contained in
             the data exchange.
         icon (bytes):
             Optional. Base64 encoded image representing
-            the data exchange. Max Size: 3.0MiB Expected
-            image dimensions are 512x512 pixels, however the
-            API only performs validation on size of the
-            encoded data. Note: For byte fields, the content
-            of the fields are base64-encoded (which
+            the data exchange. Max Size: 3.0MiB
+            Expected image dimensions are 512x512 pixels,
+            however the API only performs validation on size
+            of the encoded data. Note: For byte fields, the
+            content of the fields are base64-encoded (which
             increases the size of the data by 33-36%) when
             using JSON on the wire.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
@@ -282,21 +282,21 @@
         documentation (str):
             Optional. Documentation describing the
             listing.
         state (google.cloud.bigquery_data_exchange_v1beta1.types.Listing.State):
             Output only. Current state of the listing.
         icon (bytes):
             Optional. Base64 encoded image representing
-            the listing. Max Size: 3.0MiB Expected image
-            dimensions are 512x512 pixels, however the API
-            only performs validation on size of the encoded
-            data. Note: For byte fields, the contents of the
-            field are base64-encoded (which increases the
-            size of the data by 33-36%) when using JSON on
-            the wire.
+            the listing. Max Size: 3.0MiB
+            Expected image dimensions are 512x512 pixels,
+            however the API only performs validation on size
+            of the encoded data. Note: For byte fields, the
+            contents of the field are base64-encoded (which
+            increases the size of the data by 33-36%) when
+            using JSON on the wire.
         data_provider (google.cloud.bigquery_data_exchange_v1beta1.types.DataProvider):
             Optional. Details of the data provider who
             owns the source data.
         categories (MutableSequence[google.cloud.bigquery_data_exchange_v1beta1.types.Listing.Category]):
             Optional. Categories of the listing. Up to
             two categories are allowed.
         publisher (google.cloud.bigquery_data_exchange_v1beta1.types.Publisher):
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO` & `google-cloud-bigquery-data-exchange-0.5.5/google_cloud_bigquery_data_exchange.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-data-exchange
-Version: 0.5.4
+Version: 0.5.5
 Summary: Google Cloud Bigquery Data Exchange API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the BigQuery Analytics Hub.:  https://cloud.google.com/bigquery/docs/analytics-hub-introduction
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-data-exchange/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-bigquery-data-exchange
+    pip install google-cloud-bigquery-data-exchange
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-bigquery-data-exchange
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-bigquery-data-exchange
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for BigQuery Analytics Hub
    to see other available methods on the client.
 -  Read the `BigQuery Analytics Hub Product documentation`_ to learn
```

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt` & `google-cloud-bigquery-data-exchange-0.5.5/google_cloud_bigquery_data_exchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/setup.py` & `google-cloud-bigquery-data-exchange-0.5.5/setup.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/tests/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.5/tests/__init__.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/tests/unit/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.5/tests/unit/__init__.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.5/tests/unit/gapic/__init__.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py` & `google-cloud-bigquery-data-exchange-0.5.5/tests/unit/gapic/bigquery_data_exchange_v1beta1/__init__.py`

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

### Comparing `google-cloud-bigquery-data-exchange-0.5.4/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py` & `google-cloud-bigquery-data-exchange-0.5.5/tests/unit/gapic/bigquery_data_exchange_v1beta1/test_analytics_hub_service.py`

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

