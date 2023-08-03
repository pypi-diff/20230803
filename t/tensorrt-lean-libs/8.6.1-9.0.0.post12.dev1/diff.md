# Comparing `tmp/tensorrt-lean-libs-8.6.1.tar.gz` & `tmp/tensorrt-lean-libs-9.0.0.post12.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorrt-lean-libs-8.6.1.tar", last modified: Wed May  3 00:01:47 2023, max compression
+gzip compressed data, was "tensorrt-lean-libs-9.0.0.post12.dev1.tar", last modified: Thu Aug  3 20:55:03 2023, max compression
```

## Comparing `tensorrt-lean-libs-8.6.1.tar` & `tensorrt-lean-libs-9.0.0.post12.dev1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-03 00:01:47.518997 tensorrt-lean-libs-8.6.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      450 2023-05-03 00:01:47.000000 tensorrt-lean-libs-8.6.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-29 02:47:53.000000 tensorrt-lean-libs-8.6.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       18 2023-05-03 00:01:47.000000 tensorrt-lean-libs-8.6.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1619 2023-05-03 00:01:47.518997 tensorrt-lean-libs-8.6.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      259 2023-05-03 00:01:47.000000 tensorrt-lean-libs-8.6.1/README.rst
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-05-03 00:01:47.518997 tensorrt-lean-libs-8.6.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-29 02:47:53.000000 tensorrt-lean-libs-8.6.1/setup.py
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-03 00:01:47.518997 tensorrt-lean-libs-8.6.1/tensorrt_lean_libs.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1619 2023-05-03 00:01:47.000000 tensorrt-lean-libs-8.6.1/tensorrt_lean_libs.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      221 2023-05-03 00:01:47.000000 tensorrt-lean-libs-8.6.1/tensorrt_lean_libs.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-05-03 00:01:47.000000 tensorrt-lean-libs-8.6.1/tensorrt_lean_libs.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-05-03 00:01:47.000000 tensorrt-lean-libs-8.6.1/tensorrt_lean_libs.egg-info/top_level.txt
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-03 20:55:03.881907 tensorrt-lean-libs-9.0.0.post12.dev1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      450 2023-08-03 20:55:03.000000 tensorrt-lean-libs-9.0.0.post12.dev1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-05 21:17:33.000000 tensorrt-lean-libs-9.0.0.post12.dev1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       18 2023-08-03 20:55:03.000000 tensorrt-lean-libs-9.0.0.post12.dev1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1631 2023-08-03 20:55:03.881907 tensorrt-lean-libs-9.0.0.post12.dev1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      259 2023-08-03 20:55:03.000000 tensorrt-lean-libs-9.0.0.post12.dev1/README.rst
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-08-03 20:55:03.881907 tensorrt-lean-libs-9.0.0.post12.dev1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-05 21:17:33.000000 tensorrt-lean-libs-9.0.0.post12.dev1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-03 20:55:03.881907 tensorrt-lean-libs-9.0.0.post12.dev1/tensorrt_lean_libs.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1631 2023-08-03 20:55:03.000000 tensorrt-lean-libs-9.0.0.post12.dev1/tensorrt_lean_libs.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      221 2023-08-03 20:55:03.000000 tensorrt-lean-libs-9.0.0.post12.dev1/tensorrt_lean_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-08-03 20:55:03.000000 tensorrt-lean-libs-9.0.0.post12.dev1/tensorrt_lean_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-08-03 20:55:03.000000 tensorrt-lean-libs-9.0.0.post12.dev1/tensorrt_lean_libs.egg-info/top_level.txt
```

### Comparing `tensorrt-lean-libs-8.6.1/LICENSE.md` & `tensorrt-lean-libs-9.0.0.post12.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tensorrt-lean-libs-8.6.1/PKG-INFO` & `tensorrt-lean-libs-9.0.0.post12.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt-lean-libs
-Version: 8.6.1
+Version: 9.0.0.post12.dev1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `tensorrt-lean-libs-8.6.1/setup.py` & `tensorrt-lean-libs-9.0.0.post12.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `tensorrt-lean-libs-8.6.1/tensorrt_lean_libs.egg-info/PKG-INFO` & `tensorrt-lean-libs-9.0.0.post12.dev1/tensorrt_lean_libs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt-lean-libs
-Version: 8.6.1
+Version: 9.0.0.post12.dev1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

