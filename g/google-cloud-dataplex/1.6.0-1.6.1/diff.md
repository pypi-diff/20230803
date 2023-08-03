# Comparing `tmp/google-cloud-dataplex-1.6.0.tar.gz` & `tmp/google-cloud-dataplex-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-dataplex-1.6.0.tar", last modified: Tue Jul 25 14:42:54 2023, max compression
+gzip compressed data, was "google-cloud-dataplex-1.6.1.tar", last modified: Thu Aug  3 19:06:39 2023, max compression
```

## Comparing `google-cloud-dataplex-1.6.0.tar` & `google-cloud-dataplex-1.6.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.446795 google-cloud-dataplex-1.6.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4802 2023-07-25 14:42:54.446795 google-cloud-dataplex-1.6.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3879 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.426792 google-cloud-dataplex-1.6.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.426792 google-cloud-dataplex-1.6.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex/
--rw-rw-r--   0 root         (0)     1003     9177 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/
--rw-rw-r--   0 root         (0)     1003     8227 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    19755 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       82 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/
--rw-rw-r--   0 root         (0)     1003      769 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    62854 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    71605 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/client.py
--rw-rw-r--   0 root         (0)     1003     5658 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12118 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25618 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25992 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.430793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    62559 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    74218 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/client.py
--rw-rw-r--   0 root         (0)     1003    10807 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.434793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10921 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25499 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    25983 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.434793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   100461 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   112949 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/client.py
--rw-rw-r--   0 root         (0)     1003    16556 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.434793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/
--rw-rw-r--   0 root         (0)     1003     1246 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14730 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    35102 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    35794 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.434793 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   186272 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   199302 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/client.py
--rw-rw-r--   0 root         (0)     1003    49482 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.438794 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    26223 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    52208 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    53320 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.438794 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/
--rw-rw-r--   0 root         (0)     1003      773 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    61629 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    72083 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/client.py
--rw-rw-r--   0 root         (0)     1003    10685 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.438794 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/
--rw-rw-r--   0 root         (0)     1003     1202 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12419 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25614 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26039 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.442794 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/
--rw-rw-r--   0 root         (0)     1003     7231 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    16335 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/analyze.py
--rw-rw-r--   0 root         (0)     1003     6555 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/content.py
--rw-rw-r--   0 root         (0)     1003    22473 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_profile.py
--rw-rw-r--   0 root         (0)     1003    22328 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_quality.py
--rw-rw-r--   0 root         (0)     1003    31056 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_taxonomy.py
--rw-rw-r--   0 root         (0)     1003    25542 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/datascans.py
--rw-rw-r--   0 root         (0)     1003    34752 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/logs.py
--rw-rw-r--   0 root         (0)     1003    38145 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/metadata_.py
--rw-rw-r--   0 root         (0)     1003     5857 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/processing.py
--rw-rw-r--   0 root         (0)     1003    50791 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003     2922 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/security.py
--rw-rw-r--   0 root         (0)     1003    40691 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/service.py
--rw-rw-r--   0 root         (0)     1003    27261 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/tasks.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.442794 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/
--rw-r--r--   0 root         (0)     1003     4802 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4435 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-25 14:42:54.000000 google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-25 14:42:54.446795 google-cloud-dataplex-1.6.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2976 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.442794 google-cloud-dataplex-1.6.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.442794 google-cloud-dataplex-1.6.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.442794 google-cloud-dataplex-1.6.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-25 14:42:54.446795 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   154372 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_content_service.py
--rw-rw-r--   0 root         (0)     1003   169945 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_data_scan_service.py
--rw-rw-r--   0 root         (0)     1003   249588 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_data_taxonomy_service.py
--rw-rw-r--   0 root         (0)     1003   431954 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_dataplex_service.py
--rw-rw-r--   0 root         (0)     1003   175809 2023-07-25 14:40:01.000000 google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_metadata_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.343029 google-cloud-dataplex-1.6.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4802 2023-08-03 19:06:39.343029 google-cloud-dataplex-1.6.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3879 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.323028 google-cloud-dataplex-1.6.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.323028 google-cloud-dataplex-1.6.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.327028 google-cloud-dataplex-1.6.1/google/cloud/dataplex/
+-rw-rw-r--   0 root         (0)     1003     9177 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.327028 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/
+-rw-rw-r--   0 root         (0)     1003     8227 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19755 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       82 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.327028 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.327028 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/
+-rw-rw-r--   0 root         (0)     1003      769 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62114 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    70865 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5658 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.331028 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12118 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25618 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25992 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.331028 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62559 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    74218 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10807 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.331028 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10921 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25499 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    25983 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.331028 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   100461 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   112949 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16556 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.331028 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1246 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14730 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    35102 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    35794 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.335029 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   186272 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   199302 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/client.py
+-rw-rw-r--   0 root         (0)     1003    49482 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.335029 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26223 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    52208 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    53320 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.335029 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/
+-rw-rw-r--   0 root         (0)     1003      773 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61629 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    72083 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10685 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.335029 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1202 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12419 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25614 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26039 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.339028 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/
+-rw-rw-r--   0 root         (0)     1003     7231 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16335 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/analyze.py
+-rw-rw-r--   0 root         (0)     1003     6555 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/content.py
+-rw-rw-r--   0 root         (0)     1003    22473 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/data_profile.py
+-rw-rw-r--   0 root         (0)     1003    22328 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/data_quality.py
+-rw-rw-r--   0 root         (0)     1003    31056 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/data_taxonomy.py
+-rw-rw-r--   0 root         (0)     1003    25542 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/datascans.py
+-rw-rw-r--   0 root         (0)     1003    34752 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/logs.py
+-rw-rw-r--   0 root         (0)     1003    38145 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/metadata_.py
+-rw-rw-r--   0 root         (0)     1003     5857 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/processing.py
+-rw-rw-r--   0 root         (0)     1003    50791 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003     2922 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/security.py
+-rw-rw-r--   0 root         (0)     1003    40691 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/service.py
+-rw-rw-r--   0 root         (0)     1003    27261 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/tasks.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.343029 google-cloud-dataplex-1.6.1/google_cloud_dataplex.egg-info/
+-rw-r--r--   0 root         (0)     1003     4802 2023-08-03 19:06:39.000000 google-cloud-dataplex-1.6.1/google_cloud_dataplex.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4435 2023-08-03 19:06:39.000000 google-cloud-dataplex-1.6.1/google_cloud_dataplex.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:39.000000 google-cloud-dataplex-1.6.1/google_cloud_dataplex.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 19:06:39.000000 google-cloud-dataplex-1.6.1/google_cloud_dataplex.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:06:39.000000 google-cloud-dataplex-1.6.1/google_cloud_dataplex.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-08-03 19:06:39.000000 google-cloud-dataplex-1.6.1/google_cloud_dataplex.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 19:06:39.000000 google-cloud-dataplex-1.6.1/google_cloud_dataplex.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-08-03 19:06:39.343029 google-cloud-dataplex-1.6.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2976 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.343029 google-cloud-dataplex-1.6.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.343029 google-cloud-dataplex-1.6.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.343029 google-cloud-dataplex-1.6.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:06:39.343029 google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   154372 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/test_content_service.py
+-rw-rw-r--   0 root         (0)     1003   169945 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/test_data_scan_service.py
+-rw-rw-r--   0 root         (0)     1003   249588 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/test_data_taxonomy_service.py
+-rw-rw-r--   0 root         (0)     1003   431954 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/test_dataplex_service.py
+-rw-rw-r--   0 root         (0)     1003   175809 2023-08-03 19:03:10.000000 google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/test_metadata_service.py
```

### Comparing `google-cloud-dataplex-1.6.0/LICENSE` & `google-cloud-dataplex-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/MANIFEST.in` & `google-cloud-dataplex-1.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/PKG-INFO` & `google-cloud-dataplex-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataplex
-Version: 1.6.0
+Version: 1.6.1
 Summary: Google Cloud Dataplex API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dataplex-1.6.0/README.rst` & `google-cloud-dataplex-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex/gapic_version.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/gapic_metadata.json` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/gapic_version.py` & `google-cloud-dataplex-1.6.1/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.0"  # {x-release-please-version}
```

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/__init__.py` & `google-cloud-dataplex-1.6.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/async_client.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -736,50 +736,19 @@
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
@@ -904,50 +873,19 @@
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

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/client.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -976,50 +976,19 @@
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
@@ -1132,50 +1101,19 @@
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

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/pagers.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/base.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/grpc.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/content_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/async_client.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/client.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/pagers.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_scan_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/async_client.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/client.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/pagers.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/base.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/data_taxonomy_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/async_client.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/client.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/pagers.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/dataplex_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/async_client.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/client.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/pagers.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/base.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/services/metadata_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/__init__.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/analyze.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/analyze.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/content.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/content.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_profile.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/data_profile.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_quality.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/data_quality.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/data_taxonomy.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/data_taxonomy.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/datascans.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/datascans.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/logs.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/logs.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/metadata_.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/metadata_.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/processing.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/processing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/resources.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/security.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/security.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/service.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google/cloud/dataplex_v1/types/tasks.py` & `google-cloud-dataplex-1.6.1/google/cloud/dataplex_v1/types/tasks.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/PKG-INFO` & `google-cloud-dataplex-1.6.1/google_cloud_dataplex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-dataplex
-Version: 1.6.0
+Version: 1.6.1
 Summary: Google Cloud Dataplex API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-dataplex-1.6.0/google_cloud_dataplex.egg-info/SOURCES.txt` & `google-cloud-dataplex-1.6.1/google_cloud_dataplex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/setup.py` & `google-cloud-dataplex-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/tests/__init__.py` & `google-cloud-dataplex-1.6.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/tests/unit/__init__.py` & `google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_content_service.py` & `google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/test_content_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_data_scan_service.py` & `google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/test_data_scan_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_data_taxonomy_service.py` & `google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/test_data_taxonomy_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_dataplex_service.py` & `google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/test_dataplex_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-dataplex-1.6.0/tests/unit/gapic/dataplex_v1/test_metadata_service.py` & `google-cloud-dataplex-1.6.1/tests/unit/gapic/dataplex_v1/test_metadata_service.py`

 * *Files identical despite different names*

