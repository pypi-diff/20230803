# Comparing `tmp/google-cloud-gke-backup-0.5.0.tar.gz` & `tmp/google-cloud-gke-backup-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-gke-backup-0.5.0.tar", last modified: Wed Jul  5 15:21:41 2023, max compression
+gzip compressed data, was "google-cloud-gke-backup-0.5.1.tar", last modified: Thu Aug  3 20:27:12 2023, max compression
```

## Comparing `google-cloud-gke-backup-0.5.0.tar` & `google-cloud-gke-backup-0.5.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.248927 google-cloud-gke-backup-0.5.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4778 2023-07-05 15:21:41.248927 google-cloud-gke-backup-0.5.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3866 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.236929 google-cloud-gke-backup-0.5.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.236929 google-cloud-gke-backup-0.5.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.240929 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/
--rw-rw-r--   0 root         (0)     1003     3498 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.240929 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/
--rw-rw-r--   0 root         (0)     1003     3181 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     9647 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.240929 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.240929 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/
--rw-rw-r--   0 root         (0)     1003      761 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py
--rw-rw-r--   0 root         (0)     1003   159862 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py
--rw-rw-r--   0 root         (0)     1003   173179 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/client.py
--rw-rw-r--   0 root         (0)     1003    31038 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.244928 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22951 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py
--rw-rw-r--   0 root         (0)     1003    46982 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    47961 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   166817 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.244928 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/
--rw-rw-r--   0 root         (0)     1003     2884 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    14215 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/backup.py
--rw-rw-r--   0 root         (0)     1003    13525 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/backup_plan.py
--rw-rw-r--   0 root         (0)     1003     2520 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    36417 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/gkebackup.py
--rw-rw-r--   0 root         (0)     1003    33144 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/restore.py
--rw-rw-r--   0 root         (0)     1003     5892 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/restore_plan.py
--rw-rw-r--   0 root         (0)     1003    12236 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/volume.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.244928 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/
--rw-r--r--   0 root         (0)     1003     4778 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1851 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-05 15:21:41.000000 google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-07-05 15:21:41.248927 google-cloud-gke-backup-0.5.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2980 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.244928 google-cloud-gke-backup-0.5.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.244928 google-cloud-gke-backup-0.5.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.248927 google-cloud-gke-backup-0.5.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-05 15:21:41.248927 google-cloud-gke-backup-0.5.0/tests/unit/gapic/gke_backup_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/tests/unit/gapic/gke_backup_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   676567 2023-07-05 15:19:45.000000 google-cloud-gke-backup-0.5.0/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.928364 google-cloud-gke-backup-0.5.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4851 2023-08-03 20:27:12.928364 google-cloud-gke-backup-0.5.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3939 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.916364 google-cloud-gke-backup-0.5.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.916364 google-cloud-gke-backup-0.5.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.920364 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup/
+-rw-rw-r--   0 root         (0)     1003     3498 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.920364 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/
+-rw-rw-r--   0 root         (0)     1003     3181 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9647 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.920364 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.920364 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/
+-rw-rw-r--   0 root         (0)     1003      761 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py
+-rw-rw-r--   0 root         (0)     1003   160032 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py
+-rw-rw-r--   0 root         (0)     1003   173349 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/client.py
+-rw-rw-r--   0 root         (0)     1003    31038 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.920364 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22951 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    46982 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    47961 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   166817 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.924364 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2884 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14215 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/backup.py
+-rw-rw-r--   0 root         (0)     1003    13525 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/backup_plan.py
+-rw-rw-r--   0 root         (0)     1003     2520 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    36585 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/gkebackup.py
+-rw-rw-r--   0 root         (0)     1003    33173 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/restore.py
+-rw-rw-r--   0 root         (0)     1003     5892 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/restore_plan.py
+-rw-rw-r--   0 root         (0)     1003    12236 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/volume.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.924364 google-cloud-gke-backup-0.5.1/google_cloud_gke_backup.egg-info/
+-rw-r--r--   0 root         (0)     1003     4851 2023-08-03 20:27:12.000000 google-cloud-gke-backup-0.5.1/google_cloud_gke_backup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1851 2023-08-03 20:27:12.000000 google-cloud-gke-backup-0.5.1/google_cloud_gke_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 20:27:12.000000 google-cloud-gke-backup-0.5.1/google_cloud_gke_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 20:27:12.000000 google-cloud-gke-backup-0.5.1/google_cloud_gke_backup.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 20:27:12.000000 google-cloud-gke-backup-0.5.1/google_cloud_gke_backup.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-08-03 20:27:12.000000 google-cloud-gke-backup-0.5.1/google_cloud_gke_backup.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 20:27:12.000000 google-cloud-gke-backup-0.5.1/google_cloud_gke_backup.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-08-03 20:27:12.928364 google-cloud-gke-backup-0.5.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2980 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.924364 google-cloud-gke-backup-0.5.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.924364 google-cloud-gke-backup-0.5.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.924364 google-cloud-gke-backup-0.5.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 20:27:12.924364 google-cloud-gke-backup-0.5.1/tests/unit/gapic/gke_backup_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/tests/unit/gapic/gke_backup_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   676567 2023-08-03 20:25:16.000000 google-cloud-gke-backup-0.5.1/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py
```

### Comparing `google-cloud-gke-backup-0.5.0/LICENSE` & `google-cloud-gke-backup-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.0/MANIFEST.in` & `google-cloud-gke-backup-0.5.1/MANIFEST.in`

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

### Comparing `google-cloud-gke-backup-0.5.0/PKG-INFO` & `google-cloud-gke-backup-0.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-backup
-Version: 0.5.0
+Version: 0.5.1
 Summary: Google Cloud Gke Backup API client library
 Home-page: https://github.com/googleapis/python-gke-backup
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Backup for GKE API.:  https://cloud.google.com/kubernetes-engine/docs/add-on/backup-for-gke/concepts/backup-for-gke
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
+.. _samples/: https://github.com/googleapis/python-gke-backup/tree/main/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-gke-backup
+    pip install google-cloud-gke-backup
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-gke-backup
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-gke-backup
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Backup for GKE API
    to see other available methods on the client.
 -  Read the `Backup for GKE API Product documentation`_ to learn
```

### Comparing `google-cloud-gke-backup-0.5.0/README.rst` & `google-cloud-gke-backup-0.5.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -32,29 +32,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Backup for GKE API.:  https://cloud.google.com/kubernetes-engine/docs/add-on/backup-for-gke/concepts/backup-for-gke
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
+.. _samples/: https://github.com/googleapis/python-gke-backup/tree/main/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-gke-backup
+    pip install google-cloud-gke-backup
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-gke-backup
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-gke-backup
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Backup for GKE API
    to see other available methods on the client.
 -  Read the `Backup for GKE API Product documentation`_ to learn
```

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/__init__.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup/__init__.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup/gapic_version.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup/gapic_version.py`

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
-__version__ = "0.5.0"  # {x-release-please-version}
+__version__ = "0.5.1"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/__init__.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/__init__.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/gapic_metadata.json` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/gapic_version.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/gapic_version.py`

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
-__version__ = "0.5.0"  # {x-release-please-version}
+__version__ = "0.5.1"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/__init__.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/__init__.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py`

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
@@ -313,21 +313,23 @@
                 This corresponds to the ``backup_plan`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             backup_plan_id (:class:`str`):
                 Required. The client-provided short
                 name for the BackupPlan resource. This
                 name must:
+
                 - be between 1 and 63 characters long
-                (inclusive) - consist of only lower-case
-                ASCII letters, numbers, and dashes -
-                start with a lower-case letter
+                  (inclusive)
+                - consist of only lower-case ASCII
+                  letters, numbers, and dashes
+                - start with a lower-case letter
                 - end with a lower-case letter or number
                 - be unique within the set of
-                BackupPlans in this location
+                  BackupPlans in this location
 
                 This corresponds to the ``backup_plan_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -953,19 +955,22 @@
                 This corresponds to the ``backup`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             backup_id (:class:`str`):
                 The client-provided short name for
                 the Backup resource. This name must:
 
-                 - be between 1 and 63 characters long (inclusive)
-                 - consist of only lower-case ASCII letters, numbers, and dashes
-                 - start with a lower-case letter
-                 - end with a lower-case letter or number
-                 - be unique within the set of Backups in this BackupPlan
+                - be between 1 and 63 characters long
+                  (inclusive)
+                - consist of only lower-case ASCII
+                  letters, numbers, and dashes
+                - start with a lower-case letter
+                - end with a lower-case letter or number
+                - be unique within the set of Backups in
+                  this BackupPlan
 
                 This corresponds to the ``backup_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1848,19 +1853,22 @@
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             restore_plan_id (:class:`str`):
                 Required. The client-provided short
                 name for the RestorePlan resource. This
                 name must:
 
-                 - be between 1 and 63 characters long (inclusive)
-                 - consist of only lower-case ASCII letters, numbers, and dashes
-                 - start with a lower-case letter
-                 - end with a lower-case letter or number
-                 - be unique within the set of RestorePlans in this location
+                - be between 1 and 63 characters long
+                  (inclusive)
+                - consist of only lower-case ASCII
+                  letters, numbers, and dashes
+                - start with a lower-case letter
+                - end with a lower-case letter or number
+                - be unique within the set of
+                  RestorePlans in this location
 
                 This corresponds to the ``restore_plan_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -2499,19 +2507,22 @@
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             restore_id (:class:`str`):
                 Required. The client-provided short
                 name for the Restore resource. This name
                 must:
 
-                 - be between 1 and 63 characters long (inclusive)
-                 - consist of only lower-case ASCII letters, numbers, and dashes
-                 - start with a lower-case letter
-                 - end with a lower-case letter or number
-                 - be unique within the set of Restores in this RestorePlan.
+                - be between 1 and 63 characters long
+                  (inclusive)
+                - consist of only lower-case ASCII
+                  letters, numbers, and dashes
+                - start with a lower-case letter
+                - end with a lower-case letter or number
+                - be unique within the set of Restores
+                  in this RestorePlan.
 
                 This corresponds to the ``restore_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/client.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/client.py`

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
@@ -698,21 +698,23 @@
                 This corresponds to the ``backup_plan`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             backup_plan_id (str):
                 Required. The client-provided short
                 name for the BackupPlan resource. This
                 name must:
+
                 - be between 1 and 63 characters long
-                (inclusive) - consist of only lower-case
-                ASCII letters, numbers, and dashes -
-                start with a lower-case letter
+                  (inclusive)
+                - consist of only lower-case ASCII
+                  letters, numbers, and dashes
+                - start with a lower-case letter
                 - end with a lower-case letter or number
                 - be unique within the set of
-                BackupPlans in this location
+                  BackupPlans in this location
 
                 This corresponds to the ``backup_plan_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1320,19 +1322,22 @@
                 This corresponds to the ``backup`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             backup_id (str):
                 The client-provided short name for
                 the Backup resource. This name must:
 
-                 - be between 1 and 63 characters long (inclusive)
-                 - consist of only lower-case ASCII letters, numbers, and dashes
-                 - start with a lower-case letter
-                 - end with a lower-case letter or number
-                 - be unique within the set of Backups in this BackupPlan
+                - be between 1 and 63 characters long
+                  (inclusive)
+                - consist of only lower-case ASCII
+                  letters, numbers, and dashes
+                - start with a lower-case letter
+                - end with a lower-case letter or number
+                - be unique within the set of Backups in
+                  this BackupPlan
 
                 This corresponds to the ``backup_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -2179,19 +2184,22 @@
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             restore_plan_id (str):
                 Required. The client-provided short
                 name for the RestorePlan resource. This
                 name must:
 
-                 - be between 1 and 63 characters long (inclusive)
-                 - consist of only lower-case ASCII letters, numbers, and dashes
-                 - start with a lower-case letter
-                 - end with a lower-case letter or number
-                 - be unique within the set of RestorePlans in this location
+                - be between 1 and 63 characters long
+                  (inclusive)
+                - consist of only lower-case ASCII
+                  letters, numbers, and dashes
+                - start with a lower-case letter
+                - end with a lower-case letter or number
+                - be unique within the set of
+                  RestorePlans in this location
 
                 This corresponds to the ``restore_plan_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -2812,19 +2820,22 @@
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             restore_id (str):
                 Required. The client-provided short
                 name for the Restore resource. This name
                 must:
 
-                 - be between 1 and 63 characters long (inclusive)
-                 - consist of only lower-case ASCII letters, numbers, and dashes
-                 - start with a lower-case letter
-                 - end with a lower-case letter or number
-                 - be unique within the set of Restores in this RestorePlan.
+                - be between 1 and 63 characters long
+                  (inclusive)
+                - consist of only lower-case ASCII
+                  letters, numbers, and dashes
+                - start with a lower-case letter
+                - end with a lower-case letter or number
+                - be unique within the set of Restores
+                  in this RestorePlan.
 
                 This corresponds to the ``restore_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/__init__.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/__init__.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/backup.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/backup.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/backup_plan.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/backup_plan.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/common.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/common.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/gkebackup.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/gkebackup.py`

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
@@ -137,19 +137,22 @@
         backup_plan (google.cloud.gke_backup_v1.types.BackupPlan):
             Required. The BackupPlan resource object to
             create.
         backup_plan_id (str):
             Required. The client-provided short name for
             the BackupPlan resource. This name must:
 
-            - be between 1 and 63 characters long (inclusive)
-            - consist of only lower-case ASCII letters, numbers, and dashes
+            - be between 1 and 63 characters long
+              (inclusive)
+            - consist of only lower-case ASCII letters,
+              numbers, and dashes
             - start with a lower-case letter
             - end with a lower-case letter or number
-            - be unique within the set of BackupPlans in this location
+            - be unique within the set of BackupPlans in
+              this location
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     backup_plan: gcg_backup_plan.BackupPlan = proto.Field(
@@ -331,19 +334,22 @@
             Format: ``projects/*/locations/*/backupPlans/*``
         backup (google.cloud.gke_backup_v1.types.Backup):
             The Backup resource to create.
         backup_id (str):
             The client-provided short name for the Backup
             resource. This name must:
 
-            - be between 1 and 63 characters long (inclusive)
-            - consist of only lower-case ASCII letters, numbers, and dashes
+            - be between 1 and 63 characters long
+              (inclusive)
+            - consist of only lower-case ASCII letters,
+              numbers, and dashes
             - start with a lower-case letter
             - end with a lower-case letter or number
-            - be unique within the set of Backups in this BackupPlan
+            - be unique within the set of Backups in this
+              BackupPlan
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     backup: gcg_backup.Backup = proto.Field(
@@ -625,19 +631,22 @@
         restore_plan (google.cloud.gke_backup_v1.types.RestorePlan):
             Required. The RestorePlan resource object to
             create.
         restore_plan_id (str):
             Required. The client-provided short name for
             the RestorePlan resource. This name must:
 
-            - be between 1 and 63 characters long (inclusive)
-            - consist of only lower-case ASCII letters, numbers, and dashes
+            - be between 1 and 63 characters long
+              (inclusive)
+            - consist of only lower-case ASCII letters,
+              numbers, and dashes
             - start with a lower-case letter
             - end with a lower-case letter or number
-            - be unique within the set of RestorePlans in this location
+            - be unique within the set of RestorePlans in
+              this location
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     restore_plan: gcg_restore_plan.RestorePlan = proto.Field(
@@ -827,19 +836,22 @@
             Restore. Format: ``projects/*/locations/*/restorePlans/*``
         restore (google.cloud.gke_backup_v1.types.Restore):
             Required. The restore resource to create.
         restore_id (str):
             Required. The client-provided short name for
             the Restore resource. This name must:
 
-            - be between 1 and 63 characters long (inclusive)
-            - consist of only lower-case ASCII letters, numbers, and dashes
+            - be between 1 and 63 characters long
+              (inclusive)
+            - consist of only lower-case ASCII letters,
+              numbers, and dashes
             - start with a lower-case letter
             - end with a lower-case letter or number
-            - be unique within the set of Restores in this RestorePlan.
+            - be unique within the set of Restores in this
+              RestorePlan.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     restore: gcg_restore.Restore = proto.Field(
```

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/restore.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/restore.py`

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
@@ -411,15 +411,16 @@
         )
 
     class ClusterResourceRestoreScope(proto.Message):
         r"""Defines the scope of cluster-scoped resources to restore.
         Some group kinds are not reasonable choices for a restore, and
         will cause an error if selected here. Any scope selection that
         would restore "all valid" resources automatically excludes these
-        group kinds. - gkebackup.gke.io/BackupJob
+        group kinds.
+        - gkebackup.gke.io/BackupJob
         - gkebackup.gke.io/RestoreJob
         - metrics.k8s.io/NodeMetrics
         - migration.k8s.io/StorageState
         - migration.k8s.io/StorageVersionMigration
         - Node
         - snapshot.storage.k8s.io/VolumeSnapshotContent
         - storage.k8s.io/CSINode
@@ -592,22 +593,24 @@
                     location.
                 COPY (3):
                     The "copy" operation copies the value at a
                     specified location to the target location.
                 ADD (4):
                     The "add" operation performs one of the
                     following functions, depending upon what the
-                    target location references: 1. If the target
-                    location specifies an array index, a new value
-                    is inserted into the array at the specified
-                    index. 2. If the target location specifies an
-                    object member that does not already exist, a new
-                    member is added to the object. 3. If the target
-                    location specifies an object member that does
-                    exist, that member's value is replaced.
+                    target location references:
+
+                    1. If the target location specifies an array
+                    index, a new value is inserted into the array at
+                    the specified index. 2. If the target location
+                    specifies an object member that does not already
+                    exist, a new member is added to the object. 3.
+                    If the target location specifies an object
+                    member that does exist, that member's value is
+                    replaced.
                 TEST (5):
                     The "test" operation tests that a value at
                     the target location is equal to a specified
                     value.
                 REPLACE (6):
                     The "replace" operation replaces the value at
                     the target location with a new value.  The
```

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/restore_plan.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/restore_plan.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google/cloud/gke_backup_v1/types/volume.py` & `google-cloud-gke-backup-0.5.1/google/cloud/gke_backup_v1/types/volume.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/PKG-INFO` & `google-cloud-gke-backup-0.5.1/google_cloud_gke_backup.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-backup
-Version: 0.5.0
+Version: 0.5.1
 Summary: Google Cloud Gke Backup API client library
 Home-page: https://github.com/googleapis/python-gke-backup
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -56,29 +56,32 @@
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
 .. _Enable the Backup for GKE API.:  https://cloud.google.com/kubernetes-engine/docs/add-on/backup-for-gke/concepts/backup-for-gke
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
+.. _samples/: https://github.com/googleapis/python-gke-backup/tree/main/samples
 
 
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
-    <your-env>/bin/pip install google-cloud-gke-backup
+    pip install google-cloud-gke-backup
 
 
 Windows
 ^^^^^^^
 
 .. code-block:: console
 
-    pip install virtualenv
-    virtualenv <your-env>
-    <your-env>\Scripts\activate
-    <your-env>\Scripts\pip.exe install google-cloud-gke-backup
+    py -m venv <your-env>
+    .\<your-env>\Scripts\activate
+    pip install google-cloud-gke-backup
 
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Backup for GKE API
    to see other available methods on the client.
 -  Read the `Backup for GKE API Product documentation`_ to learn
```

### Comparing `google-cloud-gke-backup-0.5.0/google_cloud_gke_backup.egg-info/SOURCES.txt` & `google-cloud-gke-backup-0.5.1/google_cloud_gke_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.5.0/setup.py` & `google-cloud-gke-backup-0.5.1/setup.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/tests/__init__.py` & `google-cloud-gke-backup-0.5.1/tests/__init__.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/tests/unit/__init__.py` & `google-cloud-gke-backup-0.5.1/tests/unit/__init__.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/tests/unit/gapic/__init__.py` & `google-cloud-gke-backup-0.5.1/tests/unit/gapic/__init__.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/tests/unit/gapic/gke_backup_v1/__init__.py` & `google-cloud-gke-backup-0.5.1/tests/unit/gapic/gke_backup_v1/__init__.py`

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

### Comparing `google-cloud-gke-backup-0.5.0/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py` & `google-cloud-gke-backup-0.5.1/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py`

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

