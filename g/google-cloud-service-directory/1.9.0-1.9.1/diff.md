# Comparing `tmp/google-cloud-service-directory-1.9.0.tar.gz` & `tmp/google-cloud-service-directory-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-service-directory-1.9.0.tar", last modified: Mon Jul 24 20:57:12 2023, max compression
+gzip compressed data, was "google-cloud-service-directory-1.9.1.tar", last modified: Thu Aug  3 19:07:25 2023, max compression
```

## Comparing `google-cloud-service-directory-1.9.0.tar` & `google-cloud-service-directory-1.9.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.606364 google-cloud-service-directory-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4636 2023-07-24 20:57:12.606364 google-cloud-service-directory-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3695 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.582365 google-cloud-service-directory-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.582365 google-cloud-service-directory-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.586365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/
--rw-rw-r--   0 root         (0)     1003     2830 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.586365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/
--rw-rw-r--   0 root         (0)     1003     2391 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8096 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.586365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.586365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17303 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27720 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.586365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6688 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13705 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13918 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    19691 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.590365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   101350 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   114733 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/client.py
--rw-rw-r--   0 root         (0)     1003    16223 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.590365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14825 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    34111 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34839 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   116492 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.590365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/
--rw-rw-r--   0 root         (0)     1003     1911 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4109 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/endpoint.py
--rw-rw-r--   0 root         (0)     1003     4601 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/lookup_service.py
--rw-rw-r--   0 root         (0)     1003     1971 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/namespace.py
--rw-rw-r--   0 root         (0)     1003    22554 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/registration_service.py
--rw-rw-r--   0 root         (0)     1003     3634 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.594365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2396 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8106 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       91 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.594365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.594365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    17361 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    27778 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.594365 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/
--rw-rw-r--   0 root         (0)     1003     1386 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6698 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13728 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13941 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    19721 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.598364 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   101972 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   115355 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py
--rw-rw-r--   0 root         (0)     1003    16348 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.598364 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14865 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    34203 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    34931 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   117459 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.598364 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1911 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4728 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/endpoint.py
--rw-rw-r--   0 root         (0)     1003     4608 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/lookup_service.py
--rw-rw-r--   0 root         (0)     1003     2622 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/namespace.py
--rw-rw-r--   0 root         (0)     1003    23224 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/registration_service.py
--rw-rw-r--   0 root         (0)     1003     4453 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/
--rw-r--r--   0 root         (0)     1003     4636 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4919 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-24 20:57:12.000000 google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-24 20:57:12.606364 google-cloud-service-directory-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3008 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    82594 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py
--rw-rw-r--   0 root         (0)     1003   428124 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/test_registration_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-24 20:57:12.602364 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    82624 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py
--rw-rw-r--   0 root         (0)     1003   429655 2023-07-24 20:53:51.000000 google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.614970 google-cloud-service-directory-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4751 2023-08-03 19:07:25.614970 google-cloud-service-directory-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3810 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.594971 google-cloud-service-directory-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.594971 google-cloud-service-directory-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.598971 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/
+-rw-rw-r--   0 root         (0)     1003     2830 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.598971 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/
+-rw-rw-r--   0 root         (0)     1003     2391 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8096 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.598971 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.598971 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17303 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27720 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.598971 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6688 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13705 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13918 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19691 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.602970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   100610 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   113993 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16223 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.602970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14825 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    34111 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34839 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   116750 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.602970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1911 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4109 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/endpoint.py
+-rw-rw-r--   0 root         (0)     1003     4601 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/lookup_service.py
+-rw-rw-r--   0 root         (0)     1003     1971 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/namespace.py
+-rw-rw-r--   0 root         (0)     1003    22554 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/registration_service.py
+-rw-rw-r--   0 root         (0)     1003     3634 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.606970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2396 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8106 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       91 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.606970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.606970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17361 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27778 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.606970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1386 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6698 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13728 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13941 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19721 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.606970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   101232 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   114615 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16348 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14865 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    34203 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    34931 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   117717 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1911 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4728 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/endpoint.py
+-rw-rw-r--   0 root         (0)     1003     4608 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/lookup_service.py
+-rw-rw-r--   0 root         (0)     1003     2622 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/namespace.py
+-rw-rw-r--   0 root         (0)     1003    23224 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/registration_service.py
+-rw-rw-r--   0 root         (0)     1003     4453 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/
+-rw-r--r--   0 root         (0)     1003     4751 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4919 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 19:07:25.000000 google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-08-03 19:07:25.614970 google-cloud-service-directory-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3008 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.610970 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    82594 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py
+-rw-rw-r--   0 root         (0)     1003   428124 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/test_registration_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:25.614970 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    82624 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py
+-rw-rw-r--   0 root         (0)     1003   429655 2023-08-03 19:03:10.000000 google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py
```

### Comparing `google-cloud-service-directory-1.9.0/LICENSE` & `google-cloud-service-directory-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/MANIFEST.in` & `google-cloud-service-directory-1.9.1/MANIFEST.in`

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

### Comparing `google-cloud-service-directory-1.9.0/PKG-INFO` & `google-cloud-service-directory-1.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-directory
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Service Directory API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Service Directory.:  https://cloud.google.com/service-directory/
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-service-directory/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-service-directory
+    pip install google-cloud-service-directory
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-service-directory
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-service-directory
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Service Directory
    to see other available methods on the client.
 -  Read the `Service Directory Product documentation`_ to learn
```

### Comparing `google-cloud-service-directory-1.9.0/README.rst` & `google-cloud-service-directory-1.9.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Service Directory.:  https://cloud.google.com/service-directory/
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-service-directory/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-service-directory
+    pip install google-cloud-service-directory
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-service-directory
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-service-directory
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Service Directory
    to see other available methods on the client.
 -  Read the `Service Directory Product documentation`_ to learn
```

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory/gapic_version.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/gapic_metadata.json` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/gapic_version.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/client.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/lookup_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/async_client.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2002,50 +2002,19 @@
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
@@ -2145,50 +2114,19 @@
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

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/client.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2294,50 +2294,19 @@
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
@@ -2436,50 +2405,19 @@
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

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/pagers.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/services/registration_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1418,62 +1418,62 @@
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
@@ -2046,62 +2046,62 @@
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

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/endpoint.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/endpoint.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/lookup_service.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/namespace.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/namespace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/registration_service.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/registration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1/types/service.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/gapic_metadata.json` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/gapic_version.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/lookup_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2003,50 +2003,19 @@
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
@@ -2145,50 +2114,19 @@
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

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2295,50 +2295,19 @@
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
@@ -2436,50 +2405,19 @@
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

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/services/registration_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1419,62 +1419,62 @@
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
@@ -2052,62 +2052,62 @@
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

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/__init__.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/endpoint.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/endpoint.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/lookup_service.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/namespace.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/namespace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/registration_service.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/registration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google/cloud/servicedirectory_v1beta1/types/service.py` & `google-cloud-service-directory-1.9.1/google/cloud/servicedirectory_v1beta1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/PKG-INFO` & `google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-service-directory
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Service Directory API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Service Directory.:  https://cloud.google.com/service-directory/
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
+.. _samples/: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-service-directory/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-service-directory
+    pip install google-cloud-service-directory
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-service-directory
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-service-directory
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Service Directory
    to see other available methods on the client.
 -  Read the `Service Directory Product documentation`_ to learn
```

### Comparing `google-cloud-service-directory-1.9.0/google_cloud_service_directory.egg-info/SOURCES.txt` & `google-cloud-service-directory-1.9.1/google_cloud_service_directory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/setup.py` & `google-cloud-service-directory-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/tests/__init__.py` & `google-cloud-service-directory-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/tests/unit/__init__.py` & `google-cloud-service-directory-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-service-directory-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/__init__.py` & `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py` & `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/test_lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1/test_registration_service.py` & `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1/test_registration_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/__init__.py` & `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py` & `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/test_lookup_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-service-directory-1.9.0/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py` & `google-cloud-service-directory-1.9.1/tests/unit/gapic/servicedirectory_v1beta1/test_registration_service.py`

 * *Files identical despite different names*

