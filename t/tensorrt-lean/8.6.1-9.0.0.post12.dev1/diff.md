# Comparing `tmp/tensorrt_lean-8.6.1.tar.gz` & `tmp/tensorrt_lean-9.0.0.post12.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tensorrt_lean-8.6.1.tar", last modified: Wed Apr 26 22:12:22 2023, max compression
+gzip compressed data, was "tensorrt_lean-9.0.0.post12.dev1.tar", last modified: Thu Aug  3 20:54:12 2023, max compression
```

## Comparing `tensorrt_lean-8.6.1.tar` & `tensorrt_lean-9.0.0.post12.dev1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/
--rw-r--r--   0 root         (0) root         (0)    46991 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/tensorrt_lean/
--rw-r--r--   0 root         (0) root         (0)      763 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/tensorrt_lean/__init__.py
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/tensorrt_lean.egg-info/
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/tensorrt_lean.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/tensorrt_lean.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/tensorrt_lean.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/tensorrt_lean.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/tensorrt_lean.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/tensorrt_lean.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     2263 2023-04-26 22:12:22.000000 tensorrt_lean-8.6.1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-03 20:54:12.844019 tensorrt_lean-9.0.0.post12.dev1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      445 2023-08-03 20:54:12.000000 tensorrt_lean-9.0.0.post12.dev1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-05 21:17:33.000000 tensorrt_lean-9.0.0.post12.dev1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       13 2023-08-03 20:54:12.000000 tensorrt_lean-9.0.0.post12.dev1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1611 2023-08-03 20:54:12.844019 tensorrt_lean-9.0.0.post12.dev1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      244 2023-08-03 20:54:12.000000 tensorrt_lean-9.0.0.post12.dev1/README.rst
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-08-03 20:54:12.844019 tensorrt_lean-9.0.0.post12.dev1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-05 21:17:33.000000 tensorrt_lean-9.0.0.post12.dev1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-03 20:54:12.844019 tensorrt_lean-9.0.0.post12.dev1/tensorrt_lean.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1611 2023-08-03 20:54:12.000000 tensorrt_lean-9.0.0.post12.dev1/tensorrt_lean.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      201 2023-08-03 20:54:12.000000 tensorrt_lean-9.0.0.post12.dev1/tensorrt_lean.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-08-03 20:54:12.000000 tensorrt_lean-9.0.0.post12.dev1/tensorrt_lean.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-08-03 20:54:12.000000 tensorrt_lean-9.0.0.post12.dev1/tensorrt_lean.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

