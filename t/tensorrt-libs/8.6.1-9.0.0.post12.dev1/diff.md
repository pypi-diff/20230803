# Comparing `tmp/tensorrt-libs-8.6.1.tar.gz` & `tmp/tensorrt-libs-9.0.0.post12.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorrt-libs-8.6.1.tar", last modified: Wed May  3 00:04:10 2023, max compression
+gzip compressed data, was "tensorrt-libs-9.0.0.post12.dev1.tar", last modified: Thu Aug  3 20:43:44 2023, max compression
```

## Comparing `tensorrt-libs-8.6.1.tar` & `tensorrt-libs-9.0.0.post12.dev1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-03 00:04:10.701327 tensorrt-libs-8.6.1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      445 2023-05-03 00:04:10.000000 tensorrt-libs-8.6.1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-04-29 02:47:53.000000 tensorrt-libs-8.6.1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       13 2023-05-03 00:04:10.000000 tensorrt-libs-8.6.1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1599 2023-05-03 00:04:10.701327 tensorrt-libs-8.6.1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      244 2023-05-03 00:04:10.000000 tensorrt-libs-8.6.1/README.rst
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-05-03 00:04:10.701327 tensorrt-libs-8.6.1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-04-29 02:47:53.000000 tensorrt-libs-8.6.1/setup.py
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-05-03 00:04:10.701327 tensorrt-libs-8.6.1/tensorrt_libs.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1599 2023-05-03 00:04:10.000000 tensorrt-libs-8.6.1/tensorrt_libs.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      201 2023-05-03 00:04:10.000000 tensorrt-libs-8.6.1/tensorrt_libs.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-05-03 00:04:10.000000 tensorrt-libs-8.6.1/tensorrt_libs.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-05-03 00:04:10.000000 tensorrt-libs-8.6.1/tensorrt_libs.egg-info/top_level.txt
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-03 20:43:44.836446 tensorrt-libs-9.0.0.post12.dev1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      445 2023-08-03 20:43:44.000000 tensorrt-libs-9.0.0.post12.dev1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-05 21:17:33.000000 tensorrt-libs-9.0.0.post12.dev1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       13 2023-08-03 20:43:44.000000 tensorrt-libs-9.0.0.post12.dev1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1611 2023-08-03 20:43:44.836446 tensorrt-libs-9.0.0.post12.dev1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      244 2023-08-03 20:43:44.000000 tensorrt-libs-9.0.0.post12.dev1/README.rst
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-08-03 20:43:44.836446 tensorrt-libs-9.0.0.post12.dev1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-05 21:17:33.000000 tensorrt-libs-9.0.0.post12.dev1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-03 20:43:44.836446 tensorrt-libs-9.0.0.post12.dev1/tensorrt_libs.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1611 2023-08-03 20:43:44.000000 tensorrt-libs-9.0.0.post12.dev1/tensorrt_libs.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      201 2023-08-03 20:43:44.000000 tensorrt-libs-9.0.0.post12.dev1/tensorrt_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-08-03 20:43:44.000000 tensorrt-libs-9.0.0.post12.dev1/tensorrt_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-08-03 20:43:44.000000 tensorrt-libs-9.0.0.post12.dev1/tensorrt_libs.egg-info/top_level.txt
```

### Comparing `tensorrt-libs-8.6.1/LICENSE.md` & `tensorrt-libs-9.0.0.post12.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tensorrt-libs-8.6.1/PKG-INFO` & `tensorrt-libs-9.0.0.post12.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt-libs
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

### Comparing `tensorrt-libs-8.6.1/setup.py` & `tensorrt-libs-9.0.0.post12.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `tensorrt-libs-8.6.1/tensorrt_libs.egg-info/PKG-INFO` & `tensorrt-libs-9.0.0.post12.dev1/tensorrt_libs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt-libs
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

