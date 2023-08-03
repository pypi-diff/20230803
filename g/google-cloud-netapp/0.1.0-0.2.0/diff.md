# Comparing `tmp/google-cloud-netapp-0.1.0.tar.gz` & `tmp/google-cloud-netapp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-netapp-0.1.0.tar", last modified: Thu Jul 20 19:30:46 2023, max compression
+gzip compressed data, was "google-cloud-netapp-0.2.0.tar", last modified: Thu Aug  3 19:07:01 2023, max compression
```

## Comparing `google-cloud-netapp-0.1.0.tar` & `google-cloud-netapp-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.328206 google-cloud-netapp-0.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4610 2023-07-20 19:30:46.328206 google-cloud-netapp-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3704 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.316207 google-cloud-netapp-0.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.316207 google-cloud-netapp-0.1.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.320207 google-cloud-netapp-0.1.0/google/cloud/netapp/
--rw-rw-r--   0 root         (0)     1003     4919 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.320207 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/
--rw-rw-r--   0 root         (0)     1003     4608 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    14393 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.320207 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.320207 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/
--rw-rw-r--   0 root         (0)     1003      737 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/__init__.py
--rw-rw-r--   0 root         (0)     1003   199871 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/async_client.py
--rw-rw-r--   0 root         (0)     1003   213843 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/client.py
--rw-rw-r--   0 root         (0)     1003    31219 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.324206 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/
--rw-rw-r--   0 root         (0)     1003     1288 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    28082 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/base.py
--rw-rw-r--   0 root         (0)     1003    58465 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    59766 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   217525 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.324206 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     4286 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    11224 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/active_directory.py
--rw-rw-r--   0 root         (0)     1003     2878 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/cloud_netapp_service.py
--rw-rw-r--   0 root         (0)     1003     1841 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/common.py
--rw-rw-r--   0 root         (0)     1003    10282 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/kms.py
--rw-rw-r--   0 root         (0)     1003    19383 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/replication.py
--rw-rw-r--   0 root         (0)     1003     8101 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/snapshot.py
--rw-rw-r--   0 root         (0)     1003    10272 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/storage_pool.py
--rw-rw-r--   0 root         (0)     1003    30256 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/volume.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.328206 google-cloud-netapp-0.1.0/google_cloud_netapp.egg-info/
--rw-r--r--   0 root         (0)     1003     4610 2023-07-20 19:30:46.000000 google-cloud-netapp-0.1.0/google_cloud_netapp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1818 2023-07-20 19:30:46.000000 google-cloud-netapp-0.1.0/google_cloud_netapp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-20 19:30:46.000000 google-cloud-netapp-0.1.0/google_cloud_netapp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-07-20 19:30:46.000000 google-cloud-netapp-0.1.0/google_cloud_netapp.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-07-20 19:30:46.000000 google-cloud-netapp-0.1.0/google_cloud_netapp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-07-20 19:30:46.000000 google-cloud-netapp-0.1.0/google_cloud_netapp.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-07-20 19:30:46.000000 google-cloud-netapp-0.1.0/google_cloud_netapp.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-07-20 19:30:46.328206 google-cloud-netapp-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2923 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.328206 google-cloud-netapp-0.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.328206 google-cloud-netapp-0.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.328206 google-cloud-netapp-0.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-07-20 19:30:46.328206 google-cloud-netapp-0.1.0/tests/unit/gapic/netapp_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/tests/unit/gapic/netapp_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   839232 2023-07-20 19:27:31.000000 google-cloud-netapp-0.1.0/tests/unit/gapic/netapp_v1beta1/test_net_app.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.863261 google-cloud-netapp-0.2.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4610 2023-08-03 19:07:01.863261 google-cloud-netapp-0.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3704 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.851261 google-cloud-netapp-0.2.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.851261 google-cloud-netapp-0.2.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.855261 google-cloud-netapp-0.2.0/google/cloud/netapp/
+-rw-rw-r--   0 root         (0)     1003     4869 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.855261 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/
+-rw-rw-r--   0 root         (0)     1003     4603 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14383 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.855261 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.855261 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/
+-rw-rw-r--   0 root         (0)     1003      737 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/__init__.py
+-rw-rw-r--   0 root         (0)     1003   185023 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/async_client.py
+-rw-rw-r--   0 root         (0)     1003   199115 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/client.py
+-rw-rw-r--   0 root         (0)     1003    30974 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.859261 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/
+-rw-rw-r--   0 root         (0)     1003     1288 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    26638 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    52681 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    53982 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   194993 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.859261 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/
+-rw-rw-r--   0 root         (0)     1003     4286 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11199 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/active_directory.py
+-rw-rw-r--   0 root         (0)     1003     2851 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/cloud_netapp_service.py
+-rw-rw-r--   0 root         (0)     1003     1836 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    10052 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/kms.py
+-rw-rw-r--   0 root         (0)     1003    19308 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/replication.py
+-rw-rw-r--   0 root         (0)     1003     8068 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/snapshot.py
+-rw-rw-r--   0 root         (0)     1003    10062 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/storage_pool.py
+-rw-rw-r--   0 root         (0)     1003    29876 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/volume.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.863261 google-cloud-netapp-0.2.0/google_cloud_netapp.egg-info/
+-rw-r--r--   0 root         (0)     1003     4610 2023-08-03 19:07:01.000000 google-cloud-netapp-0.2.0/google_cloud_netapp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1693 2023-08-03 19:07:01.000000 google-cloud-netapp-0.2.0/google_cloud_netapp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:07:01.000000 google-cloud-netapp-0.2.0/google_cloud_netapp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-08-03 19:07:01.000000 google-cloud-netapp-0.2.0/google_cloud_netapp.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-08-03 19:07:01.000000 google-cloud-netapp-0.2.0/google_cloud_netapp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-08-03 19:07:01.000000 google-cloud-netapp-0.2.0/google_cloud_netapp.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-08-03 19:07:01.000000 google-cloud-netapp-0.2.0/google_cloud_netapp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-08-03 19:07:01.863261 google-cloud-netapp-0.2.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2923 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.863261 google-cloud-netapp-0.2.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.863261 google-cloud-netapp-0.2.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.863261 google-cloud-netapp-0.2.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-08-03 19:07:01.863261 google-cloud-netapp-0.2.0/tests/unit/gapic/netapp_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/tests/unit/gapic/netapp_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   795086 2023-08-03 19:03:10.000000 google-cloud-netapp-0.2.0/tests/unit/gapic/netapp_v1/test_net_app.py
```

### Comparing `google-cloud-netapp-0.1.0/LICENSE` & `google-cloud-netapp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.1.0/MANIFEST.in` & `google-cloud-netapp-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.1.0/PKG-INFO` & `google-cloud-netapp-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-netapp
-Version: 0.1.0
+Version: 0.2.0
 Summary: Google Cloud Netapp API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-netapp-0.1.0/README.rst` & `google-cloud-netapp-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp/__init__.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,72 +14,72 @@
 # limitations under the License.
 #
 from google.cloud.netapp import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.cloud.netapp_v1beta1.services.net_app.async_client import NetAppAsyncClient
-from google.cloud.netapp_v1beta1.services.net_app.client import NetAppClient
-from google.cloud.netapp_v1beta1.types.active_directory import (
+from google.cloud.netapp_v1.services.net_app.async_client import NetAppAsyncClient
+from google.cloud.netapp_v1.services.net_app.client import NetAppClient
+from google.cloud.netapp_v1.types.active_directory import (
     ActiveDirectory,
     CreateActiveDirectoryRequest,
     DeleteActiveDirectoryRequest,
     GetActiveDirectoryRequest,
     ListActiveDirectoriesRequest,
     ListActiveDirectoriesResponse,
     UpdateActiveDirectoryRequest,
 )
-from google.cloud.netapp_v1beta1.types.cloud_netapp_service import OperationMetadata
-from google.cloud.netapp_v1beta1.types.common import EncryptionType, ServiceLevel
-from google.cloud.netapp_v1beta1.types.kms import (
+from google.cloud.netapp_v1.types.cloud_netapp_service import OperationMetadata
+from google.cloud.netapp_v1.types.common import EncryptionType, ServiceLevel
+from google.cloud.netapp_v1.types.kms import (
     CreateKmsConfigRequest,
     DeleteKmsConfigRequest,
     EncryptVolumesRequest,
     GetKmsConfigRequest,
     KmsConfig,
     ListKmsConfigsRequest,
     ListKmsConfigsResponse,
     UpdateKmsConfigRequest,
     VerifyKmsConfigRequest,
     VerifyKmsConfigResponse,
 )
-from google.cloud.netapp_v1beta1.types.replication import (
+from google.cloud.netapp_v1.types.replication import (
     CreateReplicationRequest,
     DeleteReplicationRequest,
     DestinationVolumeParameters,
     GetReplicationRequest,
     ListReplicationsRequest,
     ListReplicationsResponse,
     Replication,
     ResumeReplicationRequest,
     ReverseReplicationDirectionRequest,
     StopReplicationRequest,
     TransferStats,
     UpdateReplicationRequest,
 )
-from google.cloud.netapp_v1beta1.types.snapshot import (
+from google.cloud.netapp_v1.types.snapshot import (
     CreateSnapshotRequest,
     DeleteSnapshotRequest,
     GetSnapshotRequest,
     ListSnapshotsRequest,
     ListSnapshotsResponse,
     Snapshot,
     UpdateSnapshotRequest,
 )
-from google.cloud.netapp_v1beta1.types.storage_pool import (
+from google.cloud.netapp_v1.types.storage_pool import (
     CreateStoragePoolRequest,
     DeleteStoragePoolRequest,
     GetStoragePoolRequest,
     ListStoragePoolsRequest,
     ListStoragePoolsResponse,
     StoragePool,
     UpdateStoragePoolRequest,
 )
-from google.cloud.netapp_v1beta1.types.volume import (
+from google.cloud.netapp_v1.types.volume import (
     AccessType,
     CreateVolumeRequest,
     DailySchedule,
     DeleteVolumeRequest,
     ExportPolicy,
     GetVolumeRequest,
     HourlySchedule,
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp/gapic_version.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,9 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from .async_client import NetAppAsyncClient
+from .client import NetAppClient
 
-__version__ = "0.1.0"  # {x-release-please-version}
+__all__ = (
+    "NetAppClient",
+    "NetAppAsyncClient",
+)
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/__init__.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.netapp_v1beta1 import gapic_version as package_version
+from google.cloud.netapp_v1 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.net_app import NetAppAsyncClient, NetAppClient
 from .types.active_directory import (
     ActiveDirectory,
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/gapic_metadata.json` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/gapic_metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'libraryPackage'": "'google.cloud.netapp_v1'", "'protoPackage'": "'google.cloud.netapp.v1'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "comment": "This file maps proto services/RPCs to the corresponding library clients/methods",
     "language": "python",
-    "libraryPackage": "google.cloud.netapp_v1beta1",
-    "protoPackage": "google.cloud.netapp.v1beta1",
+    "libraryPackage": "google.cloud.netapp_v1",
+    "protoPackage": "google.cloud.netapp.v1",
     "schema": "1.0",
     "services": {
         "NetApp": {
             "clients": {
                 "grpc": {
                     "libraryClient": "NetAppClient",
                     "rpcs": {
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/gapic_version.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,9 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-__version__ = "0.1.0"  # {x-release-please-version}
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/__init__.py` & `google-cloud-netapp-0.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/__init__.py` & `google-cloud-netapp-0.2.0/tests/unit/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from .async_client import NetAppAsyncClient
-from .client import NetAppClient
-
-__all__ = (
-    "NetAppClient",
-    "NetAppAsyncClient",
-)
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/async_client.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,41 +31,41 @@
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.api_core.client_options import ClientOptions
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.netapp_v1beta1 import gapic_version as package_version
+from google.cloud.netapp_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.location import locations_pb2  # type: ignore
 from google.longrunning import operations_pb2
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
-from google.cloud.netapp_v1beta1.services.net_app import pagers
-from google.cloud.netapp_v1beta1.types import active_directory as gcn_active_directory
-from google.cloud.netapp_v1beta1.types import active_directory
-from google.cloud.netapp_v1beta1.types import cloud_netapp_service, common, kms
-from google.cloud.netapp_v1beta1.types import replication
-from google.cloud.netapp_v1beta1.types import replication as gcn_replication
-from google.cloud.netapp_v1beta1.types import snapshot
-from google.cloud.netapp_v1beta1.types import snapshot as gcn_snapshot
-from google.cloud.netapp_v1beta1.types import storage_pool
-from google.cloud.netapp_v1beta1.types import storage_pool as gcn_storage_pool
-from google.cloud.netapp_v1beta1.types import volume
-from google.cloud.netapp_v1beta1.types import volume as gcn_volume
+from google.cloud.netapp_v1.services.net_app import pagers
+from google.cloud.netapp_v1.types import active_directory as gcn_active_directory
+from google.cloud.netapp_v1.types import active_directory
+from google.cloud.netapp_v1.types import cloud_netapp_service, common, kms
+from google.cloud.netapp_v1.types import replication
+from google.cloud.netapp_v1.types import replication as gcn_replication
+from google.cloud.netapp_v1.types import snapshot
+from google.cloud.netapp_v1.types import snapshot as gcn_snapshot
+from google.cloud.netapp_v1.types import storage_pool
+from google.cloud.netapp_v1.types import storage_pool as gcn_storage_pool
+from google.cloud.netapp_v1.types import volume
+from google.cloud.netapp_v1.types import volume as gcn_volume
 
 from .client import NetAppClient
 from .transports.base import DEFAULT_CLIENT_INFO, NetAppTransport
 from .transports.grpc_asyncio import NetAppGrpcAsyncIOTransport
 
 
 class NetAppAsyncClient:
@@ -239,62 +239,60 @@
         request: Optional[Union[storage_pool.ListStoragePoolsRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListStoragePoolsAsyncPager:
-        r"""ListStoragePools
-        Returns descriptions of all storage pools owned by the
-        caller.
+        r"""Returns descriptions of all storage pools owned by
+        the caller.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_list_storage_pools():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListStoragePoolsRequest(
+                request = netapp_v1.ListStoragePoolsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_storage_pools(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.ListStoragePoolsRequest, dict]]):
-                The request object. ListStoragePoolsRequest
+            request (Optional[Union[google.cloud.netapp_v1.types.ListStoragePoolsRequest, dict]]):
+                The request object.
             parent (:class:`str`):
                 Required. Parent value
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListStoragePoolsAsyncPager:
-                ListStoragePoolsResponse
+            google.cloud.netapp_v1.services.net_app.pagers.ListStoragePoolsAsyncPager:
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -365,39 +363,38 @@
         parent: Optional[str] = None,
         storage_pool: Optional[gcn_storage_pool.StoragePool] = None,
         storage_pool_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""CreateStoragePool
-        Creates a new storage pool.
+        r"""Creates a new storage pool.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_create_storage_pool():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                storage_pool = netapp_v1beta1.StoragePool()
+                storage_pool = netapp_v1.StoragePool()
                 storage_pool.service_level = "STANDARD"
                 storage_pool.capacity_gib = 1247
                 storage_pool.network = "network_value"
 
-                request = netapp_v1beta1.CreateStoragePoolRequest(
+                request = netapp_v1.CreateStoragePoolRequest(
                     parent="parent_value",
                     storage_pool_id="storage_pool_id_value",
                     storage_pool=storage_pool,
                 )
 
                 # Make the request
                 operation = client.create_storage_pool(request=request)
@@ -406,22 +403,22 @@
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.CreateStoragePoolRequest, dict]]):
-                The request object. CreateStoragePoolRequest
+            request (Optional[Union[google.cloud.netapp_v1.types.CreateStoragePoolRequest, dict]]):
+                The request object.
             parent (:class:`str`):
                 Required. Value for parent.
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            storage_pool (:class:`google.cloud.netapp_v1beta1.types.StoragePool`):
+            storage_pool (:class:`google.cloud.netapp_v1.types.StoragePool`):
                 Required. The required parameters to
                 create a new storage pool.
 
                 This corresponds to the ``storage_pool`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             storage_pool_id (:class:`str`):
@@ -438,19 +435,18 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.StoragePool` Resources
-                   StoragePool StoragePool is a container for volumes
-                   with a service level and capacity. Volumes can be
-                   created in a pool of sufficient available capacity.
-                   StoragePool capacity is what you are billed for.
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.StoragePool` StoragePool is a container for volumes with a service level and capacity.
+                   Volumes can be created in a pool of sufficient
+                   available capacity. StoragePool capacity is what you
+                   are billed for.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, storage_pool, storage_pool_id])
         if request is not None and has_flattened_params:
@@ -508,66 +504,63 @@
         request: Optional[Union[storage_pool.GetStoragePoolRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> storage_pool.StoragePool:
-        r"""GetStoragePool
-        Returns the description of the specified storage pool by
-        poolId.
+        r"""Returns the description of the specified storage pool
+        by poolId.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_get_storage_pool():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetStoragePoolRequest(
+                request = netapp_v1.GetStoragePoolRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_storage_pool(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.GetStoragePoolRequest, dict]]):
-                The request object. GetStoragePoolRequest
+            request (Optional[Union[google.cloud.netapp_v1.types.GetStoragePoolRequest, dict]]):
+                The request object.
             name (:class:`str`):
                 Required. Name of the storage pool
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.StoragePool:
-                Resources
-                StoragePool
-                StoragePool is a container for volumes
-                with a service level and capacity.
-                Volumes can be created in a pool of
-                sufficient available capacity.
+            google.cloud.netapp_v1.types.StoragePool:
+                StoragePool is a container for
+                volumes with a service level and
+                capacity. Volumes can be created in a
+                pool of sufficient available capacity.
                 StoragePool capacity is what you are
                 billed for.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -627,56 +620,56 @@
         *,
         storage_pool: Optional[gcn_storage_pool.StoragePool] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""UpdateStoragePool
-        Updates the storage pool properties with the full spec
+        r"""Updates the storage pool properties with the full
+        spec
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_update_storage_pool():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                storage_pool = netapp_v1beta1.StoragePool()
+                storage_pool = netapp_v1.StoragePool()
                 storage_pool.service_level = "STANDARD"
                 storage_pool.capacity_gib = 1247
                 storage_pool.network = "network_value"
 
-                request = netapp_v1beta1.UpdateStoragePoolRequest(
+                request = netapp_v1.UpdateStoragePoolRequest(
                     storage_pool=storage_pool,
                 )
 
                 # Make the request
                 operation = client.update_storage_pool(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.UpdateStoragePoolRequest, dict]]):
-                The request object. UpdateStoragePoolRequest
-            storage_pool (:class:`google.cloud.netapp_v1beta1.types.StoragePool`):
+            request (Optional[Union[google.cloud.netapp_v1.types.UpdateStoragePoolRequest, dict]]):
+                The request object.
+            storage_pool (:class:`google.cloud.netapp_v1.types.StoragePool`):
                 Required. The pool being updated
                 This corresponds to the ``storage_pool`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Field mask is used to specify the fields to be
                 overwritten in the StoragePool resource by the update.
@@ -694,19 +687,18 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.StoragePool` Resources
-                   StoragePool StoragePool is a container for volumes
-                   with a service level and capacity. Volumes can be
-                   created in a pool of sufficient available capacity.
-                   StoragePool capacity is what you are billed for.
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.StoragePool` StoragePool is a container for volumes with a service level and capacity.
+                   Volumes can be created in a pool of sufficient
+                   available capacity. StoragePool capacity is what you
+                   are billed for.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([storage_pool, update_mask])
         if request is not None and has_flattened_params:
@@ -764,51 +756,50 @@
         request: Optional[Union[storage_pool.DeleteStoragePoolRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""DeleteStoragePool
-        Warning! This operation will permanently delete the
+        r"""Warning! This operation will permanently delete the
         storage pool.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_delete_storage_pool():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteStoragePoolRequest(
+                request = netapp_v1.DeleteStoragePoolRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_storage_pool(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.DeleteStoragePoolRequest, dict]]):
-                The request object. DeleteStoragePoolRequest
+            request (Optional[Union[google.cloud.netapp_v1.types.DeleteStoragePoolRequest, dict]]):
+                The request object.
             name (:class:`str`):
                 Required. Name of the storage pool
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -887,66 +878,64 @@
         request: Optional[Union[volume.ListVolumesRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListVolumesAsyncPager:
-        r"""ListVolumes
-        Lists Volumes in a given project.
+        r"""Lists Volumes in a given project.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_list_volumes():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListVolumesRequest(
+                request = netapp_v1.ListVolumesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_volumes(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.ListVolumesRequest, dict]]):
-                The request object. ListVolumesRequest
-                Message for requesting list of Volumes
+            request (Optional[Union[google.cloud.netapp_v1.types.ListVolumesRequest, dict]]):
+                The request object. Message for requesting list of
+                Volumes
             parent (:class:`str`):
                 Required. Parent value for
                 ListVolumesRequest
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListVolumesAsyncPager:
-                ListVolumesResponse
-                Message for response to listing Volumes
-
+            google.cloud.netapp_v1.services.net_app.pagers.ListVolumesAsyncPager:
+                Message for response to listing
+                Volumes
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1013,61 +1002,58 @@
         request: Optional[Union[volume.GetVolumeRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> volume.Volume:
-        r"""GetVolume
-        Gets details of a single Volume.
+        r"""Gets details of a single Volume.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_get_volume():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetVolumeRequest(
+                request = netapp_v1.GetVolumeRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_volume(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.GetVolumeRequest, dict]]):
-                The request object. GetVolumeRequest
-                Message for getting a Volume
+            request (Optional[Union[google.cloud.netapp_v1.types.GetVolumeRequest, dict]]):
+                The request object. Message for getting a Volume
             name (:class:`str`):
                 Required. Name of the volume
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.Volume:
-                Volume
+            google.cloud.netapp_v1.types.Volume:
                 Volume provides a filesystem that you
                 can mount.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -1126,40 +1112,39 @@
         parent: Optional[str] = None,
         volume: Optional[gcn_volume.Volume] = None,
         volume_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""CreateVolume
-        Creates a new Volume in a given project and location.
+        r"""Creates a new Volume in a given project and location.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_create_volume():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                volume = netapp_v1beta1.Volume()
+                volume = netapp_v1.Volume()
                 volume.share_name = "share_name_value"
                 volume.storage_pool = "storage_pool_value"
                 volume.capacity_gib = 1247
                 volume.protocols = ['SMB']
 
-                request = netapp_v1beta1.CreateVolumeRequest(
+                request = netapp_v1.CreateVolumeRequest(
                     parent="parent_value",
                     volume_id="volume_id_value",
                     volume=volume,
                 )
 
                 # Make the request
                 operation = client.create_volume(request=request)
@@ -1168,23 +1153,22 @@
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.CreateVolumeRequest, dict]]):
-                The request object. CreateVolumeRequest
-                Message for creating a Volume
+            request (Optional[Union[google.cloud.netapp_v1.types.CreateVolumeRequest, dict]]):
+                The request object. Message for creating a Volume
             parent (:class:`str`):
                 Required. Value for parent.
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            volume (:class:`google.cloud.netapp_v1beta1.types.Volume`):
+            volume (:class:`google.cloud.netapp_v1.types.Volume`):
                 Required. The volume being created.
                 This corresponds to the ``volume`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             volume_id (:class:`str`):
                 Required. Id of the requesting volume If auto-generating
                 Id server-side, remove this field and Id from the
@@ -1199,16 +1183,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Volume` Volume
-                   Volume provides a filesystem that you can mount.
+                The result type for the operation will be
+                :class:`google.cloud.netapp_v1.types.Volume` Volume
+                provides a filesystem that you can mount.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, volume, volume_id])
         if request is not None and has_flattened_params:
@@ -1267,58 +1252,56 @@
         *,
         volume: Optional[gcn_volume.Volume] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""UpdateVolume
-        Updates the parameters of a single Volume.
+        r"""Updates the parameters of a single Volume.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_update_volume():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                volume = netapp_v1beta1.Volume()
+                volume = netapp_v1.Volume()
                 volume.share_name = "share_name_value"
                 volume.storage_pool = "storage_pool_value"
                 volume.capacity_gib = 1247
                 volume.protocols = ['SMB']
 
-                request = netapp_v1beta1.UpdateVolumeRequest(
+                request = netapp_v1.UpdateVolumeRequest(
                     volume=volume,
                 )
 
                 # Make the request
                 operation = client.update_volume(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.UpdateVolumeRequest, dict]]):
-                The request object. UpdateVolumeRequest
-                Message for updating a Volume
-            volume (:class:`google.cloud.netapp_v1beta1.types.Volume`):
+            request (Optional[Union[google.cloud.netapp_v1.types.UpdateVolumeRequest, dict]]):
+                The request object. Message for updating a Volume
+            volume (:class:`google.cloud.netapp_v1.types.Volume`):
                 Required. The volume being updated
                 This corresponds to the ``volume`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Field mask is used to specify the fields to be
                 overwritten in the Volume resource by the update. The
@@ -1336,16 +1319,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Volume` Volume
-                   Volume provides a filesystem that you can mount.
+                The result type for the operation will be
+                :class:`google.cloud.netapp_v1.types.Volume` Volume
+                provides a filesystem that you can mount.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([volume, update_mask])
         if request is not None and has_flattened_params:
@@ -1403,51 +1387,49 @@
         request: Optional[Union[volume.DeleteVolumeRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""DeleteVolume
-        Deletes a single Volume.
+        r"""Deletes a single Volume.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_delete_volume():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteVolumeRequest(
+                request = netapp_v1.DeleteVolumeRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_volume(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.DeleteVolumeRequest, dict]]):
-                The request object. DeleteVolumeRequest
-                Message for deleting a Volume
+            request (Optional[Union[google.cloud.netapp_v1.types.DeleteVolumeRequest, dict]]):
+                The request object. Message for deleting a Volume
             name (:class:`str`):
                 Required. Name of the volume
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1538,22 +1520,22 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_revert_volume():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.RevertVolumeRequest(
+                request = netapp_v1.RevertVolumeRequest(
                     name="name_value",
                     snapshot_id="snapshot_id_value",
                 )
 
                 # Make the request
                 operation = client.revert_volume(request=request)
 
@@ -1561,29 +1543,30 @@
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.RevertVolumeRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.RevertVolumeRequest, dict]]):
                 The request object. RevertVolumeRequest reverts the given
                 volume to the specified snapshot.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Volume` Volume
-                   Volume provides a filesystem that you can mount.
+                The result type for the operation will be
+                :class:`google.cloud.netapp_v1.types.Volume` Volume
+                provides a filesystem that you can mount.
 
         """
         # Create or coerce a protobuf request object.
         request = volume.RevertVolumeRequest(request)
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
@@ -1634,34 +1617,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_list_snapshots():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListSnapshotsRequest(
+                request = netapp_v1.ListSnapshotsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_snapshots(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.ListSnapshotsRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.ListSnapshotsRequest, dict]]):
                 The request object. ListSnapshotsRequest lists snapshots.
             parent (:class:`str`):
                 Required. The volume for which to retrieve snapshot
                 information, in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}``.
 
                 This corresponds to the ``parent`` field
@@ -1670,15 +1653,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListSnapshotsAsyncPager:
+            google.cloud.netapp_v1.services.net_app.pagers.ListSnapshotsAsyncPager:
                 ListSnapshotsResponse is the result
                 of ListSnapshotsRequest.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -1758,33 +1741,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_get_snapshot():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetSnapshotRequest(
+                request = netapp_v1.GetSnapshotRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_snapshot(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.GetSnapshotRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.GetSnapshotRequest, dict]]):
                 The request object. GetSnapshotRequest gets the state of
                 a snapshot.
             name (:class:`str`):
                 Required. The snapshot resource name, in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}/snapshots/{snapshot_id}``
 
                 This corresponds to the ``name`` field
@@ -1793,16 +1776,16 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.Snapshot:
-                Snapshot
+            google.cloud.netapp_v1.types.Snapshot:
+
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
@@ -1869,22 +1852,22 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_create_snapshot():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.CreateSnapshotRequest(
+                request = netapp_v1.CreateSnapshotRequest(
                     parent="parent_value",
                     snapshot_id="snapshot_id_value",
                 )
 
                 # Make the request
                 operation = client.create_snapshot(request=request)
 
@@ -1892,26 +1875,26 @@
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.CreateSnapshotRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.CreateSnapshotRequest, dict]]):
                 The request object. CreateSnapshotRequest creates a
                 snapshot.
             parent (:class:`str`):
                 Required. The NetApp volume to create the snapshots of,
                 in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            snapshot (:class:`google.cloud.netapp_v1beta1.types.Snapshot`):
+            snapshot (:class:`google.cloud.netapp_v1.types.Snapshot`):
                 Required. A snapshot resource
                 This corresponds to the ``snapshot`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             snapshot_id (:class:`str`):
                 Required. ID of the snapshot to
                 create. This value must start with a
@@ -1929,16 +1912,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.Snapshot`
-                Snapshot
+                :class:`google.cloud.netapp_v1.types.Snapshot`
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, snapshot, snapshot_id])
         if request is not None and has_flattened_params:
@@ -2007,37 +1989,37 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_delete_snapshot():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteSnapshotRequest(
+                request = netapp_v1.DeleteSnapshotRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_snapshot(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.DeleteSnapshotRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.DeleteSnapshotRequest, dict]]):
                 The request object. DeleteSnapshotRequest deletes a
                 snapshot.
             name (:class:`str`):
                 Required. The snapshot resource name, in the format
                 ``projects/*/locations/*/volumes/*/snapshots/{snapshot_id}``
 
                 This corresponds to the ``name`` field
@@ -2132,40 +2114,40 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_update_snapshot():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.UpdateSnapshotRequest(
+                request = netapp_v1.UpdateSnapshotRequest(
                 )
 
                 # Make the request
                 operation = client.update_snapshot(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.UpdateSnapshotRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.UpdateSnapshotRequest, dict]]):
                 The request object. UpdateSnapshotRequest updates
                 description and/or labels for a
                 snapshot.
-            snapshot (:class:`google.cloud.netapp_v1beta1.types.Snapshot`):
+            snapshot (:class:`google.cloud.netapp_v1.types.Snapshot`):
                 Required. A snapshot resource
                 This corresponds to the ``snapshot`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Mask of fields to update.
                 At least one path must be supplied in
@@ -2181,16 +2163,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.Snapshot`
-                Snapshot
+                :class:`google.cloud.netapp_v1.types.Snapshot`
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([snapshot, update_mask])
         if request is not None and has_flattened_params:
@@ -2250,46 +2231,45 @@
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListActiveDirectoriesAsyncPager:
-        r"""ListActiveDirectories
-        Lists active directories.
+        r"""Lists active directories.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_list_active_directories():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListActiveDirectoriesRequest(
+                request = netapp_v1.ListActiveDirectoriesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_active_directories(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.ListActiveDirectoriesRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.ListActiveDirectoriesRequest, dict]]):
                 The request object. ListActiveDirectoriesRequest for
                 requesting multiple active directories.
             parent (:class:`str`):
                 Required. Parent value for
                 ListActiveDirectoriesRequest
 
                 This corresponds to the ``parent`` field
@@ -2298,15 +2278,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListActiveDirectoriesAsyncPager:
+            google.cloud.netapp_v1.services.net_app.pagers.ListActiveDirectoriesAsyncPager:
                 ListActiveDirectoriesResponse
                 contains all the active directories
                 requested.  Iterating over this object
                 will yield results and resolve
                 additional pages automatically.
 
         """
@@ -2377,45 +2357,44 @@
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> active_directory.ActiveDirectory:
-        r"""DescribeActiveDirectory
-        Describes a specified active directory.
+        r"""Describes a specified active directory.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_get_active_directory():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetActiveDirectoryRequest(
+                request = netapp_v1.GetActiveDirectoryRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_active_directory(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.GetActiveDirectoryRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.GetActiveDirectoryRequest, dict]]):
                 The request object. GetActiveDirectory for getting a
                 single active directory.
             name (:class:`str`):
                 Required. Name of the active
                 directory.
 
                 This corresponds to the ``name`` field
@@ -2424,15 +2403,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.ActiveDirectory:
+            google.cloud.netapp_v1.types.ActiveDirectory:
                 ActiveDirectory is the public
                 representation of the active directory
                 config.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -2506,29 +2485,29 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_create_active_directory():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                active_directory = netapp_v1beta1.ActiveDirectory()
+                active_directory = netapp_v1.ActiveDirectory()
                 active_directory.domain = "domain_value"
                 active_directory.dns = "dns_value"
                 active_directory.net_bios_prefix = "net_bios_prefix_value"
                 active_directory.username = "username_value"
                 active_directory.password = "password_value"
 
-                request = netapp_v1beta1.CreateActiveDirectoryRequest(
+                request = netapp_v1.CreateActiveDirectoryRequest(
                     parent="parent_value",
                     active_directory=active_directory,
                     active_directory_id="active_directory_id_value",
                 )
 
                 # Make the request
                 operation = client.create_active_directory(request=request)
@@ -2537,23 +2516,23 @@
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.CreateActiveDirectoryRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.CreateActiveDirectoryRequest, dict]]):
                 The request object. CreateActiveDirectoryRequest for
                 creating an active directory.
             parent (:class:`str`):
                 Required. Value for parent.
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            active_directory (:class:`google.cloud.netapp_v1beta1.types.ActiveDirectory`):
+            active_directory (:class:`google.cloud.netapp_v1.types.ActiveDirectory`):
                 Required. Fields of the to be created
                 active directory.
 
                 This corresponds to the ``active_directory`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             active_directory_id (:class:`str`):
@@ -2570,15 +2549,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.ActiveDirectory`
+                :class:`google.cloud.netapp_v1.types.ActiveDirectory`
                 ActiveDirectory is the public representation of the
                 active directory config.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -2641,59 +2620,58 @@
         *,
         active_directory: Optional[gcn_active_directory.ActiveDirectory] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""UpdateActiveDirectory
-        Update the parameters of an active directories.
+        r"""Update the parameters of an active directories.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_update_active_directory():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                active_directory = netapp_v1beta1.ActiveDirectory()
+                active_directory = netapp_v1.ActiveDirectory()
                 active_directory.domain = "domain_value"
                 active_directory.dns = "dns_value"
                 active_directory.net_bios_prefix = "net_bios_prefix_value"
                 active_directory.username = "username_value"
                 active_directory.password = "password_value"
 
-                request = netapp_v1beta1.UpdateActiveDirectoryRequest(
+                request = netapp_v1.UpdateActiveDirectoryRequest(
                     active_directory=active_directory,
                 )
 
                 # Make the request
                 operation = client.update_active_directory(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.UpdateActiveDirectoryRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.UpdateActiveDirectoryRequest, dict]]):
                 The request object. UpdateActiveDirectoryRequest for
                 updating an active directory.
-            active_directory (:class:`google.cloud.netapp_v1beta1.types.ActiveDirectory`):
+            active_directory (:class:`google.cloud.netapp_v1.types.ActiveDirectory`):
                 Required. The volume being updated
                 This corresponds to the ``active_directory`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Field mask is used to specify the fields to be
                 overwritten in the Active Directory resource by the
@@ -2713,15 +2691,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.ActiveDirectory`
+                :class:`google.cloud.netapp_v1.types.ActiveDirectory`
                 ActiveDirectory is the public representation of the
                 active directory config.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -2783,49 +2761,48 @@
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""DeleteActiveDirectory
-        Delete the active directory specified in the request.
+        r"""Delete the active directory specified in the request.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_delete_active_directory():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteActiveDirectoryRequest(
+                request = netapp_v1.DeleteActiveDirectoryRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_active_directory(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.DeleteActiveDirectoryRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.DeleteActiveDirectoryRequest, dict]]):
                 The request object. DeleteActiveDirectoryRequest for
                 deleting a single active directory.
             name (:class:`str`):
                 Required. Name of the active
                 directory.
 
                 This corresponds to the ``name`` field
@@ -2908,62 +2885,60 @@
         request: Optional[Union[kms.ListKmsConfigsRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListKmsConfigsAsyncPager:
-        r"""ListKmsConfigs
-        Returns descriptions of all KMS configs owned by the
+        r"""Returns descriptions of all KMS configs owned by the
         caller.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_list_kms_configs():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListKmsConfigsRequest(
+                request = netapp_v1.ListKmsConfigsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_kms_configs(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.ListKmsConfigsRequest, dict]]):
-                The request object. ListKmsConfigsRequest
+            request (Optional[Union[google.cloud.netapp_v1.types.ListKmsConfigsRequest, dict]]):
+                The request object.
             parent (:class:`str`):
                 Required. Parent value
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListKmsConfigsAsyncPager:
-                ListKmsConfigsResponse
+            google.cloud.netapp_v1.services.net_app.pagers.ListKmsConfigsAsyncPager:
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -3032,37 +3007,36 @@
         parent: Optional[str] = None,
         kms_config: Optional[kms.KmsConfig] = None,
         kms_config_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""CreateKmsConfig
-        Creates a new KMS config.
+        r"""Creates a new KMS config.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_create_kms_config():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                kms_config = netapp_v1beta1.KmsConfig()
+                kms_config = netapp_v1.KmsConfig()
                 kms_config.crypto_key_name = "crypto_key_name_value"
 
-                request = netapp_v1beta1.CreateKmsConfigRequest(
+                request = netapp_v1.CreateKmsConfigRequest(
                     parent="parent_value",
                     kms_config_id="kms_config_id_value",
                     kms_config=kms_config,
                 )
 
                 # Make the request
                 operation = client.create_kms_config(request=request)
@@ -3071,22 +3045,22 @@
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.CreateKmsConfigRequest, dict]]):
-                The request object. CreateKmsConfigRequest
+            request (Optional[Union[google.cloud.netapp_v1.types.CreateKmsConfigRequest, dict]]):
+                The request object.
             parent (:class:`str`):
                 Required. Value for parent.
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            kms_config (:class:`google.cloud.netapp_v1beta1.types.KmsConfig`):
+            kms_config (:class:`google.cloud.netapp_v1.types.KmsConfig`):
                 Required. The required parameters to
                 create a new KmsConfig.
 
                 This corresponds to the ``kms_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             kms_config_id (:class:`str`):
@@ -3104,15 +3078,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.KmsConfig`
+                :class:`google.cloud.netapp_v1.types.KmsConfig`
                 KmsConfig is the customer managed encryption key(CMEK)
                 configuration.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -3172,59 +3146,59 @@
         request: Optional[Union[kms.GetKmsConfigRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> kms.KmsConfig:
-        r"""GetKmsConfig Returns the description of the specified KMS config
-        by kms_config_id.
+        r"""Returns the description of the specified KMS config by
+        kms_config_id.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_get_kms_config():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetKmsConfigRequest(
+                request = netapp_v1.GetKmsConfigRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_kms_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.GetKmsConfigRequest, dict]]):
-                The request object. GetKmsConfigRequest
+            request (Optional[Union[google.cloud.netapp_v1.types.GetKmsConfigRequest, dict]]):
+                The request object.
             name (:class:`str`):
                 Required. Name of the KmsConfig
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.KmsConfig:
+            google.cloud.netapp_v1.types.KmsConfig:
                 KmsConfig is the customer managed
                 encryption key(CMEK) configuration.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -3282,54 +3256,53 @@
         *,
         kms_config: Optional[kms.KmsConfig] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""UpdateKmsConfig
-        Updates the Kms config properties with the full spec
+        r"""Updates the Kms config properties with the full spec
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_update_kms_config():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                kms_config = netapp_v1beta1.KmsConfig()
+                kms_config = netapp_v1.KmsConfig()
                 kms_config.crypto_key_name = "crypto_key_name_value"
 
-                request = netapp_v1beta1.UpdateKmsConfigRequest(
+                request = netapp_v1.UpdateKmsConfigRequest(
                     kms_config=kms_config,
                 )
 
                 # Make the request
                 operation = client.update_kms_config(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.UpdateKmsConfigRequest, dict]]):
-                The request object. UpdateKmsConfigRequest
-            kms_config (:class:`google.cloud.netapp_v1beta1.types.KmsConfig`):
+            request (Optional[Union[google.cloud.netapp_v1.types.UpdateKmsConfigRequest, dict]]):
+                The request object.
+            kms_config (:class:`google.cloud.netapp_v1.types.KmsConfig`):
                 Required. The KmsConfig being updated
                 This corresponds to the ``kms_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Field mask is used to specify the fields to be
                 overwritten in the KmsConfig resource by the update. The
@@ -3348,15 +3321,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.KmsConfig`
+                :class:`google.cloud.netapp_v1.types.KmsConfig`
                 KmsConfig is the customer managed encryption key(CMEK)
                 configuration.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -3415,65 +3388,63 @@
         self,
         request: Optional[Union[kms.EncryptVolumesRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""EncryptVolumes
-        Encrypt the existing volumes without CMEK encryption
+        r"""Encrypt the existing volumes without CMEK encryption
         with the desired the KMS config for the whole region.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_encrypt_volumes():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.EncryptVolumesRequest(
+                request = netapp_v1.EncryptVolumesRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.encrypt_volumes(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.EncryptVolumesRequest, dict]]):
-                The request object. EncryptVolumesRequest
-                EncryptVolumesRequest specifies the KMS
-                config to encrypt existing volumes.
+            request (Optional[Union[google.cloud.netapp_v1.types.EncryptVolumesRequest, dict]]):
+                The request object. EncryptVolumesRequest specifies the
+                KMS config to encrypt existing volumes.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.KmsConfig`
+                :class:`google.cloud.netapp_v1.types.KmsConfig`
                 KmsConfig is the customer managed encryption key(CMEK)
                 configuration.
 
         """
         # Create or coerce a protobuf request object.
         request = kms.EncryptVolumesRequest(request)
 
@@ -3514,57 +3485,54 @@
         self,
         request: Optional[Union[kms.VerifyKmsConfigRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> kms.VerifyKmsConfigResponse:
-        r"""VerifyKmsConfigRequest
-        Verifies KMS config reachability.
+        r"""Verifies KMS config reachability.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_verify_kms_config():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.VerifyKmsConfigRequest(
+                request = netapp_v1.VerifyKmsConfigRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.verify_kms_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.VerifyKmsConfigRequest, dict]]):
-                The request object. VerifyKmsConfigRequest
-                VerifyKmsConfigRequest specifies the KMS
-                config to be validated.
+            request (Optional[Union[google.cloud.netapp_v1.types.VerifyKmsConfigRequest, dict]]):
+                The request object. VerifyKmsConfigRequest specifies the
+                KMS config to be validated.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.VerifyKmsConfigResponse:
-                VerifyKmsConfigResponse
+            google.cloud.netapp_v1.types.VerifyKmsConfigResponse:
                 VerifyKmsConfigResponse contains the
                 information if the config is correctly
                 and error message.
 
         """
         # Create or coerce a protobuf request object.
         request = kms.VerifyKmsConfigRequest(request)
@@ -3599,51 +3567,50 @@
         request: Optional[Union[kms.DeleteKmsConfigRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""DeleteKmsConfig
-        Warning! This operation will permanently delete the Kms
-        config.
+        r"""Warning! This operation will permanently delete the
+        Kms config.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_delete_kms_config():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteKmsConfigRequest(
+                request = netapp_v1.DeleteKmsConfigRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_kms_config(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.DeleteKmsConfigRequest, dict]]):
-                The request object. DeleteKmsConfigRequest
+            request (Optional[Union[google.cloud.netapp_v1.types.DeleteKmsConfigRequest, dict]]):
+                The request object.
             name (:class:`str`):
                 Required. Name of the KmsConfig.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -3734,34 +3701,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_list_replications():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListReplicationsRequest(
+                request = netapp_v1.ListReplicationsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_replications(request=request)
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.ListReplicationsRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.ListReplicationsRequest, dict]]):
                 The request object. ListReplications lists replications.
             parent (:class:`str`):
                 Required. The volume for which to retrieve replication
                 information, in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}``.
 
                 This corresponds to the ``parent`` field
@@ -3770,15 +3737,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListReplicationsAsyncPager:
+            google.cloud.netapp_v1.services.net_app.pagers.ListReplicationsAsyncPager:
                 ListReplicationsResponse is the
                 result of ListReplicationsRequest.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -3858,33 +3825,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_get_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetReplicationRequest(
+                request = netapp_v1.GetReplicationRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = await client.get_replication(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.GetReplicationRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.GetReplicationRequest, dict]]):
                 The request object. GetReplicationRequest gets the state
                 of a replication.
             name (:class:`str`):
                 Required. The replication resource name, in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}/replications/{replication_id}``
 
                 This corresponds to the ``name`` field
@@ -3893,15 +3860,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.Replication:
+            google.cloud.netapp_v1.types.Replication:
                 Replication is a nested resource
                 under Volume, that describes a
                 cross-region replication relationship
                 between 2 volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
@@ -3973,26 +3940,26 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_create_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                replication = netapp_v1beta1.Replication()
+                replication = netapp_v1.Replication()
                 replication.replication_schedule = "DAILY"
                 replication.destination_volume_parameters.storage_pool = "storage_pool_value"
 
-                request = netapp_v1beta1.CreateReplicationRequest(
+                request = netapp_v1.CreateReplicationRequest(
                     parent="parent_value",
                     replication=replication,
                     replication_id="replication_id_value",
                 )
 
                 # Make the request
                 operation = client.create_replication(request=request)
@@ -4001,26 +3968,26 @@
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.CreateReplicationRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.CreateReplicationRequest, dict]]):
                 The request object. CreateReplicationRequest creates a
                 replication.
             parent (:class:`str`):
                 Required. The NetApp volume to create the replications
                 of, in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            replication (:class:`google.cloud.netapp_v1beta1.types.Replication`):
+            replication (:class:`google.cloud.netapp_v1.types.Replication`):
                 Required. A replication resource
                 This corresponds to the ``replication`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             replication_id (:class:`str`):
                 Required. ID of the replication to
                 create. This value must start with a
@@ -4037,15 +4004,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Replication` Replication is a nested resource under Volume, that describes a
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.Replication` Replication is a nested resource under Volume, that describes a
                    cross-region replication relationship between 2
                    volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -4116,37 +4083,37 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_delete_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteReplicationRequest(
+                request = netapp_v1.DeleteReplicationRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_replication(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.DeleteReplicationRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.DeleteReplicationRequest, dict]]):
                 The request object. DeleteReplicationRequest deletes a
                 replication.
             name (:class:`str`):
                 Required. The replication resource name, in the format
                 ``projects/*/locations/*/volumes/*/replications/{replication_id}``
 
                 This corresponds to the ``name`` field
@@ -4241,45 +4208,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_update_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                replication = netapp_v1beta1.Replication()
+                replication = netapp_v1.Replication()
                 replication.replication_schedule = "DAILY"
                 replication.destination_volume_parameters.storage_pool = "storage_pool_value"
 
-                request = netapp_v1beta1.UpdateReplicationRequest(
+                request = netapp_v1.UpdateReplicationRequest(
                     replication=replication,
                 )
 
                 # Make the request
                 operation = client.update_replication(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.UpdateReplicationRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.UpdateReplicationRequest, dict]]):
                 The request object. UpdateReplicationRequest updates
                 description and/or labels for a
                 replication.
-            replication (:class:`google.cloud.netapp_v1beta1.types.Replication`):
+            replication (:class:`google.cloud.netapp_v1.types.Replication`):
                 Required. A replication resource
                 This corresponds to the ``replication`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Mask of fields to update.
                 At least one path must be supplied in
@@ -4294,15 +4261,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Replication` Replication is a nested resource under Volume, that describes a
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.Replication` Replication is a nested resource under Volume, that describes a
                    cross-region replication relationship between 2
                    volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -4372,50 +4339,50 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_stop_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.StopReplicationRequest(
+                request = netapp_v1.StopReplicationRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.stop_replication(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.StopReplicationRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.StopReplicationRequest, dict]]):
                 The request object. StopReplicationRequest stops a
                 replication until resumed.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Replication` Replication is a nested resource under Volume, that describes a
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.Replication` Replication is a nested resource under Volume, that describes a
                    cross-region replication relationship between 2
                    volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
         request = replication.StopReplicationRequest(request)
 
@@ -4467,50 +4434,50 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_resume_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ResumeReplicationRequest(
+                request = netapp_v1.ResumeReplicationRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.resume_replication(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.ResumeReplicationRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.ResumeReplicationRequest, dict]]):
                 The request object. ResumeReplicationRequest resumes a
                 stopped replication.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Replication` Replication is a nested resource under Volume, that describes a
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.Replication` Replication is a nested resource under Volume, that describes a
                    cross-region replication relationship between 2
                    volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
         request = replication.ResumeReplicationRequest(request)
 
@@ -4553,65 +4520,64 @@
             Union[replication.ReverseReplicationDirectionRequest, dict]
         ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""ReverseReplicationDirection reverses direction of
-        replication. Source becomes destination and destination
-        becomes source.
+        r"""Reverses direction of replication. Source becomes
+        destination and destination becomes source.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             async def sample_reverse_replication_direction():
                 # Create a client
-                client = netapp_v1beta1.NetAppAsyncClient()
+                client = netapp_v1.NetAppAsyncClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ReverseReplicationDirectionRequest(
+                request = netapp_v1.ReverseReplicationDirectionRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.reverse_replication_direction(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = (await operation).result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Optional[Union[google.cloud.netapp_v1beta1.types.ReverseReplicationDirectionRequest, dict]]):
+            request (Optional[Union[google.cloud.netapp_v1.types.ReverseReplicationDirectionRequest, dict]]):
                 The request object. ReverseReplicationDirectionRequest
                 reverses direction of replication.
                 Source becomes destination and
                 destination becomes source.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Replication` Replication is a nested resource under Volume, that describes a
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.Replication` Replication is a nested resource under Volume, that describes a
                    cross-region replication relationship between 2
                    volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
         request = replication.ReverseReplicationDirectionRequest(request)
 
@@ -4644,339 +4610,14 @@
             replication.Replication,
             metadata_type=cloud_netapp_service.OperationMetadata,
         )
 
         # Done; return the response.
         return response
 
-    async def list_operations(
-        self,
-        request: Optional[operations_pb2.ListOperationsRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> operations_pb2.ListOperationsResponse:
-        r"""Lists operations that match the specified filter in the request.
-
-        Args:
-            request (:class:`~.operations_pb2.ListOperationsRequest`):
-                The request object. Request message for
-                `ListOperations` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                    if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            ~.operations_pb2.ListOperationsResponse:
-                Response message for ``ListOperations`` method.
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = operations_pb2.ListOperationsRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._client._transport.list_operations,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        response = await rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-        # Done; return the response.
-        return response
-
-    async def get_operation(
-        self,
-        request: Optional[operations_pb2.GetOperationRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> operations_pb2.Operation:
-        r"""Gets the latest state of a long-running operation.
-
-        Args:
-            request (:class:`~.operations_pb2.GetOperationRequest`):
-                The request object. Request message for
-                `GetOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                    if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            ~.operations_pb2.Operation:
-                An ``Operation`` object.
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = operations_pb2.GetOperationRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._client._transport.get_operation,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        response = await rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-        # Done; return the response.
-        return response
-
-    async def delete_operation(
-        self,
-        request: Optional[operations_pb2.DeleteOperationRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> None:
-        r"""Deletes a long-running operation.
-
-        This method indicates that the client is no longer interested
-        in the operation result. It does not cancel the operation.
-        If the server doesn't support this method, it returns
-        `google.rpc.Code.UNIMPLEMENTED`.
-
-        Args:
-            request (:class:`~.operations_pb2.DeleteOperationRequest`):
-                The request object. Request message for
-                `DeleteOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                    if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            None
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = operations_pb2.DeleteOperationRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._client._transport.delete_operation,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        await rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-    async def cancel_operation(
-        self,
-        request: Optional[operations_pb2.CancelOperationRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> None:
-        r"""Starts asynchronous cancellation on a long-running operation.
-
-        The server makes a best effort to cancel the operation, but success
-        is not guaranteed.  If the server doesn't support this method, it returns
-        `google.rpc.Code.UNIMPLEMENTED`.
-
-        Args:
-            request (:class:`~.operations_pb2.CancelOperationRequest`):
-                The request object. Request message for
-                `CancelOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                    if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            None
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = operations_pb2.CancelOperationRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._client._transport.cancel_operation,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        await rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-    async def get_location(
-        self,
-        request: Optional[locations_pb2.GetLocationRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> locations_pb2.Location:
-        r"""Gets information about a location.
-
-        Args:
-            request (:class:`~.location_pb2.GetLocationRequest`):
-                The request object. Request message for
-                `GetLocation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                 if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            ~.location_pb2.Location:
-                Location object.
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = locations_pb2.GetLocationRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._client._transport.get_location,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        response = await rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-        # Done; return the response.
-        return response
-
-    async def list_locations(
-        self,
-        request: Optional[locations_pb2.ListLocationsRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> locations_pb2.ListLocationsResponse:
-        r"""Lists information about the supported locations for this service.
-
-        Args:
-            request (:class:`~.location_pb2.ListLocationsRequest`):
-                The request object. Request message for
-                `ListLocations` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                 if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            ~.location_pb2.ListLocationsResponse:
-                Response message for ``ListLocations`` method.
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = locations_pb2.ListLocationsRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._client._transport.list_locations,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        response = await rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-        # Done; return the response.
-        return response
-
     async def __aenter__(self) -> "NetAppAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/client.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,41 +35,41 @@
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.exceptions import MutualTLSChannelError  # type: ignore
 from google.auth.transport import mtls  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.netapp_v1beta1 import gapic_version as package_version
+from google.cloud.netapp_v1 import gapic_version as package_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
 from google.cloud.location import locations_pb2  # type: ignore
 from google.longrunning import operations_pb2
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
-from google.cloud.netapp_v1beta1.services.net_app import pagers
-from google.cloud.netapp_v1beta1.types import active_directory as gcn_active_directory
-from google.cloud.netapp_v1beta1.types import active_directory
-from google.cloud.netapp_v1beta1.types import cloud_netapp_service, common, kms
-from google.cloud.netapp_v1beta1.types import replication
-from google.cloud.netapp_v1beta1.types import replication as gcn_replication
-from google.cloud.netapp_v1beta1.types import snapshot
-from google.cloud.netapp_v1beta1.types import snapshot as gcn_snapshot
-from google.cloud.netapp_v1beta1.types import storage_pool
-from google.cloud.netapp_v1beta1.types import storage_pool as gcn_storage_pool
-from google.cloud.netapp_v1beta1.types import volume
-from google.cloud.netapp_v1beta1.types import volume as gcn_volume
+from google.cloud.netapp_v1.services.net_app import pagers
+from google.cloud.netapp_v1.types import active_directory as gcn_active_directory
+from google.cloud.netapp_v1.types import active_directory
+from google.cloud.netapp_v1.types import cloud_netapp_service, common, kms
+from google.cloud.netapp_v1.types import replication
+from google.cloud.netapp_v1.types import replication as gcn_replication
+from google.cloud.netapp_v1.types import snapshot
+from google.cloud.netapp_v1.types import snapshot as gcn_snapshot
+from google.cloud.netapp_v1.types import storage_pool
+from google.cloud.netapp_v1.types import storage_pool as gcn_storage_pool
+from google.cloud.netapp_v1.types import volume
+from google.cloud.netapp_v1.types import volume as gcn_volume
 
 from .transports.base import DEFAULT_CLIENT_INFO, NetAppTransport
 from .transports.grpc import NetAppGrpcTransport
 from .transports.grpc_asyncio import NetAppGrpcAsyncIOTransport
 from .transports.rest import NetAppRestTransport
 
 
@@ -597,62 +597,60 @@
         request: Optional[Union[storage_pool.ListStoragePoolsRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListStoragePoolsPager:
-        r"""ListStoragePools
-        Returns descriptions of all storage pools owned by the
-        caller.
+        r"""Returns descriptions of all storage pools owned by
+        the caller.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_list_storage_pools():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListStoragePoolsRequest(
+                request = netapp_v1.ListStoragePoolsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_storage_pools(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.ListStoragePoolsRequest, dict]):
-                The request object. ListStoragePoolsRequest
+            request (Union[google.cloud.netapp_v1.types.ListStoragePoolsRequest, dict]):
+                The request object.
             parent (str):
                 Required. Parent value
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListStoragePoolsPager:
-                ListStoragePoolsResponse
+            google.cloud.netapp_v1.services.net_app.pagers.ListStoragePoolsPager:
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -714,39 +712,38 @@
         parent: Optional[str] = None,
         storage_pool: Optional[gcn_storage_pool.StoragePool] = None,
         storage_pool_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""CreateStoragePool
-        Creates a new storage pool.
+        r"""Creates a new storage pool.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_create_storage_pool():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                storage_pool = netapp_v1beta1.StoragePool()
+                storage_pool = netapp_v1.StoragePool()
                 storage_pool.service_level = "STANDARD"
                 storage_pool.capacity_gib = 1247
                 storage_pool.network = "network_value"
 
-                request = netapp_v1beta1.CreateStoragePoolRequest(
+                request = netapp_v1.CreateStoragePoolRequest(
                     parent="parent_value",
                     storage_pool_id="storage_pool_id_value",
                     storage_pool=storage_pool,
                 )
 
                 # Make the request
                 operation = client.create_storage_pool(request=request)
@@ -755,22 +752,22 @@
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.CreateStoragePoolRequest, dict]):
-                The request object. CreateStoragePoolRequest
+            request (Union[google.cloud.netapp_v1.types.CreateStoragePoolRequest, dict]):
+                The request object.
             parent (str):
                 Required. Value for parent.
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            storage_pool (google.cloud.netapp_v1beta1.types.StoragePool):
+            storage_pool (google.cloud.netapp_v1.types.StoragePool):
                 Required. The required parameters to
                 create a new storage pool.
 
                 This corresponds to the ``storage_pool`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             storage_pool_id (str):
@@ -787,19 +784,18 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.StoragePool` Resources
-                   StoragePool StoragePool is a container for volumes
-                   with a service level and capacity. Volumes can be
-                   created in a pool of sufficient available capacity.
-                   StoragePool capacity is what you are billed for.
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.StoragePool` StoragePool is a container for volumes with a service level and capacity.
+                   Volumes can be created in a pool of sufficient
+                   available capacity. StoragePool capacity is what you
+                   are billed for.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, storage_pool, storage_pool_id])
         if request is not None and has_flattened_params:
@@ -857,66 +853,63 @@
         request: Optional[Union[storage_pool.GetStoragePoolRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> storage_pool.StoragePool:
-        r"""GetStoragePool
-        Returns the description of the specified storage pool by
-        poolId.
+        r"""Returns the description of the specified storage pool
+        by poolId.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_get_storage_pool():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetStoragePoolRequest(
+                request = netapp_v1.GetStoragePoolRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_storage_pool(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.GetStoragePoolRequest, dict]):
-                The request object. GetStoragePoolRequest
+            request (Union[google.cloud.netapp_v1.types.GetStoragePoolRequest, dict]):
+                The request object.
             name (str):
                 Required. Name of the storage pool
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.StoragePool:
-                Resources
-                StoragePool
-                StoragePool is a container for volumes
-                with a service level and capacity.
-                Volumes can be created in a pool of
-                sufficient available capacity.
+            google.cloud.netapp_v1.types.StoragePool:
+                StoragePool is a container for
+                volumes with a service level and
+                capacity. Volumes can be created in a
+                pool of sufficient available capacity.
                 StoragePool capacity is what you are
                 billed for.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -967,56 +960,56 @@
         *,
         storage_pool: Optional[gcn_storage_pool.StoragePool] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""UpdateStoragePool
-        Updates the storage pool properties with the full spec
+        r"""Updates the storage pool properties with the full
+        spec
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_update_storage_pool():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                storage_pool = netapp_v1beta1.StoragePool()
+                storage_pool = netapp_v1.StoragePool()
                 storage_pool.service_level = "STANDARD"
                 storage_pool.capacity_gib = 1247
                 storage_pool.network = "network_value"
 
-                request = netapp_v1beta1.UpdateStoragePoolRequest(
+                request = netapp_v1.UpdateStoragePoolRequest(
                     storage_pool=storage_pool,
                 )
 
                 # Make the request
                 operation = client.update_storage_pool(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.UpdateStoragePoolRequest, dict]):
-                The request object. UpdateStoragePoolRequest
-            storage_pool (google.cloud.netapp_v1beta1.types.StoragePool):
+            request (Union[google.cloud.netapp_v1.types.UpdateStoragePoolRequest, dict]):
+                The request object.
+            storage_pool (google.cloud.netapp_v1.types.StoragePool):
                 Required. The pool being updated
                 This corresponds to the ``storage_pool`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Field mask is used to specify the fields to be
                 overwritten in the StoragePool resource by the update.
@@ -1034,19 +1027,18 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.StoragePool` Resources
-                   StoragePool StoragePool is a container for volumes
-                   with a service level and capacity. Volumes can be
-                   created in a pool of sufficient available capacity.
-                   StoragePool capacity is what you are billed for.
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.StoragePool` StoragePool is a container for volumes with a service level and capacity.
+                   Volumes can be created in a pool of sufficient
+                   available capacity. StoragePool capacity is what you
+                   are billed for.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([storage_pool, update_mask])
         if request is not None and has_flattened_params:
@@ -1104,51 +1096,50 @@
         request: Optional[Union[storage_pool.DeleteStoragePoolRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""DeleteStoragePool
-        Warning! This operation will permanently delete the
+        r"""Warning! This operation will permanently delete the
         storage pool.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_delete_storage_pool():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteStoragePoolRequest(
+                request = netapp_v1.DeleteStoragePoolRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_storage_pool(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.DeleteStoragePoolRequest, dict]):
-                The request object. DeleteStoragePoolRequest
+            request (Union[google.cloud.netapp_v1.types.DeleteStoragePoolRequest, dict]):
+                The request object.
             name (str):
                 Required. Name of the storage pool
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1227,66 +1218,64 @@
         request: Optional[Union[volume.ListVolumesRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListVolumesPager:
-        r"""ListVolumes
-        Lists Volumes in a given project.
+        r"""Lists Volumes in a given project.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_list_volumes():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListVolumesRequest(
+                request = netapp_v1.ListVolumesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_volumes(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.ListVolumesRequest, dict]):
-                The request object. ListVolumesRequest
-                Message for requesting list of Volumes
+            request (Union[google.cloud.netapp_v1.types.ListVolumesRequest, dict]):
+                The request object. Message for requesting list of
+                Volumes
             parent (str):
                 Required. Parent value for
                 ListVolumesRequest
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListVolumesPager:
-                ListVolumesResponse
-                Message for response to listing Volumes
-
+            google.cloud.netapp_v1.services.net_app.pagers.ListVolumesPager:
+                Message for response to listing
+                Volumes
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -1344,61 +1333,58 @@
         request: Optional[Union[volume.GetVolumeRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> volume.Volume:
-        r"""GetVolume
-        Gets details of a single Volume.
+        r"""Gets details of a single Volume.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_get_volume():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetVolumeRequest(
+                request = netapp_v1.GetVolumeRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_volume(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.GetVolumeRequest, dict]):
-                The request object. GetVolumeRequest
-                Message for getting a Volume
+            request (Union[google.cloud.netapp_v1.types.GetVolumeRequest, dict]):
+                The request object. Message for getting a Volume
             name (str):
                 Required. Name of the volume
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.Volume:
-                Volume
+            google.cloud.netapp_v1.types.Volume:
                 Volume provides a filesystem that you
                 can mount.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -1448,40 +1434,39 @@
         parent: Optional[str] = None,
         volume: Optional[gcn_volume.Volume] = None,
         volume_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""CreateVolume
-        Creates a new Volume in a given project and location.
+        r"""Creates a new Volume in a given project and location.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_create_volume():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                volume = netapp_v1beta1.Volume()
+                volume = netapp_v1.Volume()
                 volume.share_name = "share_name_value"
                 volume.storage_pool = "storage_pool_value"
                 volume.capacity_gib = 1247
                 volume.protocols = ['SMB']
 
-                request = netapp_v1beta1.CreateVolumeRequest(
+                request = netapp_v1.CreateVolumeRequest(
                     parent="parent_value",
                     volume_id="volume_id_value",
                     volume=volume,
                 )
 
                 # Make the request
                 operation = client.create_volume(request=request)
@@ -1490,23 +1475,22 @@
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.CreateVolumeRequest, dict]):
-                The request object. CreateVolumeRequest
-                Message for creating a Volume
+            request (Union[google.cloud.netapp_v1.types.CreateVolumeRequest, dict]):
+                The request object. Message for creating a Volume
             parent (str):
                 Required. Value for parent.
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            volume (google.cloud.netapp_v1beta1.types.Volume):
+            volume (google.cloud.netapp_v1.types.Volume):
                 Required. The volume being created.
                 This corresponds to the ``volume`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             volume_id (str):
                 Required. Id of the requesting volume If auto-generating
                 Id server-side, remove this field and Id from the
@@ -1521,16 +1505,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Volume` Volume
-                   Volume provides a filesystem that you can mount.
+                The result type for the operation will be
+                :class:`google.cloud.netapp_v1.types.Volume` Volume
+                provides a filesystem that you can mount.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, volume, volume_id])
         if request is not None and has_flattened_params:
@@ -1589,58 +1574,56 @@
         *,
         volume: Optional[gcn_volume.Volume] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""UpdateVolume
-        Updates the parameters of a single Volume.
+        r"""Updates the parameters of a single Volume.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_update_volume():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                volume = netapp_v1beta1.Volume()
+                volume = netapp_v1.Volume()
                 volume.share_name = "share_name_value"
                 volume.storage_pool = "storage_pool_value"
                 volume.capacity_gib = 1247
                 volume.protocols = ['SMB']
 
-                request = netapp_v1beta1.UpdateVolumeRequest(
+                request = netapp_v1.UpdateVolumeRequest(
                     volume=volume,
                 )
 
                 # Make the request
                 operation = client.update_volume(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.UpdateVolumeRequest, dict]):
-                The request object. UpdateVolumeRequest
-                Message for updating a Volume
-            volume (google.cloud.netapp_v1beta1.types.Volume):
+            request (Union[google.cloud.netapp_v1.types.UpdateVolumeRequest, dict]):
+                The request object. Message for updating a Volume
+            volume (google.cloud.netapp_v1.types.Volume):
                 Required. The volume being updated
                 This corresponds to the ``volume`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Field mask is used to specify the fields to be
                 overwritten in the Volume resource by the update. The
@@ -1658,16 +1641,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Volume` Volume
-                   Volume provides a filesystem that you can mount.
+                The result type for the operation will be
+                :class:`google.cloud.netapp_v1.types.Volume` Volume
+                provides a filesystem that you can mount.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([volume, update_mask])
         if request is not None and has_flattened_params:
@@ -1725,51 +1709,49 @@
         request: Optional[Union[volume.DeleteVolumeRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""DeleteVolume
-        Deletes a single Volume.
+        r"""Deletes a single Volume.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_delete_volume():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteVolumeRequest(
+                request = netapp_v1.DeleteVolumeRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_volume(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.DeleteVolumeRequest, dict]):
-                The request object. DeleteVolumeRequest
-                Message for deleting a Volume
+            request (Union[google.cloud.netapp_v1.types.DeleteVolumeRequest, dict]):
+                The request object. Message for deleting a Volume
             name (str):
                 Required. Name of the volume
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -1860,22 +1842,22 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_revert_volume():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.RevertVolumeRequest(
+                request = netapp_v1.RevertVolumeRequest(
                     name="name_value",
                     snapshot_id="snapshot_id_value",
                 )
 
                 # Make the request
                 operation = client.revert_volume(request=request)
 
@@ -1883,29 +1865,30 @@
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.RevertVolumeRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.RevertVolumeRequest, dict]):
                 The request object. RevertVolumeRequest reverts the given
                 volume to the specified snapshot.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Volume` Volume
-                   Volume provides a filesystem that you can mount.
+                The result type for the operation will be
+                :class:`google.cloud.netapp_v1.types.Volume` Volume
+                provides a filesystem that you can mount.
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
         # in a volume.RevertVolumeRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
@@ -1957,34 +1940,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_list_snapshots():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListSnapshotsRequest(
+                request = netapp_v1.ListSnapshotsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_snapshots(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.ListSnapshotsRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.ListSnapshotsRequest, dict]):
                 The request object. ListSnapshotsRequest lists snapshots.
             parent (str):
                 Required. The volume for which to retrieve snapshot
                 information, in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}``.
 
                 This corresponds to the ``parent`` field
@@ -1993,15 +1976,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListSnapshotsPager:
+            google.cloud.netapp_v1.services.net_app.pagers.ListSnapshotsPager:
                 ListSnapshotsResponse is the result
                 of ListSnapshotsRequest.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -2072,33 +2055,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_get_snapshot():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetSnapshotRequest(
+                request = netapp_v1.GetSnapshotRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_snapshot(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.GetSnapshotRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.GetSnapshotRequest, dict]):
                 The request object. GetSnapshotRequest gets the state of
                 a snapshot.
             name (str):
                 Required. The snapshot resource name, in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}/snapshots/{snapshot_id}``
 
                 This corresponds to the ``name`` field
@@ -2107,16 +2090,16 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.Snapshot:
-                Snapshot
+            google.cloud.netapp_v1.types.Snapshot:
+
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
@@ -2174,22 +2157,22 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_create_snapshot():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.CreateSnapshotRequest(
+                request = netapp_v1.CreateSnapshotRequest(
                     parent="parent_value",
                     snapshot_id="snapshot_id_value",
                 )
 
                 # Make the request
                 operation = client.create_snapshot(request=request)
 
@@ -2197,26 +2180,26 @@
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.CreateSnapshotRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.CreateSnapshotRequest, dict]):
                 The request object. CreateSnapshotRequest creates a
                 snapshot.
             parent (str):
                 Required. The NetApp volume to create the snapshots of,
                 in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            snapshot (google.cloud.netapp_v1beta1.types.Snapshot):
+            snapshot (google.cloud.netapp_v1.types.Snapshot):
                 Required. A snapshot resource
                 This corresponds to the ``snapshot`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             snapshot_id (str):
                 Required. ID of the snapshot to
                 create. This value must start with a
@@ -2234,16 +2217,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.Snapshot`
-                Snapshot
+                :class:`google.cloud.netapp_v1.types.Snapshot`
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, snapshot, snapshot_id])
         if request is not None and has_flattened_params:
@@ -2312,37 +2294,37 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_delete_snapshot():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteSnapshotRequest(
+                request = netapp_v1.DeleteSnapshotRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_snapshot(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.DeleteSnapshotRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.DeleteSnapshotRequest, dict]):
                 The request object. DeleteSnapshotRequest deletes a
                 snapshot.
             name (str):
                 Required. The snapshot resource name, in the format
                 ``projects/*/locations/*/volumes/*/snapshots/{snapshot_id}``
 
                 This corresponds to the ``name`` field
@@ -2437,40 +2419,40 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_update_snapshot():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.UpdateSnapshotRequest(
+                request = netapp_v1.UpdateSnapshotRequest(
                 )
 
                 # Make the request
                 operation = client.update_snapshot(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.UpdateSnapshotRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.UpdateSnapshotRequest, dict]):
                 The request object. UpdateSnapshotRequest updates
                 description and/or labels for a
                 snapshot.
-            snapshot (google.cloud.netapp_v1beta1.types.Snapshot):
+            snapshot (google.cloud.netapp_v1.types.Snapshot):
                 Required. A snapshot resource
                 This corresponds to the ``snapshot`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Mask of fields to update.
                 At least one path must be supplied in
@@ -2486,16 +2468,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.Snapshot`
-                Snapshot
+                :class:`google.cloud.netapp_v1.types.Snapshot`
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([snapshot, update_mask])
         if request is not None and has_flattened_params:
@@ -2555,46 +2536,45 @@
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListActiveDirectoriesPager:
-        r"""ListActiveDirectories
-        Lists active directories.
+        r"""Lists active directories.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_list_active_directories():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListActiveDirectoriesRequest(
+                request = netapp_v1.ListActiveDirectoriesRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_active_directories(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.ListActiveDirectoriesRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.ListActiveDirectoriesRequest, dict]):
                 The request object. ListActiveDirectoriesRequest for
                 requesting multiple active directories.
             parent (str):
                 Required. Parent value for
                 ListActiveDirectoriesRequest
 
                 This corresponds to the ``parent`` field
@@ -2603,15 +2583,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListActiveDirectoriesPager:
+            google.cloud.netapp_v1.services.net_app.pagers.ListActiveDirectoriesPager:
                 ListActiveDirectoriesResponse
                 contains all the active directories
                 requested.  Iterating over this object
                 will yield results and resolve
                 additional pages automatically.
 
         """
@@ -2673,45 +2653,44 @@
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> active_directory.ActiveDirectory:
-        r"""DescribeActiveDirectory
-        Describes a specified active directory.
+        r"""Describes a specified active directory.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_get_active_directory():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetActiveDirectoryRequest(
+                request = netapp_v1.GetActiveDirectoryRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_active_directory(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.GetActiveDirectoryRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.GetActiveDirectoryRequest, dict]):
                 The request object. GetActiveDirectory for getting a
                 single active directory.
             name (str):
                 Required. Name of the active
                 directory.
 
                 This corresponds to the ``name`` field
@@ -2720,15 +2699,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.ActiveDirectory:
+            google.cloud.netapp_v1.types.ActiveDirectory:
                 ActiveDirectory is the public
                 representation of the active directory
                 config.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -2793,29 +2772,29 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_create_active_directory():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                active_directory = netapp_v1beta1.ActiveDirectory()
+                active_directory = netapp_v1.ActiveDirectory()
                 active_directory.domain = "domain_value"
                 active_directory.dns = "dns_value"
                 active_directory.net_bios_prefix = "net_bios_prefix_value"
                 active_directory.username = "username_value"
                 active_directory.password = "password_value"
 
-                request = netapp_v1beta1.CreateActiveDirectoryRequest(
+                request = netapp_v1.CreateActiveDirectoryRequest(
                     parent="parent_value",
                     active_directory=active_directory,
                     active_directory_id="active_directory_id_value",
                 )
 
                 # Make the request
                 operation = client.create_active_directory(request=request)
@@ -2824,23 +2803,23 @@
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.CreateActiveDirectoryRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.CreateActiveDirectoryRequest, dict]):
                 The request object. CreateActiveDirectoryRequest for
                 creating an active directory.
             parent (str):
                 Required. Value for parent.
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            active_directory (google.cloud.netapp_v1beta1.types.ActiveDirectory):
+            active_directory (google.cloud.netapp_v1.types.ActiveDirectory):
                 Required. Fields of the to be created
                 active directory.
 
                 This corresponds to the ``active_directory`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             active_directory_id (str):
@@ -2857,15 +2836,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.ActiveDirectory`
+                :class:`google.cloud.netapp_v1.types.ActiveDirectory`
                 ActiveDirectory is the public representation of the
                 active directory config.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -2928,59 +2907,58 @@
         *,
         active_directory: Optional[gcn_active_directory.ActiveDirectory] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""UpdateActiveDirectory
-        Update the parameters of an active directories.
+        r"""Update the parameters of an active directories.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_update_active_directory():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                active_directory = netapp_v1beta1.ActiveDirectory()
+                active_directory = netapp_v1.ActiveDirectory()
                 active_directory.domain = "domain_value"
                 active_directory.dns = "dns_value"
                 active_directory.net_bios_prefix = "net_bios_prefix_value"
                 active_directory.username = "username_value"
                 active_directory.password = "password_value"
 
-                request = netapp_v1beta1.UpdateActiveDirectoryRequest(
+                request = netapp_v1.UpdateActiveDirectoryRequest(
                     active_directory=active_directory,
                 )
 
                 # Make the request
                 operation = client.update_active_directory(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.UpdateActiveDirectoryRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.UpdateActiveDirectoryRequest, dict]):
                 The request object. UpdateActiveDirectoryRequest for
                 updating an active directory.
-            active_directory (google.cloud.netapp_v1beta1.types.ActiveDirectory):
+            active_directory (google.cloud.netapp_v1.types.ActiveDirectory):
                 Required. The volume being updated
                 This corresponds to the ``active_directory`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Field mask is used to specify the fields to be
                 overwritten in the Active Directory resource by the
@@ -3000,15 +2978,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.ActiveDirectory`
+                :class:`google.cloud.netapp_v1.types.ActiveDirectory`
                 ActiveDirectory is the public representation of the
                 active directory config.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -3070,49 +3048,48 @@
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""DeleteActiveDirectory
-        Delete the active directory specified in the request.
+        r"""Delete the active directory specified in the request.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_delete_active_directory():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteActiveDirectoryRequest(
+                request = netapp_v1.DeleteActiveDirectoryRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_active_directory(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.DeleteActiveDirectoryRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.DeleteActiveDirectoryRequest, dict]):
                 The request object. DeleteActiveDirectoryRequest for
                 deleting a single active directory.
             name (str):
                 Required. Name of the active
                 directory.
 
                 This corresponds to the ``name`` field
@@ -3195,62 +3172,60 @@
         request: Optional[Union[kms.ListKmsConfigsRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListKmsConfigsPager:
-        r"""ListKmsConfigs
-        Returns descriptions of all KMS configs owned by the
+        r"""Returns descriptions of all KMS configs owned by the
         caller.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_list_kms_configs():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListKmsConfigsRequest(
+                request = netapp_v1.ListKmsConfigsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_kms_configs(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.ListKmsConfigsRequest, dict]):
-                The request object. ListKmsConfigsRequest
+            request (Union[google.cloud.netapp_v1.types.ListKmsConfigsRequest, dict]):
+                The request object.
             parent (str):
                 Required. Parent value
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListKmsConfigsPager:
-                ListKmsConfigsResponse
+            google.cloud.netapp_v1.services.net_app.pagers.ListKmsConfigsPager:
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
@@ -3310,37 +3285,36 @@
         parent: Optional[str] = None,
         kms_config: Optional[kms.KmsConfig] = None,
         kms_config_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""CreateKmsConfig
-        Creates a new KMS config.
+        r"""Creates a new KMS config.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_create_kms_config():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                kms_config = netapp_v1beta1.KmsConfig()
+                kms_config = netapp_v1.KmsConfig()
                 kms_config.crypto_key_name = "crypto_key_name_value"
 
-                request = netapp_v1beta1.CreateKmsConfigRequest(
+                request = netapp_v1.CreateKmsConfigRequest(
                     parent="parent_value",
                     kms_config_id="kms_config_id_value",
                     kms_config=kms_config,
                 )
 
                 # Make the request
                 operation = client.create_kms_config(request=request)
@@ -3349,22 +3323,22 @@
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.CreateKmsConfigRequest, dict]):
-                The request object. CreateKmsConfigRequest
+            request (Union[google.cloud.netapp_v1.types.CreateKmsConfigRequest, dict]):
+                The request object.
             parent (str):
                 Required. Value for parent.
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            kms_config (google.cloud.netapp_v1beta1.types.KmsConfig):
+            kms_config (google.cloud.netapp_v1.types.KmsConfig):
                 Required. The required parameters to
                 create a new KmsConfig.
 
                 This corresponds to the ``kms_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             kms_config_id (str):
@@ -3382,15 +3356,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.KmsConfig`
+                :class:`google.cloud.netapp_v1.types.KmsConfig`
                 KmsConfig is the customer managed encryption key(CMEK)
                 configuration.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -3450,59 +3424,59 @@
         request: Optional[Union[kms.GetKmsConfigRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> kms.KmsConfig:
-        r"""GetKmsConfig Returns the description of the specified KMS config
-        by kms_config_id.
+        r"""Returns the description of the specified KMS config by
+        kms_config_id.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_get_kms_config():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetKmsConfigRequest(
+                request = netapp_v1.GetKmsConfigRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_kms_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.GetKmsConfigRequest, dict]):
-                The request object. GetKmsConfigRequest
+            request (Union[google.cloud.netapp_v1.types.GetKmsConfigRequest, dict]):
+                The request object.
             name (str):
                 Required. Name of the KmsConfig
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.KmsConfig:
+            google.cloud.netapp_v1.types.KmsConfig:
                 KmsConfig is the customer managed
                 encryption key(CMEK) configuration.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -3551,54 +3525,53 @@
         *,
         kms_config: Optional[kms.KmsConfig] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""UpdateKmsConfig
-        Updates the Kms config properties with the full spec
+        r"""Updates the Kms config properties with the full spec
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_update_kms_config():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                kms_config = netapp_v1beta1.KmsConfig()
+                kms_config = netapp_v1.KmsConfig()
                 kms_config.crypto_key_name = "crypto_key_name_value"
 
-                request = netapp_v1beta1.UpdateKmsConfigRequest(
+                request = netapp_v1.UpdateKmsConfigRequest(
                     kms_config=kms_config,
                 )
 
                 # Make the request
                 operation = client.update_kms_config(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.UpdateKmsConfigRequest, dict]):
-                The request object. UpdateKmsConfigRequest
-            kms_config (google.cloud.netapp_v1beta1.types.KmsConfig):
+            request (Union[google.cloud.netapp_v1.types.UpdateKmsConfigRequest, dict]):
+                The request object.
+            kms_config (google.cloud.netapp_v1.types.KmsConfig):
                 Required. The KmsConfig being updated
                 This corresponds to the ``kms_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Field mask is used to specify the fields to be
                 overwritten in the KmsConfig resource by the update. The
@@ -3617,15 +3590,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.KmsConfig`
+                :class:`google.cloud.netapp_v1.types.KmsConfig`
                 KmsConfig is the customer managed encryption key(CMEK)
                 configuration.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -3684,65 +3657,63 @@
         self,
         request: Optional[Union[kms.EncryptVolumesRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""EncryptVolumes
-        Encrypt the existing volumes without CMEK encryption
+        r"""Encrypt the existing volumes without CMEK encryption
         with the desired the KMS config for the whole region.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_encrypt_volumes():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.EncryptVolumesRequest(
+                request = netapp_v1.EncryptVolumesRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.encrypt_volumes(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.EncryptVolumesRequest, dict]):
-                The request object. EncryptVolumesRequest
-                EncryptVolumesRequest specifies the KMS
-                config to encrypt existing volumes.
+            request (Union[google.cloud.netapp_v1.types.EncryptVolumesRequest, dict]):
+                The request object. EncryptVolumesRequest specifies the
+                KMS config to encrypt existing volumes.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.netapp_v1beta1.types.KmsConfig`
+                :class:`google.cloud.netapp_v1.types.KmsConfig`
                 KmsConfig is the customer managed encryption key(CMEK)
                 configuration.
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
         # in a kms.EncryptVolumesRequest.
@@ -3784,57 +3755,54 @@
         self,
         request: Optional[Union[kms.VerifyKmsConfigRequest, dict]] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> kms.VerifyKmsConfigResponse:
-        r"""VerifyKmsConfigRequest
-        Verifies KMS config reachability.
+        r"""Verifies KMS config reachability.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_verify_kms_config():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.VerifyKmsConfigRequest(
+                request = netapp_v1.VerifyKmsConfigRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.verify_kms_config(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.VerifyKmsConfigRequest, dict]):
-                The request object. VerifyKmsConfigRequest
-                VerifyKmsConfigRequest specifies the KMS
-                config to be validated.
+            request (Union[google.cloud.netapp_v1.types.VerifyKmsConfigRequest, dict]):
+                The request object. VerifyKmsConfigRequest specifies the
+                KMS config to be validated.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.VerifyKmsConfigResponse:
-                VerifyKmsConfigResponse
+            google.cloud.netapp_v1.types.VerifyKmsConfigResponse:
                 VerifyKmsConfigResponse contains the
                 information if the config is correctly
                 and error message.
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
@@ -3870,51 +3838,50 @@
         request: Optional[Union[kms.DeleteKmsConfigRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""DeleteKmsConfig
-        Warning! This operation will permanently delete the Kms
-        config.
+        r"""Warning! This operation will permanently delete the
+        Kms config.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_delete_kms_config():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteKmsConfigRequest(
+                request = netapp_v1.DeleteKmsConfigRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_kms_config(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.DeleteKmsConfigRequest, dict]):
-                The request object. DeleteKmsConfigRequest
+            request (Union[google.cloud.netapp_v1.types.DeleteKmsConfigRequest, dict]):
+                The request object.
             name (str):
                 Required. Name of the KmsConfig.
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
@@ -4005,34 +3972,34 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_list_replications():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ListReplicationsRequest(
+                request = netapp_v1.ListReplicationsRequest(
                     parent="parent_value",
                 )
 
                 # Make the request
                 page_result = client.list_replications(request=request)
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.ListReplicationsRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.ListReplicationsRequest, dict]):
                 The request object. ListReplications lists replications.
             parent (str):
                 Required. The volume for which to retrieve replication
                 information, in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}``.
 
                 This corresponds to the ``parent`` field
@@ -4041,15 +4008,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.services.net_app.pagers.ListReplicationsPager:
+            google.cloud.netapp_v1.services.net_app.pagers.ListReplicationsPager:
                 ListReplicationsResponse is the
                 result of ListReplicationsRequest.
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
@@ -4120,33 +4087,33 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_get_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.GetReplicationRequest(
+                request = netapp_v1.GetReplicationRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 response = client.get_replication(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.GetReplicationRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.GetReplicationRequest, dict]):
                 The request object. GetReplicationRequest gets the state
                 of a replication.
             name (str):
                 Required. The replication resource name, in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}/replications/{replication_id}``
 
                 This corresponds to the ``name`` field
@@ -4155,15 +4122,15 @@
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.netapp_v1beta1.types.Replication:
+            google.cloud.netapp_v1.types.Replication:
                 Replication is a nested resource
                 under Volume, that describes a
                 cross-region replication relationship
                 between 2 volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
@@ -4226,26 +4193,26 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_create_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                replication = netapp_v1beta1.Replication()
+                replication = netapp_v1.Replication()
                 replication.replication_schedule = "DAILY"
                 replication.destination_volume_parameters.storage_pool = "storage_pool_value"
 
-                request = netapp_v1beta1.CreateReplicationRequest(
+                request = netapp_v1.CreateReplicationRequest(
                     parent="parent_value",
                     replication=replication,
                     replication_id="replication_id_value",
                 )
 
                 # Make the request
                 operation = client.create_replication(request=request)
@@ -4254,26 +4221,26 @@
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.CreateReplicationRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.CreateReplicationRequest, dict]):
                 The request object. CreateReplicationRequest creates a
                 replication.
             parent (str):
                 Required. The NetApp volume to create the replications
                 of, in the format
                 ``projects/{project_id}/locations/{location}/volumes/{volume_id}``
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
-            replication (google.cloud.netapp_v1beta1.types.Replication):
+            replication (google.cloud.netapp_v1.types.Replication):
                 Required. A replication resource
                 This corresponds to the ``replication`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             replication_id (str):
                 Required. ID of the replication to
                 create. This value must start with a
@@ -4290,15 +4257,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Replication` Replication is a nested resource under Volume, that describes a
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.Replication` Replication is a nested resource under Volume, that describes a
                    cross-region replication relationship between 2
                    volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -4369,37 +4336,37 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_delete_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.DeleteReplicationRequest(
+                request = netapp_v1.DeleteReplicationRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.delete_replication(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.DeleteReplicationRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.DeleteReplicationRequest, dict]):
                 The request object. DeleteReplicationRequest deletes a
                 replication.
             name (str):
                 Required. The replication resource name, in the format
                 ``projects/*/locations/*/volumes/*/replications/{replication_id}``
 
                 This corresponds to the ``name`` field
@@ -4494,45 +4461,45 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_update_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                replication = netapp_v1beta1.Replication()
+                replication = netapp_v1.Replication()
                 replication.replication_schedule = "DAILY"
                 replication.destination_volume_parameters.storage_pool = "storage_pool_value"
 
-                request = netapp_v1beta1.UpdateReplicationRequest(
+                request = netapp_v1.UpdateReplicationRequest(
                     replication=replication,
                 )
 
                 # Make the request
                 operation = client.update_replication(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.UpdateReplicationRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.UpdateReplicationRequest, dict]):
                 The request object. UpdateReplicationRequest updates
                 description and/or labels for a
                 replication.
-            replication (google.cloud.netapp_v1beta1.types.Replication):
+            replication (google.cloud.netapp_v1.types.Replication):
                 Required. A replication resource
                 This corresponds to the ``replication`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Mask of fields to update.
                 At least one path must be supplied in
@@ -4547,15 +4514,15 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Replication` Replication is a nested resource under Volume, that describes a
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.Replication` Replication is a nested resource under Volume, that describes a
                    cross-region replication relationship between 2
                    volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -4625,50 +4592,50 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_stop_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.StopReplicationRequest(
+                request = netapp_v1.StopReplicationRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.stop_replication(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.StopReplicationRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.StopReplicationRequest, dict]):
                 The request object. StopReplicationRequest stops a
                 replication until resumed.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Replication` Replication is a nested resource under Volume, that describes a
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.Replication` Replication is a nested resource under Volume, that describes a
                    cross-region replication relationship between 2
                    volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
         # in a replication.StopReplicationRequest.
@@ -4721,50 +4688,50 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_resume_replication():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ResumeReplicationRequest(
+                request = netapp_v1.ResumeReplicationRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.resume_replication(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.ResumeReplicationRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.ResumeReplicationRequest, dict]):
                 The request object. ResumeReplicationRequest resumes a
                 stopped replication.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Replication` Replication is a nested resource under Volume, that describes a
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.Replication` Replication is a nested resource under Volume, that describes a
                    cross-region replication relationship between 2
                    volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
         # in a replication.ResumeReplicationRequest.
@@ -4808,65 +4775,64 @@
             Union[replication.ReverseReplicationDirectionRequest, dict]
         ] = None,
         *,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""ReverseReplicationDirection reverses direction of
-        replication. Source becomes destination and destination
-        becomes source.
+        r"""Reverses direction of replication. Source becomes
+        destination and destination becomes source.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import netapp_v1beta1
+            from google.cloud import netapp_v1
 
             def sample_reverse_replication_direction():
                 # Create a client
-                client = netapp_v1beta1.NetAppClient()
+                client = netapp_v1.NetAppClient()
 
                 # Initialize request argument(s)
-                request = netapp_v1beta1.ReverseReplicationDirectionRequest(
+                request = netapp_v1.ReverseReplicationDirectionRequest(
                     name="name_value",
                 )
 
                 # Make the request
                 operation = client.reverse_replication_direction(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.netapp_v1beta1.types.ReverseReplicationDirectionRequest, dict]):
+            request (Union[google.cloud.netapp_v1.types.ReverseReplicationDirectionRequest, dict]):
                 The request object. ReverseReplicationDirectionRequest
                 reverses direction of replication.
                 Source becomes destination and
                 destination becomes source.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be :class:`google.cloud.netapp_v1beta1.types.Replication` Replication is a nested resource under Volume, that describes a
+                The result type for the operation will be :class:`google.cloud.netapp_v1.types.Replication` Replication is a nested resource under Volume, that describes a
                    cross-region replication relationship between 2
                    volumes in different regions.
 
         """
         # Create or coerce a protobuf request object.
         # Minor optimization to avoid making a copy if the user passes
         # in a replication.ReverseReplicationDirectionRequest.
@@ -4915,339 +4881,14 @@
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
-    def list_operations(
-        self,
-        request: Optional[operations_pb2.ListOperationsRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> operations_pb2.ListOperationsResponse:
-        r"""Lists operations that match the specified filter in the request.
-
-        Args:
-            request (:class:`~.operations_pb2.ListOperationsRequest`):
-                The request object. Request message for
-                `ListOperations` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                    if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            ~.operations_pb2.ListOperationsResponse:
-                Response message for ``ListOperations`` method.
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = operations_pb2.ListOperationsRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._transport.list_operations,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        response = rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-        # Done; return the response.
-        return response
-
-    def get_operation(
-        self,
-        request: Optional[operations_pb2.GetOperationRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> operations_pb2.Operation:
-        r"""Gets the latest state of a long-running operation.
-
-        Args:
-            request (:class:`~.operations_pb2.GetOperationRequest`):
-                The request object. Request message for
-                `GetOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                    if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            ~.operations_pb2.Operation:
-                An ``Operation`` object.
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = operations_pb2.GetOperationRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._transport.get_operation,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        response = rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-        # Done; return the response.
-        return response
-
-    def delete_operation(
-        self,
-        request: Optional[operations_pb2.DeleteOperationRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> None:
-        r"""Deletes a long-running operation.
-
-        This method indicates that the client is no longer interested
-        in the operation result. It does not cancel the operation.
-        If the server doesn't support this method, it returns
-        `google.rpc.Code.UNIMPLEMENTED`.
-
-        Args:
-            request (:class:`~.operations_pb2.DeleteOperationRequest`):
-                The request object. Request message for
-                `DeleteOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                    if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            None
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = operations_pb2.DeleteOperationRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._transport.delete_operation,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-    def cancel_operation(
-        self,
-        request: Optional[operations_pb2.CancelOperationRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> None:
-        r"""Starts asynchronous cancellation on a long-running operation.
-
-        The server makes a best effort to cancel the operation, but success
-        is not guaranteed.  If the server doesn't support this method, it returns
-        `google.rpc.Code.UNIMPLEMENTED`.
-
-        Args:
-            request (:class:`~.operations_pb2.CancelOperationRequest`):
-                The request object. Request message for
-                `CancelOperation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                    if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            None
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = operations_pb2.CancelOperationRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._transport.cancel_operation,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-    def get_location(
-        self,
-        request: Optional[locations_pb2.GetLocationRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> locations_pb2.Location:
-        r"""Gets information about a location.
-
-        Args:
-            request (:class:`~.location_pb2.GetLocationRequest`):
-                The request object. Request message for
-                `GetLocation` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                 if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            ~.location_pb2.Location:
-                Location object.
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = locations_pb2.GetLocationRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._transport.get_location,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        response = rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-        # Done; return the response.
-        return response
-
-    def list_locations(
-        self,
-        request: Optional[locations_pb2.ListLocationsRequest] = None,
-        *,
-        retry: OptionalRetry = gapic_v1.method.DEFAULT,
-        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
-        metadata: Sequence[Tuple[str, str]] = (),
-    ) -> locations_pb2.ListLocationsResponse:
-        r"""Lists information about the supported locations for this service.
-
-        Args:
-            request (:class:`~.location_pb2.ListLocationsRequest`):
-                The request object. Request message for
-                `ListLocations` method.
-            retry (google.api_core.retry.Retry): Designation of what errors,
-                 if any, should be retried.
-            timeout (float): The timeout for this request.
-            metadata (Sequence[Tuple[str, str]]): Strings which should be
-                sent along with the request as metadata.
-        Returns:
-            ~.location_pb2.ListLocationsResponse:
-                Response message for ``ListLocations`` method.
-        """
-        # Create or coerce a protobuf request object.
-        # The request isn't a proto-plus wrapped type,
-        # so it must be constructed via keyword expansion.
-        if isinstance(request, dict):
-            request = locations_pb2.ListLocationsRequest(**request)
-
-        # Wrap the RPC method; this adds retry and timeout information,
-        # and friendly error handling.
-        rpc = gapic_v1.method.wrap_method(
-            self._transport.list_locations,
-            default_timeout=None,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
-
-        # Certain fields should be provided within the metadata header;
-        # add these here.
-        metadata = tuple(metadata) + (
-            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
-        )
-
-        # Send the request.
-        response = rpc(
-            request,
-            retry=retry,
-            timeout=timeout,
-            metadata=metadata,
-        )
-
-        # Done; return the response.
-        return response
-
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 __all__ = ("NetAppClient",)
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/pagers.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/pagers.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,38 +20,38 @@
     Callable,
     Iterator,
     Optional,
     Sequence,
     Tuple,
 )
 
-from google.cloud.netapp_v1beta1.types import (
+from google.cloud.netapp_v1.types import (
     active_directory,
     kms,
     replication,
     snapshot,
     storage_pool,
     volume,
 )
 
 
 class ListStoragePoolsPager:
     """A pager for iterating through ``list_storage_pools`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListStoragePoolsResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListStoragePoolsResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``storage_pools`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListStoragePools`` requests and continue to iterate
     through the ``storage_pools`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListStoragePoolsResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListStoragePoolsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., storage_pool.ListStoragePoolsResponse],
@@ -61,17 +61,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListStoragePoolsRequest):
+            request (google.cloud.netapp_v1.types.ListStoragePoolsRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListStoragePoolsResponse):
+            response (google.cloud.netapp_v1.types.ListStoragePoolsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = storage_pool.ListStoragePoolsRequest(request)
         self._response = response
@@ -96,24 +96,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListStoragePoolsAsyncPager:
     """A pager for iterating through ``list_storage_pools`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListStoragePoolsResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListStoragePoolsResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``storage_pools`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListStoragePools`` requests and continue to iterate
     through the ``storage_pools`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListStoragePoolsResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListStoragePoolsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[storage_pool.ListStoragePoolsResponse]],
@@ -123,17 +123,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListStoragePoolsRequest):
+            request (google.cloud.netapp_v1.types.ListStoragePoolsRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListStoragePoolsResponse):
+            response (google.cloud.netapp_v1.types.ListStoragePoolsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = storage_pool.ListStoragePoolsRequest(request)
         self._response = response
@@ -162,24 +162,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListVolumesPager:
     """A pager for iterating through ``list_volumes`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListVolumesResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListVolumesResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``volumes`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListVolumes`` requests and continue to iterate
     through the ``volumes`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListVolumesResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListVolumesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., volume.ListVolumesResponse],
@@ -189,17 +189,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListVolumesRequest):
+            request (google.cloud.netapp_v1.types.ListVolumesRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListVolumesResponse):
+            response (google.cloud.netapp_v1.types.ListVolumesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = volume.ListVolumesRequest(request)
         self._response = response
@@ -224,24 +224,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListVolumesAsyncPager:
     """A pager for iterating through ``list_volumes`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListVolumesResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListVolumesResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``volumes`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListVolumes`` requests and continue to iterate
     through the ``volumes`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListVolumesResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListVolumesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[volume.ListVolumesResponse]],
@@ -251,17 +251,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListVolumesRequest):
+            request (google.cloud.netapp_v1.types.ListVolumesRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListVolumesResponse):
+            response (google.cloud.netapp_v1.types.ListVolumesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = volume.ListVolumesRequest(request)
         self._response = response
@@ -290,24 +290,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListSnapshotsPager:
     """A pager for iterating through ``list_snapshots`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListSnapshotsResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListSnapshotsResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``snapshots`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListSnapshots`` requests and continue to iterate
     through the ``snapshots`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListSnapshotsResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListSnapshotsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., snapshot.ListSnapshotsResponse],
@@ -317,17 +317,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListSnapshotsRequest):
+            request (google.cloud.netapp_v1.types.ListSnapshotsRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListSnapshotsResponse):
+            response (google.cloud.netapp_v1.types.ListSnapshotsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = snapshot.ListSnapshotsRequest(request)
         self._response = response
@@ -352,24 +352,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListSnapshotsAsyncPager:
     """A pager for iterating through ``list_snapshots`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListSnapshotsResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListSnapshotsResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``snapshots`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListSnapshots`` requests and continue to iterate
     through the ``snapshots`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListSnapshotsResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListSnapshotsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[snapshot.ListSnapshotsResponse]],
@@ -379,17 +379,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListSnapshotsRequest):
+            request (google.cloud.netapp_v1.types.ListSnapshotsRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListSnapshotsResponse):
+            response (google.cloud.netapp_v1.types.ListSnapshotsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = snapshot.ListSnapshotsRequest(request)
         self._response = response
@@ -418,24 +418,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListActiveDirectoriesPager:
     """A pager for iterating through ``list_active_directories`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListActiveDirectoriesResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListActiveDirectoriesResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``active_directories`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListActiveDirectories`` requests and continue to iterate
     through the ``active_directories`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListActiveDirectoriesResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListActiveDirectoriesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., active_directory.ListActiveDirectoriesResponse],
@@ -445,17 +445,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListActiveDirectoriesRequest):
+            request (google.cloud.netapp_v1.types.ListActiveDirectoriesRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListActiveDirectoriesResponse):
+            response (google.cloud.netapp_v1.types.ListActiveDirectoriesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = active_directory.ListActiveDirectoriesRequest(request)
         self._response = response
@@ -480,24 +480,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListActiveDirectoriesAsyncPager:
     """A pager for iterating through ``list_active_directories`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListActiveDirectoriesResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListActiveDirectoriesResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``active_directories`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListActiveDirectories`` requests and continue to iterate
     through the ``active_directories`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListActiveDirectoriesResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListActiveDirectoriesResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[
@@ -509,17 +509,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListActiveDirectoriesRequest):
+            request (google.cloud.netapp_v1.types.ListActiveDirectoriesRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListActiveDirectoriesResponse):
+            response (google.cloud.netapp_v1.types.ListActiveDirectoriesResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = active_directory.ListActiveDirectoriesRequest(request)
         self._response = response
@@ -550,24 +550,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListKmsConfigsPager:
     """A pager for iterating through ``list_kms_configs`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListKmsConfigsResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListKmsConfigsResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``kms_configs`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListKmsConfigs`` requests and continue to iterate
     through the ``kms_configs`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListKmsConfigsResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListKmsConfigsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., kms.ListKmsConfigsResponse],
@@ -577,17 +577,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListKmsConfigsRequest):
+            request (google.cloud.netapp_v1.types.ListKmsConfigsRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListKmsConfigsResponse):
+            response (google.cloud.netapp_v1.types.ListKmsConfigsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = kms.ListKmsConfigsRequest(request)
         self._response = response
@@ -612,24 +612,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListKmsConfigsAsyncPager:
     """A pager for iterating through ``list_kms_configs`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListKmsConfigsResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListKmsConfigsResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``kms_configs`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListKmsConfigs`` requests and continue to iterate
     through the ``kms_configs`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListKmsConfigsResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListKmsConfigsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[kms.ListKmsConfigsResponse]],
@@ -639,17 +639,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListKmsConfigsRequest):
+            request (google.cloud.netapp_v1.types.ListKmsConfigsRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListKmsConfigsResponse):
+            response (google.cloud.netapp_v1.types.ListKmsConfigsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = kms.ListKmsConfigsRequest(request)
         self._response = response
@@ -678,24 +678,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListReplicationsPager:
     """A pager for iterating through ``list_replications`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListReplicationsResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListReplicationsResponse` object, and
     provides an ``__iter__`` method to iterate through its
     ``replications`` field.
 
     If there are more pages, the ``__iter__`` method will make additional
     ``ListReplications`` requests and continue to iterate
     through the ``replications`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListReplicationsResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListReplicationsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., replication.ListReplicationsResponse],
@@ -705,17 +705,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiate the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListReplicationsRequest):
+            request (google.cloud.netapp_v1.types.ListReplicationsRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListReplicationsResponse):
+            response (google.cloud.netapp_v1.types.ListReplicationsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = replication.ListReplicationsRequest(request)
         self._response = response
@@ -740,24 +740,24 @@
         return "{0}<{1!r}>".format(self.__class__.__name__, self._response)
 
 
 class ListReplicationsAsyncPager:
     """A pager for iterating through ``list_replications`` requests.
 
     This class thinly wraps an initial
-    :class:`google.cloud.netapp_v1beta1.types.ListReplicationsResponse` object, and
+    :class:`google.cloud.netapp_v1.types.ListReplicationsResponse` object, and
     provides an ``__aiter__`` method to iterate through its
     ``replications`` field.
 
     If there are more pages, the ``__aiter__`` method will make additional
     ``ListReplications`` requests and continue to iterate
     through the ``replications`` field on the
     corresponding responses.
 
-    All the usual :class:`google.cloud.netapp_v1beta1.types.ListReplicationsResponse`
+    All the usual :class:`google.cloud.netapp_v1.types.ListReplicationsResponse`
     attributes are available on the pager. If multiple requests are made, only
     the most recent response is retained, and thus used for attribute lookup.
     """
 
     def __init__(
         self,
         method: Callable[..., Awaitable[replication.ListReplicationsResponse]],
@@ -767,17 +767,17 @@
         metadata: Sequence[Tuple[str, str]] = ()
     ):
         """Instantiates the pager.
 
         Args:
             method (Callable): The method that was originally called, and
                 which instantiated this pager.
-            request (google.cloud.netapp_v1beta1.types.ListReplicationsRequest):
+            request (google.cloud.netapp_v1.types.ListReplicationsRequest):
                 The initial request object.
-            response (google.cloud.netapp_v1beta1.types.ListReplicationsResponse):
+            response (google.cloud.netapp_v1.types.ListReplicationsResponse):
                 The initial response object.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         self._method = method
         self._request = replication.ListReplicationsRequest(request)
         self._response = response
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/__init__.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/base.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.cloud.location import locations_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
-from google.cloud.netapp_v1beta1 import gapic_version as package_version
-from google.cloud.netapp_v1beta1.types import active_directory as gcn_active_directory
-from google.cloud.netapp_v1beta1.types import active_directory
-from google.cloud.netapp_v1beta1.types import kms
-from google.cloud.netapp_v1beta1.types import replication
-from google.cloud.netapp_v1beta1.types import replication as gcn_replication
-from google.cloud.netapp_v1beta1.types import snapshot
-from google.cloud.netapp_v1beta1.types import snapshot as gcn_snapshot
-from google.cloud.netapp_v1beta1.types import storage_pool
-from google.cloud.netapp_v1beta1.types import storage_pool as gcn_storage_pool
-from google.cloud.netapp_v1beta1.types import volume
-from google.cloud.netapp_v1beta1.types import volume as gcn_volume
+from google.cloud.netapp_v1 import gapic_version as package_version
+from google.cloud.netapp_v1.types import active_directory as gcn_active_directory
+from google.cloud.netapp_v1.types import active_directory
+from google.cloud.netapp_v1.types import kms
+from google.cloud.netapp_v1.types import replication
+from google.cloud.netapp_v1.types import replication as gcn_replication
+from google.cloud.netapp_v1.types import snapshot
+from google.cloud.netapp_v1.types import snapshot as gcn_snapshot
+from google.cloud.netapp_v1.types import storage_pool
+from google.cloud.netapp_v1.types import storage_pool as gcn_storage_pool
+from google.cloud.netapp_v1.types import volume
+from google.cloud.netapp_v1.types import volume as gcn_volume
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 class NetAppTransport(abc.ABC):
@@ -771,66 +771,12 @@
     ) -> Callable[
         [replication.ReverseReplicationDirectionRequest],
         Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
     ]:
         raise NotImplementedError()
 
     @property
-    def list_operations(
-        self,
-    ) -> Callable[
-        [operations_pb2.ListOperationsRequest],
-        Union[
-            operations_pb2.ListOperationsResponse,
-            Awaitable[operations_pb2.ListOperationsResponse],
-        ],
-    ]:
-        raise NotImplementedError()
-
-    @property
-    def get_operation(
-        self,
-    ) -> Callable[
-        [operations_pb2.GetOperationRequest],
-        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
-    ]:
-        raise NotImplementedError()
-
-    @property
-    def cancel_operation(
-        self,
-    ) -> Callable[[operations_pb2.CancelOperationRequest], None,]:
-        raise NotImplementedError()
-
-    @property
-    def delete_operation(
-        self,
-    ) -> Callable[[operations_pb2.DeleteOperationRequest], None,]:
-        raise NotImplementedError()
-
-    @property
-    def get_location(
-        self,
-    ) -> Callable[
-        [locations_pb2.GetLocationRequest],
-        Union[locations_pb2.Location, Awaitable[locations_pb2.Location]],
-    ]:
-        raise NotImplementedError()
-
-    @property
-    def list_locations(
-        self,
-    ) -> Callable[
-        [locations_pb2.ListLocationsRequest],
-        Union[
-            locations_pb2.ListLocationsResponse,
-            Awaitable[locations_pb2.ListLocationsResponse],
-        ],
-    ]:
-        raise NotImplementedError()
-
-    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("NetAppTransport",)
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/grpc.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.cloud.location import locations_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
 
-from google.cloud.netapp_v1beta1.types import active_directory as gcn_active_directory
-from google.cloud.netapp_v1beta1.types import active_directory
-from google.cloud.netapp_v1beta1.types import kms
-from google.cloud.netapp_v1beta1.types import replication
-from google.cloud.netapp_v1beta1.types import replication as gcn_replication
-from google.cloud.netapp_v1beta1.types import snapshot
-from google.cloud.netapp_v1beta1.types import snapshot as gcn_snapshot
-from google.cloud.netapp_v1beta1.types import storage_pool
-from google.cloud.netapp_v1beta1.types import storage_pool as gcn_storage_pool
-from google.cloud.netapp_v1beta1.types import volume
-from google.cloud.netapp_v1beta1.types import volume as gcn_volume
+from google.cloud.netapp_v1.types import active_directory as gcn_active_directory
+from google.cloud.netapp_v1.types import active_directory
+from google.cloud.netapp_v1.types import kms
+from google.cloud.netapp_v1.types import replication
+from google.cloud.netapp_v1.types import replication as gcn_replication
+from google.cloud.netapp_v1.types import snapshot
+from google.cloud.netapp_v1.types import snapshot as gcn_snapshot
+from google.cloud.netapp_v1.types import storage_pool
+from google.cloud.netapp_v1.types import storage_pool as gcn_storage_pool
+from google.cloud.netapp_v1.types import volume
+from google.cloud.netapp_v1.types import volume as gcn_volume
 
 from .base import DEFAULT_CLIENT_INFO, NetAppTransport
 
 
 class NetAppGrpcTransport(NetAppTransport):
     """gRPC backend transport for NetApp.
 
@@ -259,129 +259,125 @@
     def list_storage_pools(
         self,
     ) -> Callable[
         [storage_pool.ListStoragePoolsRequest], storage_pool.ListStoragePoolsResponse
     ]:
         r"""Return a callable for the list storage pools method over gRPC.
 
-        ListStoragePools
-        Returns descriptions of all storage pools owned by the
-        caller.
+        Returns descriptions of all storage pools owned by
+        the caller.
 
         Returns:
             Callable[[~.ListStoragePoolsRequest],
                     ~.ListStoragePoolsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_storage_pools" not in self._stubs:
             self._stubs["list_storage_pools"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListStoragePools",
+                "/google.cloud.netapp.v1.NetApp/ListStoragePools",
                 request_serializer=storage_pool.ListStoragePoolsRequest.serialize,
                 response_deserializer=storage_pool.ListStoragePoolsResponse.deserialize,
             )
         return self._stubs["list_storage_pools"]
 
     @property
     def create_storage_pool(
         self,
     ) -> Callable[
         [gcn_storage_pool.CreateStoragePoolRequest], operations_pb2.Operation
     ]:
         r"""Return a callable for the create storage pool method over gRPC.
 
-        CreateStoragePool
         Creates a new storage pool.
 
         Returns:
             Callable[[~.CreateStoragePoolRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_storage_pool" not in self._stubs:
             self._stubs["create_storage_pool"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateStoragePool",
+                "/google.cloud.netapp.v1.NetApp/CreateStoragePool",
                 request_serializer=gcn_storage_pool.CreateStoragePoolRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_storage_pool"]
 
     @property
     def get_storage_pool(
         self,
     ) -> Callable[[storage_pool.GetStoragePoolRequest], storage_pool.StoragePool]:
         r"""Return a callable for the get storage pool method over gRPC.
 
-        GetStoragePool
-        Returns the description of the specified storage pool by
-        poolId.
+        Returns the description of the specified storage pool
+        by poolId.
 
         Returns:
             Callable[[~.GetStoragePoolRequest],
                     ~.StoragePool]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_storage_pool" not in self._stubs:
             self._stubs["get_storage_pool"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetStoragePool",
+                "/google.cloud.netapp.v1.NetApp/GetStoragePool",
                 request_serializer=storage_pool.GetStoragePoolRequest.serialize,
                 response_deserializer=storage_pool.StoragePool.deserialize,
             )
         return self._stubs["get_storage_pool"]
 
     @property
     def update_storage_pool(
         self,
     ) -> Callable[
         [gcn_storage_pool.UpdateStoragePoolRequest], operations_pb2.Operation
     ]:
         r"""Return a callable for the update storage pool method over gRPC.
 
-        UpdateStoragePool
-        Updates the storage pool properties with the full spec
+        Updates the storage pool properties with the full
+        spec
 
         Returns:
             Callable[[~.UpdateStoragePoolRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_storage_pool" not in self._stubs:
             self._stubs["update_storage_pool"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateStoragePool",
+                "/google.cloud.netapp.v1.NetApp/UpdateStoragePool",
                 request_serializer=gcn_storage_pool.UpdateStoragePoolRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_storage_pool"]
 
     @property
     def delete_storage_pool(
         self,
     ) -> Callable[[storage_pool.DeleteStoragePoolRequest], operations_pb2.Operation]:
         r"""Return a callable for the delete storage pool method over gRPC.
 
-        DeleteStoragePool
         Warning! This operation will permanently delete the
         storage pool.
 
         Returns:
             Callable[[~.DeleteStoragePoolRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
@@ -389,148 +385,143 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_storage_pool" not in self._stubs:
             self._stubs["delete_storage_pool"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteStoragePool",
+                "/google.cloud.netapp.v1.NetApp/DeleteStoragePool",
                 request_serializer=storage_pool.DeleteStoragePoolRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_storage_pool"]
 
     @property
     def list_volumes(
         self,
     ) -> Callable[[volume.ListVolumesRequest], volume.ListVolumesResponse]:
         r"""Return a callable for the list volumes method over gRPC.
 
-        ListVolumes
         Lists Volumes in a given project.
 
         Returns:
             Callable[[~.ListVolumesRequest],
                     ~.ListVolumesResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_volumes" not in self._stubs:
             self._stubs["list_volumes"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListVolumes",
+                "/google.cloud.netapp.v1.NetApp/ListVolumes",
                 request_serializer=volume.ListVolumesRequest.serialize,
                 response_deserializer=volume.ListVolumesResponse.deserialize,
             )
         return self._stubs["list_volumes"]
 
     @property
     def get_volume(self) -> Callable[[volume.GetVolumeRequest], volume.Volume]:
         r"""Return a callable for the get volume method over gRPC.
 
-        GetVolume
         Gets details of a single Volume.
 
         Returns:
             Callable[[~.GetVolumeRequest],
                     ~.Volume]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_volume" not in self._stubs:
             self._stubs["get_volume"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetVolume",
+                "/google.cloud.netapp.v1.NetApp/GetVolume",
                 request_serializer=volume.GetVolumeRequest.serialize,
                 response_deserializer=volume.Volume.deserialize,
             )
         return self._stubs["get_volume"]
 
     @property
     def create_volume(
         self,
     ) -> Callable[[gcn_volume.CreateVolumeRequest], operations_pb2.Operation]:
         r"""Return a callable for the create volume method over gRPC.
 
-        CreateVolume
         Creates a new Volume in a given project and location.
 
         Returns:
             Callable[[~.CreateVolumeRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_volume" not in self._stubs:
             self._stubs["create_volume"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateVolume",
+                "/google.cloud.netapp.v1.NetApp/CreateVolume",
                 request_serializer=gcn_volume.CreateVolumeRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_volume"]
 
     @property
     def update_volume(
         self,
     ) -> Callable[[gcn_volume.UpdateVolumeRequest], operations_pb2.Operation]:
         r"""Return a callable for the update volume method over gRPC.
 
-        UpdateVolume
         Updates the parameters of a single Volume.
 
         Returns:
             Callable[[~.UpdateVolumeRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_volume" not in self._stubs:
             self._stubs["update_volume"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateVolume",
+                "/google.cloud.netapp.v1.NetApp/UpdateVolume",
                 request_serializer=gcn_volume.UpdateVolumeRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_volume"]
 
     @property
     def delete_volume(
         self,
     ) -> Callable[[volume.DeleteVolumeRequest], operations_pb2.Operation]:
         r"""Return a callable for the delete volume method over gRPC.
 
-        DeleteVolume
         Deletes a single Volume.
 
         Returns:
             Callable[[~.DeleteVolumeRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_volume" not in self._stubs:
             self._stubs["delete_volume"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteVolume",
+                "/google.cloud.netapp.v1.NetApp/DeleteVolume",
                 request_serializer=volume.DeleteVolumeRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_volume"]
 
     @property
     def revert_volume(
@@ -550,15 +541,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "revert_volume" not in self._stubs:
             self._stubs["revert_volume"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/RevertVolume",
+                "/google.cloud.netapp.v1.NetApp/RevertVolume",
                 request_serializer=volume.RevertVolumeRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["revert_volume"]
 
     @property
     def list_snapshots(
@@ -576,15 +567,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_snapshots" not in self._stubs:
             self._stubs["list_snapshots"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListSnapshots",
+                "/google.cloud.netapp.v1.NetApp/ListSnapshots",
                 request_serializer=snapshot.ListSnapshotsRequest.serialize,
                 response_deserializer=snapshot.ListSnapshotsResponse.deserialize,
             )
         return self._stubs["list_snapshots"]
 
     @property
     def get_snapshot(
@@ -602,15 +593,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_snapshot" not in self._stubs:
             self._stubs["get_snapshot"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetSnapshot",
+                "/google.cloud.netapp.v1.NetApp/GetSnapshot",
                 request_serializer=snapshot.GetSnapshotRequest.serialize,
                 response_deserializer=snapshot.Snapshot.deserialize,
             )
         return self._stubs["get_snapshot"]
 
     @property
     def create_snapshot(
@@ -628,15 +619,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_snapshot" not in self._stubs:
             self._stubs["create_snapshot"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateSnapshot",
+                "/google.cloud.netapp.v1.NetApp/CreateSnapshot",
                 request_serializer=gcn_snapshot.CreateSnapshotRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_snapshot"]
 
     @property
     def delete_snapshot(
@@ -654,15 +645,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_snapshot" not in self._stubs:
             self._stubs["delete_snapshot"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteSnapshot",
+                "/google.cloud.netapp.v1.NetApp/DeleteSnapshot",
                 request_serializer=snapshot.DeleteSnapshotRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_snapshot"]
 
     @property
     def update_snapshot(
@@ -680,74 +671,72 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_snapshot" not in self._stubs:
             self._stubs["update_snapshot"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateSnapshot",
+                "/google.cloud.netapp.v1.NetApp/UpdateSnapshot",
                 request_serializer=gcn_snapshot.UpdateSnapshotRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_snapshot"]
 
     @property
     def list_active_directories(
         self,
     ) -> Callable[
         [active_directory.ListActiveDirectoriesRequest],
         active_directory.ListActiveDirectoriesResponse,
     ]:
         r"""Return a callable for the list active directories method over gRPC.
 
-        ListActiveDirectories
         Lists active directories.
 
         Returns:
             Callable[[~.ListActiveDirectoriesRequest],
                     ~.ListActiveDirectoriesResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_active_directories" not in self._stubs:
             self._stubs["list_active_directories"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListActiveDirectories",
+                "/google.cloud.netapp.v1.NetApp/ListActiveDirectories",
                 request_serializer=active_directory.ListActiveDirectoriesRequest.serialize,
                 response_deserializer=active_directory.ListActiveDirectoriesResponse.deserialize,
             )
         return self._stubs["list_active_directories"]
 
     @property
     def get_active_directory(
         self,
     ) -> Callable[
         [active_directory.GetActiveDirectoryRequest], active_directory.ActiveDirectory
     ]:
         r"""Return a callable for the get active directory method over gRPC.
 
-        DescribeActiveDirectory
         Describes a specified active directory.
 
         Returns:
             Callable[[~.GetActiveDirectoryRequest],
                     ~.ActiveDirectory]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_active_directory" not in self._stubs:
             self._stubs["get_active_directory"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetActiveDirectory",
+                "/google.cloud.netapp.v1.NetApp/GetActiveDirectory",
                 request_serializer=active_directory.GetActiveDirectoryRequest.serialize,
                 response_deserializer=active_directory.ActiveDirectory.deserialize,
             )
         return self._stubs["get_active_directory"]
 
     @property
     def create_active_directory(
@@ -768,85 +757,82 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_active_directory" not in self._stubs:
             self._stubs["create_active_directory"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateActiveDirectory",
+                "/google.cloud.netapp.v1.NetApp/CreateActiveDirectory",
                 request_serializer=gcn_active_directory.CreateActiveDirectoryRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_active_directory"]
 
     @property
     def update_active_directory(
         self,
     ) -> Callable[
         [gcn_active_directory.UpdateActiveDirectoryRequest], operations_pb2.Operation
     ]:
         r"""Return a callable for the update active directory method over gRPC.
 
-        UpdateActiveDirectory
         Update the parameters of an active directories.
 
         Returns:
             Callable[[~.UpdateActiveDirectoryRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_active_directory" not in self._stubs:
             self._stubs["update_active_directory"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateActiveDirectory",
+                "/google.cloud.netapp.v1.NetApp/UpdateActiveDirectory",
                 request_serializer=gcn_active_directory.UpdateActiveDirectoryRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_active_directory"]
 
     @property
     def delete_active_directory(
         self,
     ) -> Callable[
         [active_directory.DeleteActiveDirectoryRequest], operations_pb2.Operation
     ]:
         r"""Return a callable for the delete active directory method over gRPC.
 
-        DeleteActiveDirectory
         Delete the active directory specified in the request.
 
         Returns:
             Callable[[~.DeleteActiveDirectoryRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_active_directory" not in self._stubs:
             self._stubs["delete_active_directory"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteActiveDirectory",
+                "/google.cloud.netapp.v1.NetApp/DeleteActiveDirectory",
                 request_serializer=active_directory.DeleteActiveDirectoryRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_active_directory"]
 
     @property
     def list_kms_configs(
         self,
     ) -> Callable[[kms.ListKmsConfigsRequest], kms.ListKmsConfigsResponse]:
         r"""Return a callable for the list kms configs method over gRPC.
 
-        ListKmsConfigs
         Returns descriptions of all KMS configs owned by the
         caller.
 
         Returns:
             Callable[[~.ListKmsConfigsRequest],
                     ~.ListKmsConfigsResponse]:
                 A function that, when called, will call the underlying RPC
@@ -854,106 +840,103 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_kms_configs" not in self._stubs:
             self._stubs["list_kms_configs"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListKmsConfigs",
+                "/google.cloud.netapp.v1.NetApp/ListKmsConfigs",
                 request_serializer=kms.ListKmsConfigsRequest.serialize,
                 response_deserializer=kms.ListKmsConfigsResponse.deserialize,
             )
         return self._stubs["list_kms_configs"]
 
     @property
     def create_kms_config(
         self,
     ) -> Callable[[kms.CreateKmsConfigRequest], operations_pb2.Operation]:
         r"""Return a callable for the create kms config method over gRPC.
 
-        CreateKmsConfig
         Creates a new KMS config.
 
         Returns:
             Callable[[~.CreateKmsConfigRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_kms_config" not in self._stubs:
             self._stubs["create_kms_config"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateKmsConfig",
+                "/google.cloud.netapp.v1.NetApp/CreateKmsConfig",
                 request_serializer=kms.CreateKmsConfigRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_kms_config"]
 
     @property
     def get_kms_config(self) -> Callable[[kms.GetKmsConfigRequest], kms.KmsConfig]:
         r"""Return a callable for the get kms config method over gRPC.
 
-        GetKmsConfig Returns the description of the specified KMS config
-        by kms_config_id.
+        Returns the description of the specified KMS config by
+        kms_config_id.
 
         Returns:
             Callable[[~.GetKmsConfigRequest],
                     ~.KmsConfig]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_kms_config" not in self._stubs:
             self._stubs["get_kms_config"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetKmsConfig",
+                "/google.cloud.netapp.v1.NetApp/GetKmsConfig",
                 request_serializer=kms.GetKmsConfigRequest.serialize,
                 response_deserializer=kms.KmsConfig.deserialize,
             )
         return self._stubs["get_kms_config"]
 
     @property
     def update_kms_config(
         self,
     ) -> Callable[[kms.UpdateKmsConfigRequest], operations_pb2.Operation]:
         r"""Return a callable for the update kms config method over gRPC.
 
-        UpdateKmsConfig
         Updates the Kms config properties with the full spec
 
         Returns:
             Callable[[~.UpdateKmsConfigRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_kms_config" not in self._stubs:
             self._stubs["update_kms_config"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateKmsConfig",
+                "/google.cloud.netapp.v1.NetApp/UpdateKmsConfig",
                 request_serializer=kms.UpdateKmsConfigRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_kms_config"]
 
     @property
     def encrypt_volumes(
         self,
     ) -> Callable[[kms.EncryptVolumesRequest], operations_pb2.Operation]:
         r"""Return a callable for the encrypt volumes method over gRPC.
 
-        EncryptVolumes
         Encrypt the existing volumes without CMEK encryption
         with the desired the KMS config for the whole region.
 
         Returns:
             Callable[[~.EncryptVolumesRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
@@ -961,70 +944,68 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "encrypt_volumes" not in self._stubs:
             self._stubs["encrypt_volumes"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/EncryptVolumes",
+                "/google.cloud.netapp.v1.NetApp/EncryptVolumes",
                 request_serializer=kms.EncryptVolumesRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["encrypt_volumes"]
 
     @property
     def verify_kms_config(
         self,
     ) -> Callable[[kms.VerifyKmsConfigRequest], kms.VerifyKmsConfigResponse]:
         r"""Return a callable for the verify kms config method over gRPC.
 
-        VerifyKmsConfigRequest
         Verifies KMS config reachability.
 
         Returns:
             Callable[[~.VerifyKmsConfigRequest],
                     ~.VerifyKmsConfigResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "verify_kms_config" not in self._stubs:
             self._stubs["verify_kms_config"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/VerifyKmsConfig",
+                "/google.cloud.netapp.v1.NetApp/VerifyKmsConfig",
                 request_serializer=kms.VerifyKmsConfigRequest.serialize,
                 response_deserializer=kms.VerifyKmsConfigResponse.deserialize,
             )
         return self._stubs["verify_kms_config"]
 
     @property
     def delete_kms_config(
         self,
     ) -> Callable[[kms.DeleteKmsConfigRequest], operations_pb2.Operation]:
         r"""Return a callable for the delete kms config method over gRPC.
 
-        DeleteKmsConfig
-        Warning! This operation will permanently delete the Kms
-        config.
+        Warning! This operation will permanently delete the
+        Kms config.
 
         Returns:
             Callable[[~.DeleteKmsConfigRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_kms_config" not in self._stubs:
             self._stubs["delete_kms_config"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteKmsConfig",
+                "/google.cloud.netapp.v1.NetApp/DeleteKmsConfig",
                 request_serializer=kms.DeleteKmsConfigRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_kms_config"]
 
     @property
     def list_replications(
@@ -1045,15 +1026,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_replications" not in self._stubs:
             self._stubs["list_replications"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListReplications",
+                "/google.cloud.netapp.v1.NetApp/ListReplications",
                 request_serializer=replication.ListReplicationsRequest.serialize,
                 response_deserializer=replication.ListReplicationsResponse.deserialize,
             )
         return self._stubs["list_replications"]
 
     @property
     def get_replication(
@@ -1071,15 +1052,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_replication" not in self._stubs:
             self._stubs["get_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetReplication",
+                "/google.cloud.netapp.v1.NetApp/GetReplication",
                 request_serializer=replication.GetReplicationRequest.serialize,
                 response_deserializer=replication.Replication.deserialize,
             )
         return self._stubs["get_replication"]
 
     @property
     def create_replication(
@@ -1097,15 +1078,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_replication" not in self._stubs:
             self._stubs["create_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateReplication",
+                "/google.cloud.netapp.v1.NetApp/CreateReplication",
                 request_serializer=gcn_replication.CreateReplicationRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_replication"]
 
     @property
     def delete_replication(
@@ -1123,15 +1104,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_replication" not in self._stubs:
             self._stubs["delete_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteReplication",
+                "/google.cloud.netapp.v1.NetApp/DeleteReplication",
                 request_serializer=replication.DeleteReplicationRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_replication"]
 
     @property
     def update_replication(
@@ -1149,15 +1130,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_replication" not in self._stubs:
             self._stubs["update_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateReplication",
+                "/google.cloud.netapp.v1.NetApp/UpdateReplication",
                 request_serializer=gcn_replication.UpdateReplicationRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_replication"]
 
     @property
     def stop_replication(
@@ -1175,15 +1156,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "stop_replication" not in self._stubs:
             self._stubs["stop_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/StopReplication",
+                "/google.cloud.netapp.v1.NetApp/StopReplication",
                 request_serializer=replication.StopReplicationRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["stop_replication"]
 
     @property
     def resume_replication(
@@ -1201,31 +1182,30 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "resume_replication" not in self._stubs:
             self._stubs["resume_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ResumeReplication",
+                "/google.cloud.netapp.v1.NetApp/ResumeReplication",
                 request_serializer=replication.ResumeReplicationRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["resume_replication"]
 
     @property
     def reverse_replication_direction(
         self,
     ) -> Callable[
         [replication.ReverseReplicationDirectionRequest], operations_pb2.Operation
     ]:
         r"""Return a callable for the reverse replication direction method over gRPC.
 
-        ReverseReplicationDirection reverses direction of
-        replication. Source becomes destination and destination
-        becomes source.
+        Reverses direction of replication. Source becomes
+        destination and destination becomes source.
 
         Returns:
             Callable[[~.ReverseReplicationDirectionRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -1233,128 +1213,22 @@
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "reverse_replication_direction" not in self._stubs:
             self._stubs[
                 "reverse_replication_direction"
             ] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ReverseReplicationDirection",
+                "/google.cloud.netapp.v1.NetApp/ReverseReplicationDirection",
                 request_serializer=replication.ReverseReplicationDirectionRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["reverse_replication_direction"]
 
     def close(self):
         self.grpc_channel.close()
 
     @property
-    def delete_operation(
-        self,
-    ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
-        r"""Return a callable for the delete_operation method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "delete_operation" not in self._stubs:
-            self._stubs["delete_operation"] = self.grpc_channel.unary_unary(
-                "/google.longrunning.Operations/DeleteOperation",
-                request_serializer=operations_pb2.DeleteOperationRequest.SerializeToString,
-                response_deserializer=None,
-            )
-        return self._stubs["delete_operation"]
-
-    @property
-    def cancel_operation(
-        self,
-    ) -> Callable[[operations_pb2.CancelOperationRequest], None]:
-        r"""Return a callable for the cancel_operation method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "cancel_operation" not in self._stubs:
-            self._stubs["cancel_operation"] = self.grpc_channel.unary_unary(
-                "/google.longrunning.Operations/CancelOperation",
-                request_serializer=operations_pb2.CancelOperationRequest.SerializeToString,
-                response_deserializer=None,
-            )
-        return self._stubs["cancel_operation"]
-
-    @property
-    def get_operation(
-        self,
-    ) -> Callable[[operations_pb2.GetOperationRequest], operations_pb2.Operation]:
-        r"""Return a callable for the get_operation method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "get_operation" not in self._stubs:
-            self._stubs["get_operation"] = self.grpc_channel.unary_unary(
-                "/google.longrunning.Operations/GetOperation",
-                request_serializer=operations_pb2.GetOperationRequest.SerializeToString,
-                response_deserializer=operations_pb2.Operation.FromString,
-            )
-        return self._stubs["get_operation"]
-
-    @property
-    def list_operations(
-        self,
-    ) -> Callable[
-        [operations_pb2.ListOperationsRequest], operations_pb2.ListOperationsResponse
-    ]:
-        r"""Return a callable for the list_operations method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "list_operations" not in self._stubs:
-            self._stubs["list_operations"] = self.grpc_channel.unary_unary(
-                "/google.longrunning.Operations/ListOperations",
-                request_serializer=operations_pb2.ListOperationsRequest.SerializeToString,
-                response_deserializer=operations_pb2.ListOperationsResponse.FromString,
-            )
-        return self._stubs["list_operations"]
-
-    @property
-    def list_locations(
-        self,
-    ) -> Callable[
-        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
-    ]:
-        r"""Return a callable for the list locations method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "list_locations" not in self._stubs:
-            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
-                "/google.cloud.location.Locations/ListLocations",
-                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
-                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
-            )
-        return self._stubs["list_locations"]
-
-    @property
-    def get_location(
-        self,
-    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
-        r"""Return a callable for the list locations method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "get_location" not in self._stubs:
-            self._stubs["get_location"] = self.grpc_channel.unary_unary(
-                "/google.cloud.location.Locations/GetLocation",
-                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
-                response_deserializer=locations_pb2.Location.FromString,
-            )
-        return self._stubs["get_location"]
-
-    @property
     def kind(self) -> str:
         return "grpc"
 
 
 __all__ = ("NetAppGrpcTransport",)
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/grpc_asyncio.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/grpc_asyncio.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.cloud.location import locations_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
-from google.cloud.netapp_v1beta1.types import active_directory as gcn_active_directory
-from google.cloud.netapp_v1beta1.types import active_directory
-from google.cloud.netapp_v1beta1.types import kms
-from google.cloud.netapp_v1beta1.types import replication
-from google.cloud.netapp_v1beta1.types import replication as gcn_replication
-from google.cloud.netapp_v1beta1.types import snapshot
-from google.cloud.netapp_v1beta1.types import snapshot as gcn_snapshot
-from google.cloud.netapp_v1beta1.types import storage_pool
-from google.cloud.netapp_v1beta1.types import storage_pool as gcn_storage_pool
-from google.cloud.netapp_v1beta1.types import volume
-from google.cloud.netapp_v1beta1.types import volume as gcn_volume
+from google.cloud.netapp_v1.types import active_directory as gcn_active_directory
+from google.cloud.netapp_v1.types import active_directory
+from google.cloud.netapp_v1.types import kms
+from google.cloud.netapp_v1.types import replication
+from google.cloud.netapp_v1.types import replication as gcn_replication
+from google.cloud.netapp_v1.types import snapshot
+from google.cloud.netapp_v1.types import snapshot as gcn_snapshot
+from google.cloud.netapp_v1.types import storage_pool
+from google.cloud.netapp_v1.types import storage_pool as gcn_storage_pool
+from google.cloud.netapp_v1.types import volume
+from google.cloud.netapp_v1.types import volume as gcn_volume
 
 from .base import DEFAULT_CLIENT_INFO, NetAppTransport
 from .grpc import NetAppGrpcTransport
 
 
 class NetAppGrpcAsyncIOTransport(NetAppTransport):
     """gRPC AsyncIO backend transport for NetApp.
@@ -265,133 +265,129 @@
         self,
     ) -> Callable[
         [storage_pool.ListStoragePoolsRequest],
         Awaitable[storage_pool.ListStoragePoolsResponse],
     ]:
         r"""Return a callable for the list storage pools method over gRPC.
 
-        ListStoragePools
-        Returns descriptions of all storage pools owned by the
-        caller.
+        Returns descriptions of all storage pools owned by
+        the caller.
 
         Returns:
             Callable[[~.ListStoragePoolsRequest],
                     Awaitable[~.ListStoragePoolsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_storage_pools" not in self._stubs:
             self._stubs["list_storage_pools"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListStoragePools",
+                "/google.cloud.netapp.v1.NetApp/ListStoragePools",
                 request_serializer=storage_pool.ListStoragePoolsRequest.serialize,
                 response_deserializer=storage_pool.ListStoragePoolsResponse.deserialize,
             )
         return self._stubs["list_storage_pools"]
 
     @property
     def create_storage_pool(
         self,
     ) -> Callable[
         [gcn_storage_pool.CreateStoragePoolRequest], Awaitable[operations_pb2.Operation]
     ]:
         r"""Return a callable for the create storage pool method over gRPC.
 
-        CreateStoragePool
         Creates a new storage pool.
 
         Returns:
             Callable[[~.CreateStoragePoolRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_storage_pool" not in self._stubs:
             self._stubs["create_storage_pool"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateStoragePool",
+                "/google.cloud.netapp.v1.NetApp/CreateStoragePool",
                 request_serializer=gcn_storage_pool.CreateStoragePoolRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_storage_pool"]
 
     @property
     def get_storage_pool(
         self,
     ) -> Callable[
         [storage_pool.GetStoragePoolRequest], Awaitable[storage_pool.StoragePool]
     ]:
         r"""Return a callable for the get storage pool method over gRPC.
 
-        GetStoragePool
-        Returns the description of the specified storage pool by
-        poolId.
+        Returns the description of the specified storage pool
+        by poolId.
 
         Returns:
             Callable[[~.GetStoragePoolRequest],
                     Awaitable[~.StoragePool]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_storage_pool" not in self._stubs:
             self._stubs["get_storage_pool"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetStoragePool",
+                "/google.cloud.netapp.v1.NetApp/GetStoragePool",
                 request_serializer=storage_pool.GetStoragePoolRequest.serialize,
                 response_deserializer=storage_pool.StoragePool.deserialize,
             )
         return self._stubs["get_storage_pool"]
 
     @property
     def update_storage_pool(
         self,
     ) -> Callable[
         [gcn_storage_pool.UpdateStoragePoolRequest], Awaitable[operations_pb2.Operation]
     ]:
         r"""Return a callable for the update storage pool method over gRPC.
 
-        UpdateStoragePool
-        Updates the storage pool properties with the full spec
+        Updates the storage pool properties with the full
+        spec
 
         Returns:
             Callable[[~.UpdateStoragePoolRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_storage_pool" not in self._stubs:
             self._stubs["update_storage_pool"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateStoragePool",
+                "/google.cloud.netapp.v1.NetApp/UpdateStoragePool",
                 request_serializer=gcn_storage_pool.UpdateStoragePoolRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_storage_pool"]
 
     @property
     def delete_storage_pool(
         self,
     ) -> Callable[
         [storage_pool.DeleteStoragePoolRequest], Awaitable[operations_pb2.Operation]
     ]:
         r"""Return a callable for the delete storage pool method over gRPC.
 
-        DeleteStoragePool
         Warning! This operation will permanently delete the
         storage pool.
 
         Returns:
             Callable[[~.DeleteStoragePoolRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
@@ -399,154 +395,149 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_storage_pool" not in self._stubs:
             self._stubs["delete_storage_pool"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteStoragePool",
+                "/google.cloud.netapp.v1.NetApp/DeleteStoragePool",
                 request_serializer=storage_pool.DeleteStoragePoolRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_storage_pool"]
 
     @property
     def list_volumes(
         self,
     ) -> Callable[[volume.ListVolumesRequest], Awaitable[volume.ListVolumesResponse]]:
         r"""Return a callable for the list volumes method over gRPC.
 
-        ListVolumes
         Lists Volumes in a given project.
 
         Returns:
             Callable[[~.ListVolumesRequest],
                     Awaitable[~.ListVolumesResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_volumes" not in self._stubs:
             self._stubs["list_volumes"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListVolumes",
+                "/google.cloud.netapp.v1.NetApp/ListVolumes",
                 request_serializer=volume.ListVolumesRequest.serialize,
                 response_deserializer=volume.ListVolumesResponse.deserialize,
             )
         return self._stubs["list_volumes"]
 
     @property
     def get_volume(
         self,
     ) -> Callable[[volume.GetVolumeRequest], Awaitable[volume.Volume]]:
         r"""Return a callable for the get volume method over gRPC.
 
-        GetVolume
         Gets details of a single Volume.
 
         Returns:
             Callable[[~.GetVolumeRequest],
                     Awaitable[~.Volume]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_volume" not in self._stubs:
             self._stubs["get_volume"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetVolume",
+                "/google.cloud.netapp.v1.NetApp/GetVolume",
                 request_serializer=volume.GetVolumeRequest.serialize,
                 response_deserializer=volume.Volume.deserialize,
             )
         return self._stubs["get_volume"]
 
     @property
     def create_volume(
         self,
     ) -> Callable[
         [gcn_volume.CreateVolumeRequest], Awaitable[operations_pb2.Operation]
     ]:
         r"""Return a callable for the create volume method over gRPC.
 
-        CreateVolume
         Creates a new Volume in a given project and location.
 
         Returns:
             Callable[[~.CreateVolumeRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_volume" not in self._stubs:
             self._stubs["create_volume"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateVolume",
+                "/google.cloud.netapp.v1.NetApp/CreateVolume",
                 request_serializer=gcn_volume.CreateVolumeRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_volume"]
 
     @property
     def update_volume(
         self,
     ) -> Callable[
         [gcn_volume.UpdateVolumeRequest], Awaitable[operations_pb2.Operation]
     ]:
         r"""Return a callable for the update volume method over gRPC.
 
-        UpdateVolume
         Updates the parameters of a single Volume.
 
         Returns:
             Callable[[~.UpdateVolumeRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_volume" not in self._stubs:
             self._stubs["update_volume"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateVolume",
+                "/google.cloud.netapp.v1.NetApp/UpdateVolume",
                 request_serializer=gcn_volume.UpdateVolumeRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_volume"]
 
     @property
     def delete_volume(
         self,
     ) -> Callable[[volume.DeleteVolumeRequest], Awaitable[operations_pb2.Operation]]:
         r"""Return a callable for the delete volume method over gRPC.
 
-        DeleteVolume
         Deletes a single Volume.
 
         Returns:
             Callable[[~.DeleteVolumeRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_volume" not in self._stubs:
             self._stubs["delete_volume"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteVolume",
+                "/google.cloud.netapp.v1.NetApp/DeleteVolume",
                 request_serializer=volume.DeleteVolumeRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_volume"]
 
     @property
     def revert_volume(
@@ -566,15 +557,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "revert_volume" not in self._stubs:
             self._stubs["revert_volume"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/RevertVolume",
+                "/google.cloud.netapp.v1.NetApp/RevertVolume",
                 request_serializer=volume.RevertVolumeRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["revert_volume"]
 
     @property
     def list_snapshots(
@@ -594,15 +585,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_snapshots" not in self._stubs:
             self._stubs["list_snapshots"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListSnapshots",
+                "/google.cloud.netapp.v1.NetApp/ListSnapshots",
                 request_serializer=snapshot.ListSnapshotsRequest.serialize,
                 response_deserializer=snapshot.ListSnapshotsResponse.deserialize,
             )
         return self._stubs["list_snapshots"]
 
     @property
     def get_snapshot(
@@ -620,15 +611,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_snapshot" not in self._stubs:
             self._stubs["get_snapshot"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetSnapshot",
+                "/google.cloud.netapp.v1.NetApp/GetSnapshot",
                 request_serializer=snapshot.GetSnapshotRequest.serialize,
                 response_deserializer=snapshot.Snapshot.deserialize,
             )
         return self._stubs["get_snapshot"]
 
     @property
     def create_snapshot(
@@ -648,15 +639,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_snapshot" not in self._stubs:
             self._stubs["create_snapshot"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateSnapshot",
+                "/google.cloud.netapp.v1.NetApp/CreateSnapshot",
                 request_serializer=gcn_snapshot.CreateSnapshotRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_snapshot"]
 
     @property
     def delete_snapshot(
@@ -676,15 +667,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_snapshot" not in self._stubs:
             self._stubs["delete_snapshot"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteSnapshot",
+                "/google.cloud.netapp.v1.NetApp/DeleteSnapshot",
                 request_serializer=snapshot.DeleteSnapshotRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_snapshot"]
 
     @property
     def update_snapshot(
@@ -704,75 +695,73 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_snapshot" not in self._stubs:
             self._stubs["update_snapshot"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateSnapshot",
+                "/google.cloud.netapp.v1.NetApp/UpdateSnapshot",
                 request_serializer=gcn_snapshot.UpdateSnapshotRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_snapshot"]
 
     @property
     def list_active_directories(
         self,
     ) -> Callable[
         [active_directory.ListActiveDirectoriesRequest],
         Awaitable[active_directory.ListActiveDirectoriesResponse],
     ]:
         r"""Return a callable for the list active directories method over gRPC.
 
-        ListActiveDirectories
         Lists active directories.
 
         Returns:
             Callable[[~.ListActiveDirectoriesRequest],
                     Awaitable[~.ListActiveDirectoriesResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_active_directories" not in self._stubs:
             self._stubs["list_active_directories"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListActiveDirectories",
+                "/google.cloud.netapp.v1.NetApp/ListActiveDirectories",
                 request_serializer=active_directory.ListActiveDirectoriesRequest.serialize,
                 response_deserializer=active_directory.ListActiveDirectoriesResponse.deserialize,
             )
         return self._stubs["list_active_directories"]
 
     @property
     def get_active_directory(
         self,
     ) -> Callable[
         [active_directory.GetActiveDirectoryRequest],
         Awaitable[active_directory.ActiveDirectory],
     ]:
         r"""Return a callable for the get active directory method over gRPC.
 
-        DescribeActiveDirectory
         Describes a specified active directory.
 
         Returns:
             Callable[[~.GetActiveDirectoryRequest],
                     Awaitable[~.ActiveDirectory]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_active_directory" not in self._stubs:
             self._stubs["get_active_directory"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetActiveDirectory",
+                "/google.cloud.netapp.v1.NetApp/GetActiveDirectory",
                 request_serializer=active_directory.GetActiveDirectoryRequest.serialize,
                 response_deserializer=active_directory.ActiveDirectory.deserialize,
             )
         return self._stubs["get_active_directory"]
 
     @property
     def create_active_directory(
@@ -794,87 +783,84 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_active_directory" not in self._stubs:
             self._stubs["create_active_directory"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateActiveDirectory",
+                "/google.cloud.netapp.v1.NetApp/CreateActiveDirectory",
                 request_serializer=gcn_active_directory.CreateActiveDirectoryRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_active_directory"]
 
     @property
     def update_active_directory(
         self,
     ) -> Callable[
         [gcn_active_directory.UpdateActiveDirectoryRequest],
         Awaitable[operations_pb2.Operation],
     ]:
         r"""Return a callable for the update active directory method over gRPC.
 
-        UpdateActiveDirectory
         Update the parameters of an active directories.
 
         Returns:
             Callable[[~.UpdateActiveDirectoryRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_active_directory" not in self._stubs:
             self._stubs["update_active_directory"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateActiveDirectory",
+                "/google.cloud.netapp.v1.NetApp/UpdateActiveDirectory",
                 request_serializer=gcn_active_directory.UpdateActiveDirectoryRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_active_directory"]
 
     @property
     def delete_active_directory(
         self,
     ) -> Callable[
         [active_directory.DeleteActiveDirectoryRequest],
         Awaitable[operations_pb2.Operation],
     ]:
         r"""Return a callable for the delete active directory method over gRPC.
 
-        DeleteActiveDirectory
         Delete the active directory specified in the request.
 
         Returns:
             Callable[[~.DeleteActiveDirectoryRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_active_directory" not in self._stubs:
             self._stubs["delete_active_directory"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteActiveDirectory",
+                "/google.cloud.netapp.v1.NetApp/DeleteActiveDirectory",
                 request_serializer=active_directory.DeleteActiveDirectoryRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_active_directory"]
 
     @property
     def list_kms_configs(
         self,
     ) -> Callable[[kms.ListKmsConfigsRequest], Awaitable[kms.ListKmsConfigsResponse]]:
         r"""Return a callable for the list kms configs method over gRPC.
 
-        ListKmsConfigs
         Returns descriptions of all KMS configs owned by the
         caller.
 
         Returns:
             Callable[[~.ListKmsConfigsRequest],
                     Awaitable[~.ListKmsConfigsResponse]]:
                 A function that, when called, will call the underlying RPC
@@ -882,108 +868,105 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_kms_configs" not in self._stubs:
             self._stubs["list_kms_configs"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListKmsConfigs",
+                "/google.cloud.netapp.v1.NetApp/ListKmsConfigs",
                 request_serializer=kms.ListKmsConfigsRequest.serialize,
                 response_deserializer=kms.ListKmsConfigsResponse.deserialize,
             )
         return self._stubs["list_kms_configs"]
 
     @property
     def create_kms_config(
         self,
     ) -> Callable[[kms.CreateKmsConfigRequest], Awaitable[operations_pb2.Operation]]:
         r"""Return a callable for the create kms config method over gRPC.
 
-        CreateKmsConfig
         Creates a new KMS config.
 
         Returns:
             Callable[[~.CreateKmsConfigRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_kms_config" not in self._stubs:
             self._stubs["create_kms_config"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateKmsConfig",
+                "/google.cloud.netapp.v1.NetApp/CreateKmsConfig",
                 request_serializer=kms.CreateKmsConfigRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_kms_config"]
 
     @property
     def get_kms_config(
         self,
     ) -> Callable[[kms.GetKmsConfigRequest], Awaitable[kms.KmsConfig]]:
         r"""Return a callable for the get kms config method over gRPC.
 
-        GetKmsConfig Returns the description of the specified KMS config
-        by kms_config_id.
+        Returns the description of the specified KMS config by
+        kms_config_id.
 
         Returns:
             Callable[[~.GetKmsConfigRequest],
                     Awaitable[~.KmsConfig]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_kms_config" not in self._stubs:
             self._stubs["get_kms_config"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetKmsConfig",
+                "/google.cloud.netapp.v1.NetApp/GetKmsConfig",
                 request_serializer=kms.GetKmsConfigRequest.serialize,
                 response_deserializer=kms.KmsConfig.deserialize,
             )
         return self._stubs["get_kms_config"]
 
     @property
     def update_kms_config(
         self,
     ) -> Callable[[kms.UpdateKmsConfigRequest], Awaitable[operations_pb2.Operation]]:
         r"""Return a callable for the update kms config method over gRPC.
 
-        UpdateKmsConfig
         Updates the Kms config properties with the full spec
 
         Returns:
             Callable[[~.UpdateKmsConfigRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_kms_config" not in self._stubs:
             self._stubs["update_kms_config"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateKmsConfig",
+                "/google.cloud.netapp.v1.NetApp/UpdateKmsConfig",
                 request_serializer=kms.UpdateKmsConfigRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_kms_config"]
 
     @property
     def encrypt_volumes(
         self,
     ) -> Callable[[kms.EncryptVolumesRequest], Awaitable[operations_pb2.Operation]]:
         r"""Return a callable for the encrypt volumes method over gRPC.
 
-        EncryptVolumes
         Encrypt the existing volumes without CMEK encryption
         with the desired the KMS config for the whole region.
 
         Returns:
             Callable[[~.EncryptVolumesRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
@@ -991,70 +974,68 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "encrypt_volumes" not in self._stubs:
             self._stubs["encrypt_volumes"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/EncryptVolumes",
+                "/google.cloud.netapp.v1.NetApp/EncryptVolumes",
                 request_serializer=kms.EncryptVolumesRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["encrypt_volumes"]
 
     @property
     def verify_kms_config(
         self,
     ) -> Callable[[kms.VerifyKmsConfigRequest], Awaitable[kms.VerifyKmsConfigResponse]]:
         r"""Return a callable for the verify kms config method over gRPC.
 
-        VerifyKmsConfigRequest
         Verifies KMS config reachability.
 
         Returns:
             Callable[[~.VerifyKmsConfigRequest],
                     Awaitable[~.VerifyKmsConfigResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "verify_kms_config" not in self._stubs:
             self._stubs["verify_kms_config"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/VerifyKmsConfig",
+                "/google.cloud.netapp.v1.NetApp/VerifyKmsConfig",
                 request_serializer=kms.VerifyKmsConfigRequest.serialize,
                 response_deserializer=kms.VerifyKmsConfigResponse.deserialize,
             )
         return self._stubs["verify_kms_config"]
 
     @property
     def delete_kms_config(
         self,
     ) -> Callable[[kms.DeleteKmsConfigRequest], Awaitable[operations_pb2.Operation]]:
         r"""Return a callable for the delete kms config method over gRPC.
 
-        DeleteKmsConfig
-        Warning! This operation will permanently delete the Kms
-        config.
+        Warning! This operation will permanently delete the
+        Kms config.
 
         Returns:
             Callable[[~.DeleteKmsConfigRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_kms_config" not in self._stubs:
             self._stubs["delete_kms_config"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteKmsConfig",
+                "/google.cloud.netapp.v1.NetApp/DeleteKmsConfig",
                 request_serializer=kms.DeleteKmsConfigRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_kms_config"]
 
     @property
     def list_replications(
@@ -1076,15 +1057,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "list_replications" not in self._stubs:
             self._stubs["list_replications"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ListReplications",
+                "/google.cloud.netapp.v1.NetApp/ListReplications",
                 request_serializer=replication.ListReplicationsRequest.serialize,
                 response_deserializer=replication.ListReplicationsResponse.deserialize,
             )
         return self._stubs["list_replications"]
 
     @property
     def get_replication(
@@ -1104,15 +1085,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "get_replication" not in self._stubs:
             self._stubs["get_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/GetReplication",
+                "/google.cloud.netapp.v1.NetApp/GetReplication",
                 request_serializer=replication.GetReplicationRequest.serialize,
                 response_deserializer=replication.Replication.deserialize,
             )
         return self._stubs["get_replication"]
 
     @property
     def create_replication(
@@ -1132,15 +1113,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "create_replication" not in self._stubs:
             self._stubs["create_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/CreateReplication",
+                "/google.cloud.netapp.v1.NetApp/CreateReplication",
                 request_serializer=gcn_replication.CreateReplicationRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_replication"]
 
     @property
     def delete_replication(
@@ -1160,15 +1141,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "delete_replication" not in self._stubs:
             self._stubs["delete_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/DeleteReplication",
+                "/google.cloud.netapp.v1.NetApp/DeleteReplication",
                 request_serializer=replication.DeleteReplicationRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_replication"]
 
     @property
     def update_replication(
@@ -1188,15 +1169,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "update_replication" not in self._stubs:
             self._stubs["update_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/UpdateReplication",
+                "/google.cloud.netapp.v1.NetApp/UpdateReplication",
                 request_serializer=gcn_replication.UpdateReplicationRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_replication"]
 
     @property
     def stop_replication(
@@ -1216,15 +1197,15 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "stop_replication" not in self._stubs:
             self._stubs["stop_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/StopReplication",
+                "/google.cloud.netapp.v1.NetApp/StopReplication",
                 request_serializer=replication.StopReplicationRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["stop_replication"]
 
     @property
     def resume_replication(
@@ -1244,32 +1225,31 @@
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "resume_replication" not in self._stubs:
             self._stubs["resume_replication"] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ResumeReplication",
+                "/google.cloud.netapp.v1.NetApp/ResumeReplication",
                 request_serializer=replication.ResumeReplicationRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["resume_replication"]
 
     @property
     def reverse_replication_direction(
         self,
     ) -> Callable[
         [replication.ReverseReplicationDirectionRequest],
         Awaitable[operations_pb2.Operation],
     ]:
         r"""Return a callable for the reverse replication direction method over gRPC.
 
-        ReverseReplicationDirection reverses direction of
-        replication. Source becomes destination and destination
-        becomes source.
+        Reverses direction of replication. Source becomes
+        destination and destination becomes source.
 
         Returns:
             Callable[[~.ReverseReplicationDirectionRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -1277,124 +1257,18 @@
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
         if "reverse_replication_direction" not in self._stubs:
             self._stubs[
                 "reverse_replication_direction"
             ] = self.grpc_channel.unary_unary(
-                "/google.cloud.netapp.v1beta1.NetApp/ReverseReplicationDirection",
+                "/google.cloud.netapp.v1.NetApp/ReverseReplicationDirection",
                 request_serializer=replication.ReverseReplicationDirectionRequest.serialize,
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["reverse_replication_direction"]
 
     def close(self):
         return self.grpc_channel.close()
 
-    @property
-    def delete_operation(
-        self,
-    ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
-        r"""Return a callable for the delete_operation method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "delete_operation" not in self._stubs:
-            self._stubs["delete_operation"] = self.grpc_channel.unary_unary(
-                "/google.longrunning.Operations/DeleteOperation",
-                request_serializer=operations_pb2.DeleteOperationRequest.SerializeToString,
-                response_deserializer=None,
-            )
-        return self._stubs["delete_operation"]
-
-    @property
-    def cancel_operation(
-        self,
-    ) -> Callable[[operations_pb2.CancelOperationRequest], None]:
-        r"""Return a callable for the cancel_operation method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "cancel_operation" not in self._stubs:
-            self._stubs["cancel_operation"] = self.grpc_channel.unary_unary(
-                "/google.longrunning.Operations/CancelOperation",
-                request_serializer=operations_pb2.CancelOperationRequest.SerializeToString,
-                response_deserializer=None,
-            )
-        return self._stubs["cancel_operation"]
-
-    @property
-    def get_operation(
-        self,
-    ) -> Callable[[operations_pb2.GetOperationRequest], operations_pb2.Operation]:
-        r"""Return a callable for the get_operation method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "get_operation" not in self._stubs:
-            self._stubs["get_operation"] = self.grpc_channel.unary_unary(
-                "/google.longrunning.Operations/GetOperation",
-                request_serializer=operations_pb2.GetOperationRequest.SerializeToString,
-                response_deserializer=operations_pb2.Operation.FromString,
-            )
-        return self._stubs["get_operation"]
-
-    @property
-    def list_operations(
-        self,
-    ) -> Callable[
-        [operations_pb2.ListOperationsRequest], operations_pb2.ListOperationsResponse
-    ]:
-        r"""Return a callable for the list_operations method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "list_operations" not in self._stubs:
-            self._stubs["list_operations"] = self.grpc_channel.unary_unary(
-                "/google.longrunning.Operations/ListOperations",
-                request_serializer=operations_pb2.ListOperationsRequest.SerializeToString,
-                response_deserializer=operations_pb2.ListOperationsResponse.FromString,
-            )
-        return self._stubs["list_operations"]
-
-    @property
-    def list_locations(
-        self,
-    ) -> Callable[
-        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
-    ]:
-        r"""Return a callable for the list locations method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "list_locations" not in self._stubs:
-            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
-                "/google.cloud.location.Locations/ListLocations",
-                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
-                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
-            )
-        return self._stubs["list_locations"]
-
-    @property
-    def get_location(
-        self,
-    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
-        r"""Return a callable for the list locations method over gRPC."""
-        # Generate a "stub function" on-the-fly which will actually make
-        # the request.
-        # gRPC handles serialization and deserialization, so we just need
-        # to pass in the functions for each.
-        if "get_location" not in self._stubs:
-            self._stubs["get_location"] = self.grpc_channel.unary_unary(
-                "/google.cloud.location.Locations/GetLocation",
-                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
-                response_deserializer=locations_pb2.Location.FromString,
-            )
-        return self._stubs["get_location"]
-
 
 __all__ = ("NetAppGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/services/net_app/transports/rest.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/services/net_app/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,25 @@
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 
 from google.longrunning import operations_pb2  # type: ignore
 
-from google.cloud.netapp_v1beta1.types import active_directory as gcn_active_directory
-from google.cloud.netapp_v1beta1.types import active_directory
-from google.cloud.netapp_v1beta1.types import kms
-from google.cloud.netapp_v1beta1.types import replication
-from google.cloud.netapp_v1beta1.types import replication as gcn_replication
-from google.cloud.netapp_v1beta1.types import snapshot
-from google.cloud.netapp_v1beta1.types import snapshot as gcn_snapshot
-from google.cloud.netapp_v1beta1.types import storage_pool
-from google.cloud.netapp_v1beta1.types import storage_pool as gcn_storage_pool
-from google.cloud.netapp_v1beta1.types import volume
-from google.cloud.netapp_v1beta1.types import volume as gcn_volume
+from google.cloud.netapp_v1.types import active_directory as gcn_active_directory
+from google.cloud.netapp_v1.types import active_directory
+from google.cloud.netapp_v1.types import kms
+from google.cloud.netapp_v1.types import replication
+from google.cloud.netapp_v1.types import replication as gcn_replication
+from google.cloud.netapp_v1.types import snapshot
+from google.cloud.netapp_v1.types import snapshot as gcn_snapshot
+from google.cloud.netapp_v1.types import storage_pool
+from google.cloud.netapp_v1.types import storage_pool as gcn_storage_pool
+from google.cloud.netapp_v1.types import volume
+from google.cloud.netapp_v1.types import volume as gcn_volume
 
 from .base import DEFAULT_CLIENT_INFO as BASE_DEFAULT_CLIENT_INFO
 from .base import NetAppTransport
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=BASE_DEFAULT_CLIENT_INFO.gapic_version,
     grpc_version=None,
@@ -1181,148 +1181,14 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the NetApp server but before
         it is returned to user code.
         """
         return response
 
-    def pre_get_location(
-        self,
-        request: locations_pb2.GetLocationRequest,
-        metadata: Sequence[Tuple[str, str]],
-    ) -> Tuple[locations_pb2.GetLocationRequest, Sequence[Tuple[str, str]]]:
-        """Pre-rpc interceptor for get_location
-
-        Override in a subclass to manipulate the request or metadata
-        before they are sent to the NetApp server.
-        """
-        return request, metadata
-
-    def post_get_location(
-        self, response: locations_pb2.Location
-    ) -> locations_pb2.Location:
-        """Post-rpc interceptor for get_location
-
-        Override in a subclass to manipulate the response
-        after it is returned by the NetApp server but before
-        it is returned to user code.
-        """
-        return response
-
-    def pre_list_locations(
-        self,
-        request: locations_pb2.ListLocationsRequest,
-        metadata: Sequence[Tuple[str, str]],
-    ) -> Tuple[locations_pb2.ListLocationsRequest, Sequence[Tuple[str, str]]]:
-        """Pre-rpc interceptor for list_locations
-
-        Override in a subclass to manipulate the request or metadata
-        before they are sent to the NetApp server.
-        """
-        return request, metadata
-
-    def post_list_locations(
-        self, response: locations_pb2.ListLocationsResponse
-    ) -> locations_pb2.ListLocationsResponse:
-        """Post-rpc interceptor for list_locations
-
-        Override in a subclass to manipulate the response
-        after it is returned by the NetApp server but before
-        it is returned to user code.
-        """
-        return response
-
-    def pre_cancel_operation(
-        self,
-        request: operations_pb2.CancelOperationRequest,
-        metadata: Sequence[Tuple[str, str]],
-    ) -> Tuple[operations_pb2.CancelOperationRequest, Sequence[Tuple[str, str]]]:
-        """Pre-rpc interceptor for cancel_operation
-
-        Override in a subclass to manipulate the request or metadata
-        before they are sent to the NetApp server.
-        """
-        return request, metadata
-
-    def post_cancel_operation(self, response: None) -> None:
-        """Post-rpc interceptor for cancel_operation
-
-        Override in a subclass to manipulate the response
-        after it is returned by the NetApp server but before
-        it is returned to user code.
-        """
-        return response
-
-    def pre_delete_operation(
-        self,
-        request: operations_pb2.DeleteOperationRequest,
-        metadata: Sequence[Tuple[str, str]],
-    ) -> Tuple[operations_pb2.DeleteOperationRequest, Sequence[Tuple[str, str]]]:
-        """Pre-rpc interceptor for delete_operation
-
-        Override in a subclass to manipulate the request or metadata
-        before they are sent to the NetApp server.
-        """
-        return request, metadata
-
-    def post_delete_operation(self, response: None) -> None:
-        """Post-rpc interceptor for delete_operation
-
-        Override in a subclass to manipulate the response
-        after it is returned by the NetApp server but before
-        it is returned to user code.
-        """
-        return response
-
-    def pre_get_operation(
-        self,
-        request: operations_pb2.GetOperationRequest,
-        metadata: Sequence[Tuple[str, str]],
-    ) -> Tuple[operations_pb2.GetOperationRequest, Sequence[Tuple[str, str]]]:
-        """Pre-rpc interceptor for get_operation
-
-        Override in a subclass to manipulate the request or metadata
-        before they are sent to the NetApp server.
-        """
-        return request, metadata
-
-    def post_get_operation(
-        self, response: operations_pb2.Operation
-    ) -> operations_pb2.Operation:
-        """Post-rpc interceptor for get_operation
-
-        Override in a subclass to manipulate the response
-        after it is returned by the NetApp server but before
-        it is returned to user code.
-        """
-        return response
-
-    def pre_list_operations(
-        self,
-        request: operations_pb2.ListOperationsRequest,
-        metadata: Sequence[Tuple[str, str]],
-    ) -> Tuple[operations_pb2.ListOperationsRequest, Sequence[Tuple[str, str]]]:
-        """Pre-rpc interceptor for list_operations
-
-        Override in a subclass to manipulate the request or metadata
-        before they are sent to the NetApp server.
-        """
-        return request, metadata
-
-    def post_list_operations(
-        self, response: operations_pb2.ListOperationsResponse
-    ) -> operations_pb2.ListOperationsResponse:
-        """Post-rpc interceptor for list_operations
-
-        Override in a subclass to manipulate the response
-        after it is returned by the NetApp server but before
-        it is returned to user code.
-        """
-        return response
-
 
 @dataclasses.dataclass
 class NetAppRestStub:
     _session: AuthorizedSession
     _host: str
     _interceptor: NetAppRestInterceptor
 
@@ -1422,49 +1288,23 @@
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
         # Only create a new client if we do not already have one.
         if self._operations_client is None:
-            http_options: Dict[str, List[Dict[str, str]]] = {
-                "google.longrunning.Operations.CancelOperation": [
-                    {
-                        "method": "post",
-                        "uri": "/v1beta1/{name=projects/*/locations/*/operations/*}:cancel",
-                        "body": "*",
-                    },
-                ],
-                "google.longrunning.Operations.DeleteOperation": [
-                    {
-                        "method": "delete",
-                        "uri": "/v1beta1/{name=projects/*/locations/*/operations/*}",
-                    },
-                ],
-                "google.longrunning.Operations.GetOperation": [
-                    {
-                        "method": "get",
-                        "uri": "/v1beta1/{name=projects/*/locations/*/operations/*}",
-                    },
-                ],
-                "google.longrunning.Operations.ListOperations": [
-                    {
-                        "method": "get",
-                        "uri": "/v1beta1/{name=projects/*/locations/*}/operations",
-                    },
-                ],
-            }
+            http_options: Dict[str, List[Dict[str, str]]] = {}
 
             rest_transport = operations_v1.OperationsRestTransport(
                 host=self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 scopes=self._scopes,
                 http_options=http_options,
-                path_prefix="v1beta1",
+                path_prefix="v1",
             )
 
             self._operations_client = operations_v1.AbstractOperationsClient(
                 transport=rest_transport
             )
 
         # Return the client from cache.
@@ -1513,15 +1353,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*}/activeDirectories",
+                    "uri": "/v1/{parent=projects/*/locations/*}/activeDirectories",
                     "body": "active_directory",
                 },
             ]
             request, metadata = self._interceptor.pre_create_active_directory(
                 request, metadata
             )
             pb_request = gcn_active_directory.CreateActiveDirectoryRequest.pb(request)
@@ -1595,15 +1435,15 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the create kms config method over HTTP.
 
             Args:
                 request (~.kms.CreateKmsConfigRequest):
-                    The request object. CreateKmsConfigRequest
+                    The request object.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1613,15 +1453,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*}/kmsConfigs",
+                    "uri": "/v1/{parent=projects/*/locations/*}/kmsConfigs",
                     "body": "kms_config",
                 },
             ]
             request, metadata = self._interceptor.pre_create_kms_config(
                 request, metadata
             )
             pb_request = kms.CreateKmsConfigRequest.pb(request)
@@ -1714,15 +1554,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*/volumes/*}/replications",
+                    "uri": "/v1/{parent=projects/*/locations/*/volumes/*}/replications",
                     "body": "replication",
                 },
             ]
             request, metadata = self._interceptor.pre_create_replication(
                 request, metadata
             )
             pb_request = gcn_replication.CreateReplicationRequest.pb(request)
@@ -1815,15 +1655,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*/volumes/*}/snapshots",
+                    "uri": "/v1/{parent=projects/*/locations/*/volumes/*}/snapshots",
                     "body": "snapshot",
                 },
             ]
             request, metadata = self._interceptor.pre_create_snapshot(request, metadata)
             pb_request = gcn_snapshot.CreateSnapshotRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -1895,15 +1735,15 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the create storage pool method over HTTP.
 
             Args:
                 request (~.gcn_storage_pool.CreateStoragePoolRequest):
-                    The request object. CreateStoragePoolRequest
+                    The request object.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -1913,15 +1753,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*}/storagePools",
+                    "uri": "/v1/{parent=projects/*/locations/*}/storagePools",
                     "body": "storage_pool",
                 },
             ]
             request, metadata = self._interceptor.pre_create_storage_pool(
                 request, metadata
             )
             pb_request = gcn_storage_pool.CreateStoragePoolRequest.pb(request)
@@ -1995,16 +1835,15 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the create volume method over HTTP.
 
             Args:
                 request (~.gcn_volume.CreateVolumeRequest):
-                    The request object. CreateVolumeRequest
-                Message for creating a Volume
+                    The request object. Message for creating a Volume
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -2014,15 +1853,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*}/volumes",
+                    "uri": "/v1/{parent=projects/*/locations/*}/volumes",
                     "body": "volume",
                 },
             ]
             request, metadata = self._interceptor.pre_create_volume(request, metadata)
             pb_request = gcn_volume.CreateVolumeRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -2111,15 +1950,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/activeDirectories/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/activeDirectories/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_active_directory(
                 request, metadata
             )
             pb_request = active_directory.DeleteActiveDirectoryRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -2182,15 +2021,15 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the delete kms config method over HTTP.
 
             Args:
                 request (~.kms.DeleteKmsConfigRequest):
-                    The request object. DeleteKmsConfigRequest
+                    The request object.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -2200,15 +2039,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/kmsConfigs/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/kmsConfigs/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_kms_config(
                 request, metadata
             )
             pb_request = kms.DeleteKmsConfigRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -2290,15 +2129,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/volumes/*/replications/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/volumes/*/replications/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_replication(
                 request, metadata
             )
             pb_request = replication.DeleteReplicationRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -2380,15 +2219,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/volumes/*/snapshots/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/volumes/*/snapshots/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_snapshot(request, metadata)
             pb_request = snapshot.DeleteSnapshotRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -2449,15 +2288,15 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the delete storage pool method over HTTP.
 
             Args:
                 request (~.storage_pool.DeleteStoragePoolRequest):
-                    The request object. DeleteStoragePoolRequest
+                    The request object.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -2467,15 +2306,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/storagePools/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/storagePools/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_storage_pool(
                 request, metadata
             )
             pb_request = storage_pool.DeleteStoragePoolRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -2538,16 +2377,15 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the delete volume method over HTTP.
 
             Args:
                 request (~.volume.DeleteVolumeRequest):
-                    The request object. DeleteVolumeRequest
-                Message for deleting a Volume
+                    The request object. Message for deleting a Volume
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -2557,15 +2395,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "delete",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/volumes/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/volumes/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_delete_volume(request, metadata)
             pb_request = volume.DeleteVolumeRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -2626,17 +2464,16 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the encrypt volumes method over HTTP.
 
             Args:
                 request (~.kms.EncryptVolumesRequest):
-                    The request object. EncryptVolumesRequest
-                EncryptVolumesRequest specifies the KMS
-                config to encrypt existing volumes.
+                    The request object. EncryptVolumesRequest specifies the
+                KMS config to encrypt existing volumes.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -2646,15 +2483,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/kmsConfigs/*}:encrypt",
+                    "uri": "/v1/{name=projects/*/locations/*/kmsConfigs/*}:encrypt",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_encrypt_volumes(request, metadata)
             pb_request = kms.EncryptVolumesRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -2743,15 +2580,15 @@
                 config.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/activeDirectories/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/activeDirectories/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_active_directory(
                 request, metadata
             )
             pb_request = active_directory.GetActiveDirectoryRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -2816,15 +2653,15 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> kms.KmsConfig:
             r"""Call the get kms config method over HTTP.
 
             Args:
                 request (~.kms.GetKmsConfigRequest):
-                    The request object. GetKmsConfigRequest
+                    The request object.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -2833,15 +2670,15 @@
                 encryption key(CMEK) configuration.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/kmsConfigs/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/kmsConfigs/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_kms_config(request, metadata)
             pb_request = kms.GetKmsConfigRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -2924,15 +2761,15 @@
                 between 2 volumes in different regions.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/volumes/*/replications/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/volumes/*/replications/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_replication(request, metadata)
             pb_request = replication.GetReplicationRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -3005,21 +2842,21 @@
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.snapshot.Snapshot:
-                    Snapshot
+
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/volumes/*/snapshots/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/volumes/*/snapshots/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_snapshot(request, metadata)
             pb_request = snapshot.GetSnapshotRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -3082,38 +2919,36 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> storage_pool.StoragePool:
             r"""Call the get storage pool method over HTTP.
 
             Args:
                 request (~.storage_pool.GetStoragePoolRequest):
-                    The request object. GetStoragePoolRequest
+                    The request object.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.storage_pool.StoragePool:
-                    Resources
-                StoragePool
-                StoragePool is a container for volumes
-                with a service level and capacity.
-                Volumes can be created in a pool of
-                sufficient available capacity.
+                    StoragePool is a container for
+                volumes with a service level and
+                capacity. Volumes can be created in a
+                pool of sufficient available capacity.
                 StoragePool capacity is what you are
                 billed for.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/storagePools/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/storagePools/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_storage_pool(
                 request, metadata
             )
             pb_request = storage_pool.GetStoragePoolRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -3178,34 +3013,32 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> volume.Volume:
             r"""Call the get volume method over HTTP.
 
             Args:
                 request (~.volume.GetVolumeRequest):
-                    The request object. GetVolumeRequest
-                Message for getting a Volume
+                    The request object. Message for getting a Volume
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.volume.Volume:
-                    Volume
-                Volume provides a filesystem that you
+                    Volume provides a filesystem that you
                 can mount.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/volumes/*}",
+                    "uri": "/v1/{name=projects/*/locations/*/volumes/*}",
                 },
             ]
             request, metadata = self._interceptor.pre_get_volume(request, metadata)
             pb_request = volume.GetVolumeRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -3287,15 +3120,15 @@
                 requested.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*}/activeDirectories",
+                    "uri": "/v1/{parent=projects/*/locations/*}/activeDirectories",
                 },
             ]
             request, metadata = self._interceptor.pre_list_active_directories(
                 request, metadata
             )
             pb_request = active_directory.ListActiveDirectoriesRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -3360,30 +3193,30 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> kms.ListKmsConfigsResponse:
             r"""Call the list kms configs method over HTTP.
 
             Args:
                 request (~.kms.ListKmsConfigsRequest):
-                    The request object. ListKmsConfigsRequest
+                    The request object.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.kms.ListKmsConfigsResponse:
-                    ListKmsConfigsResponse
+
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*}/kmsConfigs",
+                    "uri": "/v1/{parent=projects/*/locations/*}/kmsConfigs",
                 },
             ]
             request, metadata = self._interceptor.pre_list_kms_configs(
                 request, metadata
             )
             pb_request = kms.ListKmsConfigsRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -3465,15 +3298,15 @@
                 result of ListReplicationsRequest.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*/volumes/*}/replications",
+                    "uri": "/v1/{parent=projects/*/locations/*/volumes/*}/replications",
                 },
             ]
             request, metadata = self._interceptor.pre_list_replications(
                 request, metadata
             )
             pb_request = replication.ListReplicationsRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -3555,15 +3388,15 @@
                 of ListSnapshotsRequest.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*/volumes/*}/snapshots",
+                    "uri": "/v1/{parent=projects/*/locations/*/volumes/*}/snapshots",
                 },
             ]
             request, metadata = self._interceptor.pre_list_snapshots(request, metadata)
             pb_request = snapshot.ListSnapshotsRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -3626,30 +3459,30 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> storage_pool.ListStoragePoolsResponse:
             r"""Call the list storage pools method over HTTP.
 
             Args:
                 request (~.storage_pool.ListStoragePoolsRequest):
-                    The request object. ListStoragePoolsRequest
+                    The request object.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.storage_pool.ListStoragePoolsResponse:
-                    ListStoragePoolsResponse
+
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*}/storagePools",
+                    "uri": "/v1/{parent=projects/*/locations/*}/storagePools",
                 },
             ]
             request, metadata = self._interceptor.pre_list_storage_pools(
                 request, metadata
             )
             pb_request = storage_pool.ListStoragePoolsRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
@@ -3714,33 +3547,33 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> volume.ListVolumesResponse:
             r"""Call the list volumes method over HTTP.
 
             Args:
                 request (~.volume.ListVolumesRequest):
-                    The request object. ListVolumesRequest
-                Message for requesting list of Volumes
+                    The request object. Message for requesting list of
+                Volumes
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.volume.ListVolumesResponse:
-                    ListVolumesResponse
-                Message for response to listing Volumes
+                    Message for response to listing
+                Volumes
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
-                    "uri": "/v1beta1/{parent=projects/*/locations/*}/volumes",
+                    "uri": "/v1/{parent=projects/*/locations/*}/volumes",
                 },
             ]
             request, metadata = self._interceptor.pre_list_volumes(request, metadata)
             pb_request = volume.ListVolumesRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
@@ -3822,15 +3655,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/volumes/*/replications/*}:resume",
+                    "uri": "/v1/{name=projects/*/locations/*/volumes/*/replications/*}:resume",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_resume_replication(
                 request, metadata
             )
             pb_request = replication.ResumeReplicationRequest.pb(request)
@@ -3924,15 +3757,15 @@
                     result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/volumes/*/replications/*}:reverseDirection",
+                    "uri": "/v1/{name=projects/*/locations/*/volumes/*/replications/*}:reverseDirection",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_reverse_replication_direction(
                 request, metadata
             )
             pb_request = replication.ReverseReplicationDirectionRequest.pb(request)
@@ -4023,15 +3856,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/volumes/*}:revert",
+                    "uri": "/v1/{name=projects/*/locations/*/volumes/*}:revert",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_revert_volume(request, metadata)
             pb_request = volume.RevertVolumeRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -4120,15 +3953,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/volumes/*/replications/*}:stop",
+                    "uri": "/v1/{name=projects/*/locations/*/volumes/*/replications/*}:stop",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_stop_replication(
                 request, metadata
             )
             pb_request = replication.StopReplicationRequest.pb(request)
@@ -4221,15 +4054,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1beta1/{active_directory.name=projects/*/locations/*/activeDirectories/*}",
+                    "uri": "/v1/{active_directory.name=projects/*/locations/*/activeDirectories/*}",
                     "body": "active_directory",
                 },
             ]
             request, metadata = self._interceptor.pre_update_active_directory(
                 request, metadata
             )
             pb_request = gcn_active_directory.UpdateActiveDirectoryRequest.pb(request)
@@ -4303,15 +4136,15 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the update kms config method over HTTP.
 
             Args:
                 request (~.kms.UpdateKmsConfigRequest):
-                    The request object. UpdateKmsConfigRequest
+                    The request object.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -4321,15 +4154,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1beta1/{kms_config.name=projects/*/locations/*/kmsConfigs/*}",
+                    "uri": "/v1/{kms_config.name=projects/*/locations/*/kmsConfigs/*}",
                     "body": "kms_config",
                 },
             ]
             request, metadata = self._interceptor.pre_update_kms_config(
                 request, metadata
             )
             pb_request = kms.UpdateKmsConfigRequest.pb(request)
@@ -4423,15 +4256,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1beta1/{replication.name=projects/*/locations/*/volumes/*/replications/*}",
+                    "uri": "/v1/{replication.name=projects/*/locations/*/volumes/*/replications/*}",
                     "body": "replication",
                 },
             ]
             request, metadata = self._interceptor.pre_update_replication(
                 request, metadata
             )
             pb_request = gcn_replication.UpdateReplicationRequest.pb(request)
@@ -4525,15 +4358,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1beta1/{snapshot.name=projects/*/locations/*/volumes/*/snapshots/*}",
+                    "uri": "/v1/{snapshot.name=projects/*/locations/*/volumes/*/snapshots/*}",
                     "body": "snapshot",
                 },
             ]
             request, metadata = self._interceptor.pre_update_snapshot(request, metadata)
             pb_request = gcn_snapshot.UpdateSnapshotRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -4605,15 +4438,15 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the update storage pool method over HTTP.
 
             Args:
                 request (~.gcn_storage_pool.UpdateStoragePoolRequest):
-                    The request object. UpdateStoragePoolRequest
+                    The request object.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -4623,15 +4456,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1beta1/{storage_pool.name=projects/*/locations/*/storagePools/*}",
+                    "uri": "/v1/{storage_pool.name=projects/*/locations/*/storagePools/*}",
                     "body": "storage_pool",
                 },
             ]
             request, metadata = self._interceptor.pre_update_storage_pool(
                 request, metadata
             )
             pb_request = gcn_storage_pool.UpdateStoragePoolRequest.pb(request)
@@ -4705,16 +4538,15 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> operations_pb2.Operation:
             r"""Call the update volume method over HTTP.
 
             Args:
                 request (~.gcn_volume.UpdateVolumeRequest):
-                    The request object. UpdateVolumeRequest
-                Message for updating a Volume
+                    The request object. Message for updating a Volume
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
@@ -4724,15 +4556,15 @@
                 result of a network API call.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
-                    "uri": "/v1beta1/{volume.name=projects/*/locations/*/volumes/*}",
+                    "uri": "/v1/{volume.name=projects/*/locations/*/volumes/*}",
                     "body": "volume",
                 },
             ]
             request, metadata = self._interceptor.pre_update_volume(request, metadata)
             pb_request = gcn_volume.UpdateVolumeRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
@@ -4802,36 +4634,34 @@
             timeout: Optional[float] = None,
             metadata: Sequence[Tuple[str, str]] = (),
         ) -> kms.VerifyKmsConfigResponse:
             r"""Call the verify kms config method over HTTP.
 
             Args:
                 request (~.kms.VerifyKmsConfigRequest):
-                    The request object. VerifyKmsConfigRequest
-                VerifyKmsConfigRequest specifies the KMS
-                config to be validated.
+                    The request object. VerifyKmsConfigRequest specifies the
+                KMS config to be validated.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.kms.VerifyKmsConfigResponse:
-                    VerifyKmsConfigResponse
-                VerifyKmsConfigResponse contains the
+                    VerifyKmsConfigResponse contains the
                 information if the config is correctly
                 and error message.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/kmsConfigs/*}:verify",
+                    "uri": "/v1/{name=projects/*/locations/*/kmsConfigs/*}:verify",
                     "body": "*",
                 },
             ]
             request, metadata = self._interceptor.pre_verify_kms_config(
                 request, metadata
             )
             pb_request = kms.VerifyKmsConfigRequest.pb(request)
@@ -5185,411 +5015,14 @@
         self,
     ) -> Callable[[kms.VerifyKmsConfigRequest], kms.VerifyKmsConfigResponse]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._VerifyKmsConfig(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
-    def get_location(self):
-        return self._GetLocation(self._session, self._host, self._interceptor)  # type: ignore
-
-    class _GetLocation(NetAppRestStub):
-        def __call__(
-            self,
-            request: locations_pb2.GetLocationRequest,
-            *,
-            retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: Optional[float] = None,
-            metadata: Sequence[Tuple[str, str]] = (),
-        ) -> locations_pb2.Location:
-
-            r"""Call the get location method over HTTP.
-
-            Args:
-                request (locations_pb2.GetLocationRequest):
-                    The request object for GetLocation method.
-                retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                    should be retried.
-                timeout (float): The timeout for this request.
-                metadata (Sequence[Tuple[str, str]]): Strings which should be
-                    sent along with the request as metadata.
-
-            Returns:
-                locations_pb2.Location: Response from GetLocation method.
-            """
-
-            http_options: List[Dict[str, str]] = [
-                {
-                    "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*}",
-                },
-            ]
-
-            request, metadata = self._interceptor.pre_get_location(request, metadata)
-            request_kwargs = json_format.MessageToDict(request)
-            transcoded_request = path_template.transcode(http_options, **request_kwargs)
-
-            uri = transcoded_request["uri"]
-            method = transcoded_request["method"]
-
-            # Jsonify the query params
-            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
-
-            # Send the request
-            headers = dict(metadata)
-            headers["Content-Type"] = "application/json"
-
-            response = getattr(self._session, method)(
-                "{host}{uri}".format(host=self._host, uri=uri),
-                timeout=timeout,
-                headers=headers,
-                params=rest_helpers.flatten_query_params(query_params),
-            )
-
-            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
-            # subclass.
-            if response.status_code >= 400:
-                raise core_exceptions.from_http_response(response)
-
-            resp = locations_pb2.Location()
-            resp = json_format.Parse(response.content.decode("utf-8"), resp)
-            resp = self._interceptor.post_get_location(resp)
-            return resp
-
-    @property
-    def list_locations(self):
-        return self._ListLocations(self._session, self._host, self._interceptor)  # type: ignore
-
-    class _ListLocations(NetAppRestStub):
-        def __call__(
-            self,
-            request: locations_pb2.ListLocationsRequest,
-            *,
-            retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: Optional[float] = None,
-            metadata: Sequence[Tuple[str, str]] = (),
-        ) -> locations_pb2.ListLocationsResponse:
-
-            r"""Call the list locations method over HTTP.
-
-            Args:
-                request (locations_pb2.ListLocationsRequest):
-                    The request object for ListLocations method.
-                retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                    should be retried.
-                timeout (float): The timeout for this request.
-                metadata (Sequence[Tuple[str, str]]): Strings which should be
-                    sent along with the request as metadata.
-
-            Returns:
-                locations_pb2.ListLocationsResponse: Response from ListLocations method.
-            """
-
-            http_options: List[Dict[str, str]] = [
-                {
-                    "method": "get",
-                    "uri": "/v1beta1/{name=projects/*}/locations",
-                },
-            ]
-
-            request, metadata = self._interceptor.pre_list_locations(request, metadata)
-            request_kwargs = json_format.MessageToDict(request)
-            transcoded_request = path_template.transcode(http_options, **request_kwargs)
-
-            uri = transcoded_request["uri"]
-            method = transcoded_request["method"]
-
-            # Jsonify the query params
-            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
-
-            # Send the request
-            headers = dict(metadata)
-            headers["Content-Type"] = "application/json"
-
-            response = getattr(self._session, method)(
-                "{host}{uri}".format(host=self._host, uri=uri),
-                timeout=timeout,
-                headers=headers,
-                params=rest_helpers.flatten_query_params(query_params),
-            )
-
-            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
-            # subclass.
-            if response.status_code >= 400:
-                raise core_exceptions.from_http_response(response)
-
-            resp = locations_pb2.ListLocationsResponse()
-            resp = json_format.Parse(response.content.decode("utf-8"), resp)
-            resp = self._interceptor.post_list_locations(resp)
-            return resp
-
-    @property
-    def cancel_operation(self):
-        return self._CancelOperation(self._session, self._host, self._interceptor)  # type: ignore
-
-    class _CancelOperation(NetAppRestStub):
-        def __call__(
-            self,
-            request: operations_pb2.CancelOperationRequest,
-            *,
-            retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: Optional[float] = None,
-            metadata: Sequence[Tuple[str, str]] = (),
-        ) -> None:
-
-            r"""Call the cancel operation method over HTTP.
-
-            Args:
-                request (operations_pb2.CancelOperationRequest):
-                    The request object for CancelOperation method.
-                retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                    should be retried.
-                timeout (float): The timeout for this request.
-                metadata (Sequence[Tuple[str, str]]): Strings which should be
-                    sent along with the request as metadata.
-            """
-
-            http_options: List[Dict[str, str]] = [
-                {
-                    "method": "post",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/operations/*}:cancel",
-                    "body": "*",
-                },
-            ]
-
-            request, metadata = self._interceptor.pre_cancel_operation(
-                request, metadata
-            )
-            request_kwargs = json_format.MessageToDict(request)
-            transcoded_request = path_template.transcode(http_options, **request_kwargs)
-
-            body = json.dumps(transcoded_request["body"])
-            uri = transcoded_request["uri"]
-            method = transcoded_request["method"]
-
-            # Jsonify the query params
-            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
-
-            # Send the request
-            headers = dict(metadata)
-            headers["Content-Type"] = "application/json"
-
-            response = getattr(self._session, method)(
-                "{host}{uri}".format(host=self._host, uri=uri),
-                timeout=timeout,
-                headers=headers,
-                params=rest_helpers.flatten_query_params(query_params),
-                data=body,
-            )
-
-            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
-            # subclass.
-            if response.status_code >= 400:
-                raise core_exceptions.from_http_response(response)
-
-            return self._interceptor.post_cancel_operation(None)
-
-    @property
-    def delete_operation(self):
-        return self._DeleteOperation(self._session, self._host, self._interceptor)  # type: ignore
-
-    class _DeleteOperation(NetAppRestStub):
-        def __call__(
-            self,
-            request: operations_pb2.DeleteOperationRequest,
-            *,
-            retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: Optional[float] = None,
-            metadata: Sequence[Tuple[str, str]] = (),
-        ) -> None:
-
-            r"""Call the delete operation method over HTTP.
-
-            Args:
-                request (operations_pb2.DeleteOperationRequest):
-                    The request object for DeleteOperation method.
-                retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                    should be retried.
-                timeout (float): The timeout for this request.
-                metadata (Sequence[Tuple[str, str]]): Strings which should be
-                    sent along with the request as metadata.
-            """
-
-            http_options: List[Dict[str, str]] = [
-                {
-                    "method": "delete",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/operations/*}",
-                },
-            ]
-
-            request, metadata = self._interceptor.pre_delete_operation(
-                request, metadata
-            )
-            request_kwargs = json_format.MessageToDict(request)
-            transcoded_request = path_template.transcode(http_options, **request_kwargs)
-
-            uri = transcoded_request["uri"]
-            method = transcoded_request["method"]
-
-            # Jsonify the query params
-            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
-
-            # Send the request
-            headers = dict(metadata)
-            headers["Content-Type"] = "application/json"
-
-            response = getattr(self._session, method)(
-                "{host}{uri}".format(host=self._host, uri=uri),
-                timeout=timeout,
-                headers=headers,
-                params=rest_helpers.flatten_query_params(query_params),
-            )
-
-            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
-            # subclass.
-            if response.status_code >= 400:
-                raise core_exceptions.from_http_response(response)
-
-            return self._interceptor.post_delete_operation(None)
-
-    @property
-    def get_operation(self):
-        return self._GetOperation(self._session, self._host, self._interceptor)  # type: ignore
-
-    class _GetOperation(NetAppRestStub):
-        def __call__(
-            self,
-            request: operations_pb2.GetOperationRequest,
-            *,
-            retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: Optional[float] = None,
-            metadata: Sequence[Tuple[str, str]] = (),
-        ) -> operations_pb2.Operation:
-
-            r"""Call the get operation method over HTTP.
-
-            Args:
-                request (operations_pb2.GetOperationRequest):
-                    The request object for GetOperation method.
-                retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                    should be retried.
-                timeout (float): The timeout for this request.
-                metadata (Sequence[Tuple[str, str]]): Strings which should be
-                    sent along with the request as metadata.
-
-            Returns:
-                operations_pb2.Operation: Response from GetOperation method.
-            """
-
-            http_options: List[Dict[str, str]] = [
-                {
-                    "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*/operations/*}",
-                },
-            ]
-
-            request, metadata = self._interceptor.pre_get_operation(request, metadata)
-            request_kwargs = json_format.MessageToDict(request)
-            transcoded_request = path_template.transcode(http_options, **request_kwargs)
-
-            uri = transcoded_request["uri"]
-            method = transcoded_request["method"]
-
-            # Jsonify the query params
-            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
-
-            # Send the request
-            headers = dict(metadata)
-            headers["Content-Type"] = "application/json"
-
-            response = getattr(self._session, method)(
-                "{host}{uri}".format(host=self._host, uri=uri),
-                timeout=timeout,
-                headers=headers,
-                params=rest_helpers.flatten_query_params(query_params),
-            )
-
-            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
-            # subclass.
-            if response.status_code >= 400:
-                raise core_exceptions.from_http_response(response)
-
-            resp = operations_pb2.Operation()
-            resp = json_format.Parse(response.content.decode("utf-8"), resp)
-            resp = self._interceptor.post_get_operation(resp)
-            return resp
-
-    @property
-    def list_operations(self):
-        return self._ListOperations(self._session, self._host, self._interceptor)  # type: ignore
-
-    class _ListOperations(NetAppRestStub):
-        def __call__(
-            self,
-            request: operations_pb2.ListOperationsRequest,
-            *,
-            retry: OptionalRetry = gapic_v1.method.DEFAULT,
-            timeout: Optional[float] = None,
-            metadata: Sequence[Tuple[str, str]] = (),
-        ) -> operations_pb2.ListOperationsResponse:
-
-            r"""Call the list operations method over HTTP.
-
-            Args:
-                request (operations_pb2.ListOperationsRequest):
-                    The request object for ListOperations method.
-                retry (google.api_core.retry.Retry): Designation of what errors, if any,
-                    should be retried.
-                timeout (float): The timeout for this request.
-                metadata (Sequence[Tuple[str, str]]): Strings which should be
-                    sent along with the request as metadata.
-
-            Returns:
-                operations_pb2.ListOperationsResponse: Response from ListOperations method.
-            """
-
-            http_options: List[Dict[str, str]] = [
-                {
-                    "method": "get",
-                    "uri": "/v1beta1/{name=projects/*/locations/*}/operations",
-                },
-            ]
-
-            request, metadata = self._interceptor.pre_list_operations(request, metadata)
-            request_kwargs = json_format.MessageToDict(request)
-            transcoded_request = path_template.transcode(http_options, **request_kwargs)
-
-            uri = transcoded_request["uri"]
-            method = transcoded_request["method"]
-
-            # Jsonify the query params
-            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
-
-            # Send the request
-            headers = dict(metadata)
-            headers["Content-Type"] = "application/json"
-
-            response = getattr(self._session, method)(
-                "{host}{uri}".format(host=self._host, uri=uri),
-                timeout=timeout,
-                headers=headers,
-                params=rest_helpers.flatten_query_params(query_params),
-            )
-
-            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
-            # subclass.
-            if response.status_code >= 400:
-                raise core_exceptions.from_http_response(response)
-
-            resp = operations_pb2.ListOperationsResponse()
-            resp = json_format.Parse(response.content.decode("utf-8"), resp)
-            resp = self._interceptor.post_list_operations(resp)
-            return resp
-
-    @property
     def kind(self) -> str:
         return "rest"
 
     def close(self):
         self._session.close()
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/__init__.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/active_directory.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/active_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.cloud.netapp.v1beta1",
+    package="google.cloud.netapp.v1",
     manifest={
         "ListActiveDirectoriesRequest",
         "ListActiveDirectoriesResponse",
         "GetActiveDirectoryRequest",
         "CreateActiveDirectoryRequest",
         "UpdateActiveDirectoryRequest",
         "DeleteActiveDirectoryRequest",
@@ -79,15 +79,15 @@
 
 
 class ListActiveDirectoriesResponse(proto.Message):
     r"""ListActiveDirectoriesResponse contains all the active
     directories requested.
 
     Attributes:
-        active_directories (MutableSequence[google.cloud.netapp_v1beta1.types.ActiveDirectory]):
+        active_directories (MutableSequence[google.cloud.netapp_v1.types.ActiveDirectory]):
             The list of active directories.
         next_page_token (str):
             A token identifying a page of results the
             server should return.
         unreachable (MutableSequence[str]):
             Locations that could not be reached.
     """
@@ -128,15 +128,15 @@
 class CreateActiveDirectoryRequest(proto.Message):
     r"""CreateActiveDirectoryRequest for creating an active
     directory.
 
     Attributes:
         parent (str):
             Required. Value for parent.
-        active_directory (google.cloud.netapp_v1beta1.types.ActiveDirectory):
+        active_directory (google.cloud.netapp_v1.types.ActiveDirectory):
             Required. Fields of the to be created active
             directory.
         active_directory_id (str):
             Required. ID of the active directory to
             create.
     """
 
@@ -163,15 +163,15 @@
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Field mask is used to specify the fields to be
             overwritten in the Active Directory resource by the update.
             The fields specified in the update_mask are relative to the
             resource, not the full request. A field will be overwritten
             if it is in the mask. If the user does not provide a mask
             then all fields will be overwritten.
-        active_directory (google.cloud.netapp_v1beta1.types.ActiveDirectory):
+        active_directory (google.cloud.netapp_v1.types.ActiveDirectory):
             Required. The volume being updated
     """
 
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=1,
         message=field_mask_pb2.FieldMask,
@@ -206,15 +206,15 @@
         name (str):
             Output only. The resource name of the active directory.
             Format:
             ``projects/{project_number}/locations/{location_id}/activeDirectories/{active_directory_id}``.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Create time of the active
             directory.
-        state (google.cloud.netapp_v1beta1.types.ActiveDirectory.State):
+        state (google.cloud.netapp_v1.types.ActiveDirectory.State):
             Output only. The state of the AD.
         domain (str):
             Required. Name of the Active Directory domain
         site (str):
             The Active Directory site the service will
             limit Domain Controller discovery too.
         dns (str):
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/cloud_netapp_service.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/cloud_netapp_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,24 +17,23 @@
 
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.cloud.netapp.v1beta1",
+    package="google.cloud.netapp.v1",
     manifest={
         "OperationMetadata",
     },
 )
 
 
 class OperationMetadata(proto.Message):
-    r"""OperationMetadata
-    Represents the metadata of the long-running operation.
+    r"""Represents the metadata of the long-running operation.
 
     Attributes:
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time the operation was
             created.
         end_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The time the operation finished
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/common.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,45 +16,43 @@
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.cloud.netapp.v1beta1",
+    package="google.cloud.netapp.v1",
     manifest={
         "ServiceLevel",
         "EncryptionType",
     },
 )
 
 
 class ServiceLevel(proto.Enum):
-    r"""ServiceLevel
-    The service levels - Storage Pool, Volumes
+    r"""The service levels - Storage Pool, Volumes
 
     Values:
         SERVICE_LEVEL_UNSPECIFIED (0):
-            Unspecified service level
+            No description available.
         PREMIUM (1):
-            Premium
+            No description available.
         EXTREME (2):
-            Extreme
+            No description available.
         STANDARD (3):
             Standard (Software offering)
     """
     SERVICE_LEVEL_UNSPECIFIED = 0
     PREMIUM = 1
     EXTREME = 2
     STANDARD = 3
 
 
 class EncryptionType(proto.Enum):
-    r"""EncryptionType
-    Defined the current volume encryption key source.
+    r"""Defined the current volume encryption key source.
 
     Values:
         ENCRYPTION_TYPE_UNSPECIFIED (0):
             The source of encryption key is not
             specified.
         SERVICE_MANAGED (1):
             Google managed encryption key.
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/kms.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/kms.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.cloud.netapp.v1beta1",
+    package="google.cloud.netapp.v1",
     manifest={
         "GetKmsConfigRequest",
         "ListKmsConfigsRequest",
         "ListKmsConfigsResponse",
         "CreateKmsConfigRequest",
         "UpdateKmsConfigRequest",
         "DeleteKmsConfigRequest",
@@ -35,29 +35,29 @@
         "VerifyKmsConfigResponse",
         "KmsConfig",
     },
 )
 
 
 class GetKmsConfigRequest(proto.Message):
-    r"""GetKmsConfigRequest
+    r"""
 
     Attributes:
         name (str):
             Required. Name of the KmsConfig
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListKmsConfigsRequest(proto.Message):
-    r"""ListKmsConfigsRequest
+    r"""
 
     Attributes:
         parent (str):
             Required. Parent value
         page_size (int):
             The maximum number of items to return.
         page_token (str):
@@ -89,18 +89,18 @@
     filter: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class ListKmsConfigsResponse(proto.Message):
-    r"""ListKmsConfigsResponse
+    r"""
 
     Attributes:
-        kms_configs (MutableSequence[google.cloud.netapp_v1beta1.types.KmsConfig]):
+        kms_configs (MutableSequence[google.cloud.netapp_v1.types.KmsConfig]):
             The list of KmsConfigs
         next_page_token (str):
             A token identifying a page of results the
             server should return.
         unreachable (MutableSequence[str]):
             Locations that could not be reached.
     """
@@ -121,24 +121,24 @@
     unreachable: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
 
 
 class CreateKmsConfigRequest(proto.Message):
-    r"""CreateKmsConfigRequest
+    r"""
 
     Attributes:
         parent (str):
             Required. Value for parent.
         kms_config_id (str):
             Required. Id of the requesting KmsConfig If auto-generating
             Id server-side, remove this field and id from the
             method_signature of Create RPC
-        kms_config (google.cloud.netapp_v1beta1.types.KmsConfig):
+        kms_config (google.cloud.netapp_v1.types.KmsConfig):
             Required. The required parameters to create a
             new KmsConfig.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
@@ -151,25 +151,25 @@
         proto.MESSAGE,
         number=3,
         message="KmsConfig",
     )
 
 
 class UpdateKmsConfigRequest(proto.Message):
-    r"""UpdateKmsConfigRequest
+    r"""
 
     Attributes:
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Field mask is used to specify the fields to be
             overwritten in the KmsConfig resource by the update. The
             fields specified in the update_mask are relative to the
             resource, not the full request. A field will be overwritten
             if it is in the mask. If the user does not provide a mask
             then all fields will be overwritten.
-        kms_config (google.cloud.netapp_v1beta1.types.KmsConfig):
+        kms_config (google.cloud.netapp_v1.types.KmsConfig):
             Required. The KmsConfig being updated
     """
 
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=1,
         message=field_mask_pb2.FieldMask,
@@ -178,63 +178,61 @@
         proto.MESSAGE,
         number=2,
         message="KmsConfig",
     )
 
 
 class DeleteKmsConfigRequest(proto.Message):
-    r"""DeleteKmsConfigRequest
+    r"""
 
     Attributes:
         name (str):
             Required. Name of the KmsConfig.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class EncryptVolumesRequest(proto.Message):
-    r"""EncryptVolumesRequest
-    EncryptVolumesRequest specifies the KMS config to encrypt
+    r"""EncryptVolumesRequest specifies the KMS config to encrypt
     existing volumes.
 
     Attributes:
         name (str):
             Required. Name of the KmsConfig.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class VerifyKmsConfigRequest(proto.Message):
-    r"""VerifyKmsConfigRequest
-    VerifyKmsConfigRequest specifies the KMS config to be validated.
+    r"""VerifyKmsConfigRequest specifies the KMS config to be
+    validated.
 
     Attributes:
         name (str):
             Required. Name of the KMS Config to be
             verified.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class VerifyKmsConfigResponse(proto.Message):
-    r"""VerifyKmsConfigResponse
-    VerifyKmsConfigResponse contains the information if the config
-    is correctly and error message.
+    r"""VerifyKmsConfigResponse contains the information if the
+    config is correctly and error message.
 
     Attributes:
         healthy (bool):
             Output only. If the customer key configured
             correctly to the encrypt volume.
         health_error (str):
             Output only. Error message if config is not
@@ -265,15 +263,15 @@
     Attributes:
         name (str):
             Output only. Name of the KmsConfig.
         crypto_key_name (str):
             Required. Customer managed crypto key resource full name.
             Format:
             projects/{project}/locations/{location}/keyRings/{key_ring}/cryptoKeys/{key}.
-        state (google.cloud.netapp_v1beta1.types.KmsConfig.State):
+        state (google.cloud.netapp_v1.types.KmsConfig.State):
             Output only. State of the KmsConfig.
         state_details (str):
             Output only. State details of the KmsConfig.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Create time of the KmsConfig.
         description (str):
             Description of the KmsConfig.
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/replication.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/replication.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.cloud.netapp.v1beta1",
+    package="google.cloud.netapp.v1",
     manifest={
         "TransferStats",
         "Replication",
         "ListReplicationsRequest",
         "ListReplicationsResponse",
         "GetReplicationRequest",
         "DestinationVolumeParameters",
@@ -141,26 +141,26 @@
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
             Output only. The resource name of the Replication. Format:
             ``projects/{project_id}/locations/{location}/volumes/{volume_id}/replications/{replication_id}``.
-        state (google.cloud.netapp_v1beta1.types.Replication.State):
+        state (google.cloud.netapp_v1.types.Replication.State):
             Output only. State of the replication.
         state_details (str):
             Output only. State details of the
             replication.
-        role (google.cloud.netapp_v1beta1.types.Replication.ReplicationRole):
+        role (google.cloud.netapp_v1.types.Replication.ReplicationRole):
             Output only. Indicates whether this points to
             source or destination.
-        replication_schedule (google.cloud.netapp_v1beta1.types.Replication.ReplicationSchedule):
+        replication_schedule (google.cloud.netapp_v1.types.Replication.ReplicationSchedule):
             Required. Indicates the schedule for
             replication.
-        mirror_state (google.cloud.netapp_v1beta1.types.Replication.MirrorState):
+        mirror_state (google.cloud.netapp_v1.types.Replication.MirrorState):
             Output only. Indicates the state of
             mirroring.
         healthy (bool):
             Output only. Condition of the relationship.
             Can be one of the following:
 
             - true: The replication relationship is healthy.
@@ -173,25 +173,25 @@
             This field is a member of `oneof`_ ``_healthy``.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Replication create time.
         destination_volume (str):
             Output only. Full name of destination volume resource.
             Example :
             "projects/{project}/locations/{location}/volumes/{volume_id}".
-        transfer_stats (google.cloud.netapp_v1beta1.types.TransferStats):
+        transfer_stats (google.cloud.netapp_v1.types.TransferStats):
             Output only. Replication transfer statistics.
         labels (MutableMapping[str, str]):
             Resource labels to represent user provided
             metadata.
         description (str):
             A description about this replication
             relationship.
 
             This field is a member of `oneof`_ ``_description``.
-        destination_volume_parameters (google.cloud.netapp_v1beta1.types.DestinationVolumeParameters):
+        destination_volume_parameters (google.cloud.netapp_v1.types.DestinationVolumeParameters):
             Required. Input only. Destination volume
             parameters
         source_volume (str):
             Output only. Full name of source volume resource. Example :
             "projects/{project}/locations/{location}/volumes/{volume_id}".
     """
 
@@ -218,16 +218,15 @@
         CREATING = 1
         READY = 2
         UPDATING = 3
         DELETING = 5
         ERROR = 6
 
     class ReplicationRole(proto.Enum):
-        r"""Replication role
-        New enum values may be added in future to support different
+        r"""New enum values may be added in future to support different
         replication topology.
 
         Values:
             REPLICATION_ROLE_UNSPECIFIED (0):
                 Unspecified replication role
             SOURCE (1):
                 Indicates Source volume.
@@ -393,15 +392,15 @@
 
 
 class ListReplicationsResponse(proto.Message):
     r"""ListReplicationsResponse is the result of
     ListReplicationsRequest.
 
     Attributes:
-        replications (MutableSequence[google.cloud.netapp_v1beta1.types.Replication]):
+        replications (MutableSequence[google.cloud.netapp_v1.types.Replication]):
             A list of replications in the project for the
             specified volume.
         next_page_token (str):
             The token you can use to retrieve the next
             page of results. Not returned if there are no
             more results in the list.
         unreachable (MutableSequence[str]):
@@ -493,15 +492,15 @@
     r"""CreateReplicationRequest creates a replication.
 
     Attributes:
         parent (str):
             Required. The NetApp volume to create the replications of,
             in the format
             ``projects/{project_id}/locations/{location}/volumes/{volume_id}``
-        replication (google.cloud.netapp_v1beta1.types.Replication):
+        replication (google.cloud.netapp_v1.types.Replication):
             Required. A replication resource
         replication_id (str):
             Required. ID of the replication to create.
             This value must start with a lowercase letter
             followed by up to 62 lowercase letters, numbers,
             or hyphens, and cannot end with a hyphen.
     """
@@ -540,15 +539,15 @@
     r"""UpdateReplicationRequest updates description and/or labels
     for a replication.
 
     Attributes:
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask of fields to update.  At least
             one path must be supplied in this field.
-        replication (google.cloud.netapp_v1beta1.types.Replication):
+        replication (google.cloud.netapp_v1.types.Replication):
             Required. A replication resource
     """
 
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=1,
         message=field_mask_pb2.FieldMask,
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/snapshot.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.cloud.netapp.v1beta1",
+    package="google.cloud.netapp.v1",
     manifest={
         "ListSnapshotsRequest",
         "ListSnapshotsResponse",
         "GetSnapshotRequest",
         "CreateSnapshotRequest",
         "DeleteSnapshotRequest",
         "UpdateSnapshotRequest",
@@ -77,15 +77,15 @@
     )
 
 
 class ListSnapshotsResponse(proto.Message):
     r"""ListSnapshotsResponse is the result of ListSnapshotsRequest.
 
     Attributes:
-        snapshots (MutableSequence[google.cloud.netapp_v1beta1.types.Snapshot]):
+        snapshots (MutableSequence[google.cloud.netapp_v1.types.Snapshot]):
             A list of snapshots in the project for the
             specified volume.
         next_page_token (str):
             The token you can use to retrieve the next
             page of results. Not returned if there are no
             more results in the list.
         unreachable (MutableSequence[str]):
@@ -130,15 +130,15 @@
     r"""CreateSnapshotRequest creates a snapshot.
 
     Attributes:
         parent (str):
             Required. The NetApp volume to create the snapshots of, in
             the format
             ``projects/{project_id}/locations/{location}/volumes/{volume_id}``
-        snapshot (google.cloud.netapp_v1beta1.types.Snapshot):
+        snapshot (google.cloud.netapp_v1.types.Snapshot):
             Required. A snapshot resource
         snapshot_id (str):
             Required. ID of the snapshot to create.
             This value must start with a lowercase letter
             followed by up to 62 lowercase letters, numbers,
             or hyphens, and cannot end with a hyphen.
     """
@@ -177,15 +177,15 @@
     r"""UpdateSnapshotRequest updates description and/or labels for a
     snapshot.
 
     Attributes:
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask of fields to update.  At least
             one path must be supplied in this field.
-        snapshot (google.cloud.netapp_v1beta1.types.Snapshot):
+        snapshot (google.cloud.netapp_v1.types.Snapshot):
             Required. A snapshot resource
     """
 
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=1,
         message=field_mask_pb2.FieldMask,
@@ -194,21 +194,21 @@
         proto.MESSAGE,
         number=2,
         message="Snapshot",
     )
 
 
 class Snapshot(proto.Message):
-    r"""Snapshot
+    r"""
 
     Attributes:
         name (str):
             Output only. The resource name of the snapshot. Format:
             ``projects/{project_id}/locations/{location}/volumes/{volume_id}/snapshots/{snapshot_id}``.
-        state (google.cloud.netapp_v1beta1.types.Snapshot.State):
+        state (google.cloud.netapp_v1.types.Snapshot.State):
             Output only. The snapshot state.
         state_details (str):
             Output only. State details of the storage
             pool
         description (str):
             A description of the snapshot with 2048
             characters or less. Requests with longer
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/storage_pool.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/storage_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,46 +17,46 @@
 
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
-from google.cloud.netapp_v1beta1.types import common
+from google.cloud.netapp_v1.types import common
 
 __protobuf__ = proto.module(
-    package="google.cloud.netapp.v1beta1",
+    package="google.cloud.netapp.v1",
     manifest={
         "GetStoragePoolRequest",
         "ListStoragePoolsRequest",
         "ListStoragePoolsResponse",
         "CreateStoragePoolRequest",
         "UpdateStoragePoolRequest",
         "DeleteStoragePoolRequest",
         "StoragePool",
     },
 )
 
 
 class GetStoragePoolRequest(proto.Message):
-    r"""GetStoragePoolRequest
+    r"""
 
     Attributes:
         name (str):
             Required. Name of the storage pool
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListStoragePoolsRequest(proto.Message):
-    r"""ListStoragePoolsRequest
+    r"""
 
     Attributes:
         parent (str):
             Required. Parent value
         page_size (int):
             The maximum number of items to return.
         page_token (str):
@@ -88,18 +88,18 @@
     filter: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class ListStoragePoolsResponse(proto.Message):
-    r"""ListStoragePoolsResponse
+    r"""
 
     Attributes:
-        storage_pools (MutableSequence[google.cloud.netapp_v1beta1.types.StoragePool]):
+        storage_pools (MutableSequence[google.cloud.netapp_v1.types.StoragePool]):
             The list of StoragePools
         next_page_token (str):
             A token identifying a page of results the
             server should return.
         unreachable (MutableSequence[str]):
             Locations that could not be reached.
     """
@@ -120,24 +120,24 @@
     unreachable: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
 
 
 class CreateStoragePoolRequest(proto.Message):
-    r"""CreateStoragePoolRequest
+    r"""
 
     Attributes:
         parent (str):
             Required. Value for parent.
         storage_pool_id (str):
             Required. Id of the requesting storage pool If
             auto-generating Id server-side, remove this field and id
             from the method_signature of Create RPC
-        storage_pool (google.cloud.netapp_v1beta1.types.StoragePool):
+        storage_pool (google.cloud.netapp_v1.types.StoragePool):
             Required. The required parameters to create a
             new storage pool.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
@@ -150,25 +150,25 @@
         proto.MESSAGE,
         number=3,
         message="StoragePool",
     )
 
 
 class UpdateStoragePoolRequest(proto.Message):
-    r"""UpdateStoragePoolRequest
+    r"""
 
     Attributes:
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Field mask is used to specify the fields to be
             overwritten in the StoragePool resource by the update. The
             fields specified in the update_mask are relative to the
             resource, not the full request. A field will be overwritten
             if it is in the mask. If the user does not provide a mask
             then all fields will be overwritten.
-        storage_pool (google.cloud.netapp_v1beta1.types.StoragePool):
+        storage_pool (google.cloud.netapp_v1.types.StoragePool):
             Required. The pool being updated
     """
 
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=1,
         message=field_mask_pb2.FieldMask,
@@ -177,51 +177,49 @@
         proto.MESSAGE,
         number=2,
         message="StoragePool",
     )
 
 
 class DeleteStoragePoolRequest(proto.Message):
-    r"""DeleteStoragePoolRequest
+    r"""
 
     Attributes:
         name (str):
             Required. Name of the storage pool
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class StoragePool(proto.Message):
-    r"""Resources
-    StoragePool
-    StoragePool is a container for volumes with a service level and
-    capacity. Volumes can be created in a pool of sufficient
+    r"""StoragePool is a container for volumes with a service level
+    and capacity. Volumes can be created in a pool of sufficient
     available capacity. StoragePool capacity is what you are billed
     for.
 
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
             Output only. Name of the storage pool
-        service_level (google.cloud.netapp_v1beta1.types.ServiceLevel):
+        service_level (google.cloud.netapp_v1.types.ServiceLevel):
             Required. Service level of the storage pool
         capacity_gib (int):
             Required. Capacity in GIB of the pool
         volume_capacity_gib (int):
             Output only. Allocated size of all volumes in
             GIB in the storage pool
         volume_count (int):
             Output only. Volume count of the storage pool
-        state (google.cloud.netapp_v1beta1.types.StoragePool.State):
+        state (google.cloud.netapp_v1.types.StoragePool.State):
             Output only. State of the storage pool
         state_details (str):
             Output only. State details of the storage
             pool
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Create time of the storage pool
         description (str):
@@ -241,15 +239,15 @@
         ldap_enabled (bool):
             Flag indicating if the pool is NFS LDAP
             enabled or not.
         psa_range (str):
             Name of the Private Service Access allocated
             range. If not provided, any available range will
             be chosen.
-        encryption_type (google.cloud.netapp_v1beta1.types.EncryptionType):
+        encryption_type (google.cloud.netapp_v1.types.EncryptionType):
             Output only. Specifies the current pool
             encryption key source.
         global_access_allowed (bool):
             Optional. Allows SO pool to access AD or DNS
             server from other regions.
 
             This field is a member of `oneof`_ ``_global_access_allowed``.
```

### Comparing `google-cloud-netapp-0.1.0/google/cloud/netapp_v1beta1/types/volume.py` & `google-cloud-netapp-0.2.0/google/cloud/netapp_v1/types/volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
-from google.cloud.netapp_v1beta1.types import common
+from google.cloud.netapp_v1.types import common
 
 __protobuf__ = proto.module(
-    package="google.cloud.netapp.v1beta1",
+    package="google.cloud.netapp.v1",
     manifest={
         "Protocols",
         "AccessType",
         "SMBSettings",
         "SecurityStyle",
         "ListVolumesRequest",
         "ListVolumesResponse",
@@ -48,16 +48,15 @@
         "MountOption",
         "RestoreParameters",
     },
 )
 
 
 class Protocols(proto.Enum):
-    r"""Protocols
-    The protocols
+    r"""
 
     Values:
         PROTOCOLS_UNSPECIFIED (0):
             Unspecified protocol
         NFSV3 (1):
             NFS V3 protocol
         NFSV4 (2):
@@ -68,16 +67,15 @@
     PROTOCOLS_UNSPECIFIED = 0
     NFSV3 = 1
     NFSV4 = 2
     SMB = 3
 
 
 class AccessType(proto.Enum):
-    r"""AccessType
-    The access types
+    r"""
 
     Values:
         ACCESS_TYPE_UNSPECIFIED (0):
             Unspecified Access Type
         READ_ONLY (1):
             Read Only
         READ_WRITE (2):
@@ -143,16 +141,15 @@
     """
     SECURITY_STYLE_UNSPECIFIED = 0
     NTFS = 1
     UNIX = 2
 
 
 class ListVolumesRequest(proto.Message):
-    r"""ListVolumesRequest
-    Message for requesting list of Volumes
+    r"""Message for requesting list of Volumes
 
     Attributes:
         parent (str):
             Required. Parent value for ListVolumesRequest
         page_size (int):
             Requested page size. Server may return fewer
             items than requested. If unspecified, the server
@@ -185,19 +182,18 @@
     order_by: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class ListVolumesResponse(proto.Message):
-    r"""ListVolumesResponse
-    Message for response to listing Volumes
+    r"""Message for response to listing Volumes
 
     Attributes:
-        volumes (MutableSequence[google.cloud.netapp_v1beta1.types.Volume]):
+        volumes (MutableSequence[google.cloud.netapp_v1.types.Volume]):
             The list of Volume
         next_page_token (str):
             A token identifying a page of results the
             server should return.
         unreachable (MutableSequence[str]):
             Locations that could not be reached.
     """
@@ -218,40 +214,38 @@
     unreachable: MutableSequence[str] = proto.RepeatedField(
         proto.STRING,
         number=3,
     )
 
 
 class GetVolumeRequest(proto.Message):
-    r"""GetVolumeRequest
-    Message for getting a Volume
+    r"""Message for getting a Volume
 
     Attributes:
         name (str):
             Required. Name of the volume
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class CreateVolumeRequest(proto.Message):
-    r"""CreateVolumeRequest
-    Message for creating a Volume
+    r"""Message for creating a Volume
 
     Attributes:
         parent (str):
             Required. Value for parent.
         volume_id (str):
             Required. Id of the requesting volume If auto-generating Id
             server-side, remove this field and Id from the
             method_signature of Create RPC
-        volume (google.cloud.netapp_v1beta1.types.Volume):
+        volume (google.cloud.netapp_v1.types.Volume):
             Required. The volume being created.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
@@ -263,26 +257,25 @@
         proto.MESSAGE,
         number=3,
         message="Volume",
     )
 
 
 class UpdateVolumeRequest(proto.Message):
-    r"""UpdateVolumeRequest
-    Message for updating a Volume
+    r"""Message for updating a Volume
 
     Attributes:
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Field mask is used to specify the fields to be
             overwritten in the Volume resource by the update. The fields
             specified in the update_mask are relative to the resource,
             not the full request. A field will be overwritten if it is
             in the mask. If the user does not provide a mask then all
             fields will be overwritten.
-        volume (google.cloud.netapp_v1beta1.types.Volume):
+        volume (google.cloud.netapp_v1.types.Volume):
             Required. The volume being updated
     """
 
     update_mask: field_mask_pb2.FieldMask = proto.Field(
         proto.MESSAGE,
         number=1,
         message=field_mask_pb2.FieldMask,
@@ -291,16 +284,15 @@
         proto.MESSAGE,
         number=2,
         message="Volume",
     )
 
 
 class DeleteVolumeRequest(proto.Message):
-    r"""DeleteVolumeRequest
-    Message for deleting a Volume
+    r"""Message for deleting a Volume
 
     Attributes:
         name (str):
             Required. Name of the volume
         force (bool):
             If this field is set as true, CCFE will not
             block the volume resource deletion even if it
@@ -316,16 +308,16 @@
     force: bool = proto.Field(
         proto.BOOL,
         number=2,
     )
 
 
 class RevertVolumeRequest(proto.Message):
-    r"""RevertVolumeRequest reverts the given volume to the
-    specified snapshot.
+    r"""RevertVolumeRequest reverts the given volume to the specified
+    snapshot.
 
     Attributes:
         name (str):
             Required. The resource name of the volume, in the format of
             projects/{project_id}/locations/{location}/volumes/{volume_id}.
         snapshot_id (str):
             Required. The snapshot resource ID, in the format
@@ -341,21 +333,20 @@
     snapshot_id: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class Volume(proto.Message):
-    r"""Volume
-    Volume provides a filesystem that you can mount.
+    r"""Volume provides a filesystem that you can mount.
 
     Attributes:
         name (str):
             Output only. Name of the volume
-        state (google.cloud.netapp_v1beta1.types.Volume.State):
+        state (google.cloud.netapp_v1.types.Volume.State):
             Output only. State of the volume
         state_details (str):
             Output only. State details of the volume
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Create time of the volume
         share_name (str):
             Required. Share name of the volume
@@ -365,67 +356,67 @@
             provided, any available range will be chosen.
         storage_pool (str):
             Required. StoragePool name of the volume
         network (str):
             Output only. VPC Network name.
             Format:
             projects/{project}/global/networks/{network}
-        service_level (google.cloud.netapp_v1beta1.types.ServiceLevel):
+        service_level (google.cloud.netapp_v1.types.ServiceLevel):
             Output only. Service level of the volume
         capacity_gib (int):
             Required. Capacity in GIB of the volume
-        export_policy (google.cloud.netapp_v1beta1.types.ExportPolicy):
+        export_policy (google.cloud.netapp_v1.types.ExportPolicy):
             Optional. Export policy of the volume
-        protocols (MutableSequence[google.cloud.netapp_v1beta1.types.Protocols]):
+        protocols (MutableSequence[google.cloud.netapp_v1.types.Protocols]):
             Required. Protocols required for the volume
-        smb_settings (MutableSequence[google.cloud.netapp_v1beta1.types.SMBSettings]):
+        smb_settings (MutableSequence[google.cloud.netapp_v1.types.SMBSettings]):
             Optional. SMB share settings for the volume.
-        mount_options (MutableSequence[google.cloud.netapp_v1beta1.types.MountOption]):
+        mount_options (MutableSequence[google.cloud.netapp_v1.types.MountOption]):
             Output only. Mount options of this volume
         unix_permissions (str):
             Optional. Default unix style permission (e.g.
             777) the mount point will be created with.
             Applicable for NFS protocol types only.
         labels (MutableMapping[str, str]):
             Optional. Labels as key value pairs
         description (str):
             Optional. Description of the volume
-        snapshot_policy (google.cloud.netapp_v1beta1.types.SnapshotPolicy):
+        snapshot_policy (google.cloud.netapp_v1.types.SnapshotPolicy):
             Optional. SnapshotPolicy for a volume.
         snap_reserve (float):
             Optional. Snap_reserve specifies percentage of volume
             storage reserved for snapshot storage. Default is 0 percent.
         snapshot_directory (bool):
             Optional. Snapshot_directory if enabled (true) the volume
             will contain a read-only .snapshot directory which provides
             access to each of the volume's snapshots.
         used_gib (int):
             Output only. Used capacity in GIB of the
             volume. This is computed periodically and it
             does not represent the realtime usage.
-        security_style (google.cloud.netapp_v1beta1.types.SecurityStyle):
+        security_style (google.cloud.netapp_v1.types.SecurityStyle):
             Optional. Security Style of the Volume
         kerberos_enabled (bool):
             Optional. Flag indicating if the volume is a
             kerberos volume or not, export policy rules
             control kerberos security modes (krb5, krb5i,
             krb5p).
         ldap_enabled (bool):
             Output only. Flag indicating if the volume is
             NFS LDAP enabled or not.
         active_directory (str):
             Output only. Specifies the ActiveDirectory
             name of a SMB volume.
-        restore_parameters (google.cloud.netapp_v1beta1.types.RestoreParameters):
+        restore_parameters (google.cloud.netapp_v1.types.RestoreParameters):
             Optional. Specifies the source of the volume
             to be created from.
         kms_config (str):
             Output only. Specifies the KMS config to be
             used for volume encryption.
-        encryption_type (google.cloud.netapp_v1beta1.types.EncryptionType):
+        encryption_type (google.cloud.netapp_v1.types.EncryptionType):
             Output only. Specified the current volume
             encryption key source.
         has_replication (bool):
             Output only. Indicates whether the volume is
             part of a replication relationship.
     """
 
@@ -586,47 +577,44 @@
     has_replication: bool = proto.Field(
         proto.BOOL,
         number=29,
     )
 
 
 class ExportPolicy(proto.Message):
-    r"""ExportPolicy
-    Defined the export policy for the volume.
+    r"""Defines the export policy for the volume.
 
     Attributes:
-        rules (MutableSequence[google.cloud.netapp_v1beta1.types.SimpleExportPolicyRule]):
+        rules (MutableSequence[google.cloud.netapp_v1.types.SimpleExportPolicyRule]):
             Required. List of export policy rules
     """
 
     rules: MutableSequence["SimpleExportPolicyRule"] = proto.RepeatedField(
         proto.MESSAGE,
         number=1,
         message="SimpleExportPolicyRule",
     )
 
 
 class SimpleExportPolicyRule(proto.Message):
-    r"""SimpleExportPolicyRule
-    An export policy rule describing various export options.
-
+    r"""An export policy rule describing various export options.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         allowed_clients (str):
             Comma separated list of allowed clients IP
             addresses
 
             This field is a member of `oneof`_ ``_allowed_clients``.
         has_root_access (str):
             Whether Unix root access will be granted.
 
             This field is a member of `oneof`_ ``_has_root_access``.
-        access_type (google.cloud.netapp_v1beta1.types.AccessType):
+        access_type (google.cloud.netapp_v1.types.AccessType):
             Access type (ReadWrite, ReadOnly, None)
 
             This field is a member of `oneof`_ ``_access_type``.
         nfsv3 (bool):
             NFS V3 protocol.
 
             This field is a member of `oneof`_ ``_nfsv3``.
@@ -752,27 +740,27 @@
 
     Attributes:
         enabled (bool):
             If enabled, make snapshots automatically
             according to the schedules. Default is false.
 
             This field is a member of `oneof`_ ``_enabled``.
-        hourly_schedule (google.cloud.netapp_v1beta1.types.HourlySchedule):
+        hourly_schedule (google.cloud.netapp_v1.types.HourlySchedule):
             Hourly schedule policy.
 
             This field is a member of `oneof`_ ``_hourly_schedule``.
-        daily_schedule (google.cloud.netapp_v1beta1.types.DailySchedule):
+        daily_schedule (google.cloud.netapp_v1.types.DailySchedule):
             Daily schedule policy.
 
             This field is a member of `oneof`_ ``_daily_schedule``.
-        weekly_schedule (google.cloud.netapp_v1beta1.types.WeeklySchedule):
+        weekly_schedule (google.cloud.netapp_v1.types.WeeklySchedule):
             Weekly schedule policy.
 
             This field is a member of `oneof`_ ``_weekly_schedule``.
-        monthly_schedule (google.cloud.netapp_v1beta1.types.MonthlySchedule):
+        monthly_schedule (google.cloud.netapp_v1.types.MonthlySchedule):
             Monthly schedule policy.
 
             This field is a member of `oneof`_ ``_monthly_schedule``.
     """
 
     enabled: bool = proto.Field(
         proto.BOOL,
@@ -983,23 +971,22 @@
         proto.STRING,
         number=4,
         optional=True,
     )
 
 
 class MountOption(proto.Message):
-    r"""MountOption
-    View only mount options for a volume.
+    r"""View only mount options for a volume.
 
     Attributes:
         export (str):
             Export string
         export_full (str):
             Full export string
-        protocol (google.cloud.netapp_v1beta1.types.Protocols):
+        protocol (google.cloud.netapp_v1.types.Protocols):
             Protocol to mount with.
         instructions (str):
             Instructions for mounting
     """
 
     export: str = proto.Field(
         proto.STRING,
```

### Comparing `google-cloud-netapp-0.1.0/google_cloud_netapp.egg-info/PKG-INFO` & `google-cloud-netapp-0.2.0/google_cloud_netapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-netapp
-Version: 0.1.0
+Version: 0.2.0
 Summary: Google Cloud Netapp API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-netapp-0.1.0/google_cloud_netapp.egg-info/SOURCES.txt` & `google-cloud-netapp-0.2.0/google_cloud_netapp.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
 google/cloud/netapp/__init__.py
 google/cloud/netapp/gapic_version.py
 google/cloud/netapp/py.typed
-google/cloud/netapp_v1beta1/__init__.py
-google/cloud/netapp_v1beta1/gapic_metadata.json
-google/cloud/netapp_v1beta1/gapic_version.py
-google/cloud/netapp_v1beta1/py.typed
-google/cloud/netapp_v1beta1/services/__init__.py
-google/cloud/netapp_v1beta1/services/net_app/__init__.py
-google/cloud/netapp_v1beta1/services/net_app/async_client.py
-google/cloud/netapp_v1beta1/services/net_app/client.py
-google/cloud/netapp_v1beta1/services/net_app/pagers.py
-google/cloud/netapp_v1beta1/services/net_app/transports/__init__.py
-google/cloud/netapp_v1beta1/services/net_app/transports/base.py
-google/cloud/netapp_v1beta1/services/net_app/transports/grpc.py
-google/cloud/netapp_v1beta1/services/net_app/transports/grpc_asyncio.py
-google/cloud/netapp_v1beta1/services/net_app/transports/rest.py
-google/cloud/netapp_v1beta1/types/__init__.py
-google/cloud/netapp_v1beta1/types/active_directory.py
-google/cloud/netapp_v1beta1/types/cloud_netapp_service.py
-google/cloud/netapp_v1beta1/types/common.py
-google/cloud/netapp_v1beta1/types/kms.py
-google/cloud/netapp_v1beta1/types/replication.py
-google/cloud/netapp_v1beta1/types/snapshot.py
-google/cloud/netapp_v1beta1/types/storage_pool.py
-google/cloud/netapp_v1beta1/types/volume.py
+google/cloud/netapp_v1/__init__.py
+google/cloud/netapp_v1/gapic_metadata.json
+google/cloud/netapp_v1/gapic_version.py
+google/cloud/netapp_v1/py.typed
+google/cloud/netapp_v1/services/__init__.py
+google/cloud/netapp_v1/services/net_app/__init__.py
+google/cloud/netapp_v1/services/net_app/async_client.py
+google/cloud/netapp_v1/services/net_app/client.py
+google/cloud/netapp_v1/services/net_app/pagers.py
+google/cloud/netapp_v1/services/net_app/transports/__init__.py
+google/cloud/netapp_v1/services/net_app/transports/base.py
+google/cloud/netapp_v1/services/net_app/transports/grpc.py
+google/cloud/netapp_v1/services/net_app/transports/grpc_asyncio.py
+google/cloud/netapp_v1/services/net_app/transports/rest.py
+google/cloud/netapp_v1/types/__init__.py
+google/cloud/netapp_v1/types/active_directory.py
+google/cloud/netapp_v1/types/cloud_netapp_service.py
+google/cloud/netapp_v1/types/common.py
+google/cloud/netapp_v1/types/kms.py
+google/cloud/netapp_v1/types/replication.py
+google/cloud/netapp_v1/types/snapshot.py
+google/cloud/netapp_v1/types/storage_pool.py
+google/cloud/netapp_v1/types/volume.py
 google_cloud_netapp.egg-info/PKG-INFO
 google_cloud_netapp.egg-info/SOURCES.txt
 google_cloud_netapp.egg-info/dependency_links.txt
 google_cloud_netapp.egg-info/namespace_packages.txt
 google_cloud_netapp.egg-info/not-zip-safe
 google_cloud_netapp.egg-info/requires.txt
 google_cloud_netapp.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
-tests/unit/gapic/netapp_v1beta1/__init__.py
-tests/unit/gapic/netapp_v1beta1/test_net_app.py
+tests/unit/gapic/netapp_v1/__init__.py
+tests/unit/gapic/netapp_v1/test_net_app.py
```

### Comparing `google-cloud-netapp-0.1.0/setup.py` & `google-cloud-netapp-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.1.0/tests/__init__.py` & `google-cloud-netapp-0.2.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.1.0/tests/unit/__init__.py` & `google-cloud-netapp-0.2.0/tests/unit/gapic/netapp_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-netapp-0.1.0/tests/unit/gapic/netapp_v1beta1/test_net_app.py` & `google-cloud-netapp-0.2.0/tests/unit/gapic/netapp_v1/test_net_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,31 +53,31 @@
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
 
-from google.cloud.netapp_v1beta1.services.net_app import (
+from google.cloud.netapp_v1.services.net_app import (
     NetAppAsyncClient,
     NetAppClient,
     pagers,
     transports,
 )
-from google.cloud.netapp_v1beta1.types import active_directory as gcn_active_directory
-from google.cloud.netapp_v1beta1.types import active_directory
-from google.cloud.netapp_v1beta1.types import cloud_netapp_service, common, kms
-from google.cloud.netapp_v1beta1.types import replication
-from google.cloud.netapp_v1beta1.types import replication as gcn_replication
-from google.cloud.netapp_v1beta1.types import snapshot
-from google.cloud.netapp_v1beta1.types import snapshot as gcn_snapshot
-from google.cloud.netapp_v1beta1.types import storage_pool
-from google.cloud.netapp_v1beta1.types import storage_pool as gcn_storage_pool
-from google.cloud.netapp_v1beta1.types import volume
-from google.cloud.netapp_v1beta1.types import volume as gcn_volume
+from google.cloud.netapp_v1.types import active_directory as gcn_active_directory
+from google.cloud.netapp_v1.types import active_directory
+from google.cloud.netapp_v1.types import cloud_netapp_service, common, kms
+from google.cloud.netapp_v1.types import replication
+from google.cloud.netapp_v1.types import replication as gcn_replication
+from google.cloud.netapp_v1.types import snapshot
+from google.cloud.netapp_v1.types import snapshot as gcn_snapshot
+from google.cloud.netapp_v1.types import storage_pool
+from google.cloud.netapp_v1.types import storage_pool as gcn_storage_pool
+from google.cloud.netapp_v1.types import volume
+from google.cloud.netapp_v1.types import volume as gcn_volume
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -600,15 +600,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_net_app_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.netapp_v1beta1.services.net_app.transports.NetAppGrpcTransport.__init__"
+        "google.cloud.netapp_v1.services.net_app.transports.NetAppGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = NetAppClient(client_options={"api_endpoint": "squid.clam.whelk"})
         grpc_transport.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host="squid.clam.whelk",
@@ -10587,15 +10587,15 @@
         client.list_storage_pools(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*}/storagePools"
+            "%s/v1/{parent=projects/*/locations/*}/storagePools"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_storage_pools_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -10970,15 +10970,15 @@
         client.create_storage_pool(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*}/storagePools"
+            "%s/v1/{parent=projects/*/locations/*}/storagePools"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_storage_pool_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -11268,15 +11268,15 @@
         client.get_storage_pool(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/storagePools/*}"
+            "%s/v1/{name=projects/*/locations/*/storagePools/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_storage_pool_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -11586,15 +11586,15 @@
         client.update_storage_pool(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{storage_pool.name=projects/*/locations/*/storagePools/*}"
+            "%s/v1/{storage_pool.name=projects/*/locations/*/storagePools/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_storage_pool_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -11850,15 +11850,15 @@
         client.delete_storage_pool(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/storagePools/*}"
+            "%s/v1/{name=projects/*/locations/*/storagePools/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_storage_pool_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -12133,16 +12133,15 @@
         client.list_volumes(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*}/volumes"
-            % client.transport._host,
+            "%s/v1/{parent=projects/*/locations/*}/volumes" % client.transport._host,
             args[1],
         )
 
 
 def test_list_volumes_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -12492,16 +12491,15 @@
         client.get_volume(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/volumes/*}"
-            % client.transport._host,
+            "%s/v1/{name=projects/*/locations/*/volumes/*}" % client.transport._host,
             args[1],
         )
 
 
 def test_get_volume_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -12932,16 +12930,15 @@
         client.create_volume(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*}/volumes"
-            % client.transport._host,
+            "%s/v1/{parent=projects/*/locations/*}/volumes" % client.transport._host,
             args[1],
         )
 
 
 def test_create_volume_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -13360,15 +13357,15 @@
         client.update_volume(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{volume.name=projects/*/locations/*/volumes/*}"
+            "%s/v1/{volume.name=projects/*/locations/*/volumes/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_volume_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -13620,16 +13617,15 @@
         client.delete_volume(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/volumes/*}"
-            % client.transport._host,
+            "%s/v1/{name=projects/*/locations/*/volumes/*}" % client.transport._host,
             args[1],
         )
 
 
 def test_delete_volume_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -14122,15 +14118,15 @@
         client.list_snapshots(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*/volumes/*}/snapshots"
+            "%s/v1/{parent=projects/*/locations/*/volumes/*}/snapshots"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_snapshots_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -14453,15 +14449,15 @@
         client.get_snapshot(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/volumes/*/snapshots/*}"
+            "%s/v1/{name=projects/*/locations/*/volumes/*/snapshots/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_snapshot_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -14761,15 +14757,15 @@
         client.create_snapshot(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*/volumes/*}/snapshots"
+            "%s/v1/{parent=projects/*/locations/*/volumes/*}/snapshots"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_snapshot_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -15028,15 +15024,15 @@
         client.delete_snapshot(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/volumes/*/snapshots/*}"
+            "%s/v1/{name=projects/*/locations/*/volumes/*/snapshots/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_snapshot_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -15326,15 +15322,15 @@
         client.update_snapshot(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{snapshot.name=projects/*/locations/*/volumes/*/snapshots/*}"
+            "%s/v1/{snapshot.name=projects/*/locations/*/volumes/*/snapshots/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_snapshot_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -15622,15 +15618,15 @@
         client.list_active_directories(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*}/activeDirectories"
+            "%s/v1/{parent=projects/*/locations/*}/activeDirectories"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_active_directories_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -15987,15 +15983,15 @@
         client.get_active_directory(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/activeDirectories/*}"
+            "%s/v1/{name=projects/*/locations/*/activeDirectories/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_active_directory_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -16328,15 +16324,15 @@
         client.create_active_directory(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*}/activeDirectories"
+            "%s/v1/{parent=projects/*/locations/*}/activeDirectories"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_active_directory_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -16663,15 +16659,15 @@
         client.update_active_directory(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{active_directory.name=projects/*/locations/*/activeDirectories/*}"
+            "%s/v1/{active_directory.name=projects/*/locations/*/activeDirectories/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_active_directory_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -16931,15 +16927,15 @@
         client.delete_active_directory(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/activeDirectories/*}"
+            "%s/v1/{name=projects/*/locations/*/activeDirectories/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_active_directory_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -17214,16 +17210,15 @@
         client.list_kms_configs(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*}/kmsConfigs"
-            % client.transport._host,
+            "%s/v1/{parent=projects/*/locations/*}/kmsConfigs" % client.transport._host,
             args[1],
         )
 
 
 def test_list_kms_configs_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -17577,16 +17572,15 @@
         client.create_kms_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*}/kmsConfigs"
-            % client.transport._host,
+            "%s/v1/{parent=projects/*/locations/*}/kmsConfigs" % client.transport._host,
             args[1],
         )
 
 
 def test_create_kms_config_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -17853,16 +17847,15 @@
         client.get_kms_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/kmsConfigs/*}"
-            % client.transport._host,
+            "%s/v1/{name=projects/*/locations/*/kmsConfigs/*}" % client.transport._host,
             args[1],
         )
 
 
 def test_get_kms_config_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -18149,15 +18142,15 @@
         client.update_kms_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{kms_config.name=projects/*/locations/*/kmsConfigs/*}"
+            "%s/v1/{kms_config.name=projects/*/locations/*/kmsConfigs/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_kms_config_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -18827,16 +18820,15 @@
         client.delete_kms_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/kmsConfigs/*}"
-            % client.transport._host,
+            "%s/v1/{name=projects/*/locations/*/kmsConfigs/*}" % client.transport._host,
             args[1],
         )
 
 
 def test_delete_kms_config_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -19116,15 +19108,15 @@
         client.list_replications(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*/volumes/*}/replications"
+            "%s/v1/{parent=projects/*/locations/*/volumes/*}/replications"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_replications_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -19468,15 +19460,15 @@
         client.get_replication(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/volumes/*/replications/*}"
+            "%s/v1/{name=projects/*/locations/*/volumes/*/replications/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_replication_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -19818,15 +19810,15 @@
         client.create_replication(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{parent=projects/*/locations/*/volumes/*}/replications"
+            "%s/v1/{parent=projects/*/locations/*/volumes/*}/replications"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_replication_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -20087,15 +20079,15 @@
         client.delete_replication(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{name=projects/*/locations/*/volumes/*/replications/*}"
+            "%s/v1/{name=projects/*/locations/*/volumes/*/replications/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_replication_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -20427,15 +20419,15 @@
         client.update_replication(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta1/{replication.name=projects/*/locations/*/volumes/*/replications/*}"
+            "%s/v1/{replication.name=projects/*/locations/*/volumes/*/replications/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_replication_rest_flattened_error(transport: str = "rest"):
     client = NetAppClient(
@@ -21219,15 +21211,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_net_app_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.netapp_v1beta1.services.net_app.transports.NetAppTransport.__init__"
+        "google.cloud.netapp_v1.services.net_app.transports.NetAppTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.NetAppTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -21265,20 +21257,14 @@
         "get_replication",
         "create_replication",
         "delete_replication",
         "update_replication",
         "stop_replication",
         "resume_replication",
         "reverse_replication_direction",
-        "get_location",
-        "list_locations",
-        "get_operation",
-        "cancel_operation",
-        "delete_operation",
-        "list_operations",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
@@ -21298,15 +21284,15 @@
 
 
 def test_net_app_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.netapp_v1beta1.services.net_app.transports.NetAppTransport._prep_wrapped_messages"
+        "google.cloud.netapp_v1.services.net_app.transports.NetAppTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.NetAppTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -21317,15 +21303,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_net_app_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.netapp_v1beta1.services.net_app.transports.NetAppTransport._prep_wrapped_messages"
+        "google.cloud.netapp_v1.services.net_app.transports.NetAppTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.NetAppTransport()
         adc.assert_called_once()
 
 
@@ -22137,1214 +22123,14 @@
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
 
 
-def test_get_location_rest_bad_request(
-    transport: str = "rest", request_type=locations_pb2.GetLocationRequest
-):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    request = request_type()
-    request = json_format.ParseDict(
-        {"name": "projects/sample1/locations/sample2"}, request
-    )
-
-    # Mock the http request call within the method and fake a BadRequest error.
-    with mock.patch.object(Session, "request") as req, pytest.raises(
-        core_exceptions.BadRequest
-    ):
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 400
-        response_value.request = Request()
-        req.return_value = response_value
-        client.get_location(request)
-
-
-@pytest.mark.parametrize(
-    "request_type",
-    [
-        locations_pb2.GetLocationRequest,
-        dict,
-    ],
-)
-def test_get_location_rest(request_type):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="rest",
-    )
-    request_init = {"name": "projects/sample1/locations/sample2"}
-    request = request_type(**request_init)
-    # Mock the http request call within the method and fake a response.
-    with mock.patch.object(type(client.transport._session), "request") as req:
-        # Designate an appropriate value for the returned response.
-        return_value = locations_pb2.Location()
-
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 200
-        json_return_value = json_format.MessageToJson(return_value)
-
-        response_value._content = json_return_value.encode("UTF-8")
-        req.return_value = response_value
-
-        response = client.get_location(request)
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, locations_pb2.Location)
-
-
-def test_list_locations_rest_bad_request(
-    transport: str = "rest", request_type=locations_pb2.ListLocationsRequest
-):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    request = request_type()
-    request = json_format.ParseDict({"name": "projects/sample1"}, request)
-
-    # Mock the http request call within the method and fake a BadRequest error.
-    with mock.patch.object(Session, "request") as req, pytest.raises(
-        core_exceptions.BadRequest
-    ):
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 400
-        response_value.request = Request()
-        req.return_value = response_value
-        client.list_locations(request)
-
-
-@pytest.mark.parametrize(
-    "request_type",
-    [
-        locations_pb2.ListLocationsRequest,
-        dict,
-    ],
-)
-def test_list_locations_rest(request_type):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="rest",
-    )
-    request_init = {"name": "projects/sample1"}
-    request = request_type(**request_init)
-    # Mock the http request call within the method and fake a response.
-    with mock.patch.object(type(client.transport._session), "request") as req:
-        # Designate an appropriate value for the returned response.
-        return_value = locations_pb2.ListLocationsResponse()
-
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 200
-        json_return_value = json_format.MessageToJson(return_value)
-
-        response_value._content = json_return_value.encode("UTF-8")
-        req.return_value = response_value
-
-        response = client.list_locations(request)
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, locations_pb2.ListLocationsResponse)
-
-
-def test_cancel_operation_rest_bad_request(
-    transport: str = "rest", request_type=operations_pb2.CancelOperationRequest
-):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    request = request_type()
-    request = json_format.ParseDict(
-        {"name": "projects/sample1/locations/sample2/operations/sample3"}, request
-    )
-
-    # Mock the http request call within the method and fake a BadRequest error.
-    with mock.patch.object(Session, "request") as req, pytest.raises(
-        core_exceptions.BadRequest
-    ):
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 400
-        response_value.request = Request()
-        req.return_value = response_value
-        client.cancel_operation(request)
-
-
-@pytest.mark.parametrize(
-    "request_type",
-    [
-        operations_pb2.CancelOperationRequest,
-        dict,
-    ],
-)
-def test_cancel_operation_rest(request_type):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="rest",
-    )
-    request_init = {"name": "projects/sample1/locations/sample2/operations/sample3"}
-    request = request_type(**request_init)
-    # Mock the http request call within the method and fake a response.
-    with mock.patch.object(type(client.transport._session), "request") as req:
-        # Designate an appropriate value for the returned response.
-        return_value = None
-
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 200
-        json_return_value = "{}"
-
-        response_value._content = json_return_value.encode("UTF-8")
-        req.return_value = response_value
-
-        response = client.cancel_operation(request)
-
-    # Establish that the response is the type that we expect.
-    assert response is None
-
-
-def test_delete_operation_rest_bad_request(
-    transport: str = "rest", request_type=operations_pb2.DeleteOperationRequest
-):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    request = request_type()
-    request = json_format.ParseDict(
-        {"name": "projects/sample1/locations/sample2/operations/sample3"}, request
-    )
-
-    # Mock the http request call within the method and fake a BadRequest error.
-    with mock.patch.object(Session, "request") as req, pytest.raises(
-        core_exceptions.BadRequest
-    ):
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 400
-        response_value.request = Request()
-        req.return_value = response_value
-        client.delete_operation(request)
-
-
-@pytest.mark.parametrize(
-    "request_type",
-    [
-        operations_pb2.DeleteOperationRequest,
-        dict,
-    ],
-)
-def test_delete_operation_rest(request_type):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="rest",
-    )
-    request_init = {"name": "projects/sample1/locations/sample2/operations/sample3"}
-    request = request_type(**request_init)
-    # Mock the http request call within the method and fake a response.
-    with mock.patch.object(type(client.transport._session), "request") as req:
-        # Designate an appropriate value for the returned response.
-        return_value = None
-
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 200
-        json_return_value = "{}"
-
-        response_value._content = json_return_value.encode("UTF-8")
-        req.return_value = response_value
-
-        response = client.delete_operation(request)
-
-    # Establish that the response is the type that we expect.
-    assert response is None
-
-
-def test_get_operation_rest_bad_request(
-    transport: str = "rest", request_type=operations_pb2.GetOperationRequest
-):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    request = request_type()
-    request = json_format.ParseDict(
-        {"name": "projects/sample1/locations/sample2/operations/sample3"}, request
-    )
-
-    # Mock the http request call within the method and fake a BadRequest error.
-    with mock.patch.object(Session, "request") as req, pytest.raises(
-        core_exceptions.BadRequest
-    ):
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 400
-        response_value.request = Request()
-        req.return_value = response_value
-        client.get_operation(request)
-
-
-@pytest.mark.parametrize(
-    "request_type",
-    [
-        operations_pb2.GetOperationRequest,
-        dict,
-    ],
-)
-def test_get_operation_rest(request_type):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="rest",
-    )
-    request_init = {"name": "projects/sample1/locations/sample2/operations/sample3"}
-    request = request_type(**request_init)
-    # Mock the http request call within the method and fake a response.
-    with mock.patch.object(type(client.transport._session), "request") as req:
-        # Designate an appropriate value for the returned response.
-        return_value = operations_pb2.Operation()
-
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 200
-        json_return_value = json_format.MessageToJson(return_value)
-
-        response_value._content = json_return_value.encode("UTF-8")
-        req.return_value = response_value
-
-        response = client.get_operation(request)
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, operations_pb2.Operation)
-
-
-def test_list_operations_rest_bad_request(
-    transport: str = "rest", request_type=operations_pb2.ListOperationsRequest
-):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    request = request_type()
-    request = json_format.ParseDict(
-        {"name": "projects/sample1/locations/sample2"}, request
-    )
-
-    # Mock the http request call within the method and fake a BadRequest error.
-    with mock.patch.object(Session, "request") as req, pytest.raises(
-        core_exceptions.BadRequest
-    ):
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 400
-        response_value.request = Request()
-        req.return_value = response_value
-        client.list_operations(request)
-
-
-@pytest.mark.parametrize(
-    "request_type",
-    [
-        operations_pb2.ListOperationsRequest,
-        dict,
-    ],
-)
-def test_list_operations_rest(request_type):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport="rest",
-    )
-    request_init = {"name": "projects/sample1/locations/sample2"}
-    request = request_type(**request_init)
-    # Mock the http request call within the method and fake a response.
-    with mock.patch.object(type(client.transport._session), "request") as req:
-        # Designate an appropriate value for the returned response.
-        return_value = operations_pb2.ListOperationsResponse()
-
-        # Wrap the value into a proper Response obj
-        response_value = Response()
-        response_value.status_code = 200
-        json_return_value = json_format.MessageToJson(return_value)
-
-        response_value._content = json_return_value.encode("UTF-8")
-        req.return_value = response_value
-
-        response = client.list_operations(request)
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, operations_pb2.ListOperationsResponse)
-
-
-def test_delete_operation(transport: str = "grpc"):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = operations_pb2.DeleteOperationRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = None
-        response = client.delete_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert response is None
-
-
-@pytest.mark.asyncio
-async def test_delete_operation_async(transport: str = "grpc"):
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = operations_pb2.DeleteOperationRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
-        response = await client.delete_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert response is None
-
-
-def test_delete_operation_field_headers():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = operations_pb2.DeleteOperationRequest()
-    request.name = "locations"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
-        call.return_value = None
-
-        client.delete_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations",
-    ) in kw["metadata"]
-
-
-@pytest.mark.asyncio
-async def test_delete_operation_field_headers_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = operations_pb2.DeleteOperationRequest()
-    request.name = "locations"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
-        await client.delete_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations",
-    ) in kw["metadata"]
-
-
-def test_delete_operation_from_dict():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = None
-
-        response = client.delete_operation(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
-@pytest.mark.asyncio
-async def test_delete_operation_from_dict_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
-        response = await client.delete_operation(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
-def test_cancel_operation(transport: str = "grpc"):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = operations_pb2.CancelOperationRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = None
-        response = client.cancel_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert response is None
-
-
-@pytest.mark.asyncio
-async def test_cancel_operation_async(transport: str = "grpc"):
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = operations_pb2.CancelOperationRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
-        response = await client.cancel_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert response is None
-
-
-def test_cancel_operation_field_headers():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = operations_pb2.CancelOperationRequest()
-    request.name = "locations"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
-        call.return_value = None
-
-        client.cancel_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations",
-    ) in kw["metadata"]
-
-
-@pytest.mark.asyncio
-async def test_cancel_operation_field_headers_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = operations_pb2.CancelOperationRequest()
-    request.name = "locations"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
-        await client.cancel_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations",
-    ) in kw["metadata"]
-
-
-def test_cancel_operation_from_dict():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = None
-
-        response = client.cancel_operation(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
-@pytest.mark.asyncio
-async def test_cancel_operation_from_dict_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
-        response = await client.cancel_operation(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
-def test_get_operation(transport: str = "grpc"):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = operations_pb2.GetOperationRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = operations_pb2.Operation()
-        response = client.get_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, operations_pb2.Operation)
-
-
-@pytest.mark.asyncio
-async def test_get_operation_async(transport: str = "grpc"):
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = operations_pb2.GetOperationRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            operations_pb2.Operation()
-        )
-        response = await client.get_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, operations_pb2.Operation)
-
-
-def test_get_operation_field_headers():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = operations_pb2.GetOperationRequest()
-    request.name = "locations"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
-        call.return_value = operations_pb2.Operation()
-
-        client.get_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations",
-    ) in kw["metadata"]
-
-
-@pytest.mark.asyncio
-async def test_get_operation_field_headers_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = operations_pb2.GetOperationRequest()
-    request.name = "locations"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            operations_pb2.Operation()
-        )
-        await client.get_operation(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations",
-    ) in kw["metadata"]
-
-
-def test_get_operation_from_dict():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = operations_pb2.Operation()
-
-        response = client.get_operation(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
-@pytest.mark.asyncio
-async def test_get_operation_from_dict_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            operations_pb2.Operation()
-        )
-        response = await client.get_operation(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
-def test_list_operations(transport: str = "grpc"):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = operations_pb2.ListOperationsRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = operations_pb2.ListOperationsResponse()
-        response = client.list_operations(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, operations_pb2.ListOperationsResponse)
-
-
-@pytest.mark.asyncio
-async def test_list_operations_async(transport: str = "grpc"):
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = operations_pb2.ListOperationsRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            operations_pb2.ListOperationsResponse()
-        )
-        response = await client.list_operations(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, operations_pb2.ListOperationsResponse)
-
-
-def test_list_operations_field_headers():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = operations_pb2.ListOperationsRequest()
-    request.name = "locations"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
-        call.return_value = operations_pb2.ListOperationsResponse()
-
-        client.list_operations(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations",
-    ) in kw["metadata"]
-
-
-@pytest.mark.asyncio
-async def test_list_operations_field_headers_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = operations_pb2.ListOperationsRequest()
-    request.name = "locations"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            operations_pb2.ListOperationsResponse()
-        )
-        await client.list_operations(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations",
-    ) in kw["metadata"]
-
-
-def test_list_operations_from_dict():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = operations_pb2.ListOperationsResponse()
-
-        response = client.list_operations(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
-@pytest.mark.asyncio
-async def test_list_operations_from_dict_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            operations_pb2.ListOperationsResponse()
-        )
-        response = await client.list_operations(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
-def test_list_locations(transport: str = "grpc"):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = locations_pb2.ListLocationsRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = locations_pb2.ListLocationsResponse()
-        response = client.list_locations(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, locations_pb2.ListLocationsResponse)
-
-
-@pytest.mark.asyncio
-async def test_list_locations_async(transport: str = "grpc"):
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = locations_pb2.ListLocationsRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            locations_pb2.ListLocationsResponse()
-        )
-        response = await client.list_locations(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, locations_pb2.ListLocationsResponse)
-
-
-def test_list_locations_field_headers():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = locations_pb2.ListLocationsRequest()
-    request.name = "locations"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
-        call.return_value = locations_pb2.ListLocationsResponse()
-
-        client.list_locations(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations",
-    ) in kw["metadata"]
-
-
-@pytest.mark.asyncio
-async def test_list_locations_field_headers_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = locations_pb2.ListLocationsRequest()
-    request.name = "locations"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            locations_pb2.ListLocationsResponse()
-        )
-        await client.list_locations(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations",
-    ) in kw["metadata"]
-
-
-def test_list_locations_from_dict():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = locations_pb2.ListLocationsResponse()
-
-        response = client.list_locations(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
-@pytest.mark.asyncio
-async def test_list_locations_from_dict_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            locations_pb2.ListLocationsResponse()
-        )
-        response = await client.list_locations(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
-def test_get_location(transport: str = "grpc"):
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = locations_pb2.GetLocationRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = locations_pb2.Location()
-        response = client.get_location(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, locations_pb2.Location)
-
-
-@pytest.mark.asyncio
-async def test_get_location_async(transport: str = "grpc_asyncio"):
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-        transport=transport,
-    )
-
-    # Everything is optional in proto3 as far as the runtime is concerned,
-    # and we are mocking out the actual API, so just send an empty request.
-    request = locations_pb2.GetLocationRequest()
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            locations_pb2.Location()
-        )
-        response = await client.get_location(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the response is the type that we expect.
-    assert isinstance(response, locations_pb2.Location)
-
-
-def test_get_location_field_headers():
-    client = NetAppClient(credentials=ga_credentials.AnonymousCredentials())
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = locations_pb2.GetLocationRequest()
-    request.name = "locations/abc"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
-        call.return_value = locations_pb2.Location()
-
-        client.get_location(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations/abc",
-    ) in kw["metadata"]
-
-
-@pytest.mark.asyncio
-async def test_get_location_field_headers_async():
-    client = NetAppAsyncClient(credentials=ga_credentials.AnonymousCredentials())
-
-    # Any value that is part of the HTTP/1.1 URI should be sent as
-    # a field header. Set these to a non-empty value.
-    request = locations_pb2.GetLocationRequest()
-    request.name = "locations/abc"
-
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            locations_pb2.Location()
-        )
-        await client.get_location(request)
-        # Establish that the underlying gRPC stub method was called.
-        assert len(call.mock_calls) == 1
-        _, args, _ = call.mock_calls[0]
-        assert args[0] == request
-
-    # Establish that the field header was sent.
-    _, _, kw = call.mock_calls[0]
-    assert (
-        "x-goog-request-params",
-        "name=locations/abc",
-    ) in kw["metadata"]
-
-
-def test_get_location_from_dict():
-    client = NetAppClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = locations_pb2.Location()
-
-        response = client.get_location(
-            request={
-                "name": "locations/abc",
-            }
-        )
-        call.assert_called()
-
-
-@pytest.mark.asyncio
-async def test_get_location_from_dict_async():
-    client = NetAppAsyncClient(
-        credentials=ga_credentials.AnonymousCredentials(),
-    )
-    # Mock the actual call within the gRPC stub, and fake the request.
-    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
-        # Designate an appropriate return value for the call.
-        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
-            locations_pb2.Location()
-        )
-        response = await client.get_location(
-            request={
-                "name": "locations",
-            }
-        )
-        call.assert_called()
-
-
 def test_transport_close():
     transports = {
         "rest": "_session",
         "grpc": "_grpc_channel",
     }
 
     for transport, close_name in transports.items():
```

