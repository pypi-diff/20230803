# Comparing `tmp/pasqal-cloud-0.3.3.tar.gz` & `tmp/pasqal-cloud-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.3.3.tar", last modified: Wed Jul  5 14:05:54 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.3.4.tar", last modified: Thu Aug  3 08:43:43 2023, max compression
```

## Comparing `pasqal-cloud-0.3.3.tar` & `pasqal-cloud-0.3.4.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.270878 pasqal-cloud-0.3.3/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.270878 pasqal-cloud-0.3.3/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.270878 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.270878 pasqal-cloud-0.3.3/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.270878 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-05 14:05:54.000000 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-05 14:05:54.000000 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:05:54.000000 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-05 14:05:54.000000 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-05 14:05:54.000000 pasqal-cloud-0.3.3/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:54.274878 pasqal-cloud-0.3.3/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-05 14:05:41.000000 pasqal-cloud-0.3.3/tests/test_project_renaming_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.836665 pasqal-cloud-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-03 08:43:43.836665 pasqal-cloud-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/utils/strenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pasqal_cloud/workload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-03 08:43:43.000000 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-03 08:43:43.000000 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:43:43.000000 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-03 08:43:43.000000 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 08:43:43.000000 pasqal-cloud-0.3.4/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.832665 pasqal-cloud-0.3.4/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-03 08:43:43.836665 pasqal-cloud-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.836665 pasqal-cloud-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:43.836665 pasqal-cloud-0.3.4/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_project_renaming_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-03 08:43:31.000000 pasqal-cloud-0.3.4/tests/test_workload.py
```

### Comparing `pasqal-cloud-0.3.3/LICENSE` & `pasqal-cloud-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.3/PKG-INFO` & `pasqal-cloud-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.3.3
+Version: 0.3.4
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
@@ -99,14 +99,31 @@
 # To access the full results, or in the event that the results aren't expected
 # to contain a "counter" you can do:
 for job in batch.jobs.values():
     print(job.full_result)
 
 ```
 
+### Workload Creation
+
+You can create a workload through the SDK with the following command: 
+```python
+workload=sdk.create_workload(workload_type="<WORKLOAD_TYPE>",backend="<BACKEND>",config={"config_param_1":"value"})
+
+#You can cancel the workload by doing:
+sdk.cancel_workload(workload.id)
+
+#Or refresh the workload status/results by with the following:
+workload=sdk.get_workload(workload.id)
+
+#Once the workload has been processed you can fetch the result like this:
+print(workload.result)
+```
+
+
 ## Advanced usage
 
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
 
 ```python
```

### Comparing `pasqal-cloud-0.3.3/README.md` & `pasqal-cloud-0.3.4/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pasqal-cloud
+Version: 0.3.4
+Summary: Software development kit for Pasqal cloud platform.
+Home-page: https://github.com/pasqal-io/pasqal-cloud
+Maintainer: Pasqal Cloud Services
+Maintainer-email: pcs@pasqal.io
+License: Apache 2.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
 
 To install the latest release of the `pasqal-cloud` (formerly pasqal-sdk), have Python 3.8.0 or higher installed, then use pip:
@@ -84,14 +99,31 @@
 # To access the full results, or in the event that the results aren't expected
 # to contain a "counter" you can do:
 for job in batch.jobs.values():
     print(job.full_result)
 
 ```
 
+### Workload Creation
+
+You can create a workload through the SDK with the following command: 
+```python
+workload=sdk.create_workload(workload_type="<WORKLOAD_TYPE>",backend="<BACKEND>",config={"config_param_1":"value"})
+
+#You can cancel the workload by doing:
+sdk.cancel_workload(workload.id)
+
+#Or refresh the workload status/results by with the following:
+workload=sdk.get_workload(workload.id)
+
+#Once the workload has been processed you can fetch the result like this:
+print(workload.result)
+```
+
+
 ## Advanced usage
 
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
 
 ```python
```

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/__init__.py` & `pasqal-cloud-0.3.4/pasqal_cloud/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,16 +16,22 @@
 from typing import Any, Dict, List, Optional
 from warnings import warn
 
 from pasqal_cloud.authentication import TokenProvider
 from pasqal_cloud.batch import Batch, RESULT_POLLING_INTERVAL
 from pasqal_cloud.client import Client
 from pasqal_cloud.device import BaseConfig, EmulatorType
-from pasqal_cloud.endpoints import AUTH0_CONFIG, Auth0Conf, Endpoints, PASQAL_ENDPOINTS
+from pasqal_cloud.endpoints import (  # noqa: F401
+    AUTH0_CONFIG,
+    Auth0Conf,
+    Endpoints,
+    PASQAL_ENDPOINTS,
+)
 from pasqal_cloud.job import Job
+from pasqal_cloud.workload import Workload
 
 
 class SDK:
     _client: Client
 
     def __init__(
         self,
@@ -45,15 +51,15 @@
         email/password combination or a TokenProvider instance.
         You may omit the password, you will then be prompted to enter one.
 
         Args:
             username: email of the user to login as.
             password: password of the user to login as.
             token_provider: The token provider is an alternative log-in method \
-                not for human users.
+              not for human users.
             webhook: Webhook where the job results are automatically sent to.
             endpoints: Endpoints targeted of the public apis.
             auth0: Auth0Config object to define the auth0 tenant to target.
             project_id: ID of the owner project of the batch.
             group_id (deprecated): Use project_id instead.
         """
 
@@ -77,14 +83,15 @@
             username=username,
             password=password,
             token_provider=token_provider,
             endpoints=endpoints,
             auth0=auth0,
         )
         self.batches: Dict[str, Batch] = {}
+        self.workloads: Dict[str, Workload] = {}
         self.webhook = webhook
 
     def create_batch(
         self,
         serialized_sequence: str,
         jobs: List[Dict[str, Any]],
         emulator: Optional[EmulatorType] = None,
@@ -95,31 +102,31 @@
         """Create a new batch and send it to the API.
         For Iroise MVP, the batch must contain at least one job and will be declared as
         complete immediately.
 
         Args:
             serialized_sequence: Serialized pulser sequence.
             jobs: List of jobs to be added to the batch at creation.
-                (#TODO: Make optional after Iroise MVP)
             emulator: The type of emulator to use,
               If set to None, the device_type will be set to the one
               stored in the serialized sequence
             configuration: A dictionary with extra configuration for the emulators
-                that accept it.
+             that accept it.
             wait: Whether to wait for the batch to be done and fetch results
-            fetch_results (Deprecated): Whether to wait for the batch to be done and fetch results
+            fetch_results (deprecated): Whether to wait for the batch to
+              be done and fetch results
 
 
         Returns:
             Batch: The new batch that has been created in the database.
         """
         if fetch_results:
             warn(
-                "Argument `fetch_results` is deprecated and will be removed in a future"
-                " version. Please use argument `wait` instead.",
+                "Argument `fetch_results` is deprecated and will be removed in a"
+                " future version. Please use argument `wait` instead.",
                 DeprecationWarning,
                 stacklevel=2,
             )
 
         req = {
             "sequence_builder": serialized_sequence,
             "webhook": self.webhook,
@@ -148,23 +155,25 @@
         self.batches[batch.id] = batch
         return batch
 
     def get_batch(self, id: str, fetch_results: bool = False) -> Batch:
         """Retrieve a batch's data and all its jobs.
 
         Args:
+            fetch_results (deprecated): Whether to wait for the batch to be
+              done and fetch results
             id: ID of the batch.
 
         Returns:
             Batch: the batch stored in the PCS database.
         """
         if fetch_results:
             warn(
-                "Argument `fetch_results` is deprecated and will be removed in a future"
-                " version. Results are fetched anyway with this function.",
+                "Argument `fetch_results` is deprecated and will be removed in a"
+                " future version. Results are fetched anyway with this function.",
                 DeprecationWarning,
                 stacklevel=2,
             )
         batch_rsp = self._client._get_batch(id)
         batch = Batch(**batch_rsp, _client=self._client)
         self.batches[batch.id] = batch
         return batch
@@ -203,14 +212,69 @@
         Args:
             id: ID of the job.
         """
         job_rsp = self._client._cancel_job(id)
         job = Job(**job_rsp, _client=self._client)
         return job
 
+    def wait_for_workload(
+        self, id: str, workload_rsp: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        while workload_rsp["status"] in ["PENDING", "RUNNING"]:
+            time.sleep(RESULT_POLLING_INTERVAL)
+            workload_rsp = self._client._get_workload(id)
+        return workload_rsp
+
+    def create_workload(
+        self,
+        workload_type: str,
+        backend: str,
+        config: Dict[str, Any],
+        wait: bool = False,
+    ) -> Workload:
+        req = {
+            "workload_type": workload_type,
+            "backend": backend,
+            "config": config,
+        }
+        workload_rsp = self._client._send_workload(req)
+        if wait:
+            workload_rsp = self.wait_for_workload(workload_rsp["id"], workload_rsp)
+
+        workload = Workload(**workload_rsp, _client=self._client)
+
+        self.workloads[workload.id] = workload
+        return workload
+
+    def get_workload(self, id: str, wait: bool = False) -> Workload:
+        """Retrieve a workload's data.
+
+        Args:
+            id: ID of the workload.
+            wait: Whether to wait for the workload to be done
+
+        Returns:
+            Job: the workload stored in the PCS database.
+        """
+        workload_rsp = self._client._get_workload(id)
+        if wait:
+            workload_rsp = self.wait_for_workload(id, workload_rsp)
+        workload = Workload(**workload_rsp, _client=self._client)
+        return workload
+
+    def cancel_workload(self, id: str) -> Workload:
+        """Cancel the given workload on the PCS
+
+        Args:
+            id: Workload id.
+        """
+        workload_rsp = self._client._cancel_workload(id)
+        workload = Workload(**workload_rsp, _client=self._client)
+        return workload
+
     def get_device_specs_dict(self) -> Dict[str, str]:
         """Retrieve the list of available device specifications.
 
         Returns:
             DeviceSpecs: the list of available device specifications.
         """
```

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/_version.py` & `pasqal-cloud-0.3.4/pasqal_cloud/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
```

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/authentication.py` & `pasqal-cloud-0.3.4/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/batch.py` & `pasqal-cloud-0.3.4/pasqal_cloud/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,27 +23,27 @@
         - created_at: Timestamp of the creation of the batch.
         - updated_at: Timestamp of the last update of the batch.
         - device_type: Type of device to run the batch on.
         - project_id: ID of the owner project of the batch.
         - id: Unique identifier for the batch.
         - user_id: Unique identifier of the user that created the batch.
         - priority: Level of priority of the batch.
-        - status: Status of the batch. Possible values are: \
+        - status: Status of the batch. Possible values are:
             PENDING, RUNNING, DONE, CANCELED, TIMED_OUT, ERROR, PAUSED.
         - webhook: Webhook where the job results are automatically sent to.
         - _client: A Client instance to connect to PCS.
         - sequence_builder: Pulser sequence of the batch.
         - start_datetime: Timestamp of the time the batch was sent to the QPU.
         - end_datetime: Timestamp of when the batch process was finished.
         - device_status: Status of the device where the batch is running.
         - jobs: Dictionary of all the jobs added to the batch.
         - jobs_count: Number of jobs added to the batch.
         - jobs_count_per_status: Number of jobs per status.
         - configuration: Further configuration for certain emulators.
-        - group_id: This parameter is deprecated, use project_id instead.
+        - group_id (deprecated): Use project_id instead.
     """
 
     complete: bool
     created_at: str
     updated_at: str
     device_type: str
     project_id: str
@@ -75,19 +75,22 @@
         if not isinstance(configuration, dict):
             return configuration
         conf_class: Type[BaseConfig] = BaseConfig
         if values["device_type"] == EmulatorType.EMU_TN.value:
             conf_class = EmuTNConfig
         elif values["device_type"] == EmulatorType.EMU_FREE.value:
             conf_class = EmuFreeConfig
-
         return conf_class.from_dict(configuration)
 
     @root_validator(pre=True)
     def _build_job_dict(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        """This root validator will modify the 'jobs' attribute (which is a list
+        of jobs dictionaries ordered by creation time before instantiation) and
+        will transform it to a dictionary of jobs dictionaries.
+        """
         jobs = values.get("jobs", [])
         job_dict = {}
         for job in jobs:
             job_dict[job["id"]] = {**job, "_client": values["_client"]}
         values["jobs"] = job_dict
         return values
 
@@ -123,15 +126,15 @@
     def declare_complete(
         self, wait: bool = False, fetch_results: bool = False
     ) -> Dict[str, Any]:
         """Declare to PCS that the batch is complete.
 
         Args:
             wait: Whether to wait for the batch to be done and fetch results.
-            fetch_results (Deprecated): Whether to wait for the batch \
+            fetch_results (deprecated): Whether to wait for the batch \
                 to be done and fetch results.
 
         A batch that is complete awaits no extra jobs. All jobs previously added
         will be executed before the batch is terminated. When all its jobs are done,
         the complete batch is unassigned to its running device.
         """
         batch_rsp = self._client._complete_batch(self.id)
```

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/client.py` & `pasqal-cloud-0.3.4/pasqal_cloud/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from getpass import getpass
 from typing import Any, Dict, Optional
 
 import requests
 from requests.auth import AuthBase
 
 from pasqal_cloud.authentication import (
-    TokenProvider,
     Auth0TokenProvider,
     HTTPBearerAuthenticator,
+    TokenProvider,
 )
-from pasqal_cloud.endpoints import Endpoints, Auth0Conf
+from pasqal_cloud.endpoints import Auth0Conf, Endpoints
 from pasqal_cloud.errors import HTTPError
 from pasqal_cloud.utils.jsend import JSendPayload
 
 TIMEOUT = 30  # client http requests timeout after 30s
 
 
 class Client:
@@ -155,12 +155,33 @@
 
     def _cancel_job(self, job_id: str) -> Dict[str, Any]:
         job: Dict[str, Any] = self._request(
             "PUT", f"{self.endpoints.core}/api/v1/jobs/{job_id}/cancel"
         )["data"]
         return job
 
+    def _send_workload(self, workload_data: Dict[str, Any]) -> Dict[str, Any]:
+        workload_data.update({"project_id": self.project_id})
+        workload_data = self._request(
+            "POST",
+            f"{self.endpoints.core}/api/v1/workloads",
+            workload_data,
+        )["data"]
+        return workload_data
+
+    def _get_workload(self, workload_id: str) -> Dict[str, Any]:
+        workload: Dict[str, Any] = self._request(
+            "GET", f"{self.endpoints.core}/api/v1/workloads/{workload_id}"
+        )["data"]
+        return workload
+
+    def _cancel_workload(self, workload_id: str) -> Dict[str, Any]:
+        workload: Dict[str, Any] = self._request(
+            "PUT", f"{self.endpoints.core}/api/v1/workloads/{workload_id}/cancel"
+        )["data"]
+        return workload
+
     def get_device_specs_dict(self) -> Dict[str, str]:
         device_specs: Dict[str, str] = self._request(
             "GET", f"{self.endpoints.core}/api/v1/devices/specs"
         )["data"]
         return device_specs
```

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.3.4/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 @dataclass
 class EmuTNConfig(BaseConfig):
     """Configuration for the EmuTN device type.
 
     Args:
         dt (float): The time step in nanoseconds of the simulation. Defaults to 10.0.
         precision (str): The precision of the simulation. Defaults to "normal".
-        max_bond_dim (int): The maximum bond dimension of the Matrix Product State (MPS). Defaults to 500.
+        max_bond_dim (int): The maximum bond dimension of the Matrix Product
+          State (MPS). Defaults to 500.
     """
 
     dt: float = 10.0
     precision: str = "normal"
     max_bond_dim: int = 500
 
     def _validate(self) -> None:
```

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.3.4/pasqal_cloud/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from sys import version_info
-
 from dataclasses import dataclass
+from sys import version_info
 
 if version_info[:2] >= (3, 8):
     from typing import Final
 else:
     from typing_extensions import Final  # type: ignore
```

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/errors.py` & `pasqal-cloud-0.3.4/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/job.py` & `pasqal-cloud-0.3.4/pasqal_cloud/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,26 @@
     """Class for job data.
 
     Attributes:
         - runs: Number of times the job should be run.
         - batch_id: ID of the batch which the job belongs to.
         - id: Unique identifier for the job.
         - project_id: ID of the project which the users scheduling the job belong to.
-        - status: Status of the job. Possible values are: PENDING, RUNNING, DONE, CANCELED, TIMED_OUT, ERROR, PAUSED.
+        - status: Status of the job. Possible values are:
+            PENDING, RUNNING, DONE, CANCELED, TIMED_OUT, ERROR, PAUSED.
         - _client: A Client instance to connect to PCS.
         - created_at: Timestamp of the creation of the job.
         - updated_at: Timestamp of the last update of the job.
         - errors: Error messages that occurred while processing job.
         - start_timestamp: The timestamp of when the job began processing.
         - end_timestamp: The timestamp of when the job finished processing.
         - result: Result of the job.
         - variables: Dictionary of variables of the job.
-          None if the associated batch is non-parametrized.
-        - group_id: This parameter is deprecated, use project_id instead.
+            None if the associated batch is non-parametrized.
+        - group_id (deprecated): Use project_id instead.
     """
 
     runs: int
     batch_id: str
     id: str
     project_id: str
     status: str
```

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.3.4/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.3.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pasqal-cloud
-Version: 0.3.3
-Summary: Software development kit for Pasqal cloud platform.
-Home-page: https://github.com/pasqal-io/pasqal-cloud
-Maintainer: Pasqal Cloud Services
-Maintainer-email: pcs@pasqal.io
-License: Apache 2.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
 
 To install the latest release of the `pasqal-cloud` (formerly pasqal-sdk), have Python 3.8.0 or higher installed, then use pip:
@@ -99,14 +84,31 @@
 # To access the full results, or in the event that the results aren't expected
 # to contain a "counter" you can do:
 for job in batch.jobs.values():
     print(job.full_result)
 
 ```
 
+### Workload Creation
+
+You can create a workload through the SDK with the following command: 
+```python
+workload=sdk.create_workload(workload_type="<WORKLOAD_TYPE>",backend="<BACKEND>",config={"config_param_1":"value"})
+
+#You can cancel the workload by doing:
+sdk.cancel_workload(workload.id)
+
+#Or refresh the workload status/results by with the following:
+workload=sdk.get_workload(workload.id)
+
+#Once the workload has been processed you can fetch the result like this:
+print(workload.result)
+```
+
+
 ## Advanced usage
 
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
 
 ```python
```

### Comparing `pasqal-cloud-0.3.3/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.3.4/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pasqal_cloud/authentication.py
 pasqal_cloud/batch.py
 pasqal_cloud/client.py
 pasqal_cloud/endpoints.py
 pasqal_cloud/errors.py
 pasqal_cloud/job.py
 pasqal_cloud/py.typed
+pasqal_cloud/workload.py
 pasqal_cloud.egg-info/PKG-INFO
 pasqal_cloud.egg-info/SOURCES.txt
 pasqal_cloud.egg-info/dependency_links.txt
 pasqal_cloud.egg-info/requires.txt
 pasqal_cloud.egg-info/top_level.txt
 pasqal_cloud/device/__init__.py
 pasqal_cloud/device/emulator_types.py
@@ -38,9 +39,10 @@
 tests/test_batch.py
 tests/test_client.py
 tests/test_cloud_sdk_import.py
 tests/test_config.py
 tests/test_device_specs.py
 tests/test_job.py
 tests/test_project_renaming_compatibility.py
+tests/test_workload.py
 tests/test_doubles/__init__.py
 tests/test_doubles/authentication.py
```

### Comparing `pasqal-cloud-0.3.3/sdk/setup.py` & `pasqal-cloud-0.3.4/sdk/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from setuptools import setup
 import os
 
+from setuptools import setup
+
 VERSION = "0.1.15"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
```

### Comparing `pasqal-cloud-0.3.3/setup.py` & `pasqal-cloud-0.3.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,36 +24,33 @@
     packages=find_packages(),
     package_data={"pasqal_cloud": ["py.typed"]},
     include_package_data=True,
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     maintainer="Pasqal Cloud Services",
     maintainer_email="pcs@pasqal.io",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     license="Apache 2.0",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
     ],
     url="https://github.com/pasqal-io/pasqal-cloud",
     install_requires=[
-        "auth0-python >= 3.23.1, <4.0.0 ",
+        "auth0-python >= 3.23.1, <4.0.0",
         "requests>=2.25.1, <3.0.0",
         "pyjwt[crypto]>=2.5.0, <3.0.0",
         "pydantic>=1.10, <2.0",
     ],
     extras_require={
         "dev": {
-            "black==22.3.0",
-            "flake8==3.9.0",
-            "flake8-import-order==0.18.1",
+            "black==23.3.0",
+            "flake8==6.0.0",
+            "isort==5.12.0",
             "mypy==0.982",
-            "pytest==6.2.5",
-            "pytest-cov==2.11.1",
-            "types-requests==2.25.1",
-            "requests-mock==1.9.3",
-        },
-        ":python_version == '3.7'": [
-            "typing-extensions==4.4.0",
-        ],
+            "pytest==7.4.0",
+            "pytest-cov==4.1.0",
+            "types-requests==2.31.0.1",
+            "requests-mock==1.11.0",
+        }
     },
 )
```

### Comparing `pasqal-cloud-0.3.3/tests/conftest.py` & `pasqal-cloud-0.3.4/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 from unittest.mock import patch
 
 import pytest
 import requests_mock
 
-from pasqal_cloud import Client, Batch, Job
+from pasqal_cloud import Batch, Client, Job, Workload
 from pasqal_cloud.endpoints import Endpoints
 from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
 
 TEST_API_FIXTURES_PATH = "tests/fixtures/api"
 JSON_FILE = "_.{}.json"
 
 
@@ -63,14 +63,31 @@
         username="00000000-0000-0000-0000-000000000001",
         password="password",
     )
     return client
 
 
 @pytest.fixture
+def workload(pasqal_client_mock):
+    workload_data = {
+        "id": "00000000-0000-0000-0000-000000000001",
+        "project_id": "00000000-0000-0000-0000-000000000001",
+        "status": "PENDING",
+        "_client": pasqal_client_mock,
+        "created_at": "2022-12-31T23:59:59.999Z",
+        "updated_at": "2023-01-01T00:00:00.000Z",
+        "errors": [],
+        "backend": "backend_test",
+        "workload_type": "workload_type_test",
+        "config": {"test1": "test1", "test2": 2},
+    }
+    return Workload(**workload_data)
+
+
+@pytest.fixture
 def batch(pasqal_client_mock):
     batch_data = {
         "complete": False,
         "created_at": "2022-12-31T23:59:59.999Z",
         "updated_at": "2023-01-01T00:00:00.000Z",
         "device_type": "qpu",
         "project_id": "00000000-0000-0000-0000-000000000002",
@@ -80,15 +97,14 @@
         "status": "PENDING",
         "webhook": "https://example.com/webhook",
         "_client": pasqal_client_mock,
         "sequence_builder": "pulser",
         "start_datetime": "2023-01-01T00:00:00.000Z",
         "end_datetime": None,
         "device_status": "available",
-        "jobs": {},
     }
     return Batch(**batch_data)
 
 
 @pytest.fixture
 def job(pasqal_client_mock):
     job_data = {
```

### Comparing `pasqal-cloud-0.3.3/tests/test_batch.py` & `pasqal-cloud-0.3.4/tests/test_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,48 +6,65 @@
 from pasqal_cloud import Batch, Job, SDK
 from pasqal_cloud.device import BaseConfig, EmuFreeConfig, EmulatorType, EmuTNConfig
 from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
 
 
 class TestBatch:
     @pytest.fixture(autouse=True)
-    @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
+    @patch(
+        "pasqal_cloud.client.Auth0TokenProvider",
+        FakeAuth0AuthenticationSuccess,
+    )
     def init_sdk(self, start_mock_request):
         self.sdk = SDK(
-            username="me@test.com", password="password", project_id=str(uuid4())
+            username="me@test.com",
+            password="password",
+            project_id=str(uuid4()),
         )
         self.pulser_sequence = "pulser_test_sequence"
         self.batch_id = "00000000-0000-0000-0000-000000000001"
         self.job_result = {"1001": 12, "0110": 35, "1111": 1}
         self.job_full_result = {
             "counter": {"1001": 12, "0110": 35, "1111": 1},
             "raw": ["1001", "1001", "0110", "1001", "0110"],
         }
         self.n_job_runs = 50
         self.job_id = "00000000-0000-0000-0000-000000022010"
-        self.job_variables = {"Omega_max": 14.4, "last_target": "q1", "ts": [200, 500]}
+        self.job_variables = {
+            "Omega_max": 14.4,
+            "last_target": "q1",
+            "ts": [200, 500],
+        }
 
     @pytest.mark.parametrize("emulator", [None] + [e.value for e in EmulatorType])
     def test_create_batch(self, emulator):
-        job = {"runs": self.n_job_runs, "variables": self.job_variables}
+        job = {
+            "runs": self.n_job_runs,
+            "variables": self.job_variables,
+        }
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
             jobs=[job],
             emulator=emulator,
         )
         assert batch.id == self.batch_id
         assert batch.sequence_builder == self.pulser_sequence
-        # TODO: Remove after IROISE MVP
         assert batch.complete
         assert batch.jobs[self.job_id].batch_id == batch.id
-        assert batch.jobs[self.job_id].runs == self.n_job_runs
 
+    @pytest.mark.filterwarnings(
+        "ignore:Argument `fetch_results` is deprecated and will be removed "
+        "in a future version. Please use argument `wait` instead"
+    )
     @pytest.mark.parametrize("wait,fetch_results", [(True, False), (False, True)])
     def test_create_batch_and_wait(self, request_mock, wait, fetch_results):
-        job = {"runs": self.n_job_runs, "variables": self.job_variables}
+        job = {
+            "runs": self.n_job_runs,
+            "variables": self.job_variables,
+        }
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
             jobs=[job],
             wait=wait,
             fetch_results=fetch_results,
         )
         assert (
@@ -67,26 +84,26 @@
         assert batch_requested.id == self.batch_id
 
     def test_cancel_batch_self(self, request_mock, batch):
         batch.cancel()
         assert batch.status == "CANCELED"
         assert request_mock.last_request.method == "PUT"
         assert (
-            request_mock.last_request.url
-            == f"{self.sdk._client.endpoints.core}/api/v1/batches/{self.batch_id}/cancel"
+            request_mock.last_request.url == f"{self.sdk._client.endpoints.core}"
+            f"/api/v1/batches/{self.batch_id}/cancel"
         )
 
     def test_cancel_batch_sdk(self, request_mock):
         client_rsp = self.sdk.cancel_batch(self.batch_id)
         assert type(client_rsp) == Batch
         assert client_rsp.status == "CANCELED"
         assert request_mock.last_request.method == "PUT"
         assert (
-            request_mock.last_request.url
-            == f"{self.sdk._client.endpoints.core}/api/v1/batches/{self.batch_id}/cancel"
+            request_mock.last_request.url == f"{self.sdk._client.endpoints.core}"
+            f"/api/v1/batches/{self.batch_id}/cancel"
         )
 
     def test_get_job(self, job):
         job_requested = self.sdk.get_job(job.id)
         print(self.sdk)
         assert job_requested.id == job.id
 
@@ -125,15 +142,19 @@
     @pytest.mark.skip(reason="Not enabled during Iroise MVP")
     def test_batch_add_job_and_wait_for_results(self, request_mock):
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
         )
         job = batch.add_job(
             runs=self.n_job_runs,
-            variables={"Omega_max": 14.4, "last_target": "q1", "ts": [200, 500]},
+            variables={
+                "Omega_max": 14.4,
+                "last_target": "q1",
+                "ts": [200, 500],
+            },
             wait=True,
         )
         assert job.batch_id == batch.id
         assert job.runs == self.n_job_runs
         assert request_mock.last_request.method == "GET"
         assert (
             request_mock.last_request.url
@@ -181,15 +202,18 @@
                 "SomethingElse",
                 BaseConfig(),
                 BaseConfig(extra_config={"dt": 10.0, "precision": "normal"}),
             ),
         ],
     )
     def test_create_batch_configuration(self, emulator, configuration, expected):
-        job = {"runs": self.n_job_runs, "variables": self.job_variables}
+        job = {
+            "runs": self.n_job_runs,
+            "variables": self.job_variables,
+        }
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
             jobs=[job],
             emulator=emulator,
             configuration=configuration,
         )
         assert batch.configuration == expected
@@ -209,15 +233,18 @@
         assert (
             new_batch.new_field == "any_value"
         )  # The new value should be stored regardless
 
     def test_create_batch_fetch_results_deprecated(
         self,
     ):
-        job = {"runs": self.n_job_runs, "variables": self.job_variables}
+        job = {
+            "runs": self.n_job_runs,
+            "variables": self.job_variables,
+        }
         with pytest.warns(DeprecationWarning):
             self.sdk.create_batch(
                 serialized_sequence=self.pulser_sequence,
                 jobs=[job],
                 fetch_results=True,
             )
```

### Comparing `pasqal-cloud-0.3.3/tests/test_client.py` & `pasqal-cloud-0.3.4/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest.mock import patch
 
 import pytest
 from auth0.v3.exceptions import Auth0Error  # type: ignore
 
-from pasqal_cloud import Auth0Conf, Endpoints, SDK, AUTH0_CONFIG, PASQAL_ENDPOINTS
+from pasqal_cloud import AUTH0_CONFIG, Auth0Conf, Endpoints, PASQAL_ENDPOINTS, SDK
 from pasqal_cloud.authentication import TokenProvider
 from tests.test_doubles.authentication import (
     FakeAuth0AuthenticationFailure,
     FakeAuth0AuthenticationSuccess,
 )
```

### Comparing `pasqal-cloud-0.3.3/tests/test_config.py` & `pasqal-cloud-0.3.4/tests/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import re
 
 import pytest
+
 from pasqal_cloud.device import EmuFreeConfig
 from pasqal_cloud.device.configuration.base_config import (
     BaseConfig,
     INVALID_KEY_ERROR_MSG,
     INVALID_RESULT_TYPES,
     InvalidConfiguration,
 )
```

### Comparing `pasqal-cloud-0.3.3/tests/test_device_specs.py` & `pasqal-cloud-0.3.4/tests/test_device_specs.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
-from uuid import uuid4
 from unittest.mock import patch
+from uuid import uuid4
 
 import pytest
 
 from pasqal_cloud import SDK
 from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
```

### Comparing `pasqal-cloud-0.3.3/tests/test_doubles/authentication.py` & `pasqal-cloud-0.3.4/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.3/tests/test_job.py` & `pasqal-cloud-0.3.4/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.3.3/tests/test_project_renaming_compatibility.py` & `pasqal-cloud-0.3.4/tests/test_project_renaming_compatibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from unittest.mock import patch
 
 import pytest
 
 from pasqal_cloud import SDK
 from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
 
-
 """
 Ticket (#622), Python file to be entirely removed
 """
 
 
 @patch("pasqal_cloud.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
 class TestInitSDKWithGroupId:
```

