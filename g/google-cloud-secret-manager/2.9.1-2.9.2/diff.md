# Comparing `tmp/google-cloud-secret-manager-2.9.1.tar.gz` & `tmp/google-cloud-secret-manager-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-secret-manager-2.9.1.tar", last modified: Mon Mar  7 16:50:27 2022, max compression
+gzip compressed data, was "google-cloud-secret-manager-2.9.2.tar", last modified: Mon Mar 14 14:00:01 2022, max compression
```

## Comparing `google-cloud-secret-manager-2.9.1.tar` & `google-cloud-secret-manager-2.9.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.961887 google-cloud-secret-manager-2.9.1/
--rw-rw-r--   0 root         (0)     1003    11358 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4183 2022-03-07 16:50:27.961887 google-cloud-secret-manager-2.9.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3231 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.949893 google-cloud-secret-manager-2.9.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.949893 google-cloud-secret-manager-2.9.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.949893 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager/
--rw-rw-r--   0 root         (0)     1003     3460 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager/__init__.py
--rw-rw-r--   0 root         (0)     1003       87 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.953891 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/
--rw-rw-r--   0 root         (0)     1003     2659 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     4379 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       87 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.953891 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.953891 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/
--rw-rw-r--   0 root         (0)     1003      793 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    73977 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    84926 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/client.py
--rw-rw-r--   0 root         (0)     1003    10850 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.953891 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/transports/
--rw-rw-r--   0 root         (0)     1003     1256 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    12298 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    30425 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    31130 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.953891 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/types/
--rw-rw-r--   0 root         (0)     1003     1941 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    22376 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    14730 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.953891 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/
--rw-rw-r--   0 root         (0)     1003     2182 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003       87 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.953891 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      601 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.957889 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/
--rw-rw-r--   0 root         (0)     1003      795 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    62536 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    72060 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/client.py
--rw-rw-r--   0 root         (0)     1003    10940 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.957889 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/
--rw-rw-r--   0 root         (0)     1003     1258 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11628 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    29769 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    30512 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.957889 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1701 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     7295 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    12440 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.957889 google-cloud-secret-manager-2.9.1/google_cloud_secret_manager.egg-info/
--rw-r--r--   0 root         (0)     1003     4183 2022-03-07 16:50:27.000000 google-cloud-secret-manager-2.9.1/google_cloud_secret_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2817 2022-03-07 16:50:27.000000 google-cloud-secret-manager-2.9.1/google_cloud_secret_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-03-07 16:50:27.000000 google-cloud-secret-manager-2.9.1/google_cloud_secret_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-03-07 16:50:27.000000 google-cloud-secret-manager-2.9.1/google_cloud_secret_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-03-07 16:50:27.000000 google-cloud-secret-manager-2.9.1/google_cloud_secret_manager.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      151 2022-03-07 16:50:27.000000 google-cloud-secret-manager-2.9.1/google_cloud_secret_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-03-07 16:50:27.000000 google-cloud-secret-manager-2.9.1/google_cloud_secret_manager.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.957889 google-cloud-secret-manager-2.9.1/scripts/
--rw-rw-r--   0 root         (0)     1003     6743 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/scripts/fixup_secretmanager_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6654 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/scripts/fixup_secretmanager_v1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-03-07 16:50:27.961887 google-cloud-secret-manager-2.9.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2851 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.957889 google-cloud-secret-manager-2.9.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.957889 google-cloud-secret-manager-2.9.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.957889 google-cloud-secret-manager-2.9.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.961887 google-cloud-secret-manager-2.9.1/tests/unit/gapic/secretmanager_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/tests/unit/gapic/secretmanager_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   182660 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/tests/unit/gapic/secretmanager_v1/test_secret_manager_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-03-07 16:50:27.961887 google-cloud-secret-manager-2.9.1/tests/unit/gapic/secretmanager_v1beta1/
--rw-rw-r--   0 root         (0)     1003      601 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/tests/unit/gapic/secretmanager_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   164362 2022-03-07 16:47:38.000000 google-cloud-secret-manager-2.9.1/tests/unit/gapic/secretmanager_v1beta1/test_secret_manager_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.705615 google-cloud-secret-manager-2.9.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4183 2022-03-14 14:00:01.705615 google-cloud-secret-manager-2.9.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3231 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.693615 google-cloud-secret-manager-2.9.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.693615 google-cloud-secret-manager-2.9.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.697615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager/
+-rw-rw-r--   0 root         (0)     1003     3460 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager/__init__.py
+-rw-rw-r--   0 root         (0)     1003       87 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.697615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/
+-rw-rw-r--   0 root         (0)     1003     2659 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4379 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       87 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.697615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.697615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/
+-rw-rw-r--   0 root         (0)     1003      793 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    73977 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    84926 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10850 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.697615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1256 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12298 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    30425 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    31130 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.697615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1941 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22376 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    14730 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.701615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     2182 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003       87 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.701615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      601 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.701615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/
+-rw-rw-r--   0 root         (0)     1003      795 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    62536 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    72060 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10940 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.701615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1258 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11628 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    29769 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    30512 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.701615 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1701 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7295 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    12440 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.701615 google-cloud-secret-manager-2.9.2/google_cloud_secret_manager.egg-info/
+-rw-r--r--   0 root         (0)     1003     4183 2022-03-14 14:00:01.000000 google-cloud-secret-manager-2.9.2/google_cloud_secret_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2817 2022-03-14 14:00:01.000000 google-cloud-secret-manager-2.9.2/google_cloud_secret_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-03-14 14:00:01.000000 google-cloud-secret-manager-2.9.2/google_cloud_secret_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-03-14 14:00:01.000000 google-cloud-secret-manager-2.9.2/google_cloud_secret_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-03-14 14:00:01.000000 google-cloud-secret-manager-2.9.2/google_cloud_secret_manager.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      151 2022-03-14 14:00:01.000000 google-cloud-secret-manager-2.9.2/google_cloud_secret_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-03-14 14:00:01.000000 google-cloud-secret-manager-2.9.2/google_cloud_secret_manager.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.705615 google-cloud-secret-manager-2.9.2/scripts/
+-rw-rw-r--   0 root         (0)     1003     6743 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/scripts/fixup_secretmanager_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6654 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/scripts/fixup_secretmanager_v1beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-03-14 14:00:01.705615 google-cloud-secret-manager-2.9.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2851 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.705615 google-cloud-secret-manager-2.9.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.705615 google-cloud-secret-manager-2.9.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.705615 google-cloud-secret-manager-2.9.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.705615 google-cloud-secret-manager-2.9.2/tests/unit/gapic/secretmanager_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/tests/unit/gapic/secretmanager_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   182660 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/tests/unit/gapic/secretmanager_v1/test_secret_manager_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-03-14 14:00:01.705615 google-cloud-secret-manager-2.9.2/tests/unit/gapic/secretmanager_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      601 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/tests/unit/gapic/secretmanager_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   164362 2022-03-14 13:57:12.000000 google-cloud-secret-manager-2.9.2/tests/unit/gapic/secretmanager_v1beta1/test_secret_manager_service.py
```

### Comparing `google-cloud-secret-manager-2.9.1/LICENSE` & `google-cloud-secret-manager-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/MANIFEST.in` & `google-cloud-secret-manager-2.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/PKG-INFO` & `google-cloud-secret-manager-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-secret-manager
-Version: 2.9.1
+Version: 2.9.2
 Summary: Secret Manager API API client library
 Home-page: https://github.com/googleapis/python-secret-manager
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-secret-manager-2.9.1/README.rst` & `google-cloud-secret-manager-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/gapic_metadata.json` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/async_client.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/client.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/pagers.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/transports/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/transports/base.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/transports/grpc.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/services/secret_manager_service/transports/grpc_asyncio.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/services/secret_manager_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/types/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/types/resources.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1/types/service.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/async_client.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/client.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/pagers.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/base.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/grpc.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/grpc_asyncio.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/services/secret_manager_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/types/__init__.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/types/resources.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google/cloud/secretmanager_v1beta1/types/service.py` & `google-cloud-secret-manager-2.9.2/google/cloud/secretmanager_v1beta1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/google_cloud_secret_manager.egg-info/PKG-INFO` & `google-cloud-secret-manager-2.9.2/google_cloud_secret_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-secret-manager
-Version: 2.9.1
+Version: 2.9.2
 Summary: Secret Manager API API client library
 Home-page: https://github.com/googleapis/python-secret-manager
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-secret-manager-2.9.1/google_cloud_secret_manager.egg-info/SOURCES.txt` & `google-cloud-secret-manager-2.9.2/google_cloud_secret_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/scripts/fixup_secretmanager_v1_keywords.py` & `google-cloud-secret-manager-2.9.2/scripts/fixup_secretmanager_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/scripts/fixup_secretmanager_v1beta1_keywords.py` & `google-cloud-secret-manager-2.9.2/scripts/fixup_secretmanager_v1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/setup.py` & `google-cloud-secret-manager-2.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import os
 
 import setuptools
 
 
 name = "google-cloud-secret-manager"
 description = "Secret Manager API API client library"
-version = "2.9.1"
+version = "2.9.2"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
     # Until this issue is closed
     # https://github.com/googleapis/google-cloud-python/issues/10566
     "google-api-core[grpc] >= 1.31.5, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0",
     "grpc-google-iam-v1 >= 0.12.3, < 0.13dev",
```

### Comparing `google-cloud-secret-manager-2.9.1/tests/__init__.py` & `google-cloud-secret-manager-2.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/tests/unit/__init__.py` & `google-cloud-secret-manager-2.9.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/tests/unit/gapic/__init__.py` & `google-cloud-secret-manager-2.9.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/tests/unit/gapic/secretmanager_v1/__init__.py` & `google-cloud-secret-manager-2.9.2/tests/unit/gapic/secretmanager_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/tests/unit/gapic/secretmanager_v1/test_secret_manager_service.py` & `google-cloud-secret-manager-2.9.2/tests/unit/gapic/secretmanager_v1/test_secret_manager_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/tests/unit/gapic/secretmanager_v1beta1/__init__.py` & `google-cloud-secret-manager-2.9.2/tests/unit/gapic/secretmanager_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-secret-manager-2.9.1/tests/unit/gapic/secretmanager_v1beta1/test_secret_manager_service.py` & `google-cloud-secret-manager-2.9.2/tests/unit/gapic/secretmanager_v1beta1/test_secret_manager_service.py`

 * *Files identical despite different names*

