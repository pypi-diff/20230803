# Comparing `tmp/tensorrt_dispatch-8.6.1.tar.gz` & `tmp/tensorrt_dispatch-9.0.0.post12.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tensorrt_dispatch-8.6.1.tar", last modified: Wed Apr 26 22:12:22 2023, max compression
+gzip compressed data, was "tensorrt_dispatch-9.0.0.post12.dev1.tar", last modified: Thu Aug  3 20:59:32 2023, max compression
```

## Comparing `tensorrt_dispatch-8.6.1.tar` & `tensorrt_dispatch-9.0.0.post12.dev1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/tensorrt_dispatch/
--rw-r--r--   0 root         (0) root         (0)      763 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/tensorrt_dispatch/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46991 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      581 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2267 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/tensorrt_dispatch.egg-info/
--rw-r--r--   0 root         (0) root         (0)      581 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/tensorrt_dispatch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/tensorrt_dispatch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/tensorrt_dispatch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/tensorrt_dispatch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/tensorrt_dispatch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 22:12:22.000000 tensorrt_dispatch-8.6.1/tensorrt_dispatch.egg-info/zip-safe
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-03 20:59:32.627886 tensorrt_dispatch-9.0.0.post12.dev1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      449 2023-08-03 20:59:32.000000 tensorrt_dispatch-9.0.0.post12.dev1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-05 21:17:33.000000 tensorrt_dispatch-9.0.0.post12.dev1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2023-08-03 20:59:32.000000 tensorrt_dispatch-9.0.0.post12.dev1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1627 2023-08-03 20:59:32.627886 tensorrt_dispatch-9.0.0.post12.dev1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      256 2023-08-03 20:59:32.000000 tensorrt_dispatch-9.0.0.post12.dev1/README.rst
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-08-03 20:59:32.627886 tensorrt_dispatch-9.0.0.post12.dev1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-05 21:17:33.000000 tensorrt_dispatch-9.0.0.post12.dev1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-03 20:59:32.627886 tensorrt_dispatch-9.0.0.post12.dev1/tensorrt_dispatch.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1627 2023-08-03 20:59:32.000000 tensorrt_dispatch-9.0.0.post12.dev1/tensorrt_dispatch.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2023-08-03 20:59:32.000000 tensorrt_dispatch-9.0.0.post12.dev1/tensorrt_dispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-08-03 20:59:32.000000 tensorrt_dispatch-9.0.0.post12.dev1/tensorrt_dispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-08-03 20:59:32.000000 tensorrt_dispatch-9.0.0.post12.dev1/tensorrt_dispatch.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

