# Comparing `tmp/google-cloud-containeranalysis-2.9.2.tar.gz` & `tmp/google-cloud-containeranalysis-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-containeranalysis-2.9.2.tar", last modified: Tue Oct  4 00:20:20 2022, max compression
+gzip compressed data, was "google-cloud-containeranalysis-2.9.3.tar", last modified: Mon Oct 10 16:29:29 2022, max compression
```

## Comparing `google-cloud-containeranalysis-2.9.2.tar` & `google-cloud-containeranalysis-2.9.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5123 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4213 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.979618 google-cloud-containeranalysis-2.9.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.979618 google-cloud-containeranalysis-2.9.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.983619 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.983619 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis/
--rw-rw-r--   0 root         (0)     1003     1279 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis/__init__.py
--rw-rw-r--   0 root         (0)     1003      100 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.983619 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/
--rw-rw-r--   0 root         (0)     1003     1055 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1668 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/gapic_metadata.json
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.983619 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/proto/
--rw-rw-r--   0 root         (0)     1003     6309 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/proto/containeranalysis.proto
--rw-rw-r--   0 root         (0)     1003      100 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.983619 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.983619 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/
--rw-rw-r--   0 root         (0)     1003      781 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/__init__.py
--rw-rw-r--   0 root         (0)     1003    36356 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/async_client.py
--rw-rw-r--   0 root         (0)     1003    44626 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/
--rw-rw-r--   0 root         (0)     1003     1221 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7838 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17521 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17808 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/types/
--rw-rw-r--   0 root         (0)     1003      822 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3091 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/types/containeranalysis.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/google_cloud_containeranalysis.egg-info/
--rw-r--r--   0 root         (0)     1003     5123 2022-10-04 00:20:20.000000 google-cloud-containeranalysis-2.9.2/google_cloud_containeranalysis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1866 2022-10-04 00:20:20.000000 google-cloud-containeranalysis-2.9.2/google_cloud_containeranalysis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:20:20.000000 google-cloud-containeranalysis-2.9.2/google_cloud_containeranalysis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       42 2022-10-04 00:20:20.000000 google-cloud-containeranalysis-2.9.2/google_cloud_containeranalysis.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-04 00:20:20.000000 google-cloud-containeranalysis-2.9.2/google_cloud_containeranalysis.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      244 2022-10-04 00:20:20.000000 google-cloud-containeranalysis-2.9.2/google_cloud_containeranalysis.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-04 00:20:20.000000 google-cloud-containeranalysis-2.9.2/google_cloud_containeranalysis.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/scripts/
--rw-rw-r--   0 root         (0)     1003     6187 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/scripts/fixup_containeranalysis_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2770 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-04 00:20:20.987619 google-cloud-containeranalysis-2.9.2/tests/unit/gapic/containeranalysis_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/tests/unit/gapic/containeranalysis_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    88674 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/tests/unit/gapic/containeranalysis_v1/test_container_analysis.py
--rw-rw-r--   0 root         (0)     1003      468 2022-10-04 00:17:17.000000 google-cloud-containeranalysis-2.9.2/tests/unit/test_get_grafeas_client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.619286 google-cloud-containeranalysis-2.9.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5123 2022-10-10 16:29:29.619286 google-cloud-containeranalysis-2.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4213 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.611285 google-cloud-containeranalysis-2.9.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.611285 google-cloud-containeranalysis-2.9.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.611285 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.611285 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis/
+-rw-rw-r--   0 root         (0)     1003     1279 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis/__init__.py
+-rw-rw-r--   0 root         (0)     1003      100 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.615286 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/
+-rw-rw-r--   0 root         (0)     1003     1055 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1668 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/gapic_metadata.json
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.615286 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/proto/
+-rw-rw-r--   0 root         (0)     1003     6309 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/proto/containeranalysis.proto
+-rw-rw-r--   0 root         (0)     1003      100 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.615286 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.615286 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/
+-rw-rw-r--   0 root         (0)     1003      781 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/__init__.py
+-rw-rw-r--   0 root         (0)     1003    36356 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/async_client.py
+-rw-rw-r--   0 root         (0)     1003    44626 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.615286 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/
+-rw-rw-r--   0 root         (0)     1003     1221 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7838 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17521 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17808 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.615286 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/types/
+-rw-rw-r--   0 root         (0)     1003      822 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3091 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/types/containeranalysis.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.619286 google-cloud-containeranalysis-2.9.3/google_cloud_containeranalysis.egg-info/
+-rw-r--r--   0 root         (0)     1003     5123 2022-10-10 16:29:29.000000 google-cloud-containeranalysis-2.9.3/google_cloud_containeranalysis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1866 2022-10-10 16:29:29.000000 google-cloud-containeranalysis-2.9.3/google_cloud_containeranalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:29:29.000000 google-cloud-containeranalysis-2.9.3/google_cloud_containeranalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       42 2022-10-10 16:29:29.000000 google-cloud-containeranalysis-2.9.3/google_cloud_containeranalysis.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:29:29.000000 google-cloud-containeranalysis-2.9.3/google_cloud_containeranalysis.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      316 2022-10-10 16:29:29.000000 google-cloud-containeranalysis-2.9.3/google_cloud_containeranalysis.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:29:29.000000 google-cloud-containeranalysis-2.9.3/google_cloud_containeranalysis.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.619286 google-cloud-containeranalysis-2.9.3/scripts/
+-rw-rw-r--   0 root         (0)     1003     6187 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/scripts/fixup_containeranalysis_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:29:29.619286 google-cloud-containeranalysis-2.9.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2839 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.619286 google-cloud-containeranalysis-2.9.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.619286 google-cloud-containeranalysis-2.9.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.619286 google-cloud-containeranalysis-2.9.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:29:29.619286 google-cloud-containeranalysis-2.9.3/tests/unit/gapic/containeranalysis_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/tests/unit/gapic/containeranalysis_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    88674 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/tests/unit/gapic/containeranalysis_v1/test_container_analysis.py
+-rw-rw-r--   0 root         (0)     1003      468 2022-10-10 16:25:48.000000 google-cloud-containeranalysis-2.9.3/tests/unit/test_get_grafeas_client.py
```

### Comparing `google-cloud-containeranalysis-2.9.2/LICENSE` & `google-cloud-containeranalysis-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/MANIFEST.in` & `google-cloud-containeranalysis-2.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/PKG-INFO` & `google-cloud-containeranalysis-2.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-containeranalysis
-Version: 2.9.2
+Version: 2.9.3
 Summary: Container Analysis API API client library
 Home-page: https://github.com/googleapis/python-containeranalysis
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-containeranalysis-2.9.2/README.rst` & `google-cloud-containeranalysis-2.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis/__init__.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/__init__.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/gapic_metadata.json` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/proto/containeranalysis.proto` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/proto/containeranalysis.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/__init__.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/__init__.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/async_client.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/client.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/__init__.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/base.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/grpc.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/grpc_asyncio.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/services/container_analysis/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/types/__init__.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google/cloud/devtools/containeranalysis_v1/types/containeranalysis.py` & `google-cloud-containeranalysis-2.9.3/google/cloud/devtools/containeranalysis_v1/types/containeranalysis.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/google_cloud_containeranalysis.egg-info/PKG-INFO` & `google-cloud-containeranalysis-2.9.3/google_cloud_containeranalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-containeranalysis
-Version: 2.9.2
+Version: 2.9.3
 Summary: Container Analysis API API client library
 Home-page: https://github.com/googleapis/python-containeranalysis
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-containeranalysis-2.9.2/google_cloud_containeranalysis.egg-info/SOURCES.txt` & `google-cloud-containeranalysis-2.9.3/google_cloud_containeranalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/scripts/fixup_containeranalysis_v1_keywords.py` & `google-cloud-containeranalysis-2.9.3/scripts/fixup_containeranalysis_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/setup.py` & `google-cloud-containeranalysis-2.9.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 import os
 
 import setuptools
 
 
 name = "google-cloud-containeranalysis"
 description = "Container Analysis API API client library"
-version = "2.9.2"
+version = "2.9.3"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
     "proto-plus >= 1.22.0, <2.0.0dev",
-    "protobuf >= 3.20.2, <5.0.0dev",
+    "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "grafeas >=1.4.1, <2.0dev",
 ]
 extras = {"libcst": "libcst >= 0.2.5"}
 
 
 package_root = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `google-cloud-containeranalysis-2.9.2/tests/__init__.py` & `google-cloud-containeranalysis-2.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/tests/unit/__init__.py` & `google-cloud-containeranalysis-2.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/tests/unit/gapic/__init__.py` & `google-cloud-containeranalysis-2.9.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/tests/unit/gapic/containeranalysis_v1/__init__.py` & `google-cloud-containeranalysis-2.9.3/tests/unit/gapic/containeranalysis_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-containeranalysis-2.9.2/tests/unit/gapic/containeranalysis_v1/test_container_analysis.py` & `google-cloud-containeranalysis-2.9.3/tests/unit/gapic/containeranalysis_v1/test_container_analysis.py`

 * *Files identical despite different names*

