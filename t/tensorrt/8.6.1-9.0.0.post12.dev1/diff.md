# Comparing `tmp/tensorrt-8.6.1.tar.gz` & `tmp/tensorrt-9.0.0.post12.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tensorrt-8.6.1.tar", last modified: Wed Apr 26 22:12:22 2023, max compression
+gzip compressed data, was "tensorrt-9.0.0.post12.dev1.tar", last modified: Thu Aug  3 20:41:16 2023, max compression
```

## Comparing `tensorrt-8.6.1.tar` & `tensorrt-9.0.0.post12.dev1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 22:12:22.000000 tensorrt-8.6.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 22:12:22.000000 tensorrt-8.6.1/tensorrt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-26 22:12:22.000000 tensorrt-8.6.1/tensorrt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-26 22:12:22.000000 tensorrt-8.6.1/tensorrt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 22:12:22.000000 tensorrt-8.6.1/tensorrt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-04-26 22:12:22.000000 tensorrt-8.6.1/tensorrt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-26 22:12:22.000000 tensorrt-8.6.1/tensorrt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 22:12:22.000000 tensorrt-8.6.1/tensorrt.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)    46991 2023-04-26 22:12:22.000000 tensorrt-8.6.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-26 22:12:22.000000 tensorrt-8.6.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 22:12:22.000000 tensorrt-8.6.1/tensorrt/
--rw-r--r--   0 root         (0) root         (0)      763 2023-04-26 22:12:22.000000 tensorrt-8.6.1/tensorrt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-26 22:12:22.000000 tensorrt-8.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2258 2023-04-26 22:12:22.000000 tensorrt-8.6.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-03 20:41:16.162842 tensorrt-9.0.0.post12.dev1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      440 2023-08-03 20:41:16.000000 tensorrt-9.0.0.post12.dev1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-05 21:17:33.000000 tensorrt-9.0.0.post12.dev1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        8 2023-08-03 20:41:16.000000 tensorrt-9.0.0.post12.dev1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1591 2023-08-03 20:41:16.162842 tensorrt-9.0.0.post12.dev1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      229 2023-08-03 20:41:16.000000 tensorrt-9.0.0.post12.dev1/README.rst
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-08-03 20:41:16.162842 tensorrt-9.0.0.post12.dev1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-05 21:17:33.000000 tensorrt-9.0.0.post12.dev1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-03 20:41:16.162842 tensorrt-9.0.0.post12.dev1/tensorrt.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1591 2023-08-03 20:41:16.000000 tensorrt-9.0.0.post12.dev1/tensorrt.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      181 2023-08-03 20:41:16.000000 tensorrt-9.0.0.post12.dev1/tensorrt.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-08-03 20:41:16.000000 tensorrt-9.0.0.post12.dev1/tensorrt.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-08-03 20:41:16.000000 tensorrt-9.0.0.post12.dev1/tensorrt.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

