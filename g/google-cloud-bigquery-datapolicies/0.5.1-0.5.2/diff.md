# Comparing `tmp/google-cloud-bigquery-datapolicies-0.5.1.tar.gz` & `tmp/google-cloud-bigquery-datapolicies-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-bigquery-datapolicies-0.5.1.tar", last modified: Wed Jul  5 15:51:05 2023, max compression
+gzip compressed data, was "google-cloud-bigquery-datapolicies-0.5.2.tar", last modified: Thu Aug  3 19:06:26 2023, max compression
```

## Comparing `google-cloud-bigquery-datapolicies-0.5.1.tar` & `google-cloud-bigquery-datapolicies-0.5.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.987064 google-cloud-bigquery-datapolicies-0.5.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4804 2023-07-05 15:51:05.987064 google-cloud-bigquery-datapolicies-0.5.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3868 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.971063 google-cloud-bigquery-datapolicies-0.5.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.971063 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.975064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies/
--rw-rw-r--   0 root         (0)     1003     1625 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.975064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/
--rw-rw-r--   0 root         (0)     1003     1451 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4125 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.975064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.979064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    56521 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    63689 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/client.py
--rw-rw-r--   0 root         (0)     1003     5969 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.979064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12955 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21504 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21939 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    59846 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.979064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/types/
--rw-rw-r--   0 root         (0)     1003     1141 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    11389 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/types/datapolicy.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.979064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1396 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2620 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.979064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.983064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/
--rw-rw-r--   0 root         (0)     1003      781 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    51774 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    58954 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/client.py
--rw-rw-r--   0 root         (0)     1003     6014 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.983064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/
--rw-rw-r--   0 root         (0)     1003     1220 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12185 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    20383 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20782 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.983064 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1081 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10282 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/types/datapolicy.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.983064 google-cloud-bigquery-datapolicies-0.5.1/google_cloud_bigquery_datapolicies.egg-info/
--rw-r--r--   0 root         (0)     1003     4804 2023-07-05 15:51:05.000000 google-cloud-bigquery-datapolicies-0.5.1/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3204 2023-07-05 15:51:05.000000 google-cloud-bigquery-datapolicies-0.5.1/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:05.000000 google-cloud-bigquery-datapolicies-0.5.1/google_cloud_bigquery_datapolicies.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:51:05.000000 google-cloud-bigquery-datapolicies-0.5.1/google_cloud_bigquery_datapolicies.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:51:05.000000 google-cloud-bigquery-datapolicies-0.5.1/google_cloud_bigquery_datapolicies.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:51:05.000000 google-cloud-bigquery-datapolicies-0.5.1/google_cloud_bigquery_datapolicies.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:51:05.000000 google-cloud-bigquery-datapolicies-0.5.1/google_cloud_bigquery_datapolicies.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:51:05.987064 google-cloud-bigquery-datapolicies-0.5.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3021 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.983064 google-cloud-bigquery-datapolicies-0.5.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.983064 google-cloud-bigquery-datapolicies-0.5.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.983064 google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.987064 google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/bigquery_datapolicies_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/bigquery_datapolicies_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   223028 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/bigquery_datapolicies_v1/test_data_policy_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:51:05.987064 google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/bigquery_datapolicies_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/bigquery_datapolicies_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   122748 2023-07-05 15:46:58.000000 google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/bigquery_datapolicies_v1beta1/test_data_policy_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.622642 google-cloud-bigquery-datapolicies-0.5.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4923 2023-08-03 19:06:26.622642 google-cloud-bigquery-datapolicies-0.5.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3987 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.610642 google-cloud-bigquery-datapolicies-0.5.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.610642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.614642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies/
+-rw-rw-r--   0 root         (0)     1003     1625 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.614642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/
+-rw-rw-r--   0 root         (0)     1003     1451 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4125 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.614642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.614642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    55781 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62949 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5969 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.618642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12955 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21504 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21939 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    60104 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.618642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1141 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11389 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/types/datapolicy.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.618642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1396 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2620 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.618642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.618642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/
+-rw-rw-r--   0 root         (0)     1003      781 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    51034 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    58214 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6014 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.618642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1220 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12185 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    20383 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20782 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.618642 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1081 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10282 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/types/datapolicy.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.622642 google-cloud-bigquery-datapolicies-0.5.2/google_cloud_bigquery_datapolicies.egg-info/
+-rw-r--r--   0 root         (0)     1003     4923 2023-08-03 19:06:26.000000 google-cloud-bigquery-datapolicies-0.5.2/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3204 2023-08-03 19:06:26.000000 google-cloud-bigquery-datapolicies-0.5.2/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:26.000000 google-cloud-bigquery-datapolicies-0.5.2/google_cloud_bigquery_datapolicies.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 19:06:26.000000 google-cloud-bigquery-datapolicies-0.5.2/google_cloud_bigquery_datapolicies.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:26.000000 google-cloud-bigquery-datapolicies-0.5.2/google_cloud_bigquery_datapolicies.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-08-03 19:06:26.000000 google-cloud-bigquery-datapolicies-0.5.2/google_cloud_bigquery_datapolicies.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 19:06:26.000000 google-cloud-bigquery-datapolicies-0.5.2/google_cloud_bigquery_datapolicies.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-08-03 19:06:26.622642 google-cloud-bigquery-datapolicies-0.5.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3021 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.622642 google-cloud-bigquery-datapolicies-0.5.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.622642 google-cloud-bigquery-datapolicies-0.5.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.622642 google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.622642 google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/bigquery_datapolicies_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/bigquery_datapolicies_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   223028 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/bigquery_datapolicies_v1/test_data_policy_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:26.622642 google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/bigquery_datapolicies_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/bigquery_datapolicies_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   122748 2023-08-03 19:03:10.000000 google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/bigquery_datapolicies_v1beta1/test_data_policy_service.py
```

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/LICENSE` & `google-cloud-bigquery-datapolicies-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/MANIFEST.in` & `google-cloud-bigquery-datapolicies-0.5.2/MANIFEST.in`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/PKG-INFO` & `google-cloud-bigquery-datapolicies-0.5.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-datapolicies
-Version: 0.5.1
+Version: 0.5.2
 Summary: Google Cloud Bigquery Datapolicies API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the BigQuery Data Policy.:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-datapolicies/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-bigquery-datapolicies
+    pip install google-cloud-bigquery-datapolicies
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-bigquery-datapolicies
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-bigquery-datapolicies
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for BigQuery Data Policy
    to see other available methods on the client.
 -  Read the `BigQuery Data Policy Product documentation`_ to learn
```

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/README.rst` & `google-cloud-bigquery-datapolicies-0.5.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the BigQuery Data Policy.:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-datapolicies/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-bigquery-datapolicies
+    pip install google-cloud-bigquery-datapolicies
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-bigquery-datapolicies
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-bigquery-datapolicies
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for BigQuery Data Policy
    to see other available methods on the client.
 -  Read the `BigQuery Data Policy Product documentation`_ to learn
```

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies/gapic_version.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies/gapic_version.py`

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
-__version__ = "0.5.1"  # {x-release-please-version}
+__version__ = "0.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
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
-from google.cloud.bigquery_datapolicies_v1 import gapic_version as package_version
+from google.cloud.bigquery_datapolicies_v1beta1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.data_policy_service import (
     DataPolicyServiceAsyncClient,
     DataPolicyServiceClient,
@@ -26,24 +26,22 @@
     CreateDataPolicyRequest,
     DataMaskingPolicy,
     DataPolicy,
     DeleteDataPolicyRequest,
     GetDataPolicyRequest,
     ListDataPoliciesRequest,
     ListDataPoliciesResponse,
-    RenameDataPolicyRequest,
     UpdateDataPolicyRequest,
 )
 
 __all__ = (
     "DataPolicyServiceAsyncClient",
     "CreateDataPolicyRequest",
     "DataMaskingPolicy",
     "DataPolicy",
     "DataPolicyServiceClient",
     "DeleteDataPolicyRequest",
     "GetDataPolicyRequest",
     "ListDataPoliciesRequest",
     "ListDataPoliciesResponse",
-    "RenameDataPolicyRequest",
     "UpdateDataPolicyRequest",
 )
```

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/gapic_metadata.json` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/gapic_version.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/gapic_version.py`

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
-__version__ = "0.5.1"  # {x-release-please-version}
+__version__ = "0.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/async_client.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/async_client.py`

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
@@ -1008,50 +1008,19 @@
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
@@ -1159,50 +1128,19 @@
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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/client.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/client.py`

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
@@ -1183,50 +1183,19 @@
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
@@ -1324,50 +1293,19 @@
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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/pagers.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/pagers.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/base.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/base.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/rest.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/services/data_policy_service/transports/rest.py`

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
@@ -748,62 +748,62 @@
                 conditions in their IAM policies, see the `IAM
                 documentation <https://cloud.google.com/iam/help/conditions/resource-policies>`__.
 
                 **JSON example:**
 
                 ::
 
-                    {
-                      "bindings": [
-                        {
-                          "role": "roles/resourcemanager.organizationAdmin",
-                          "members": [
-                            "user:mike@example.com",
-                            "group:admins@example.com",
-                            "domain:google.com",
-                            "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                          ]
-                        },
-                        {
-                          "role": "roles/resourcemanager.organizationViewer",
-                          "members": [
-                            "user:eve@example.com"
-                          ],
-                          "condition": {
-                            "title": "expirable access",
-                            "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')",
-                          }
-                        }
-                      ],
-                      "etag": "BwWWja0YfJA=",
-                      "version": 3
-                    }
+                       {
+                         "bindings": [
+                           {
+                             "role": "roles/resourcemanager.organizationAdmin",
+                             "members": [
+                               "user:mike@example.com",
+                               "group:admins@example.com",
+                               "domain:google.com",
+                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
+                             ]
+                           },
+                           {
+                             "role": "roles/resourcemanager.organizationViewer",
+                             "members": [
+                               "user:eve@example.com"
+                             ],
+                             "condition": {
+                               "title": "expirable access",
+                               "description": "Does not grant access after Sep 2020",
+                               "expression": "request.time <
+                               timestamp('2020-10-01T00:00:00.000Z')",
+                             }
+                           }
+                         ],
+                         "etag": "BwWWja0YfJA=",
+                         "version": 3
+                       }
 
                 **YAML example:**
 
                 ::
 
-                    bindings:
-                    - members:
-                      - user:mike@example.com
-                      - group:admins@example.com
-                      - domain:google.com
-                      - serviceAccount:my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin
-                    - members:
-                      - user:eve@example.com
-                      role: roles/resourcemanager.organizationViewer
-                      condition:
-                        title: expirable access
-                        description: Does not grant access after Sep 2020
-                        expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
-                    etag: BwWWja0YfJA=
-                    version: 3
+                       bindings:
+                       - members:
+                         - user:mike@example.com
+                         - group:admins@example.com
+                         - domain:google.com
+                         - serviceAccount:my-project-id@appspot.gserviceaccount.com
+                         role: roles/resourcemanager.organizationAdmin
+                       - members:
+                         - user:eve@example.com
+                         role: roles/resourcemanager.organizationViewer
+                         condition:
+                           title: expirable access
+                           description: Does not grant access after Sep 2020
+                           expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
+                       etag: BwWWja0YfJA=
+                       version: 3
 
                 For a description of IAM and its features, see the `IAM
                 documentation <https://cloud.google.com/iam/docs/>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
@@ -1107,62 +1107,62 @@
                 conditions in their IAM policies, see the `IAM
                 documentation <https://cloud.google.com/iam/help/conditions/resource-policies>`__.
 
                 **JSON example:**
 
                 ::
 
-                    {
-                      "bindings": [
-                        {
-                          "role": "roles/resourcemanager.organizationAdmin",
-                          "members": [
-                            "user:mike@example.com",
-                            "group:admins@example.com",
-                            "domain:google.com",
-                            "serviceAccount:my-project-id@appspot.gserviceaccount.com"
-                          ]
-                        },
-                        {
-                          "role": "roles/resourcemanager.organizationViewer",
-                          "members": [
-                            "user:eve@example.com"
-                          ],
-                          "condition": {
-                            "title": "expirable access",
-                            "description": "Does not grant access after Sep 2020",
-                            "expression": "request.time <
-                            timestamp('2020-10-01T00:00:00.000Z')",
-                          }
-                        }
-                      ],
-                      "etag": "BwWWja0YfJA=",
-                      "version": 3
-                    }
+                       {
+                         "bindings": [
+                           {
+                             "role": "roles/resourcemanager.organizationAdmin",
+                             "members": [
+                               "user:mike@example.com",
+                               "group:admins@example.com",
+                               "domain:google.com",
+                               "serviceAccount:my-project-id@appspot.gserviceaccount.com"
+                             ]
+                           },
+                           {
+                             "role": "roles/resourcemanager.organizationViewer",
+                             "members": [
+                               "user:eve@example.com"
+                             ],
+                             "condition": {
+                               "title": "expirable access",
+                               "description": "Does not grant access after Sep 2020",
+                               "expression": "request.time <
+                               timestamp('2020-10-01T00:00:00.000Z')",
+                             }
+                           }
+                         ],
+                         "etag": "BwWWja0YfJA=",
+                         "version": 3
+                       }
 
                 **YAML example:**
 
                 ::
 
-                    bindings:
-                    - members:
-                      - user:mike@example.com
-                      - group:admins@example.com
-                      - domain:google.com
-                      - serviceAccount:my-project-id@appspot.gserviceaccount.com
-                      role: roles/resourcemanager.organizationAdmin
-                    - members:
-                      - user:eve@example.com
-                      role: roles/resourcemanager.organizationViewer
-                      condition:
-                        title: expirable access
-                        description: Does not grant access after Sep 2020
-                        expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
-                    etag: BwWWja0YfJA=
-                    version: 3
+                       bindings:
+                       - members:
+                         - user:mike@example.com
+                         - group:admins@example.com
+                         - domain:google.com
+                         - serviceAccount:my-project-id@appspot.gserviceaccount.com
+                         role: roles/resourcemanager.organizationAdmin
+                       - members:
+                         - user:eve@example.com
+                         role: roles/resourcemanager.organizationViewer
+                         condition:
+                           title: expirable access
+                           description: Does not grant access after Sep 2020
+                           expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
+                       etag: BwWWja0YfJA=
+                       version: 3
 
                 For a description of IAM and its features, see the `IAM
                 documentation <https://cloud.google.com/iam/docs/>`__.
 
             """
 
             http_options: List[Dict[str, str]] = [
```

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/types/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/types/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1/types/datapolicy.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/types/datapolicy.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
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
-from google.cloud.bigquery_datapolicies_v1beta1 import gapic_version as package_version
+from google.cloud.bigquery_datapolicies_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.data_policy_service import (
     DataPolicyServiceAsyncClient,
     DataPolicyServiceClient,
@@ -26,22 +26,24 @@
     CreateDataPolicyRequest,
     DataMaskingPolicy,
     DataPolicy,
     DeleteDataPolicyRequest,
     GetDataPolicyRequest,
     ListDataPoliciesRequest,
     ListDataPoliciesResponse,
+    RenameDataPolicyRequest,
     UpdateDataPolicyRequest,
 )
 
 __all__ = (
     "DataPolicyServiceAsyncClient",
     "CreateDataPolicyRequest",
     "DataMaskingPolicy",
     "DataPolicy",
     "DataPolicyServiceClient",
     "DeleteDataPolicyRequest",
     "GetDataPolicyRequest",
     "ListDataPoliciesRequest",
     "ListDataPoliciesResponse",
+    "RenameDataPolicyRequest",
     "UpdateDataPolicyRequest",
 )
```

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/gapic_metadata.json` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/gapic_version.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/gapic_version.py`

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
-__version__ = "0.5.1"  # {x-release-please-version}
+__version__ = "0.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/async_client.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/async_client.py`

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
@@ -890,50 +890,19 @@
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
@@ -1041,50 +1010,19 @@
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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/client.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/client.py`

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
@@ -1072,50 +1072,19 @@
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
@@ -1213,50 +1182,19 @@
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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/pagers.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/pagers.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/base.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/base.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/services/data_policy_service/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/types/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/types/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google/cloud/bigquery_datapolicies_v1beta1/types/datapolicy.py` & `google-cloud-bigquery-datapolicies-0.5.2/google/cloud/bigquery_datapolicies_v1beta1/types/datapolicy.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO` & `google-cloud-bigquery-datapolicies-0.5.2/google_cloud_bigquery_datapolicies.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-bigquery-datapolicies
-Version: 0.5.1
+Version: 0.5.2
 Summary: Google Cloud Bigquery Datapolicies API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the BigQuery Data Policy.:  https://cloud.google.com/bigquery/docs/reference/bigquerydatapolicy/rest
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-bigquery-datapolicies/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-bigquery-datapolicies
+    pip install google-cloud-bigquery-datapolicies
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-bigquery-datapolicies
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-bigquery-datapolicies
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for BigQuery Data Policy
    to see other available methods on the client.
 -  Read the `BigQuery Data Policy Product documentation`_ to learn
```

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt` & `google-cloud-bigquery-datapolicies-0.5.2/google_cloud_bigquery_datapolicies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/setup.py` & `google-cloud-bigquery-datapolicies-0.5.2/setup.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/tests/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/tests/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/tests/unit/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/tests/unit/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/bigquery_datapolicies_v1/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/bigquery_datapolicies_v1/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/bigquery_datapolicies_v1/test_data_policy_service.py` & `google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/bigquery_datapolicies_v1/test_data_policy_service.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/bigquery_datapolicies_v1beta1/__init__.py` & `google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/bigquery_datapolicies_v1beta1/__init__.py`

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

### Comparing `google-cloud-bigquery-datapolicies-0.5.1/tests/unit/gapic/bigquery_datapolicies_v1beta1/test_data_policy_service.py` & `google-cloud-bigquery-datapolicies-0.5.2/tests/unit/gapic/bigquery_datapolicies_v1beta1/test_data_policy_service.py`

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

