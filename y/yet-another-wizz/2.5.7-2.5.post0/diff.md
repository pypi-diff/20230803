# Comparing `tmp/yet_another_wizz-2.5.7.tar.gz` & `tmp/yet_another_wizz-2.5.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_wizz-2.5.7.tar", last modified: Thu Aug  3 18:08:42 2023, max compression
+gzip compressed data, was "yet_another_wizz-2.5.post0.tar", last modified: Mon Jul 10 08:18:48 2023, max compression
```

## Comparing `yet_another_wizz-2.5.7.tar` & `yet_another_wizz-2.5.post0.tar`

### file list

```diff
@@ -1,74 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.767669 yet_another_wizz-2.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-08-03 18:08:42.767669 yet_another_wizz-2.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 18:08:42.767669 yet_another_wizz-2.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.759669 yet_another_wizz-2.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.759669 yet_another_wizz-2.5.7/src/yaw/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.759669 yet_another_wizz-2.5.7/src/yaw/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/linkage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.763669 yet_another_wizz-2.5.7/src/yaw/catalogs/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/scipy/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/scipy/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/scipy/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/scipy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.763669 yet_another_wizz-2.5.7/src/yaw/catalogs/treecorr/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/treecorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/catalogs/treecorr/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.763669 yet_another_wizz-2.5.7/src/yaw/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/config/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/config/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/config/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/config/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/config/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/config/resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/config/scales.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.763669 yet_another_wizz-2.5.7/src/yaw/core/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/core/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/core/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/core/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/core/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/core/math.c
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.763669 yet_another_wizz-2.5.7/src/yaw/correlation/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40606 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/correlation/corrfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/correlation/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    41950 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/correlation/paircounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.767669 yet_another_wizz-2.5.7/src/yaw/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.767669 yet_another_wizz-2.5.7/src/yaw/deprecated/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/deprecated/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/deprecated/config/binning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.767669 yet_another_wizz-2.5.7/src/yaw/deprecated/correlation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/deprecated/correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/deprecated/correlation/corrfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/deprecated/correlation/paircounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/deprecated/redshifts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.767669 yet_another_wizz-2.5.7/src/yaw/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129479 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/examples/auto_reference.hdf
--rw-r--r--   0 runner    (1001) docker     (123)   123032 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/examples/auto_unknown_1.hdf
--rw-r--r--   0 runner    (1001) docker     (123)   100475 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/examples/cross_1.hdf
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-08-03 18:07:41.000000 yet_another_wizz-2.5.7/src/yaw/redshifts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:08:42.767669 yet_another_wizz-2.5.7/src/yet_another_wizz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-08-03 18:08:42.000000 yet_another_wizz-2.5.7/src/yet_another_wizz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-03 18:08:42.000000 yet_another_wizz-2.5.7/src/yet_another_wizz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:08:42.000000 yet_another_wizz-2.5.7/src/yet_another_wizz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-03 18:08:42.000000 yet_another_wizz-2.5.7/src/yet_another_wizz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 18:08:42.000000 yet_another_wizz-2.5.7/src/yet_another_wizz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.318014 yet_another_wizz-2.5.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.322014 yet_another_wizz-2.5.post0/src/yaw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.322014 yet_another_wizz-2.5.post0/src/yaw/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/linkage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.326015 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.326015 yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15092 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.330015 yet_another_wizz-2.5.post0/src/yaw/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/scales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.334015 yet_another_wizz-2.5.post0/src/yaw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/math.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.334015 yet_another_wizz-2.5.post0/src/yaw/correlation/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40475 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/corrfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/paircounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.334015 yet_another_wizz-2.5.post0/src/yaw/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129479 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/auto_reference.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)   123032 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/auto_unknown_1.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)   100475 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/cross_1.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22413 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/redshifts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.338015 yet_another_wizz-2.5.post0/src/yaw_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.338015 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.338015 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/default_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/top_level.txt
```

### Comparing `yet_another_wizz-2.5.7/LICENSE` & `yet_another_wizz-2.5.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/PKG-INFO` & `yet_another_wizz-2.5.post0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 Metadata-Version: 2.1
 Name: yet_another_wizz
-Version: 2.5.7
-Summary: Implementation of the Schmidt et al. (2013) clustering redshift method.
+Version: 2.5.post0
+Summary: Implementation of the Schmidt et al. (2013) clustering redshift method and wrapper scripts to produce cross-correlation (CC) redshifts.
 Home-page: https://github.com/jlvdb/yet_another_wizz.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: cli
 Provides-Extra: plot
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: style
 Provides-Extra: dev
 License-File: LICENSE
 
-.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz/main/docs/source/_static/logo-dark.png
-    :width: 1000
-    :alt: yet_another_wizz
-
-|
-
-.. image:: https://img.shields.io/pypi/v/yet_another_wizz?logo=pypi&logoColor=blue
-    :target: https://pypi.org/project/yet_another_wizz/
-.. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/docker-publish.yml/badge.svg
-    :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/docker-publish.yml
-.. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml/badge.svg
-    :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml
+yet_another_wizz
+================
+
+.. image:: https://badge.fury.io/py/yet-another-wizz.svg
+    :target: https://badge.fury.io/py/yet-another-wizz
 .. image:: https://readthedocs.org/projects/yet-another-wizz/badge/?version=latest
     :target: https://yet-another-wizz.readthedocs.io/en/latest/?badge=latest
+.. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml/badge.svg
+    :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
 
-|
 
 *yet_another_wizz* is a python package to efficiently compute cross-correlation
 redshifts, also know as clustering redshifts and is hosted on github:
 
 - code: https://github.com/jlvdb/yet_another_wizz.git
 - docs: https://yet-another-wizz.readthedocs.io/
 - PyPI: https://pypi.org/project/yet_another_wizz/
-- Docker: https://hub.docker.com/r/jlvdb/yet_another_wizz/
 
 The method allows to estimate the unknown redshift distribution of a galaxy
 sample by correlating the on-sky positions with a reference sample with known
 redshifts. This implementation is based on the single bin correlation
 measurement of the correlation amplitude, introduced by Schmidt et al. (2013,
 `arXiv:1303.0292 <https://arxiv.org/abs/1303.0292>`_).
 
@@ -61,63 +57,41 @@
 Installation
 ------------
 
 The yet_another_wizz package can be installed directly with pip::
 
     pip install yet_another_wizz
 
-This will install the python library ``yaw``.
-
-Commandline tool
-~~~~~~~~~~~~~~~~
-
-There also exists a separate command line tool called
-`yet_another_wizz_cli <https://github.com/jlvdb/yet_another_wizz_cli>`_
-(``yaw_cli``) that is available at PyPI and github. To install it alongside the
-python library, type::
-
-    pip install yet_another_wizz[cli]
-
-LSST-DESC RAIL plugin
-~~~~~~~~~~~~~~~~~~~~~
-
-Currently there is also a
-`plugin interface <https://github.com/jlvdb/yet_another_wizz_rail>`_  for the
-Redshift Assessment Infrastructure Layers
-(`RAIL <https://github.com/LSSTDESC/rail>`_) pipeline under development. To
-install it alongside the python library, including ``rail`` itself, type::
-
-    pip install yet_another_wizz[rail]
+This will install the python package ``yaw``, as well as the ``yaw_cli``
+executable command line tool.
 
 
 Usage
 -----
 
 There are two main ways to use yet_another_wizz,
 
-- the python library ``yaw`` itself and
-- the (separate) ``yaw_cli`` commmand line tool.
-- the (separate) ``yaw_rail`` RAIL plugin (coming soon).
+- the ``yaw_cli`` commmand line tool and
+- the python package ``yaw`` directly.
 
-Most users will probably get started with the command line tool, which should
+Most people will probably get started with the command line tool, which should
 cover all necessary tasks for a standard clustering redshift calibration. For
-custom solutions, use the python library. A basic example as well as the API
+custom solutions, use the python package. A basic example as well as the API
 reference can be found in the official documentation.
 
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
 
 https://github.com/jlvdb/yet_another_wizz/issues
 
 
-Maintainers
------------
+**Maintainers:**
 
 - Jan Luca van den Busch
   (*author*, Ruhr-Universität Bochum, Astronomisches Institut)
 
 
 Acknowledgements
 ----------------
```

### Comparing `yet_another_wizz-2.5.7/README.rst` & `yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,50 @@
-.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz/main/docs/source/_static/logo-dark.png
-    :width: 1000
-    :alt: yet_another_wizz
-
-|
-
-.. image:: https://img.shields.io/pypi/v/yet_another_wizz?logo=pypi&logoColor=blue
-    :target: https://pypi.org/project/yet_another_wizz/
-.. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/docker-publish.yml/badge.svg
-    :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/docker-publish.yml
-.. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml/badge.svg
-    :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml
+Metadata-Version: 2.1
+Name: yet-another-wizz
+Version: 2.5.post0
+Summary: Implementation of the Schmidt et al. (2013) clustering redshift method and wrapper scripts to produce cross-correlation (CC) redshifts.
+Home-page: https://github.com/jlvdb/yet_another_wizz.git
+Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
+License: GPL-3.0-or-later
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: plot
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: style
+Provides-Extra: dev
+License-File: LICENSE
+
+yet_another_wizz
+================
+
+.. image:: https://badge.fury.io/py/yet-another-wizz.svg
+    :target: https://badge.fury.io/py/yet-another-wizz
 .. image:: https://readthedocs.org/projects/yet-another-wizz/badge/?version=latest
     :target: https://yet-another-wizz.readthedocs.io/en/latest/?badge=latest
+.. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml/badge.svg
+    :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
 
-|
 
 *yet_another_wizz* is a python package to efficiently compute cross-correlation
 redshifts, also know as clustering redshifts and is hosted on github:
 
 - code: https://github.com/jlvdb/yet_another_wizz.git
 - docs: https://yet-another-wizz.readthedocs.io/
 - PyPI: https://pypi.org/project/yet_another_wizz/
-- Docker: https://hub.docker.com/r/jlvdb/yet_another_wizz/
 
 The method allows to estimate the unknown redshift distribution of a galaxy
 sample by correlating the on-sky positions with a reference sample with known
 redshifts. This implementation is based on the single bin correlation
 measurement of the correlation amplitude, introduced by Schmidt et al. (2013,
 `arXiv:1303.0292 <https://arxiv.org/abs/1303.0292>`_).
 
@@ -40,63 +57,41 @@
 Installation
 ------------
 
 The yet_another_wizz package can be installed directly with pip::
 
     pip install yet_another_wizz
 
-This will install the python library ``yaw``.
-
-Commandline tool
-~~~~~~~~~~~~~~~~
-
-There also exists a separate command line tool called
-`yet_another_wizz_cli <https://github.com/jlvdb/yet_another_wizz_cli>`_
-(``yaw_cli``) that is available at PyPI and github. To install it alongside the
-python library, type::
-
-    pip install yet_another_wizz[cli]
-
-LSST-DESC RAIL plugin
-~~~~~~~~~~~~~~~~~~~~~
-
-Currently there is also a
-`plugin interface <https://github.com/jlvdb/yet_another_wizz_rail>`_  for the
-Redshift Assessment Infrastructure Layers
-(`RAIL <https://github.com/LSSTDESC/rail>`_) pipeline under development. To
-install it alongside the python library, including ``rail`` itself, type::
-
-    pip install yet_another_wizz[rail]
+This will install the python package ``yaw``, as well as the ``yaw_cli``
+executable command line tool.
 
 
 Usage
 -----
 
 There are two main ways to use yet_another_wizz,
 
-- the python library ``yaw`` itself and
-- the (separate) ``yaw_cli`` commmand line tool.
-- the (separate) ``yaw_rail`` RAIL plugin (coming soon).
+- the ``yaw_cli`` commmand line tool and
+- the python package ``yaw`` directly.
 
-Most users will probably get started with the command line tool, which should
+Most people will probably get started with the command line tool, which should
 cover all necessary tasks for a standard clustering redshift calibration. For
-custom solutions, use the python library. A basic example as well as the API
+custom solutions, use the python package. A basic example as well as the API
 reference can be found in the official documentation.
 
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
 
 https://github.com/jlvdb/yet_another_wizz/issues
 
 
-Maintainers
------------
+**Maintainers:**
 
 - Jan Luca van den Busch
   (*author*, Ruhr-Universität Bochum, Astronomisches Institut)
 
 
 Acknowledgements
 ----------------
```

### Comparing `yet_another_wizz-2.5.7/pyproject.toml` & `yet_another_wizz-2.5.post0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,56 +4,55 @@
 
 [project]
 name = "yet_another_wizz"
 dynamic = ["version"]
 authors = [
     {name = "Jan Luca van den Busch", email = "jlvdb@astro.ruhr-uni-bochum.de"},
 ]
-description = "Implementation of the Schmidt et al. (2013) clustering redshift method."
+description = "Implementation of the Schmidt et al. (2013) clustering redshift method and wrapper scripts to produce cross-correlation (CC) redshifts."
 readme = "README.rst"
 license = {text = "GPL-3.0-or-later"}
 classifiers = [
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Astronomy",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
 ]
 requires-python = ">=3.8"
 dependencies = [
     "typing_extensions;python_version<'3.10'",
     "more_itertools;python_version<'3.10'",
     "deprecated",
-    "tqdm",
     "numpy",
+    "pyarrow",
+    "tqdm",
+    "h5py",
     "pandas",
     "astropandas>=1.2.1",
     "scipy",
     "astropy",
-    "pyarrow",
-    "h5py",
-    "pyyaml",
     "treecorr>=4.3",
+    "emcee",
+    "matplotlib",
 ]
 
+[project.scripts]
+yaw_cli = "yaw_cli:Commandline.main"
+
 [project.optional-dependencies]
-cli = ["yet_another_wizz_cli>=1.2.1"]
-# rail = ["yet_another_wizz_rail @ git+ssh://git@github.com/jlvdb/yet_another_wizz_rail"]
 plot = ["matplotlib"]
-# note that yaw_cli is currently necessary to generate the joint docs
 docs = [
     "sphinx",
     "sphinx-design",
     "sphinx-copybutton",
     "pydata-sphinx-theme",
-    "yet_another_wizz[cli]",
 ]
 test = [
     "typing_extensions",
     "more_itertools",
-    "yet_another_wizz[plot]",
     "coverage",
     "pytest",
     "pytest-cov",
 ]
 style = [
     "black",
     "isort",
@@ -78,21 +77,17 @@
     "examples/*.hdf",
     "examples/*.dat",
     "examples/*.cov",
     "examples/*.smp",
 ]
 
 [tool.pytest.ini_options]
-testpaths = [
-    "tests",
-]
-addopts = [
-    "--cov=yaw",
-    "--cov-report=xml",
-]
+minversion = "6.0"
+addopts = "-ra -q"
+testpaths = ["tests"]
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 include = ".pyi?$"
 exclude = """
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,21 +24,24 @@
 _logging.getLogger(__name__).addHandler(_logging.NullHandler())  # noqa
 
 from yaw.catalogs import NewCatalog
 from yaw.config import Configuration, ResamplingConfig
 from yaw.core.cosmology import Scale
 from yaw.core.math import global_covariance
 from yaw.correlation import CorrData, CorrFunc, autocorrelate, crosscorrelate
+from yaw.deprecated import (
+    CorrelationData,
+    CorrelationFunction,
+    HistogramData,
+    PairCountResult,
+)
 from yaw.randoms import UniformRandoms
 from yaw.redshifts import HistData, RedshiftData
 
-# isort: split
-from yaw.deprecated.correlation.corrfuncs import CorrelationData, CorrelationFunction
-from yaw.deprecated.correlation.paircounts import PairCountResult
-from yaw.deprecated.redshifts import HistogramData
+__version__ = "2.5.post0"
 
 __all__ = [
     "NewCatalog",
     "Configuration",
     "ResamplingConfig",
     "Scale",
     "global_covariance",
@@ -51,8 +54,7 @@
     "RedshiftData",
     # deprecated
     "CorrelationData",
     "CorrelationFunction",
     "HistogramData",
     "PairCountResult",
 ]
-__version__ = "2.5.7"
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/catalogs/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/catalogs/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import logging
-from abc import abstractmethod
+from abc import abstractclassmethod, abstractmethod, abstractproperty
 from collections.abc import Iterator
 from typing import TYPE_CHECKING, Any, TypeVar
 
 import astropandas as apd
 import numpy as np
 from numpy.typing import NDArray
 
@@ -113,38 +113,37 @@
         else:
             raise TypeError(
                 "'patches' must be either of type 'str' (col. name), 'int' "
                 "(number of patches), or 'Catalog' or 'Coordinate' (specify "
                 "centers)"
             )
 
-        cls._logger.info("reading catalog file '%s'", filepath)
+        cls._logger.info(f"reading catalog file '{filepath}'")
         data = apd.read_auto(filepath, columns=columns, ext=file_ext, **kwargs)
         if sparse is not None:
-            cls._logger.debug("sparse sampling data %ix", sparse)
+            cls._logger.debug(f"sparse sampling data {sparse}x")
             data = data[::sparse]
         return cls(
             data,
             ra,
             dec,
             **patch_kwarg,
             redshift_name=redshift,
             weight_name=weight,
             cache_directory=cache_directory,
             progress=progress,
         )
 
-    @classmethod
-    @abstractmethod
+    @abstractclassmethod
     def from_cache(cls, cache_directory: str, progress: bool = False) -> BaseCatalog:
         """Restore the catalogue from its cache directory.
 
         Catalogs should be instantiated through the factory class, see
         :meth:`yaw.catalogs.NewCatalog.from_cache`."""
-        cls._logger.info("restoring from cache directory '%s'", cache_directory)
+        cls._logger.info(f"restoring from cache directory '{cache_directory}'")
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
         args = dict(
             loaded=self.is_loaded(),
             nobjects=len(self),
             npatches=self.n_patches,
@@ -157,16 +156,15 @@
     def __len__(self) -> int:
         pass
 
     @abstractmethod
     def __getitem__(self, item: int) -> Any:
         pass
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def ids(self) -> list[int]:
         """Return a list of unique patch indices in the catalog."""
         pass
 
     @abstractmethod
     def n_patches(self) -> int:
         """The number of spatial patches of this catalogue."""
@@ -213,77 +211,69 @@
         """Get a vector of the object sky positions in radians.
 
         Returns:
             :obj:`yaw.core.coordinates.CoordSky`
         """
         return CoordSky(self.ra, self.dec)
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def ra(self) -> NDArray[np.float_]:
         """Get an array of the right ascension values in radians."""
         pass
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def dec(self) -> NDArray[np.float_]:
         """Get an array of the declination values in radians."""
         pass
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def redshifts(self) -> NDArray[np.float_] | None:
         """Get the redshifts as array or ``None`` if not available."""
         pass
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def weights(self) -> NDArray[np.float_]:
         """Get the object weights as array or ``None`` if not available."""
         pass
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def patch(self) -> NDArray[np.int_]:
         """Get the patch indices of each object as array."""
         pass
 
     @abstractmethod
     def get_min_redshift(self) -> float:
         """Get the minimum redshift or ``None`` if not available."""
         pass
 
     @abstractmethod
     def get_max_redshift(self) -> float:
         """Get the maximum redshift or ``None`` if not available."""
         pass
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def total(self) -> float:
         """Get the sum of weights or the number of objects if weights are not
         available."""
 
     @abstractmethod
     def get_totals(self) -> NDArray[np.float_]:
         """Get an array of the sum of weights or number of objects in each
         patch."""
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def centers(self) -> CoordSky:
         """Get a vector of sky coordinates of the patch centers in radians.
 
         Returns:
             :obj:`yaw.core.coordinates.CoordSky`
         """
         pass
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def radii(self) -> DistSky:
         """Get a vector of angular separations in radians that describe the
         patch sizes.
 
         The radius of the patch is defined as the maximum angular distance of
         any object from the patch center.
 
@@ -343,19 +333,16 @@
 
         The catalogue from the calling instance of :meth:`correlate` has always
         redshift binning applied.
         """
         n1 = long_num_format(len(self))
         n2 = long_num_format(len(self) if other is None else len(other))
         self._logger.debug(
-            "correlating with %sbinned catalog (%sx%s) in %d redshift bins",
-            "" if binned else "un",
-            n1,
-            n2,
-            config.binning.zbin_num,
+            f"correlating with {'' if binned else 'un'}binned catalog "
+            f"({n1}x{n2}) in {config.binning.zbin_num} redshift bins"
         )
 
     @abstractmethod
     def true_redshifts(
         self,
         config: Configuration,
         sampling_config: ResamplingConfig | None = None,
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/catalogs/factory.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/factory.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/catalogs/linkage.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/linkage.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,29 +72,29 @@
             max_query_radius = r_kpc_to_angle(
                 config.scales.as_array(), z_ref, config.cosmology
             ).max()
         else:
             max_query_radius = 0.0  # only relevant for cross-patch
         max_query_radius = DistSky(max_query_radius)
 
-        logger.debug("computing patch linkage with %.3e", max_query_radius.values)
+        logger.debug(f"computing patch linkage with {max_query_radius=:.3e}")
         centers_3d = catalog.centers.to_3d().values
         radii = catalog.radii.values
         # compute distance between all patch centers
         dist_mat_3d = Dist3D(distance_matrix(centers_3d, centers_3d))
         # compare minimum separation required for patchs to not overlap
         size_sum = DistSky(np.add.outer(radii, radii))
 
         # check which patches overlap when factoring in the query radius
         overlaps = dist_mat_3d.to_sky() < (size_sum + max_query_radius)
         patch_pairs = []
         for id1, overlap in enumerate(overlaps):
             patch_pairs.extend((id1, id2) for id2 in np.where(overlap)[0])
         logger.debug(
-            "found %d patch links for %d patches", len(patch_pairs), catalog.n_patches
+            f"found {len(patch_pairs)} patch links " f"for {catalog.n_patches} patches"
         )
         return cls(patch_pairs)
 
     def __len__(self) -> int:
         return len(self.pairs)
 
     def __repr__(self) -> str:
@@ -191,15 +191,15 @@
         return matrix
 
     def get_patches(
         self,
         collection1: BaseCatalog,
         collection2: BaseCatalog | None = None,
         crosspatch: bool = True,
-    ) -> tuple[list, list]:
+    ) -> tuple[list[BaseCatalog], list[BaseCatalog]]:
         """Return linked pairs of patch data ready for processing.
 
         Instead of returning a list of patch index pairs, the actual patch data
         is returned in two aligned list, where item 1 form the first list is
         linked to item 1 of the second list. Depending on if one or two catalogs
         are provided as input, the result resembles a cross- or autocorrelation
         patch linkage.
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/catalogs/scipy/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/catalog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,362 +1,444 @@
 from __future__ import annotations
 
-import multiprocessing
+import itertools
 import os
+import sys
 from collections.abc import Iterator
-from itertools import repeat
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, NoReturn, Tuple
+
+try:  # pragma: no cover
+    from typing import TypeAlias
+except ImportError:  # pragma: no cover
+    from typing_extensions import TypeAlias
 
 import numpy as np
 import pandas as pd
+from numpy.typing import NDArray
+from treecorr import Catalog, NNCorrelation
 
-from yaw.catalogs import BaseCatalog, PatchLinkage
-from yaw.catalogs.scipy import utils
-from yaw.catalogs.scipy.patches import (
-    PatchCatalog,
-    assign_patches,
-    create_patches,
-    patch_id_from_path,
-)
+from yaw.catalogs import BaseCatalog
 from yaw.config import Configuration, ResamplingConfig
 from yaw.core.coordinates import Coord3D, Coordinate, CoordSky, DistSky
 from yaw.core.logging import TimedLog
-from yaw.core.utils import LimitTracker, job_progress_bar, long_num_format
-from yaw.correlation.paircounts import NormalisedCounts
+from yaw.correlation.paircounts import (
+    NormalisedCounts,
+    PatchedCount,
+    PatchedTotal,
+    pack_results,
+)
 from yaw.redshifts import HistData
 
 if TYPE_CHECKING:  # pragma: no cover
-    from numpy.typing import NDArray
-    from pandas import DataFrame
+    from pandas import DataFrame, Interval
+
+    from yaw.catalogs import PatchLinkage
+
+__all__ = ["EmptyCatalog", "TreecorrCatalog"]
+
+
+TypeNNResult: TypeAlias = Dict[Tuple[int, int], NNCorrelation]  # supports py3.8
 
-    from yaw.core.containers import PatchCorrelationData
 
+def _iter_bin_masks(
+    data: NDArray, bins: NDArray, closed: str = "left"
+) -> Iterator[tuple[Interval, NDArray[np.bool_]]]:
+    """Split data into bins and return an iterator that yields the boolean masks
+    that select the data of the current bin out of the input data array."""
+    if closed not in ("left", "right"):
+        raise ValueError("'closed' must be either of 'left', 'right'")
+    intervals = pd.IntervalIndex.from_breaks(bins, closed=closed)
+    bin_ids = np.digitize(data, bins, right=(closed == "right"))
+    for i, interval in enumerate(intervals, 1):
+        yield interval, (bin_ids == i)
+
+
+def take_subset(
+    cat: TreecorrCatalog, items: NDArray[np.bool_] | NDArray[np.int_] | slice
+) -> TreecorrCatalog | EmptyCatalog:
+    """Construct a new TreecorrCatalog with a subset of its entries."""
+    ra = cat.ra[items]
+    if len(ra) == 0:
+        return EmptyCatalog(n_patches=cat.n_patches)
+    kwargs = dict(
+        ra=ra,
+        ra_units="radian",
+        dec=cat.dec[items],
+        dec_units="radian",
+        patch=cat.patch[items],
+    )
+    if cat.has_redshifts():
+        kwargs["r"] = cat.redshifts[items]
+    if cat.has_weights():
+        kwargs["w"] = cat.weights[items]
+    return TreecorrCatalog.from_treecorr(Catalog(**kwargs))
 
-__all__ = ["ScipyCatalog"]
 
+class EmptyCatalog:
+    """A minimal representation of a TreecorrCatalog that contains no data."""
 
-def _worker_correlate(
-    args: tuple[PatchCatalog, PatchCatalog, Configuration, bool, bool]
-) -> PatchCorrelationData:
-    return utils.count_pairs_patches(*args)
+    def __init__(self, n_patches: int) -> None:
+        self.n_patches = n_patches
 
+    def __len__(self) -> int:
+        return 0
+
+    def total(self) -> float:
+        return 0.0
 
-def _worker_true_redshifts(
-    args: tuple[PatchCatalog, NDArray[np.float_]]
-) -> NDArray[np.float_]:
-    return utils.count_histogram_patch(*args)
+    def get_totals(self) -> NDArray[np.float_]:
+        return np.zeros(self.n_patches)
 
 
-class ScipyCatalog(BaseCatalog):
-    """An implementation of the :obj:`BaseCatalog` using a wrapper around
-    :obj:`scipy.spatial.cKDTree` for the pair counting, which is implemented in
-    :obj:`yaw.catalogs.scipy.kdtree`. Fully supports caching.
+class TreecorrCatalog(BaseCatalog):
+    """An implementation of the :obj:`BaseCatalog` using ``TreeCorr`` for the
+    pair counting.
 
     .. Note::
 
-        This is currently the default backend and has the best support and
-        performance. Currently, trees cannot be shared across the
-        multiprocessing interface and must be rebuilt every time a patch is
-        used for pair counting again.
+        The current implementation is not very efficient, because the internal
+        fields of the underlying :obj:`treecorr.Catalog` must be rebuilt every
+        time the catalog is iterated in redshift bins for the pair counting.
+
+    .. Warning::
+
+        Currently this backend does not support restoration from cache and
+        raises an :obj:`NotImplementedError`` when calling the
+        :meth:`from_cache` method.
     """
 
     def __init__(
         self,
         data: DataFrame,
         ra_name: str,
         dec_name: str,
         *,
         patch_name: str | None = None,
         patch_centers: BaseCatalog | Coordinate | None = None,
         n_patches: int | None = None,
         redshift_name: str | None = None,
         weight_name: str | None = None,
         cache_directory: str | None = None,
-        progress: bool = True,
+        progress: bool = False,
     ) -> None:
-        if len(data) == 0:
-            raise ValueError("data catalog is empty")
-        # check if the columns exist
-        renames = {ra_name: "ra", dec_name: "dec"}
-        if redshift_name is not None:
-            renames[redshift_name] = "redshift"
-        if weight_name is not None:
-            renames[weight_name] = "weights"
-        for col_name, kind in renames.items():
-            if col_name not in data:
-                raise KeyError(f"column {kind}='{col_name}' not found in data")
-
-        # check if patches should be written and unloaded from memory
-        unload = cache_directory is not None
-        if patch_name is not None:
-            patch_mode = "dividing"
-        else:
-            if n_patches is not None:
-                patch_mode = "creating"
-            elif patch_centers is not None:
-                patch_mode = "applying"
-            else:
-                raise ValueError(
-                    "either of 'patch_name', 'patch_centers', or 'n_patches' "
-                    "must be provided"
-                )
-        if unload:
+        # construct the underlying TreeCorr catalogue
+        kwargs = dict()
+        if cache_directory is not None:
+            kwargs["save_patch_dir"] = cache_directory
             if not os.path.exists(cache_directory):
                 raise FileNotFoundError(
                     f"patch directory does not exist: '{cache_directory}'"
                 )
-            self._logger.debug("using cache directory '%s'", cache_directory)
+            self._logger.info(f"using cache directory '{cache_directory}'")
 
-        # create new patches
-        if patch_mode != "dividing":
-            position = CoordSky.from_array(
-                np.deg2rad(data[[ra_name, dec_name]].to_numpy())
-            )
-            if patch_mode == "creating":
-                patch_centers, patch_ids = create_patches(
-                    position=position, n_patches=n_patches
-                )
-                log_msg = "creating %i patches"
-            else:
-                if isinstance(patch_centers, BaseCatalog):
-                    patch_centers = patch_centers.centers.to_3d()
-                patch_ids = assign_patches(centers=patch_centers, position=position)
-                n_patches = len(patch_centers)
-                log_msg = "applying %i patches from external data"
-            patch_name = "patch"  # the default name
-            data[patch_name] = patch_ids
-            centers = {pid: pos for pid, pos in enumerate(patch_centers)}
+        if n_patches is not None:
+            kwargs["npatch"] = n_patches
+            log_msg = f"creating {n_patches} patches"
+        elif patch_name is not None:
+            kwargs["patch"] = data[patch_name]
+            log_msg = "splitting data into predefined patches"
+        elif isinstance(patch_centers, BaseCatalog):
+            kwargs["patch_centers"] = patch_centers.centers.to_3d().values
+            n_patches = patch_centers.n_patches
+            log_msg = f"applying {n_patches} patches from external data"
+        elif isinstance(patch_centers, Coordinate):
+            centers = patch_centers.to_3d()
+            kwargs["patch_centers"] = centers.values
+            n_patches = len(centers)
+            log_msg = f"applying {n_patches} patches from external data"
         else:
-            n_patches = len(data[patch_name].unique())
-            log_msg = "dividing data into %i predefined patches"
-            centers = dict()  # this can be empty
-        self._logger.debug(log_msg, n_patches)
-
-        # run groupby first to avoid any intermediate copies of full data
-        n_obj_str = long_num_format(len(data))
-        with TimedLog(self._logger.info, f"processed {n_obj_str} records"):
-            limits = LimitTracker()
-            patches: dict[int, PatchCatalog] = {}
-            patch_iter = data.groupby(patch_name)
-            if progress:
-                patch_iter = job_progress_bar(patch_iter, total=n_patches)
-            for patch_id, patch_data in patch_iter:
-                if patch_id < 0:
-                    raise ValueError("negative patch IDs are not supported")
-                # drop extra columns
-                patch_data = patch_data.drop(
-                    columns=[col for col in patch_data.columns if col not in renames]
-                )
-                patch_data.rename(columns=renames, inplace=True)
-                patch_data.reset_index(drop=True, inplace=True)
-                # look up the center of the patch if given
-                kwargs = dict(center=centers.get(patch_id))
-                if unload:
-                    # data will be written as feather file and loaded on demand
-                    kwargs["cachefile"] = os.path.join(
-                        cache_directory, f"patch_{patch_id:.0f}.feather"
-                    )
-                patch = PatchCatalog(int(patch_id), patch_data, **kwargs)
-                limits.update(patch.redshifts)
-                if unload:
-                    patch.unload()
-                patches[patch.id] = patch
-            if progress:  # clean up if any patch was empty and skipped
-                patch_iter.close()
-            self._zmin, self._zmax = limits.get()
-            self._patches = patches
-
-        # also store the patch properties
-        if unload:
-            centers = self.centers.to_3d()
-            property_df = pd.DataFrame(
-                dict(
-                    ids=self.ids,
-                    x=centers.x,
-                    y=centers.y,
-                    z=centers.z,
-                    r=self.radii.values,
-                )
+            raise ValueError(
+                "either of 'patch_name', 'patch_centers', or 'n_patches' "
+                "must be provided"
             )
-            fpath = os.path.join(cache_directory, "properties.feather")
-            property_df.to_feather(fpath)
+
+        with TimedLog(self._logger.info, log_msg):
+            self._catalog = Catalog(
+                ra=data[ra_name],
+                ra_units="degrees",
+                dec=data[dec_name],
+                dec_units="degrees",
+                r=None if redshift_name is None else data[redshift_name],
+                w=None if weight_name is None else data[weight_name],
+                **kwargs,
+            )
+            self._make_patches()
+
+        if cache_directory is not None:
+            self.unload()
 
     @classmethod
-    def from_cache(cls, cache_directory: str, progress: bool = False) -> ScipyCatalog:
-        super().from_cache(cache_directory)
+    def from_cache(cls, cache_directory: str, progress: bool = False) -> NoReturn:
+        """
+        Raises:
+            NotImplementedError
+
+        .. Warning::
+
+            Currently this backend does not support restoration from cache.
+        """
+        # super().from_cache(cache_directory)
+        # self._make_patches()
+        raise NotImplementedError("restoring from cache is currently not supported")
+
+    @classmethod
+    def from_treecorr(cls, cat: Catalog) -> TreecorrCatalog:
+        """Create a new instace from a :obj:`treecorr.Catalog`."""
         new = cls.__new__(cls)
-        # load the patch properties
-        fpath = os.path.join(cache_directory, "properties.feather")
-        property_df = pd.read_feather(fpath)
-        # transform data frame to dictionaries
-        ids = property_df["ids"]
-        centers = Coord3D.from_array(property_df[["x", "y", "z"]].to_numpy())
-        radii = DistSky(property_df["r"].to_numpy())
-        # transform to dictionary
-        centers = {pid: center for pid, center in zip(ids, centers)}
-        radii = {pid: radius for pid, radius in zip(ids, radii)}
-        # load the patches
-        limits = LimitTracker()
-        new._patches = {}
-        patch_files = list(os.listdir(cache_directory))
-        if progress:
-            patch_files = job_progress_bar(patch_files)
-        for path in patch_files:
-            if not path.startswith("patch"):
-                continue
-            abspath = os.path.join(cache_directory, path)
-            if not os.path.isfile(abspath):
-                continue
-            patch_id = patch_id_from_path(path)
-            patch = PatchCatalog.from_cached(
-                abspath, center=centers.get(patch_id), radius=radii.get(patch_id)
-            )
-            limits.update(patch.redshifts)
-            patch.unload()
-            new._patches[patch.id] = patch
-        new._zmin, new._zmax = limits.get()
+        new._catalog = cat
+        new._make_patches()
         return new
 
+    def _make_patches(self) -> None:
+        c = self._catalog
+        if c._patches is None:
+            low_mem = (not self.is_loaded()) and (c.save_patch_dir is not None)
+            c.get_patches(low_mem=low_mem)
+
+    def to_treecorr(self) -> Catalog:
+        """Get the internal :obj:`treecorr.Catalog` instance."""
+        return self._catalog
+
     def __len__(self) -> int:
-        return sum(len(patch) for patch in self._patches.values())
+        return self._catalog.ntot
 
-    def __getitem__(self, item: int) -> PatchCatalog:
-        return self._patches[item]
+    def __getitem__(self, item: int) -> Catalog:
+        return self._catalog._patches[item]
 
     @property
     def ids(self) -> list[int]:
-        return sorted(self._patches.keys())
+        return list(range(self.n_patches))
 
     @property
     def n_patches(self) -> int:
-        # seems ok to drop the last patch if that is empty and therefore missing
-        return max(self._patches.keys()) + 1
+        return self._catalog.npatch
 
-    def __iter__(self) -> Iterator[PatchCatalog]:
-        for patch_id in self.ids:
-            patch = self._patches[patch_id]
-            loaded = patch.is_loaded()
-            patch.load()
+    def __iter__(self) -> Iterator[Catalog]:
+        for patch in self._catalog._patches:
             yield patch
-            if not loaded:
-                patch.unload()
 
     def is_loaded(self) -> bool:
-        return all([patch.is_loaded() for patch in self._patches.values()])
+        return self._catalog.loaded
 
     def load(self) -> None:
         super().load()
-        for patch in self._patches.values():
-            patch.load()
+        self._catalog.load()
 
     def unload(self) -> None:
         super().unload()
-        for patch in self._patches.values():
-            patch.unload()
+        self._catalog.unload()
 
     def has_redshifts(self) -> bool:
-        return all(patch.has_redshifts() for patch in self._patches.values())
+        return self.redshifts is not None
 
     def has_weights(self) -> bool:
-        return all(patch.has_weights() for patch in self._patches.values())
+        return self.weights is not None
 
     @property
     def ra(self) -> NDArray[np.float_]:
-        return np.concatenate([patch.ra for patch in iter(self)])
+        return self._catalog.ra
 
     @property
     def dec(self) -> NDArray[np.float_]:
-        return np.concatenate([patch.dec for patch in iter(self)])
+        return self._catalog.dec
 
     @property
     def redshifts(self) -> NDArray[np.float_] | None:
-        if self.has_redshifts():
-            return np.concatenate([patch.redshifts for patch in iter(self)])
-        else:
-            return None
+        return self._catalog.r
 
     @property
     def weights(self) -> NDArray[np.float_]:
-        weights = []
-        for patch in iter(self):
-            if patch.has_weights():
-                weights.append(patch.weights)
-            else:
-                weights.append(np.ones(len(patch)))
-        return np.concatenate(weights)
+        return self._catalog.w
 
     @property
     def patch(self) -> NDArray[np.int_]:
-        return np.concatenate([np.full(len(patch), patch.id) for patch in iter(self)])
+        return self._catalog.patch
 
     def get_min_redshift(self) -> float:
+        if not hasattr(self, "_zmin"):
+            if self.has_redshifts():
+                self._zmin = self.redshifts.min()
+            else:
+                self._zmin = None
         return self._zmin
 
     def get_max_redshift(self) -> float:
+        if not hasattr(self, "_zmax"):
+            if self.has_redshifts():
+                self._zmax = self.redshifts.max()
+            else:
+                self._zmax = None
         return self._zmax
 
     @property
     def total(self) -> float:
-        return self.get_totals().sum()
+        return self._catalog.sumw
 
     def get_totals(self) -> NDArray[np.float_]:
-        return np.array([patch.total for patch in self._patches.values()])
+        return np.array([patch.sumw for patch in iter(self)])
 
     @property
     def centers(self) -> CoordSky:
-        return CoordSky.from_coords([self._patches[pid].center for pid in self.ids])
+        centers = Coord3D.from_array(self._catalog.get_patch_centers())
+        return centers.to_sky()
 
     @property
     def radii(self) -> DistSky:
-        return DistSky.from_dists([self._patches[pid].radius for pid in self.ids])
+        radii = []
+        cls = self.__class__
+        for cat in iter(self):
+            # build a new TreecorrCatalog without any postprocessing
+            patch = cls.__new__(cls)
+            patch._catalog = cat
+            # compute the angular radius from the maximum separation in 3D
+            position = patch.pos.to_3d()
+            radius = patch.centers.to_3d().distance(position).max()
+            radii.append(radius.to_sky())
+        return DistSky.from_dists(radii)
+
+    def iter_bins(
+        self, z_bins: NDArray[np.float_], allow_no_redshift: bool = False
+    ) -> Iterator[tuple[Interval, TreecorrCatalog | EmptyCatalog]]:
+        """Iterate the catalogue in bins of redshift.
+
+        Args:
+            z_bins (:obj:`NDArray`):
+                Edges of the redshift bins.
+            allow_no_redshift (:obj:`bool`):
+                If true and the data has no redshifts, the iterator yields the
+                whole catalogue at each iteration step.
+
+        Yields:
+            (tuple): tuple containing:
+                - **intv** (:obj:`pandas.Interval`): the selection for this bin.
+                - **cat** (:obj:`TreecorrCatalog`): instance containing the data
+                  for this bin.
+        """
+        if not allow_no_redshift and not self.has_redshifts():
+            raise ValueError("no redshifts for iteration provdided")
+        if allow_no_redshift:
+            for intv in pd.IntervalIndex.from_breaks(z_bins, closed="left"):
+                yield intv, self
+        else:
+            for interval, bin_mask in _iter_bin_masks(self.redshifts, z_bins):
+                yield interval, take_subset(self, bin_mask)
 
     def correlate(
         self,
         config: Configuration,
         binned: bool,
-        other: ScipyCatalog | None = None,
+        other: TreecorrCatalog = None,
         linkage: PatchLinkage | None = None,
         progress: bool = False,
     ) -> NormalisedCounts | dict[str, NormalisedCounts]:
         super().correlate(config, binned, other, linkage)
+
         auto = other is None
-        patch1_list, patch2_list = utils.get_patch_list(
-            self, other, config, linkage, auto
+        if not auto and not isinstance(other, TreecorrCatalog):
+            raise TypeError
+        nncorr_config = dict(
+            sep_units="radian",
+            metric="Arc",
+            nbins=(1 if config.scales.rweight is None else config.scales.rbin_num),
+            bin_slop=config.backend.rbin_slop,
+            num_threads=config.backend.get_threads(),
         )
 
-        # process the patch pairs, add an optional progress bar
-        n_jobs = len(patch1_list)
-        bin1 = self.has_redshifts()
-        bin2 = binned if other is not None else True
-        iter_args = zip(
-            patch1_list, patch2_list, repeat(config), repeat(bin1), repeat(bin2)
+        # bin the catalogues if necessary
+        cats1 = self.iter_bins(config.binning.zbins)
+        if auto:
+            cats2 = itertools.repeat((None, None))
+        else:
+            if binned:
+                cats2 = other.iter_bins(config.binning.zbins)
+            else:
+                cats2 = itertools.repeat((None, other))
+
+        # allocate output data containers
+        binning = pd.IntervalIndex.from_breaks(config.binning.zbins)
+        n_bins = len(binning)
+        n_patches = self.n_patches
+        totals1 = np.zeros((n_patches, n_bins))
+        totals2 = np.zeros((n_patches, n_bins))
+        count_dict = {
+            str(scale): PatchedCount.zeros(binning, n_patches, auto=auto)
+            for scale in config.scales
+        }
+
+        # iterate the bins and compute the correlation
+        self._logger.debug(
+            f"running treecorr on {config.backend.get_threads()} threads"
         )
+        for i, ((intv, bincat1), (_, bincat2)) in enumerate(zip(cats1, cats2)):
+            if progress:
+                _prog_msg = f"processing bin {i+1} / {n_bins}\r"
+                sys.stderr.write(_prog_msg)
+                sys.stderr.flush()
+
+            angles = [
+                scale.to_radian(intv.mid, config.cosmology) for scale in config.scales
+            ]
+            # extract the total number of objects per patch
+            totals1[:, i] = bincat1.get_totals()
+            if bincat2 is None:
+                totals2[:, i] = totals1[:, i]
+            else:
+                totals2[:, i] = bincat2.get_totals()
+
+            # trivial case: no data in redshift interval, no counts to update
+            if isinstance(bincat1, EmptyCatalog) or isinstance(bincat2, EmptyCatalog):
+                continue
+
+            for scale, (ang_min, ang_max) in zip(config.scales, angles):
+                # run the correlation measurement
+                correlation = NNCorrelation(
+                    min_sep=ang_min, max_sep=ang_max, **nncorr_config
+                )
+                correlation.process(
+                    bincat1.to_treecorr(),
+                    None if bincat2 is None else bincat2.to_treecorr(),
+                )
+
+                # extract the pair counts
+                scale_counts = count_dict[str(scale)]
+                result: TypeNNResult = correlation.results
+                for (pid1, pid2), corr_result in result.items():
+                    scale_counts.counts[pid1, pid2, i] = corr_result.weight
+
         if progress:
-            iter_args = job_progress_bar(iter_args, total=n_jobs)
-        with multiprocessing.Pool(config.backend.get_threads(n_jobs)) as pool:
-            patch_datasets = list(pool.imap_unordered(_worker_correlate, iter_args))
+            sys.stderr.write((" " * len(_prog_msg)) + "\r")  # clear line
 
-        # merge the pair counts from all patch combinations
-        return utils.merge_pairs_patches(patch_datasets, config, self.n_patches, auto)
+        total = PatchedTotal(  # not scale-dependent
+            binning=binning, totals1=totals1, totals2=totals2, auto=auto
+        )
+        return pack_results(count_dict, total)
 
     def true_redshifts(
         self,
         config: Configuration,
         sampling_config: ResamplingConfig | None = None,
         progress: bool = False,
     ) -> HistData:
+        if sampling_config is None:
+            sampling_config = ResamplingConfig()  # default values
+
         super().true_redshifts(config)
         if not self.has_redshifts():
             raise ValueError("catalog has no redshifts")
-
         # compute the reshift histogram in each patch
-        n_jobs = self.n_patches
-        iter_args = zip(self._patches.values(), repeat(config.binning.zbins))
-        if progress:
-            iter_args = job_progress_bar(iter_args, total=n_jobs)
-        with multiprocessing.Pool(config.backend.get_threads(n_jobs)) as pool:
-            hist_counts = list(pool.imap_unordered(_worker_true_redshifts, iter_args))
+        hist_counts = []
+        for patch in iter(self):
+            counts, bins = np.histogram(patch.r, config.binning.zbins, weights=patch.w)
+            hist_counts.append(counts)
+        hist_counts = np.array(hist_counts)
 
         # construct the output data samples
-        return utils.merge_histogram_patches(
-            np.array(hist_counts), config.binning.zbins, sampling_config
+        binning = pd.IntervalIndex.from_breaks(config.binning.zbins)
+        patch_idx = sampling_config.get_samples(self.n_patches)
+        nz_data = hist_counts.sum(axis=0)
+        nz_samp = np.sum(hist_counts[patch_idx], axis=1)
+        return HistData(
+            binning=binning,
+            data=nz_data,
+            samples=nz_samp,
+            method=sampling_config.method,
         )
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/catalogs/scipy/kdtree.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/kdtree.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/catalogs/scipy/patches.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/patches.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/catalogs/treecorr/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/core/containers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,444 +1,454 @@
+"""This module defines a few containers used throughout other modules.
+
+Most importantly, they implement two containers for data with attached samples
+(e.g. jackknife or bootstrap). Scalar values are implemented in
+:obj:`SampledValue`, data that has been computed from redshift bins in
+:obj:`SampledData`, which also serves as base class for most other containers
+with redshift binning.
+"""
+
 from __future__ import annotations
 
-import itertools
-import os
-import sys
-from collections.abc import Iterator
-from typing import TYPE_CHECKING, Dict, NoReturn, Tuple
-
-try:  # pragma: no cover
-    from typing import TypeAlias
-except ImportError:  # pragma: no cover
-    from typing_extensions import TypeAlias
+import warnings
+from collections.abc import Iterator, Sequence
+from dataclasses import dataclass, field, fields
+from typing import TYPE_CHECKING, Callable, Generic, NamedTuple, TypeVar
 
 import numpy as np
 import pandas as pd
-from numpy.typing import NDArray
-from treecorr import Catalog, NNCorrelation
 
-from yaw.catalogs import BaseCatalog
-from yaw.config import Configuration, ResamplingConfig
-from yaw.core.coordinates import Coord3D, Coordinate, CoordSky, DistSky
-from yaw.core.logging import TimedLog
-from yaw.correlation.paircounts import (
-    NormalisedCounts,
-    PatchedCount,
-    PatchedTotal,
-    pack_results,
-)
-from yaw.redshifts import HistData
+from yaw.config import OPTIONS
+from yaw.core.abc import BinnedQuantity, concatenate_bin_edges
+from yaw.core.math import cov_from_samples
 
 if TYPE_CHECKING:  # pragma: no cover
-    from pandas import DataFrame, Interval
+    from numpy.typing import NDArray
+    from pandas import DataFrame, IntervalIndex, Series
 
-    from yaw.catalogs import PatchLinkage
+__all__ = ["Indexer", "PatchIDs", "PatchCorrelationData", "SampledValue", "SampledData"]
 
-__all__ = ["EmptyCatalog", "TreecorrCatalog"]
 
+_TK = TypeVar("_TK")
+_TV = TypeVar("_TV")
 
-TypeNNResult: TypeAlias = Dict[Tuple[int, int], NNCorrelation]  # supports py3.8
 
+class Indexer(Generic[_TK, _TV], Iterator):
+    """Helper class to implemented a class attribute that can be used as
+    indexer and iterator for the classes stored data (e.g. indexing patches or
+    redshift bins).
+    """
 
-def _iter_bin_masks(
-    data: NDArray, bins: NDArray, closed: str = "left"
-) -> Iterator[tuple[Interval, NDArray[np.bool_]]]:
-    """Split data into bins and return an iterator that yields the boolean masks
-    that select the data of the current bin out of the input data array."""
-    if closed not in ("left", "right"):
-        raise ValueError("'closed' must be either of 'left', 'right'")
-    intervals = pd.IntervalIndex.from_breaks(bins, closed=closed)
-    bin_ids = np.digitize(data, bins, right=(closed == "right"))
-    for i, interval in enumerate(intervals, 1):
-        yield interval, (bin_ids == i)
+    def __init__(self, inst: _TV, builder: Callable[[_TV, _TK], _TV]) -> None:
+        """Construct a new indexer.
 
+        Args:
+            inst:
+                Class instance on which the indexing operations are applied.
+            builder:
+                Callable signature ``builder(inst, item) -> inst`` that
+                constructs a new class instance with the indexing specified from
+                ``item`` applied.
 
-def take_subset(
-    cat: TreecorrCatalog, items: NDArray[np.bool_] | NDArray[np.int_] | slice
-) -> TreecorrCatalog | EmptyCatalog:
-    """Construct a new TreecorrCatalog with a subset of its entries."""
-    ra = cat.ra[items]
-    if len(ra) == 0:
-        return EmptyCatalog(n_patches=cat.n_patches)
-    kwargs = dict(
-        ra=ra,
-        ra_units="radian",
-        dec=cat.dec[items],
-        dec_units="radian",
-        patch=cat.patch[items],
-    )
-    if cat.has_redshifts():
-        kwargs["r"] = cat.redshifts[items]
-    if cat.has_weights():
-        kwargs["w"] = cat.weights[items]
-    return TreecorrCatalog.from_treecorr(Catalog(**kwargs))
 
+        The resulting indexer supports indexing and slicing (depending on the
+        subclass implementation), as well as iteration, where instances holding
+        individual items are yielded.
+        """
+        self._inst = inst
+        self._builder = builder
+        self._iter_loc = 0
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({self._inst.__class__.__name__})"
+
+    def __getitem__(self, item: _TK) -> _TV:
+        return self._builder(self._inst, item)
+
+    def __next__(self) -> _TV:
+        """Returns the next value and increments the iterator location index."""
+        try:
+            val = self[self._iter_loc]
+        except IndexError:
+            raise StopIteration
+        else:
+            self._iter_loc += 1
+            return val
 
-class EmptyCatalog:
-    """A minimal representation of a TreecorrCatalog that contains no data."""
+    def __iter__(self) -> Iterator[_TV]:
+        """Returns a new instance of this class to have an independent iterator
+        location index"""
+        return self.__class__(inst=self._inst, builder=self._builder)
+
+
+class PatchIDs(NamedTuple):
+    """Named tuple that can hold a pair of patch indices."""
+
+    id1: int
+    """First patch index."""
+    id2: int
+    """Second patch index."""
+
+
+@dataclass(frozen=True)
+class PatchCorrelationData:
+    """Container to hold the result of a pair counting operation between two
+    spatial patches.
+
+    Args:
+        patches (:obj:`PatchIDs`):
+            The indices of used the patches.
+        totals1 (:obj:`NDArray`):
+            Total number of objects after binning by redshift in first patch.
+        totals1 (:obj:`NDArray`):
+            Total number of objects after binning by redshift in second patch.
+        counts (:obj:`dict`):
+            Dictionary listing the number of counted pairs after binning by
+            redshift. Each item represents results from a different scale.
+    """
 
-    def __init__(self, n_patches: int) -> None:
-        self.n_patches = n_patches
+    patches: PatchIDs
+    totals1: NDArray
+    totals2: NDArray
+    counts: dict[str, NDArray]
 
-    def __len__(self) -> int:
-        return 0
 
-    def total(self) -> float:
-        return 0.0
+_Tscalar = TypeVar("_Tscalar", bound=np.number)
 
-    def get_totals(self) -> NDArray[np.float_]:
-        return np.zeros(self.n_patches)
 
+@dataclass(frozen=True)
+class SampledValue(Generic[_Tscalar]):
+    """Container to hold a scalar value with an empirically estimated
+    uncertainty from resampling.
 
-class TreecorrCatalog(BaseCatalog):
-    """An implementation of the :obj:`BaseCatalog` using ``TreeCorr`` for the
-    pair counting.
+    Supports comparison of the values and samples with ``==`` and ``!=``.
 
-    .. Note::
+    .. rubric:: Examples
 
-        The current implementation is not very efficient, because the internal
-        fields of the underlying :obj:`treecorr.Catalog` must be rebuilt every
-        time the catalog is iterated in redshift bins for the pair counting.
+    Create a value container with 100 assumed jackknife samples that scatter
+    around zero with a standard deviation of 0.1:
 
-    .. Warning::
+    >>> from numpy.random import normal
+    >>> samples = normal(loc=0.0, scale=0.01, size=101)
+    >>> value = yaw.core.SampledValue(0.0, samples, method="jackknife")
+    >>> value
+    SampledValue(value=0, error=0.963, n_samples=100, method='jackknife')
 
-        Currently this backend does not support restoration from cache and
-        raises an :obj:`NotImplementedError`` when calling the
-        :meth:`from_cache` method.
+    Args:
+        value:
+            Numerical, scalar value.
+        samples (:obj:`NDArray`):
+            Samples of ``value`` obtained from resampling methods.
+        method (:obj:`str`):
+            Resampling method used to obtain the data samples, see
+            :class:`~yaw.ResamplingConfig` for available options.
     """
 
-    def __init__(
-        self,
-        data: DataFrame,
-        ra_name: str,
-        dec_name: str,
-        *,
-        patch_name: str | None = None,
-        patch_centers: BaseCatalog | Coordinate | None = None,
-        n_patches: int | None = None,
-        redshift_name: str | None = None,
-        weight_name: str | None = None,
-        cache_directory: str | None = None,
-        progress: bool = False,
-    ) -> None:
-        # construct the underlying TreeCorr catalogue
-        kwargs = dict()
-        if cache_directory is not None:
-            kwargs["save_patch_dir"] = cache_directory
-            if not os.path.exists(cache_directory):
-                raise FileNotFoundError(
-                    f"patch directory does not exist: '{cache_directory}'"
-                )
-            self._logger.info("using cache directory '%s'", cache_directory)
-
-        if n_patches is not None:
-            kwargs["npatch"] = n_patches
-            log_msg = f"creating {n_patches} patches"
-        elif patch_name is not None:
-            kwargs["patch"] = data[patch_name]
-            log_msg = "splitting data into predefined patches"
-        elif isinstance(patch_centers, BaseCatalog):
-            kwargs["patch_centers"] = patch_centers.centers.to_3d().values
-            n_patches = patch_centers.n_patches
-            log_msg = f"applying {n_patches} patches from external data"
-        elif isinstance(patch_centers, Coordinate):
-            centers = patch_centers.to_3d()
-            kwargs["patch_centers"] = centers.values
-            n_patches = len(centers)
-            log_msg = f"applying {n_patches} patches from external data"
-        else:
-            raise ValueError(
-                "either of 'patch_name', 'patch_centers', or 'n_patches' "
-                "must be provided"
+    value: _Tscalar
+    """Numerical, scalar value."""
+    samples: NDArray[_Tscalar]
+    """Samples of ``value`` obtained from resampling methods."""
+    method: str
+    """Resampling method used to obtain the data samples, see
+    :class:`~yaw.ResamplingConfig` for available options."""
+    error: _Tscalar = field(init=False)
+    """The uncertainty (standard error) of the value."""
+
+    def __post_init__(self) -> None:
+        if self.method not in OPTIONS.method:
+            raise ValueError(f"unknown sampling method '{self.method}'")
+        if self.method == "bootstrap":
+            error = np.std(self.samples, ddof=1, axis=0)
+        else:  # jackknife
+            error = np.std(self.samples, ddof=0, axis=0) * (self.n_samples - 1)
+        object.__setattr__(self, "error", error)
+
+    def __repr__(self) -> str:
+        string = self.__class__.__name__
+        value = self.value
+        error = self.error
+        n_samples = self.n_samples
+        method = self.method
+        return f"{string}({value=:.3g}, {error=:.3g}, {n_samples=}, {method=})"
+
+    def __str__(self) -> str:
+        return f"{self.value:+.3g}+/-{self.error:.3g}"
+
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, self.__class__):
+            if self.samples.shape != other.samples.shape:
+                return False
+            return (
+                self.method == other.method
+                and self.value == other.value
+                and np.all(self.samples == other.samples)
             )
+        else:
+            return False
 
-        with TimedLog(self._logger.info, log_msg):
-            self._catalog = Catalog(
-                ra=data[ra_name],
-                ra_units="degrees",
-                dec=data[dec_name],
-                dec_units="degrees",
-                r=None if redshift_name is None else data[redshift_name],
-                w=None if weight_name is None else data[weight_name],
-                **kwargs,
-            )
-            self._make_patches()
-
-        if cache_directory is not None:
-            self.unload()
-
-    @classmethod
-    def from_cache(cls, cache_directory: str, progress: bool = False) -> NoReturn:
-        """
-        Raises:
-            NotImplementedError
-
-        .. Warning::
-
-            Currently this backend does not support restoration from cache.
-        """
-        # super().from_cache(cache_directory)
-        # self._make_patches()
-        raise NotImplementedError("restoring from cache is currently not supported")
-
-    @classmethod
-    def from_treecorr(cls, cat: Catalog) -> TreecorrCatalog:
-        """Create a new instace from a :obj:`treecorr.Catalog`."""
-        new = cls.__new__(cls)
-        new._catalog = cat
-        new._make_patches()
-        return new
-
-    def _make_patches(self) -> None:
-        c = self._catalog
-        if c._patches is None:
-            low_mem = (not self.is_loaded()) and (c.save_patch_dir is not None)
-            c.get_patches(low_mem=low_mem)
-
-    def to_treecorr(self) -> Catalog:
-        """Get the internal :obj:`treecorr.Catalog` instance."""
-        return self._catalog
-
-    def __len__(self) -> int:
-        return self._catalog.ntot
-
-    def __getitem__(self, item: int) -> Catalog:
-        return self._catalog._patches[item]
-
-    @property
-    def ids(self) -> list[int]:
-        return list(range(self.n_patches))
+    def __ne__(self, other: object) -> bool:
+        return not self.__eq__(other)
 
     @property
-    def n_patches(self) -> int:
-        return self._catalog.npatch
-
-    def __iter__(self) -> Iterator[Catalog]:
-        for patch in self._catalog._patches:
-            yield patch
-
-    def is_loaded(self) -> bool:
-        return self._catalog.loaded
+    def n_samples(self) -> int:
+        """Number of samples used for error estimate."""
+        return len(self.samples)
+
+
+_Tdata = TypeVar("_Tdata", bound="SampledData")
+
+
+@dataclass(frozen=True, repr=False)
+class SampledData(BinnedQuantity):
+    """Container for data and resampled data with redshift binning.
+
+    Contains the redshift binning, data vector, and resampled data vector (e.g.
+    jackknife or bootstrap samples). The resampled values are used to compute
+    error estimates and covariance/correlation matrices.
+
+    Args:
+        binning (:obj:`pandas.IntervalIndex`):
+            The redshift binning applied to the data.
+        data (:obj:`NDArray`):
+            The data values, one for each redshift bin.
+        samples (:obj:`NDArray`):
+            The resampled data values (e.g. jackknife or bootstrap samples).
+        method (:obj:`str`):
+            The resampling method used, see :class:`~yaw.ResamplingConfig` for
+            available options.
+
+    The container supports addition and subtraction, which return a new instance
+    of the container, holding the modified data. This requires that both
+    operands are compatible (same binning and same sampling). The operands are
+    applied to the ``data`` and ``samples`` attribtes.
+
+    Furthermore, the container supports indexing and iteration over the redshift
+    bins using the :obj:`SampledData.bins` attribute. This attribute yields
+    instances of :obj:`SampledData` containing a single bin when iterating.
+    Slicing and indexing follows the same rules as the underlying ``data``
+    :obj:`NDArray`. Refer to :obj:`~yaw.correlation.CorrData` for some indexing
+    and iteration examples.
+
+    .. rubric:: Examples
+
+    Create a redshift binning:
+
+    >>> import pandas as pd
+    >>> bins = pd.IntervalIndex.from_breaks([0.1, 0.2, 0.3])
+    >>> bins
+    IntervalIndex([(0.1, 0.2], (0.2, 0.3]], dtype='interval[float64, right]')
+
+    Create some sample data for the bins with value 1 and five assumed jackknife
+    samples normal-distributed around 1.
+
+    >>> import numpy as np
+    >>> n_bins, n_samples = len(bins), 5
+    >>> data = np.ones(n_bins)
+    >>> samples = np.random.normal(1.0, size=(n_samples, n_bins))
+
+    Create the container:
+
+    >>> values = yaw.core.SampledData(bins, data, samples, method="jackknife")
+    >>> values
+    SampledData(n_bins=2, z='0.100...0.300', n_samples=10, method='jackknife')
+
+    Add the container to itself and verify that the values are doubled:
+
+    >>> summed = values + values
+    >>> summed.data
+    array([2., 2.])
+
+    The same applies to the samples:
+
+    >>> summed.samples / values.samples
+    array([[2., 2.],
+           [2., 2.],
+           [2., 2.],
+           [2., 2.],
+           [2., 2.]])
+    """
 
-    def load(self) -> None:
-        super().load()
-        self._catalog.load()
+    binning: IntervalIndex
+    """The redshift bin intervals."""
+    data: NDArray
+    """The data values, one for each redshift bin."""
+    samples: NDArray
+    """Samples of the data values, shape (# samples, # bins)."""
+    method: str
+    """The resampling method used."""
+    covariance: NDArray = field(init=False)
+    """Covariance matrix automatically computed from the resampled values."""
+
+    def __post_init__(self) -> None:
+        if self.data.shape != (self.n_bins,):
+            raise ValueError("unexpected shape of 'data' array")
+        if not self.samples.shape[1] == self.n_bins:
+            raise ValueError("number of bins for 'data' and 'samples' do not match")
+        if self.method not in OPTIONS.method:
+            raise ValueError(f"unknown sampling method '{self.method}'")
+
+        covmat = cov_from_samples(self.samples, self.method)
+        object.__setattr__(self, "covariance", np.atleast_2d(covmat))
+
+    def __repr__(self) -> str:
+        string = super().__repr__()[:-1]
+        n_samples = self.n_samples
+        method = self.method
+        return f"{string}, {n_samples=}, {method=})"
+
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, self.__class__):
+            if self.samples.shape != other.samples.shape:
+                return False
+            return (
+                self.method == other.method
+                and np.all(self.data == other.data)
+                and np.all(self.samples == other.samples)
+                and (self.binning == other.binning).all()
+            )
+        else:
+            return False
 
-    def unload(self) -> None:
-        super().unload()
-        self._catalog.unload()
+    def __ne__(self, other: object) -> bool:
+        return not self.__eq__(other)
 
-    def has_redshifts(self) -> bool:
-        return self.redshifts is not None
+    def __add__(self, other: _Tdata) -> _Tdata:
+        self.is_compatible(other, require=True)
+        return self.__class__(
+            binning=self.get_binning(),
+            data=self.data + other.data,
+            samples=self.samples + other.samples,
+            method=self.method,
+        )
 
-    def has_weights(self) -> bool:
-        return self.weights is not None
+    def __sub__(self, other: _Tdata) -> _Tdata:
+        self.is_compatible(other, require=True)
+        return self.__class__(
+            binning=self.get_binning(),
+            data=self.data - other.data,
+            samples=self.samples - other.samples,
+            method=self.method,
+        )
 
     @property
-    def ra(self) -> NDArray[np.float_]:
-        return self._catalog.ra
+    def bins(self: _Tdata) -> Indexer[int | slice | Sequence, _Tdata]:
+        def builder(inst: _Tdata, item: int | slice | Sequence) -> _Tdata:
+            if isinstance(item, int):
+                item = [item]
+            # try to take subsets along bin axis
+            binning = inst.get_binning()[item]
+            data = inst.data[item]
+            samples = inst.samples[:, item]
+            # determine which extra attributes need to be copied
+            init_attrs = {field.name for field in fields(inst) if field.init}
+            copy_attrs = init_attrs - {"binning", "data", "samples"}
+
+            kwargs = dict(binning=binning, data=data, samples=samples)
+            kwargs.update({attr: getattr(inst, attr) for attr in copy_attrs})
+            return inst.__class__(**kwargs)
 
-    @property
-    def dec(self) -> NDArray[np.float_]:
-        return self._catalog.dec
+        return Indexer(self, builder)
 
     @property
-    def redshifts(self) -> NDArray[np.float_] | None:
-        return self._catalog.r
+    def n_samples(self) -> int:
+        """Number of samples used for error estimate."""
+        return len(self.samples)
 
     @property
-    def weights(self) -> NDArray[np.float_]:
-        return self._catalog.w
+    def error(self) -> NDArray:
+        """The uncertainty (standard error) of the data.
 
-    @property
-    def patch(self) -> NDArray[np.int_]:
-        return self._catalog.patch
+        Returns:
+            :obj:`NDArray`
+        """
+        return np.sqrt(np.diag(self.covariance))
 
-    def get_min_redshift(self) -> float:
-        if not hasattr(self, "_zmin"):
-            if self.has_redshifts():
-                self._zmin = self.redshifts.min()
-            else:
-                self._zmin = None
-        return self._zmin
-
-    def get_max_redshift(self) -> float:
-        if not hasattr(self, "_zmax"):
-            if self.has_redshifts():
-                self._zmax = self.redshifts.max()
-            else:
-                self._zmax = None
-        return self._zmax
+    def get_binning(self) -> IntervalIndex:
+        return self.binning
 
-    @property
-    def total(self) -> float:
-        return self._catalog.sumw
+    def is_compatible(self, other: SampledData, require: bool = False) -> bool:
+        """Check whether this instance is compatible with another instance.
 
-    def get_totals(self) -> NDArray[np.float_]:
-        return np.array([patch.sumw for patch in iter(self)])
+        Ensures that both objects are instances of the same class, that the
+        redshift binning is identical, that the number of samples agree, and
+        that the resampling method is identical.
 
-    @property
-    def centers(self) -> CoordSky:
-        centers = Coord3D.from_array(self._catalog.get_patch_centers())
-        return centers.to_sky()
+        Args:
+            other (:obj:`BinnedQuantity`):
+                Object instance to compare to.
+            require (:obj:`bool`, optional)
+                Raise a ValueError if any of the checks fail.
 
-    @property
-    def radii(self) -> DistSky:
-        radii = []
-        cls = self.__class__
-        for cat in iter(self):
-            # build a new TreecorrCatalog without any postprocessing
-            patch = cls.__new__(cls)
-            patch._catalog = cat
-            # compute the angular radius from the maximum separation in 3D
-            position = patch.pos.to_3d()
-            radius = patch.centers.to_3d().distance(position).max()
-            radii.append(radius.to_sky())
-        return DistSky.from_dists(radii)
-
-    def iter_bins(
-        self, z_bins: NDArray[np.float_], allow_no_redshift: bool = False
-    ) -> Iterator[tuple[Interval, TreecorrCatalog | EmptyCatalog]]:
-        """Iterate the catalogue in bins of redshift.
+        Returns:
+            :obj:`bool`
+        """
+        if not super().is_compatible(other, require):
+            return False
+        if self.n_samples != other.n_samples:
+            if require:
+                raise ValueError("number of samples do not agree")
+            return False
+        if self.method != other.method:
+            if require:
+                raise ValueError("resampling method does not agree")
+            return False
+        return True
+
+    def concatenate_bins(self: _Tdata, *data: _Tdata) -> _Tdata:
+        for other in data:
+            self.is_compatible(other, require=True)
+        all_data: list[_Tdata] = [self, *data]
+        binning = concatenate_bin_edges(*all_data)
+        # concatenate data
+        data = np.concatenate([d.data for d in all_data])
+        samples = np.concatenate([d.samples for d in all_data], axis=1)
+        # determine which extra attributes need to be copied
+        init_attrs = {field.name for field in fields(self) if field.init}
+        copy_attrs = init_attrs - {"binning", "data", "samples"}
+
+        kwargs = dict(binning=binning, data=data, samples=samples)
+        kwargs.update({attr: getattr(self, attr) for attr in copy_attrs})
+        return self.__class__(**kwargs)
+
+    def get_data(self) -> Series:
+        """Get the data as :obj:`pandas.Series` with the binning as index."""
+        return pd.Series(self.data, index=self.binning)
+
+    def get_samples(self) -> DataFrame:
+        """Get the data as :obj:`pandas.DataFrame` with the binning as index.
+        The columns are labelled numerically and each represent one of the
+        samples."""
+        return pd.DataFrame(self.samples.T, index=self.binning)
+
+    def get_error(self) -> Series:
+        """Get value error estimate (diagonal of covariance matrix) as series
+        with its corresponding redshift bin intervals as index.
 
-        Args:
-            z_bins (:obj:`NDArray`):
-                Edges of the redshift bins.
-            allow_no_redshift (:obj:`bool`):
-                If true and the data has no redshifts, the iterator yields the
-                whole catalogue at each iteration step.
-
-        Yields:
-            (tuple): tuple containing:
-                - **intv** (:obj:`pandas.Interval`): the selection for this bin.
-                - **cat** (:obj:`TreecorrCatalog`): instance containing the data
-                  for this bin.
+        Returns:
+            :obj:`pandas.Series`
         """
-        if not allow_no_redshift and not self.has_redshifts():
-            raise ValueError("no redshifts for iteration provdided")
-        if allow_no_redshift:
-            for intv in pd.IntervalIndex.from_breaks(z_bins, closed="left"):
-                yield intv, self
-        else:
-            for interval, bin_mask in _iter_bin_masks(self.redshifts, z_bins):
-                yield interval, take_subset(self, bin_mask)
+        return pd.Series(self.error, index=self.binning)
 
-    def correlate(
-        self,
-        config: Configuration,
-        binned: bool,
-        other: TreecorrCatalog = None,
-        linkage: PatchLinkage | None = None,
-        progress: bool = False,
-    ) -> NormalisedCounts | dict[str, NormalisedCounts]:
-        super().correlate(config, binned, other, linkage)
-
-        auto = other is None
-        if not auto and not isinstance(other, TreecorrCatalog):
-            raise TypeError
-        nncorr_config = dict(
-            sep_units="radian",
-            metric="Arc",
-            nbins=(1 if config.scales.rweight is None else config.scales.rbin_num),
-            bin_slop=config.backend.rbin_slop,
-            num_threads=config.backend.get_threads(),
-        )
+    def get_covariance(self) -> DataFrame:
+        """Get value covariance matrix as data frame with its corresponding
+        redshift bin intervals as index and column labels.
 
-        # bin the catalogues if necessary
-        cats1 = self.iter_bins(config.binning.zbins)
-        if auto:
-            cats2 = itertools.repeat((None, None))
-        else:
-            if binned:
-                cats2 = other.iter_bins(config.binning.zbins)
-            else:
-                cats2 = itertools.repeat((None, other))
-
-        # allocate output data containers
-        binning = pd.IntervalIndex.from_breaks(config.binning.zbins)
-        n_bins = len(binning)
-        n_patches = self.n_patches
-        totals1 = np.zeros((n_patches, n_bins))
-        totals2 = np.zeros((n_patches, n_bins))
-        count_dict = {
-            str(scale): PatchedCount.zeros(binning, n_patches, auto=auto)
-            for scale in config.scales
-        }
-
-        # iterate the bins and compute the correlation
-        self._logger.debug(
-            "running treecorr on %i threads", config.backend.get_threads()
+        Returns:
+            :obj:`pandas.DataFrame`
+        """
+        return pd.DataFrame(
+            data=self.covariance, index=self.binning, columns=self.binning
         )
-        for i, ((intv, bincat1), (_, bincat2)) in enumerate(zip(cats1, cats2)):
-            if progress:
-                _prog_msg = f"processing bin {i+1} / {n_bins}\r"
-                sys.stderr.write(_prog_msg)
-                sys.stderr.flush()
-
-            angles = [
-                scale.to_radian(intv.mid, config.cosmology) for scale in config.scales
-            ]
-            # extract the total number of objects per patch
-            totals1[:, i] = bincat1.get_totals()
-            if bincat2 is None:
-                totals2[:, i] = totals1[:, i]
-            else:
-                totals2[:, i] = bincat2.get_totals()
-
-            # trivial case: no data in redshift interval, no counts to update
-            if isinstance(bincat1, EmptyCatalog) or isinstance(bincat2, EmptyCatalog):
-                continue
-
-            for scale, (ang_min, ang_max) in zip(config.scales, angles):
-                # run the correlation measurement
-                correlation = NNCorrelation(
-                    min_sep=ang_min, max_sep=ang_max, **nncorr_config
-                )
-                correlation.process(
-                    bincat1.to_treecorr(),
-                    None if bincat2 is None else bincat2.to_treecorr(),
-                )
-
-                # extract the pair counts
-                scale_counts = count_dict[str(scale)]
-                result: TypeNNResult = correlation.results
-                for (pid1, pid2), corr_result in result.items():
-                    scale_counts.counts[pid1, pid2, i] = corr_result.weight
-
-        if progress:
-            sys.stderr.write((" " * len(_prog_msg)) + "\r")  # clear line
 
-        total = PatchedTotal(  # not scale-dependent
-            binning=binning, totals1=totals1, totals2=totals2, auto=auto
-        )
-        return pack_results(count_dict, total)
+    def get_correlation(self) -> DataFrame:
+        """Get value correlation matrix as data frame with its corresponding
+        redshift bin intervals as index and column labels.
 
-    def true_redshifts(
-        self,
-        config: Configuration,
-        sampling_config: ResamplingConfig | None = None,
-        progress: bool = False,
-    ) -> HistData:
-        if sampling_config is None:
-            sampling_config = ResamplingConfig()  # default values
-
-        super().true_redshifts(config)
-        if not self.has_redshifts():
-            raise ValueError("catalog has no redshifts")
-        # compute the reshift histogram in each patch
-        hist_counts = []
-        for patch in iter(self):
-            counts, bins = np.histogram(patch.r, config.binning.zbins, weights=patch.w)
-            hist_counts.append(counts)
-        hist_counts = np.array(hist_counts)
-
-        # construct the output data samples
-        binning = pd.IntervalIndex.from_breaks(config.binning.zbins)
-        patch_idx = sampling_config.get_samples(self.n_patches)
-        nz_data = hist_counts.sum(axis=0)
-        nz_samp = np.sum(hist_counts[patch_idx], axis=1)
-        return HistData(
-            binning=binning,
-            data=nz_data,
-            samples=nz_samp,
-            method=sampling_config.method,
-        )
+        Returns:
+            :obj:`pandas.DataFrame`
+        """
+        stdev = np.sqrt(np.diag(self.covariance))
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            corr = self.covariance / np.outer(stdev, stdev)
+        corr[self.covariance == 0] = 0
+        return pd.DataFrame(data=corr, index=self.binning, columns=self.binning)
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/config/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module implements the configuration for ``yaw``, which are the free
 parameters for the correlation function measurements. These parameters control
 
 1. the scales on which correlations are measured (:obj:`ScalesConfig`),
-2. the redshift binning for the redshift reconstruction (:obj:`BinningConfig`),
+2. the redshift binning for the redshift reconstruction
+   (:obj:`AutoBinningConfig` or :obj:`ManualBinningConfig`),
 3. backend related parameters (:obj:`BackendConfig`), and
 4. the resampling method for error estimation (:obj:`ResamplingConfig`).
 
 Each of these four configuration classes are implemented as immuateble
 dataclasses, i.e. their values cannot be modified after creation.
 
 For convenience, the first three configuration classes are grouped together in
@@ -24,26 +25,22 @@
 """
 
 from yaw.config import default as DEFAULT
 from yaw.config.options import OPTIONS
 
 # isort: split
 from yaw.config.backend import BackendConfig
-from yaw.config.binning import BinningConfig
+from yaw.config.binning import AutoBinningConfig, ManualBinningConfig
 from yaw.config.config import Configuration
 from yaw.config.resampling import ResamplingConfig
 from yaw.config.scales import ScalesConfig
 
-# isort: split
-from yaw.deprecated.config.binning import AutoBinningConfig, ManualBinningConfig
-
 __all__ = [
     "DEFAULT",
-    "AutoBinningConfig",
     "BackendConfig",
-    "BinningConfig",
-    "Configuration",
+    "AutoBinningConfig",
     "ManualBinningConfig",
+    "Configuration",
     "OPTIONS",
     "ResamplingConfig",
     "ScalesConfig",
 ]
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/config/backend.py` & `yet_another_wizz-2.5.post0/src/yaw/config/backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import os
 from dataclasses import dataclass, field
 
-from yaw.config import DEFAULT
-from yaw.config.abc import BaseConfig
+from yaw.config import default as DEFAULT
+from yaw.core.abc import DictRepresentation
 from yaw.core.docs import Parameter
 
 __all__ = ["BackendConfig"]
 
 
 @dataclass(frozen=True)
-class BackendConfig(BaseConfig):
+class BackendConfig(DictRepresentation):
     """Configuration of backends used for correlation measurements.
 
     Args:
         thread_num (:obj:`int`, optional):
             Number of threads to use for parallel processing.
         crosspatch (:obj:`bool`, optional):
             Whether to count pairs across patch boundaries (``scipy`` backend
@@ -56,35 +56,21 @@
     )
     """`TreeCorr` ``rbin_slop`` parameter (``treecorr`` backend only)."""
 
     def __post_init__(self) -> None:
         if self.thread_num is None:
             object.__setattr__(self, "thread_num", os.cpu_count())
 
-    def modify(
-        self,
-        thread_num: int | None = DEFAULT.NotSet,
-        crosspatch: bool = DEFAULT.NotSet,
-        rbin_slop: float = DEFAULT.NotSet,
-    ) -> BackendConfig:
-        return super().modify(
-            thread_num=thread_num, crosspatch=crosspatch, rbin_slop=rbin_slop
-        )
-
     def get_threads(self, max=None) -> int:
         """Get the number of threads for parallel processing.
 
-        The value is capped at an optional maximum value.
-
-        Args:
-            max (:obj:`int`, optional):
-                Maximum number to return.
-
-        Returns:
-            :obj:`int`
+        The value is capped at the number of logical cores available.
         """
-        thread_num = self.thread_num
+        if self.thread_num is None:
+            thread_num = os.cpu_count()
+        else:
+            thread_num = self.thread_num
         if max is not None:
             if max < 1:
                 raise ValueError("'max' must be positive")
             thread_num = min(max, thread_num)
         return thread_num
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/config/binning.py` & `yet_another_wizz-2.5.post0/src/yaw/config/binning.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,131 @@
 from __future__ import annotations
 
-import warnings
+import logging
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 
-from yaw.config import DEFAULT, OPTIONS
-from yaw.config.abc import BaseConfig
+from yaw.config import OPTIONS
+from yaw.config import default as DEFAULT
 from yaw.config.utils import ConfigError
+from yaw.core.abc import DictRepresentation
 from yaw.core.cosmology import BinFactory, TypeCosmology
 from yaw.core.docs import Parameter
 from yaw.core.math import array_equal
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
-__all__ = ["BinningConfig"]
+__all__ = ["AutoBinningConfig", "ManualBinningConfig", "make_binning_config"]
 
 
-@dataclass(frozen=True)
-class BinningConfig(BaseConfig):
-    """TODO"""
+logger = logging.getLogger(__name__)
+
+
+class BaseBinningConfig(DictRepresentation):
+    """Base class for redshift binning configuration."""
+
+    zbins: NDArray[np.float_]
+    """Edges of redshift bins."""
+    method: str
+    """Method used to create redshift binning, ``manual`` or either of
+    :obj:`~yaw.config.options.Options.binning`."""
+
+    def __repr__(self) -> str:
+        name = self.__class__.__name__
+        zbin_num = self.zbin_num
+        z = f"{self.zmin:.3f}...{self.zmax:.3f}"
+        method = self.method
+        return f"{name}({zbin_num=}, {z=}, {method=})"
+
+
+@dataclass(frozen=True, repr=False)
+class ManualBinningConfig(BaseBinningConfig):
+    """Configuration that specifies a manual redshift binning.
+
+    Args:
+        zbins (:obj:`NDArray`):
+            Edges of redshift bins, must increase monotonically.
+    """
 
     zbins: NDArray[np.float_] = field(
         metadata=Parameter(
             type=float,
             nargs="*",
-            help="list of custom redshift bin edges, if method is set to 'manual'",
+            help="list of custom redshift bin edges, if provided, other "
+            "binning parameters are omitted, method is set to 'manual'",
         )
     )
-    """Edges of redshift bins."""
+
+    def __post_init__(self) -> None:
+        if len(self.zbins) < 2:
+            raise ConfigError("'zbins' must have at least two edges")
+        BinFactory.check(self.zbins)
+        object.__setattr__(self, "zbins", np.asarray(self.zbins))
+
+    def __eq__(self, other: ManualBinningConfig) -> bool:
+        if not array_equal(self.zbins, other.zbins):
+            return False
+        return True
+
+    @property
+    def method(self) -> str:
+        """Method used to create redshift binning, always ``manual``."""
+        return "manual"
+
+    @property
+    def zmin(self) -> float:
+        """Lowest redshift bin edge."""
+        return float(self.zbins[0])
+
+    @property
+    def zmax(self) -> float:
+        """Highest redshift bin edge."""
+        return float(self.zbins[-1])
+
+    @property
+    def zbin_num(self) -> int:
+        """Number of redshift bins."""
+        return len(self.zbins) - 1
+
+    @classmethod
+    def from_dict(cls, the_dict: dict[str, Any], **kwargs) -> ManualBinningConfig:
+        return cls(np.asarray(the_dict["zbins"]))
+
+    def to_dict(self) -> dict[str, Any]:
+        return dict(method=self.method, zbins=self.zbins.tolist())
+
+
+@dataclass(frozen=True, repr=False)
+class AutoBinningConfig(BaseBinningConfig):
+    """Configuration that generates a redshift binning.
+
+    To generate a redshift binning use the :meth:`generate` method.
+
+    Args:
+        zbins (:obj:`NDArray`):
+            Edges of redshift bins, must increase monotonically.
+        method (:obj:`str`):
+            Method used to create redshift binning, either of
+            :obj:`~yaw.config.options.Options.binning`.
+    """
+
+    zbins: NDArray[np.float_]
     method: str = field(
-        default=DEFAULT.Binning.method,
+        default=DEFAULT.Configuration.binning.method,
         metadata=Parameter(
-            type=str,
             choices=OPTIONS.binning,
             help="redshift binning method, 'logspace' means equal size in log(1+z)",
             default_text="(default: %(default)s)",
         ),
     )
-    """Method used to create redshift binning (defaults to 'manual' if `zbins`
-    are provided), see :obj:`~yaw.config.options.Options.binning` for options."""
+    """Method used to create redshift binning, see
+    :obj:`~yaw.config.options.Options.binning`."""
     zmin: float = field(
         init=False,
         metadata=Parameter(
             type=float,
             help="lower redshift limit",
             default_text="(default: %(default)s)",
         ),
@@ -57,80 +137,45 @@
             type=float,
             help="upper redshift limit",
             default_text="(default: %(default)s)",
         ),
     )
     """Highest redshift bin edge."""
     zbin_num: int = field(
-        default=DEFAULT.Binning.zbin_num,
+        default=DEFAULT.AutoBinning.zbin_num,
         init=False,
         metadata=Parameter(
             type=int,
             help="number of redshift bins",
             default_text="(default: %(default)s)",
         ),
     )
     """Number of redshift bins."""
 
     def __post_init__(self) -> None:
-        if len(self.zbins) < 2:
-            raise ConfigError("'zbins' must have at least two edges")
-        object.__setattr__(self, "zbins", np.asarray(self.zbins))
-        BinFactory.check(self.zbins)
         object.__setattr__(self, "zmin", float(self.zbins[0]))
         object.__setattr__(self, "zmax", float(self.zbins[-1]))
         object.__setattr__(self, "zbin_num", len(self.zbins) - 1)
 
-    def __eq__(self, other) -> bool:
-        if not isinstance(other, self.__class__):
-            return False
-        if self.method != other.method or not array_equal(self.zbins, other.zbins):
-            return False
-        return True
-
-    def __repr__(self) -> str:
-        name = self.__class__.__name__
-        zbin_num = self.zbin_num
-        z = f"{self.zmin:.3f}...{self.zmax:.3f}"
-        method = self.method
-        return f"{name}({zbin_num=}, {z=}, {method=})"
-
-    @property
-    def is_manual(self) -> bool:
-        """Whether the redshift bins are set manually."""
-        return self.method == "manual"
-
     @classmethod
-    def create(
+    def generate(
         cls,
-        *,
-        zbins: NDArray[np.float_] | None = None,
-        zmin: float | None = None,
-        zmax: float | None = None,
-        zbin_num: int = DEFAULT.Binning.zbin_num,
-        method: str = DEFAULT.Binning.method,
-        cosmology: TypeCosmology | str | None = None,
-    ) -> BinningConfig:
-        """Create a new redshift binning configuration.
-
-        If redshift bins (``zbins``) are provided, ``method`` is set to
-        ``"manual"`` and the bins edges are used. If ``zmin`` and ``zmax`` are
-        provided, instead generates a specified number of bins between this
-        lower and upper redshift limit. The spacing of the bins depends the
-        generation method, the default is a linear spacing.
-
-        .. Note::
-
-            The ``cosmology`` parameter is only used when generating binnings
-            that require cosmological distance computations.
+        zmin: float,
+        zmax: float,
+        zbin_num: int = DEFAULT.AutoBinning.zbin_num,
+        method: str = DEFAULT.AutoBinning.method,
+        cosmology: TypeCosmology | None = None,
+    ) -> AutoBinningConfig:
+        """Generate a new redshift binning configuration.
+
+        Generates a specified number of bins between a lower and upper redshift
+        limit. The spacing of the bins depends the generation method, the
+        default is a linear spacing.
 
         Args:
-            zbins (:obj:`NDArray[np.float_]`):
-                Monotonically increasing redshift bin edges, including the upper
-                edge (ignored if ``zmin`` and ``zmax`` are provided).
             zmin (:obj:`float`):
                 Minimum redshift, lowest redshift edge.
             zmax (:obj:`float`):
                 Maximum redshift, highest redshift edge.
             zbin_num (:obj:`int`, optional):
                 Number of redshift bins to generate.
             method (:obj:`str`, optional):
@@ -138,87 +183,77 @@
                 options and their description see
                 :obj:`~yaw.config.options.Options.binning`.
             cosmology (:obj:`astropy.cosmology.FLRW`, :obj:`~yaw.core.cosmology.CustomCosmology`, optional):
                 Cosmological model used for distance calculations. For a custom
                 model, refer to :mod:`yaw.core.cosmology`.
 
         Returns:
-            :obj:`BinningConfig`
+            :obj:`AutoBinningConfig`
         """
-        auto_args_set = (zmin is not None, zmax is not None)
-        manual_args_set = (zbins is not None,)
-        if not all(manual_args_set) and not all(auto_args_set):
-            raise ConfigError("either 'zbins' or 'zmin' and 'zmax' are required")
-
-        elif all(auto_args_set):  # generate zbins
-            if all(manual_args_set):
-                warnings.warn(
-                    "'zbins' set but ignored since 'zmin' and 'zmax' are provided"
-                )
-            if not isinstance(method, str):
-                raise ValueError("'method' must a string")
-            zbins = BinFactory(zmin, zmax, zbin_num, cosmology).get(method)
-
-        else:  # use provided zbins
-            method = "manual"
-
-        return cls(zbins=zbins, method=method)
-
-    def modify(
-        self,
-        zbins: NDArray[np.float_] | None = DEFAULT.NotSet,
-        zmin: float | None = DEFAULT.NotSet,
-        zmax: float | None = DEFAULT.NotSet,
-        zbin_num: int = DEFAULT.NotSet,
-        method: str = DEFAULT.NotSet,
-        cosmology: TypeCosmology | str | None = None,
-    ) -> BinningConfig:
-        """Create a copy of the current configuration with updated parameter
-        values.
-
-        The method arguments are identical to :meth:`create`. Values that should
-        not be modified are by default represented by the special value
-        :obj:`~yaw.config.default.NotSet`.
+        zbins = BinFactory(zmin, zmax, zbin_num, cosmology).get(method)
+        return cls(zbins, method)
 
-        .. Note::
-
-            The ``cosmology`` parameter is only used when generating binnings
-            that require cosmological distance computations.
-        """
-        if zbins is not DEFAULT.NotSet:
-            kwargs = dict(zbins=zbins)
-        else:
-            inputs = dict(zmin=zmin, zmax=zmax, zbin_num=zbin_num, method=method)
-            mods = {k: v for k, v in inputs.items() if v is not DEFAULT.NotSet}
-            if self.is_manual:  # use every input as parameter
-                kwargs = mods
-            else:  # keep the existing parameters and update with inputs
-                kwargs = self.to_dict()
-                kwargs.update(mods)
-        return self.__class__.create(**kwargs, cosmology=cosmology)
-
-    def to_dict(self) -> dict[str, Any]:
-        if self.is_manual:
-            return dict(method=self.method, zbins=self.zbins.tolist())
-        else:
-            return dict(
-                zmin=self.zmin,
-                zmax=self.zmax,
-                zbin_num=self.zbin_num,
-                method=self.method,
-            )
+    def __eq__(self, other: ManualBinningConfig) -> bool:
+        if not array_equal(self.zbins, other.zbins):
+            return False
+        if self.method != other.method:
+            return False
+        return True
 
     @classmethod
     def from_dict(
         cls, the_dict: dict[str, Any], cosmology: TypeCosmology | None = None
-    ) -> BinningConfig:
+    ) -> AutoBinningConfig:
         """Create a class instance from a dictionary representation of the
         minimally required data.
 
         Args:
             the_dict (:obj:`dict`):
                 Dictionary containing the data.
             cosmology (:obj:`astropy.cosmology.FLRW`, :obj:`~yaw.core.cosmology.CustomCosmology`, optional):
                 Cosmological model used for distance calculations. For a custom
                 model, refer to :mod:`yaw.core.cosmology`.
         """
-        return cls.create(**the_dict, cosmology=cosmology)
+        return cls.generate(**the_dict, cosmology=cosmology)
+
+    def to_dict(self) -> dict[str, Any]:
+        return dict(
+            zmin=self.zmin, zmax=self.zmax, zbin_num=self.zbin_num, method=self.method
+        )
+
+
+def warn_binning_args_ignored(
+    zmin: bool | float | None, zmax: bool | float | None, zbin_num: bool | int | None
+) -> None:
+    """Issue a warning that values are ignored, if any of the arguments is
+    set."""
+    # NOTE: NotSet is also False
+    if zmin or zmax or zbin_num:
+        logger.warn("'zmin', 'zmax', 'nbins' are ignored if 'zbins' is provided")
+
+
+def make_binning_config(
+    cosmology: TypeCosmology | str | None,
+    zmin: float | None = None,
+    zmax: float | None = None,
+    zbin_num: int | None = None,
+    method: str | None = None,
+    zbins: NDArray[np.float_] | None = None,
+) -> ManualBinningConfig | AutoBinningConfig:
+    """
+    Helper function to construct a binning configuration.
+
+    The ``cosmology`` argument is always required. If redshift bins (``zbins``)
+    are provided, a :obj:`ManualBinningConfig` is returned, otherwise an
+    :obj:`AutoBinningConfig`. Issues a warning if any argument is set but
+    ignored by the returned configuration instance.
+    """
+    auto_args_set = (zmin is not None, zmax is not None, zbin_num is not None)
+    if zbins is None and not all(auto_args_set):
+        raise ConfigError("either 'zbins' or 'zmin', 'zmax', 'zbin_num' are required")
+    elif all(auto_args_set):
+        return AutoBinningConfig.generate(
+            zmin=zmin, zmax=zmax, zbin_num=zbin_num, method=method, cosmology=cosmology
+        )
+    else:
+        warn_binning_args_ignored(*auto_args_set)
+        return ManualBinningConfig(zbins)
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/config/config.py` & `yet_another_wizz-2.5.post0/src/yaw/config/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 
 import logging
 from dataclasses import asdict, dataclass, field
 from typing import TYPE_CHECKING, Any, get_args
 
 import numpy as np
 import yaml
-from deprecated import deprecated
 
 from yaw.config import OPTIONS
 from yaw.config import default as DEFAULT
 from yaw.config import utils
-from yaw.config.abc import BaseConfig
 from yaw.config.backend import BackendConfig
-from yaw.config.binning import BinningConfig
+from yaw.config.binning import (
+    AutoBinningConfig,
+    ManualBinningConfig,
+    make_binning_config,
+    warn_binning_args_ignored,
+)
 from yaw.config.scales import ScalesConfig
+from yaw.core.abc import DictRepresentation
 from yaw.core.cosmology import TypeCosmology, get_default_cosmology, r_kpc_to_angle
 from yaw.core.docs import Parameter
 
 if TYPE_CHECKING:  # pragma: no cover
     from matplotlib.figure import Figure
     from numpy.typing import ArrayLike, NDArray
 
@@ -28,52 +32,53 @@
 __all__ = ["Configuration"]
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
-class Configuration(BaseConfig):
+class Configuration(DictRepresentation):
     """The central configration for correlation measurements.
 
     Bundles the configuration of measurement scales, redshift binning, and
     backend parameters in a single, hierarchical configuration class.
     Additionally holds the cosmological model used for distance calculations.
 
     .. Note::
 
         The structure and meaning of the parameters is described in more detail
         in the specialised configuration objects :obj:`ScalesConfig`,
-        :obj:`BinningConfig`, :obj:`BackendConfig`, which are stored as class
-        attributes :obj:`scales`, :obj:`binning`, and :obj:`backend`.
+        :obj:`AutoBinningConfig` / :obj:`ManualBinningConfig`,
+        :obj:`BackendConfig`, which are stored as class attributes
+        :obj:`scales`, :obj:`binning`, and :obj:`backend`.
 
         To access e.g. the lower measurement scale limit, use
 
         >>> Configuration.scales.rmin
         ...
 
         which accesses the :obj:`ScalesConfig.rmin` attribute.
 
     A new instance should be constructed with the :meth:`create` method or
     as a modified variant with the :meth:`modify` method.
 
     Args:
         scales (:obj:`~yaw.config.ScalesConfig`):
             The configuration of the measurement scales.
-        binning (:obj:`~yaw.config.BinningConfig`):
+        binning (:obj:`~yaw.config.AutoBinningConfig`, :obj:`~yaw.config.ManualBinningConfig`):
             The redshift binning configuration.
         backend (:obj:`~yaw.config.BackendConfig`):
             The backend-specific configuration.
         cosmology (:obj:`astropy.cosmology.FLRW`, :obj:`~yaw.core.cosmology.CustomCosmology`, :obj:`str`, :obj:`None`, optional)
             The cosmological model for distance calculations.
     """
 
     scales: ScalesConfig
     """The configuration of the measurement scales."""
-    binning: BinningConfig
+    binning: AutoBinningConfig | ManualBinningConfig
     """The redshift binning configuration."""
     backend: BackendConfig = field(default_factory=BackendConfig)
     """The backend-specific configuration."""
     cosmology: TypeCosmology | str | None = field(
         default=DEFAULT.Configuration.cosmology,
         metadata=Parameter(
             type=str,
@@ -87,15 +92,15 @@
     def __post_init__(self) -> None:
         # parse cosmology
         if self.cosmology is None:
             cosmology = get_default_cosmology()
         elif isinstance(self.cosmology, str):
             cosmology = utils.yaml_to_cosmology(self.cosmology)
         elif not isinstance(self.cosmology, get_args(TypeCosmology)):
-            which = ", ".join(str(c) for c in get_args(TypeCosmology))
+            which = ", ".join(get_args(TypeCosmology))
             raise utils.ConfigError(f"'cosmology' must be instance of: {which}")
         else:
             cosmology = self.cosmology
         cosmology = utils.parse_cosmology(self.cosmology)
         object.__setattr__(self, "cosmology", cosmology)
 
     @classmethod
@@ -104,30 +109,31 @@
         *,
         cosmology: TypeCosmology | str | None = DEFAULT.Configuration.cosmology,
         # ScalesConfig
         rmin: ArrayLike,
         rmax: ArrayLike,
         rweight: float | None = DEFAULT.Configuration.scales.rweight,
         rbin_num: int = DEFAULT.Configuration.scales.rbin_num,
-        # BinningConfig
+        # AutoBinningConfig / ManualBinningConfig
         zmin: ArrayLike = None,
         zmax: ArrayLike = None,
         zbin_num: int | None = DEFAULT.Configuration.binning.zbin_num,
         method: str = DEFAULT.Configuration.binning.method,
         zbins: NDArray[np.float_] | None = None,
         # BackendConfig
         thread_num: int | None = DEFAULT.Configuration.backend.thread_num,
         crosspatch: bool = DEFAULT.Configuration.backend.crosspatch,
         rbin_slop: float = DEFAULT.Configuration.backend.rbin_slop,
     ) -> Configuration:
         """Create a new configuration object.
 
         Except for the ``cosmology`` parameter, all other parameters are passed
         to the constructors of the respective :obj:`ScalesConfig`,
-        :obj:`BinningConfig`, and :obj:`BackendConfig` classes.
+        :obj:`AutoBinningConfig` / :obj:`ManualBinningConfig`,
+        :obj:`BackendConfig` classes.
 
         .. Note::
 
             If custom bin edges are provided through the ``zbins`` parameter,
             ``zmin``, ``zmax``, ``zbin_num`` (optional), and ``method``
             (optional) are ignored. Otherwise, at least ``zmin``, ``zmax`` are
             required and a binning will be generated automatically.
@@ -168,82 +174,96 @@
             rbin_slop (:obj:`float`, optional):
                 TreeCorr 'rbin_slop' parameter
 
         Returns:
             :obj:`Configuration`
         """
         cosmology = utils.parse_cosmology(cosmology)
-        scales = ScalesConfig.create(
-            rmin=rmin, rmax=rmax, rweight=rweight, rbin_num=rbin_num
-        )
-        binning = BinningConfig.create(
+        scales = ScalesConfig(rmin=rmin, rmax=rmax, rweight=rweight, rbin_num=rbin_num)
+        binning = make_binning_config(
             cosmology=cosmology,
             zmin=zmin,
             zmax=zmax,
             zbin_num=zbin_num,
             method=method,
             zbins=zbins,
         )
-        backend = BackendConfig.create(
+        backend = BackendConfig(
             thread_num=thread_num, crosspatch=crosspatch, rbin_slop=rbin_slop
         )
         return cls(scales=scales, binning=binning, backend=backend, cosmology=cosmology)
 
     def modify(
         self,
         *,
         cosmology: TypeCosmology | str | None = DEFAULT.NotSet,
         # ScalesConfig
         rmin: ArrayLike | None = DEFAULT.NotSet,
         rmax: ArrayLike | None = DEFAULT.NotSet,
         rweight: float | None = DEFAULT.NotSet,
         rbin_num: int | None = DEFAULT.NotSet,
-        # BinningConfig
+        # AutoBinningConfig /  ManualBinningConfig
         zmin: float | None = DEFAULT.NotSet,
         zmax: float | None = DEFAULT.NotSet,
         zbin_num: int | None = DEFAULT.NotSet,
         method: str | None = DEFAULT.NotSet,
         zbins: NDArray[np.float_] | None = DEFAULT.NotSet,
         # BackendConfig
         thread_num: int | None = DEFAULT.NotSet,
         crosspatch: bool | None = DEFAULT.NotSet,
         rbin_slop: float | None = DEFAULT.NotSet,
     ) -> Configuration:
-        if cosmology is DEFAULT.NotSet:
-            cosmology = self.cosmology
-        elif isinstance(cosmology, str):
-            cosmology = utils.yaml_to_cosmology(cosmology)
-        scales = self.scales.modify(
-            rmin=rmin, rmax=rmax, rweight=rweight, rbin_num=rbin_num
-        )
-        binning = self.binning.modify(
-            zmin=zmin,
-            zmax=zmax,
-            method=method,
-            zbin_num=zbin_num,
-            zbins=zbins,
-            cosmology=cosmology,
-        )
-        backend = self.backend.modify(
-            thread_num=thread_num, crosspatch=crosspatch, rbin_slop=rbin_slop
-        )
-        return self.__class__(
-            cosmology=cosmology, scales=scales, binning=binning, backend=backend
-        )
+        """Create a copy of the current configuration with updated parameter
+        values.
+
+        The method arguments are identical to :meth:`create`. Values that should
+        not be modified are by default represented by the special value
+        :obj:`~yaw.config.default.NotSet`.
+        """
+        config = self.to_dict()
+        if cosmology is not DEFAULT.NotSet:
+            if isinstance(cosmology, str):
+                cosmology = utils.yaml_to_cosmology(cosmology)
+            config["cosmology"] = utils.cosmology_to_yaml(cosmology)
+        # ScalesConfig
+        if rmin is not DEFAULT.NotSet:
+            config["scales"]["rmin"] = rmin
+        if rmax is not DEFAULT.NotSet:
+            config["scales"]["rmax"] = rmax
+        if rweight is not DEFAULT.NotSet:
+            config["scales"]["rweight"] = rweight
+        if rbin_num is not DEFAULT.NotSet:
+            config["scales"]["rbin_num"] = rbin_num
+        # AutoBinningConfig /  ManualBinningConfig
+        if zbins is not DEFAULT.NotSet:
+            warn_binning_args_ignored(zmin, zmax, zbin_num)
+            config["binning"]["zbins"] = zbins
+        else:
+            if zmin is not DEFAULT.NotSet:
+                config["binning"]["zmin"] = zmin
+            if zmax is not DEFAULT.NotSet:
+                config["binning"]["zmax"] = zmax
+            if zbin_num is not DEFAULT.NotSet:
+                config["binning"]["zbin_num"] = zbin_num
+            if method is not DEFAULT.NotSet:
+                config["binning"]["method"] = method
+        # BackendConfig
+        if thread_num is not DEFAULT.NotSet:
+            config["backend"]["thread_num"] = thread_num
+        if crosspatch is not DEFAULT.NotSet:
+            config["backend"]["crosspatch"] = crosspatch
+        if rbin_slop is not DEFAULT.NotSet:
+            config["backend"]["rbin_slop"] = rbin_slop
+        return self.__class__.from_dict(config)
 
-    @deprecated(reason="no longer maintained", version="2.5.3")
     def plot_scales(
         self, catalog: BaseCatalog, log: bool = True, legend: bool = True
-    ) -> Figure:  # pragma: no cover
+    ) -> Figure:
         """Plot the configured correlation scales at different redshifts in
-        comparison to the size of patches in a data catalogue.
-
-        .. deprecated:: 2.5.3
-            No longer maintained.
-        """
+        comparison to the size of patches in a data catalogue."""
         import matplotlib.pyplot as plt
 
         fig, ax_scale = plt.subplots(1, 1)
         # plot scale of annulus
         for r_min, r_max in self.scales.as_array():
             ang_min, ang_max = np.transpose(
                 [
@@ -283,27 +303,30 @@
     def from_dict(cls, the_dict: dict[str, Any], **kwargs) -> Configuration:
         config = {k: v for k, v in the_dict.items()}
         cosmology = utils.parse_cosmology(
             config.pop("cosmology", DEFAULT.Configuration.cosmology)
         )
         # parse the required subgroups
         try:
-            scales_dict = config.pop("scales")
-            scales = ScalesConfig.from_dict(scales_dict)
+            scales = ScalesConfig.from_dict(config.pop("scales"))
         except (TypeError, KeyError) as e:
             utils.parse_section_error(e, "scales")
         try:
-            binning_dict = config.pop("binning")
-            binning = BinningConfig.from_dict(binning_dict, cosmology=cosmology)
+            binning_conf = config.pop("binning")
+            if "zbins" in binning_conf:
+                binning = ManualBinningConfig(binning_conf["zbins"])
+            else:
+                binning = AutoBinningConfig.generate(
+                    cosmology=cosmology, **binning_conf
+                )
         except (TypeError, KeyError) as e:
             utils.parse_section_error(e, "binning")
         # parse the optional subgroups
         try:
-            backend_dict = config.pop("backend")
-            backend = BackendConfig.from_dict(backend_dict)
+            backend = BackendConfig.from_dict(config.pop("backend"))
         except KeyError:
             backend = BackendConfig()
         except TypeError as e:
             utils.parse_section_error(e, "backend")
         # check that there are no entries left
         if len(config) > 0:
             key = next(iter(config.keys()))
@@ -327,23 +350,23 @@
         Args:
             path (:obj:`pathlib.Path`, :obj:`str`):
                 Path to the YAML file containing the configuration.
 
         Returns:
             :obj:`Configuration`
         """
-        logger.info("reading configuration file '%s'", path)
+        logger.info(f"reading configuration file '{path}'")
         with open(str(path)) as f:
             config = yaml.safe_load(f.read())
         return cls.from_dict(config)
 
     def to_yaml(self, path: TypePathStr) -> None:
         """Store the configuration as YAML file.
 
         Args:
             path (:obj:`pathlib.Path`, :obj:`str`):
                 Path to which the YAML file is written.
         """
-        logger.info("writing configuration file '%s'", path)
+        logger.info(f"writing configuration file '{path}'")
         string = yaml.dump(self.to_dict())
         with open(str(path), "w") as f:
             f.write(string)
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/config/default.py` & `yet_another_wizz-2.5.post0/src/yaw/config/default.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 objects. Each of the ``*Config`` objects has a corresponding class holding just
 the default values, as listed below.
 """
 
 __all__ = [
     "NotSet",
     "Scales",
-    "Binning",
+    "AutoBinning",
     "Backend",
     "Configuration",
     "Resampling",
     "backend",
 ]
 
 
@@ -22,39 +22,33 @@
         return False
 
 
 class NotSet(metaclass=_NotSet_meta):
     pass
 
 
-# docs: render code below
-
-
 class Scales:
     rweight = None
     rbin_num = 50
 
 
-class Binning:
+class AutoBinning:
     method = "linear"
     zbin_num = 30
 
 
-AutoBinning = Binning  # keep for backwards compatibilty
-
-
 class Backend:
     thread_num = None
     crosspatch = True
     rbin_slop = 0.01
 
 
 class Configuration:
     scales = Scales
-    binning = Binning
+    binning = AutoBinning
     backend = Backend
     cosmology = "Planck15"
 
 
 class Resampling:
     method = "jackknife"
     crosspatch = True
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/config/options.py` & `yet_another_wizz-2.5.post0/src/yaw/config/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,29 +16,25 @@
         from yaw.catalogs import BaseCatalog
 
         return tuple(sorted(BaseCatalog._backends.keys()))
 
     @property
     def binning(self) -> tuple[str]:
         """Lists the currently implemented methods to generate redshift bins
-        with the :obj:`~yaw.config.BinningConfig` class.
+        with the :obj:`~yaw.config.AutoBinningConfig` class.
 
         .. rubric:: Values
 
         ``comoving``: Generate a binning with equal width in radial comoving
         distance.
 
         ``linear``: Generate a binning with equal width in redshift.
 
         ``logspace``: Generate a binning with equal width in logarithmic
         redshift :math:`\\log(1+z)`.
-
-        .. Note::
-
-            Class also accepts ``manual`` if custom bin edges are provided.
         """
         return ("comoving", "linear", "logspace")
 
     @property
     def cosmology(self) -> tuple[str]:
         """Lists the availble named cosmologies in :obj:`astropy`.
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/config/resampling.py` & `yet_another_wizz-2.5.post0/src/yaw/config/resampling.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
 
-from dataclasses import asdict, dataclass, field
+from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 
 from yaw.config import OPTIONS
 from yaw.config import default as DEFAULT
-from yaw.config.abc import BaseConfig
 from yaw.config.utils import ConfigError
-from yaw.core.docs import Parameter
+from yaw.core.abc import DictRepresentation
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
 __all__ = ["ResamplingConfig"]
 
 
 @dataclass(frozen=True)
-class ResamplingConfig(BaseConfig):
+class ResamplingConfig(DictRepresentation):
     """Configuration for error estimation from spatial resampling.
 
     Used for all functions and methods that use spatial patches for error
     estimation. Use the :meth:`get_samples` method to generate samples from the
     spatial patches, which can be reused to ensure consistent error estimates
     for different data products that use the same patches.
 
@@ -37,89 +36,49 @@
         global_norm (:obj:`bool`):
             Whether to normalise paircounts globally or for each sample. Usually
             not recommended.
         seed (:obj:`int`):
             Random seed to use.
     """
 
-    method: str = field(
-        default=DEFAULT.Resampling.method,
-        metadata=Parameter(type=str, help="resampling method to use"),
-    )
+    method: str = DEFAULT.Resampling.method
     """Resampling method to use, see :obj:`~yaw.config.options.Options.method`.
     """
-    crosspatch: bool = field(
-        default=DEFAULT.Resampling.crosspatch,
-        metadata=Parameter(
-            type=bool, help="whether to use cross-patch pair count measurements"
-        ),
-    )
+    crosspatch: bool = DEFAULT.Resampling.crosspatch
     """Whether to use cross-patch pair count measurements."""
-    n_boot: int = field(
-        default=DEFAULT.Resampling.n_boot,
-        metadata=Parameter(
-            type=int, help="number of samples to generate if method='bootstrap'"
-        ),
-    )
+    n_boot: int = DEFAULT.Resampling.n_boot
     """Number of samples to generate for the ``bootstrap`` method."""
-    global_norm: bool = field(
-        default=DEFAULT.Resampling.global_norm,
-        metadata=Parameter(
-            type=bool,
-            help="whether to normalise paircounts globally or for each sample",
-        ),
-    )
+    global_norm: bool = DEFAULT.Resampling.global_norm
     """Whether to normalise paircounts globally or for each sample."""
-    seed: int = field(
-        default=DEFAULT.Resampling.seed,
-        metadata=Parameter(type=int, help="random seed to use"),
-    )
+    seed: int = DEFAULT.Resampling.seed
     """Random seed to use."""
     _resampling_idx: NDArray[np.int_] | None = field(
         default=None, init=False, repr=False
     )
 
     def __post_init__(self) -> None:
         if self.method not in OPTIONS.method:
             opts = ", ".join(f"'{s}'" for s in OPTIONS.method)
             raise ConfigError(
                 f"invalid resampling method '{self.method}', must either of {opts}"
             )
 
-    def modify(
-        self,
-        method: str = DEFAULT.NotSet,
-        crosspatch: bool = DEFAULT.NotSet,
-        n_boot: int = DEFAULT.NotSet,
-        global_norm: bool = DEFAULT.NotSet,
-        seed: int = DEFAULT.NotSet,
-    ) -> ResamplingConfig:
-        return super().modify(
-            method=method,
-            crosspatch=crosspatch,
-            n_boot=n_boot,
-            global_norm=global_norm,
-            seed=seed,
-        )
-
     @property
     def n_patches(self) -> int | None:
         """The number of spatial patches for which this configuratin is valid.
 
         Available only after generating samples with :meth:`get_samples`.
 
         Returns:
             int if samples have been generated, else None.
         """
         if self._resampling_idx is None:
             return None
-        elif self.method == "bootstrap":
-            return self._resampling_idx.shape[1]
         else:
-            return self._resampling_idx.shape[0]
+            return self._resampling_idx.shape[1]
 
     def _generate_bootstrap(self, n_patches: int) -> NDArray[np.int_]:
         """Generate samples for the bootstrap resampling method.
 
         For N patches, draw M realisations each containing N randomly chosen
         patches.
         """
@@ -171,16 +130,10 @@
     def reset(self) -> None:
         """Reset the internally stored patch indices generated by
         :meth:`get_samples`."""
         object.__setattr__(self, "_resampling_idx", None)
 
     def to_dict(self) -> dict[str, Any]:
         if self.method == "jackknife":
-            return dict(
-                method=self.method,
-                crosspatch=self.crosspatch,
-                global_norm=self.global_norm,
-            )
+            return dict(method=self.method, crosspatch=self.crosspatch)
         else:
-            the_dict = asdict(self)
-            the_dict.pop("_resampling_idx")
-            return the_dict
+            return super().to_dict()
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/config/scales.py` & `yet_another_wizz-2.5.post0/src/yaw/config/scales.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
 import numpy as np
 from deprecated import deprecated
 
 from yaw.config import default as DEFAULT
-from yaw.config.abc import BaseConfig
 from yaw.config.utils import ConfigError
+from yaw.core.abc import DictRepresentation
 from yaw.core.cosmology import Scale
 from yaw.core.docs import Parameter
 from yaw.core.math import array_equal
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
 __all__ = ["ScalesConfig"]
 
 
 @dataclass(frozen=True)
-class ScalesConfig(BaseConfig):
+class ScalesConfig(DictRepresentation):
     """Configuration of scales used for correlation measurements.
 
     Correlation functions are measured on one or many intervals
     :math:`r_{\\rm min} \\leq r < r_{\\rm max}` angular diameter distance in
     kpc. When measuring correlations, this scale is coverted to angles at the
     current redshift.
 
@@ -33,37 +33,37 @@
     :math:`r^\\alpha` if a power-law exponent is provided through ``rweight``.
     The weighting is applied logarithmically spaced bins of separation (based
     on the logarithmic bin centers). This is an approximation to actually
     weighting each pair individually and the resolution of this approximation
     can be controlled by setting the number of bins.
 
     Args:
-        rmin (:obj:`float`, :obj:`list[float]`):
+        rmin (:obj:`float`, :obj:`Sequence[float]`):
             Single or multiple lower scale limits in kpc (angular diameter
             distance).
-        rmax (:obj:`float`, :obj:`list[float]`):
+        rmax (:obj:`float`, :obj:`Sequence[float]`):
             Single or multiple upper scale limits in kpc (angular diameter
             distance).
         rweight (:obj:`float`, optional):
             Power-law exponent used to weight pairs by their separation.
         rbin_num (:obj:`int`, optional):
             Number of radial logarithmic bin used to approximate the weighting
             by separation.
     """
 
-    rmin: list[float] | float = field(
+    rmin: Sequence[float] | float = field(
         metadata=Parameter(
             type=float,
             nargs="*",
             required=True,
             help="(list of) lower scale limit in kpc (pyhsical)",
         )
     )
     """Lower scale limit(s) in kpc (angular diameter distance)."""
-    rmax: list[float] | float = field(
+    rmax: Sequence[float] | float = field(
         metadata=Parameter(
             type=float,
             nargs="*",
             required=True,
             help="(list of) upper scale limit in kpc (pyhsical)",
         )
     )
@@ -116,40 +116,31 @@
             object.__setattr__(self, "rmin", float(self.rmin))
             object.__setattr__(self, "rmax", float(self.rmax))
             if self.rmin >= self.rmax:
                 raise ConfigError(msg_scale_error)
         else:
             raise ConfigError("'rmin' and 'rmax' must be both sequences or float")
 
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, self.__class__):
-            return (
-                array_equal(self.as_array(), other.as_array())
-                and self.rweight == other.rweight
-                and self.rbin_num == other.rbin_num
-            )
-        return NotImplemented
+    def __eq__(self, other: ScalesConfig) -> bool:
+        if not array_equal(self.as_array(), other.as_array()):
+            return False
+        if self.rweight != other.rweight:
+            return False
+        if self.rbin_num != other.rbin_num:
+            return False
+        return True
 
     def __getitem__(self, idx: int) -> Scale:
         scales = self.as_array()
         return Scale(rmin=scales[idx, 0], rmax=scales[idx, 1])
 
     def __iter__(self) -> Iterator[Scale]:
         for rmin, rmax in self.as_array():
             yield Scale(rmin=rmin, rmax=rmax)
 
-    def modify(
-        self,
-        rmin: list[float] | float = DEFAULT.NotSet,
-        rmax: list[float] | float = DEFAULT.NotSet,
-        rweight: float | None = DEFAULT.NotSet,
-        rbin_num: int = DEFAULT.NotSet,
-    ) -> ScalesConfig:
-        return super().modify(rmin=rmin, rmax=rmax, rweight=rweight, rbin_num=rbin_num)
-
     def as_array(self) -> NDArray[np.float_]:
         """Obtain the scales cuts as array of shape (2, N)"""
         return np.atleast_2d(np.transpose([self.rmin, self.rmax]))
 
     @deprecated("use [str(scale) for scale in ScalesConfig] instead", version="2.3.1")
     def dict_keys(self) -> list[str]:
         """Get the scale cuts formatted as a list of strings.
@@ -160,8 +151,8 @@
 
         .. deprecated:: 2.3.1
             Use instead
 
             >>> [str(scale) for scale in ScalesConfig]
             ...
         """
-        return [str(scale) for scale in self]  # pragma: no cover
+        return [str(scale) for scale in self]
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/config/utils.py` & `yet_another_wizz-2.5.post0/src/yaw/config/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import NoReturn, get_args
 
 import astropy.cosmology
 
-from yaw.core.cosmology import CustomCosmology, TypeCosmology, get_default_cosmology
+from yaw.core.cosmology import TypeCosmology, get_default_cosmology
 
 __all__ = [
     "cosmology_to_yaml",
     "yaml_to_cosmology",
     "parse_cosmology",
     "parse_section_error",
 ]
@@ -19,18 +19,16 @@
 
 
 def cosmology_to_yaml(cosmology: TypeCosmology) -> str:
     """Try to represent the cosmological model in a YAML-friendly way.
 
     If it is one of the names :obj:`astropy` cosmologies, returns the name,
     otherwise raises an :exc:`ConfigError`."""
-    if isinstance(cosmology, CustomCosmology):
+    if not isinstance(cosmology, astropy.cosmology.FLRW):
         raise ConfigError("cannot serialise custom cosmoligies to YAML")
-    elif not isinstance(cosmology, astropy.cosmology.FLRW):
-        raise TypeError(f"invalid type '{type(cosmology)}' for cosmology")
     if cosmology.name not in astropy.cosmology.available:
         raise ConfigError("can only serialise predefined astropy cosmologies to YAML")
     return cosmology.name
 
 
 def yaml_to_cosmology(cosmo_name: str) -> TypeCosmology:
     """Reinstantiate the cosmological model from its name representation."""
@@ -50,39 +48,35 @@
     :obj:`astropy` cosmologies or subclass of
     :obj:`yaw.core.cosmology.CustomCosmology`."""
     if cosmology is None:
         cosmology = get_default_cosmology()
     elif isinstance(cosmology, str):
         cosmology = yaml_to_cosmology(cosmology)
     elif not isinstance(cosmology, get_args(TypeCosmology)):
-        which = ", ".join(str(c) for c in get_args(TypeCosmology))
+        which = ", ".join(get_args(TypeCosmology))
         raise ConfigError(f"'cosmology' must be instance of: {which}")
     return cosmology
 
 
 def parse_section_error(
     exception: Exception, section: str, reraise: Exception = ConfigError
 ) -> NoReturn:
     """Reraises are a more descriptive exception from an existing exception when
     parsing a YAML configuration.
 
     Covered cases are undefined key names, missing required key names or
     entirely missing subsection in the configuration.
     """
-    if len(exception.args) > 0:
-        msg = exception.args[0]
-        try:
-            item = msg.split("'")[1]
-        except IndexError:
-            item = msg
-        if isinstance(exception, TypeError):
-            if "got an unexpected keyword argument" in msg:
-                raise reraise(
-                    f"encountered unknown option '{item}' in section '{section}'"
-                ) from exception
-            elif "missing" in msg:
-                raise reraise(
-                    f"missing option '{item}' in section '{section}'"
-                ) from exception
-        elif isinstance(exception, KeyError):
-            raise reraise(f"missing section '{section}'") from exception
+    msg = exception.args[0]
+    item = msg.split("'")[1]
+    if isinstance(exception, TypeError):
+        if "__init__() got an unexpected keyword argument" in msg:
+            raise reraise(
+                f"encountered unknown option '{item}' in section '{section}'"
+            ) from exception
+        elif "missing" in msg:
+            raise reraise(
+                f"missing option '{item}' in section '{section}'"
+            ) from exception
+    elif isinstance(exception, KeyError):
+        raise reraise(f"missing section '{section}'") from exception
     raise
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/core/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/core/abc.py` & `yet_another_wizz-2.5.post0/src/yaw/core/abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module implements some abstract base classes that define the interfaces
 for high level containers in other modules.
 """
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
+from abc import ABC, abstractclassmethod, abstractmethod, abstractproperty
 from dataclasses import asdict
 from typing import TYPE_CHECKING, Any, Type, TypeVar
 
 import h5py
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
@@ -30,36 +30,34 @@
 
 _Tpatched = TypeVar("_Tpatched", bound="PatchedQuantity")
 
 
 class PatchedQuantity(ABC):
     """Base class for an object that has data organised in spatial patches."""
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def n_patches(self) -> int:
         """Get the number of spatial patches."""
         pass
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def patches(self) -> Indexer:
         """An :obj:`~yaw.core.containers.Indexer` attribute that supports
         iteration over the spatial patches or selecting a subset of the patches.
 
         The indexer always returns new container instances with the indexed
         data subset or the current item when iterating.
 
         .. Note::
             Indexing rules for a one-dimensional numpy array apply.
 
         Returns:
             :obj:`yaw.core.containers.Indexer`
         """
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def concatenate_patches(self: _Tpatched, *data: _Tpatched) -> _Tpatched:
         """Concatenate pair count data containers with equal redshift binning.
 
         The data is merged by extending the dimension of the patch axes. The
         resulting data array will be a block matrix of the input data arrays,
@@ -75,31 +73,30 @@
             *data:
                 Containers of same type that are appended to the patch dimension
                 of this container.
 
         Returns:
             New instance of this container with combined data.
         """
-        pass
+        raise NotImplementedError
 
 
 _Tbinned = TypeVar("_Tbinned", bound="BinnedQuantity")
 
 
 class BinnedQuantity(ABC):
     """Base class for an object that has data organised in redshift bins."""
 
-    @abstractmethod
     def get_binning(self) -> IntervalIndex:
         """Get the underlying, exact redshift bin intervals.
 
         Returns:
             :obj:`pandas.IntervalIndex`
         """
-        pass
+        raise NotImplementedError
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
         n_bins = self.n_bins
         binning = self.get_binning()
         z = f"{binning[0].left:.3f}...{binning[-1].right:.3f}"
         return f"{name}({n_bins=}, {z=})"
@@ -127,16 +124,15 @@
 
     @property
     def closed(self) -> str:
         """Specifies on which side the redshift bin intervals are closed, can
         be: ``left``, ``right``, ``both``, ``neither``."""
         return self.get_binning().closed
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def bins(self) -> Indexer:
         """An :obj:`~yaw.core.containers.Indexer` attribute that supports
         iteration over the bins or selecting a subset of the bins.
 
         The indexer always returns new container instances with the indexed
         data subset or the current item when iterating.
 
@@ -144,15 +140,15 @@
             Indexing rules for a one-dimensional numpy array apply, however if
             the resulting binning is not contiguous or contains repeated bins,
             some operations on the returned container may fail.
 
         Returns:
             :obj:`yaw.core.containers.Indexer`
         """
-        pass
+        raise NotImplementedError
 
     def is_compatible(self: _Tbinned, other: _Tbinned, require: bool = False) -> bool:
         """Check whether this instance is compatible with another instance.
 
         Ensures that both objects are instances of the same class and that the
         redshift binning is identical.
 
@@ -197,15 +193,15 @@
             *data:
                 Containers of same type that are appended to the patch dimension
                 of this container.
 
         Returns:
             New instance of this container with combined data.
         """
-        pass
+        raise NotImplementedError
 
 
 def concatenate_bin_edges(*patched: BinnedQuantity) -> IntervalIndex:
     """Concatenate the binning a set of data containers.
 
     The input containers are automatically sorted by the lowest edge of the
     redshift binning. Necessary condidtions for mergning are are that the patch
@@ -226,37 +222,36 @@
 
 _Thdf = TypeVar("_Thdf", bound="HDFSerializable")
 
 
 class HDFSerializable(ABC):
     """Base class for an object that can be serialised into a HDF5 file."""
 
-    @classmethod
-    @abstractmethod
+    @abstractclassmethod
     def from_hdf(cls: Type[_Thdf], source: h5py.Group) -> _Thdf:
         """Create a class instance by deserialising data from a HDF5 group.
 
         Args:
             source (:obj:`h5py.Group`):
                 Group in an opened HDF5 file that contains the serialised data.
 
         Returns:
             :obj:`HDFSerializablep`
         """
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def to_hdf(self, dest: h5py.Group) -> None:
         """Serialise the class instance into an existing HDF5 group.
 
         Args:
             dest (:obj:`h5py.Group`):
                 Group in which the serialised data structures are created.
         """
-        pass
+        raise NotImplementedError
 
     @classmethod
     def from_file(cls: Type[_Thdf], path: TypePathStr) -> _Thdf:
         """Create a class instance by deserialising data from a HDF5 file.
 
         Args:
             path (:obj:`pathlib.Path`, :obj:`str`):
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/core/containers.py` & `yet_another_wizz-2.5.post0/src/yaw/redshifts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,448 +1,602 @@
-"""This module defines a few containers used throughout other modules.
-
-Most importantly, they implement two containers for data with attached samples
-(e.g. jackknife or bootstrap). Scalar values are implemented in
-:obj:`SampledValue`, data that has been computed from redshift bins in
-:obj:`SampledData`, which also serves as base class for most other containers
-with redshift binning.
+"""This module implements a special containers that compute and describe
+redshift distributions. These containers provide methods for error and
+covariance estimation, plotting and computing mean redshifts.
+
+True redshift distributions can be expressed through the :obj:`HistData` class
+and can be computed from the :meth:`~yaw.catalogs.BaseCatalog.true_redshifts`
+method of :obj:`~yaw.catalogs.BaseCatalog`.
+
+Clustering redshift estimates can be expressed through the :obj:`RedshiftData`
+class. Its different constructor methods, :meth:`~RedshiftData.from_corrdata`
+and :meth:`~RedshiftData.from_corrfuncs`, provide easy interfaces to compute the
+clustering redshifts and to mitigate the evolving galaxy bias, if the
+corresponding autocorrelation functions (e.g. of the reference sample) are
+known.
 """
 
 from __future__ import annotations
 
+import logging
 import warnings
-from collections.abc import Iterator, Sequence
-from dataclasses import dataclass, field, fields
-from typing import TYPE_CHECKING, Callable, Generic, NamedTuple, TypeVar
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
+import scipy.optimize
+from deprecated import deprecated
 
-from yaw.config import OPTIONS
-from yaw.core.abc import BinnedQuantity, concatenate_bin_edges
-from yaw.core.math import cov_from_samples
+from yaw.config import ResamplingConfig
+from yaw.core.containers import SampledValue
+from yaw.core.logging import LogCustomWarning, TimedLog
+from yaw.core.math import rebin, shift_histogram
+from yaw.core.utils import TypePathStr
+from yaw.correlation import CorrData
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
-    from pandas import DataFrame, IntervalIndex, Series
 
-__all__ = ["Indexer", "PatchIDs", "PatchCorrelationData", "SampledValue", "SampledData"]
+    from yaw.correlation import CorrFunc
 
+__all__ = ["RedshiftData", "HistData"]
 
-_TK = TypeVar("_TK")
-_TV = TypeVar("_TV")
 
+logger = logging.getLogger(__name__)
 
-class Indexer(Generic[_TK, _TV], Iterator):
-    """Helper class to implemented a class attribute that can be used as
-    indexer and iterator for the classes stored data (e.g. indexing patches or
-    redshift bins).
-    """
 
-    def __init__(self, inst: _TV, builder: Callable[[_TV, _TK], _TV]) -> None:
-        """Construct a new indexer.
+@dataclass(frozen=True, repr=False, eq=False)
+class RedshiftData(CorrData):
+    """Container class object for redshift estimates.
 
-        Args:
-            inst:
-                Class instance on which the indexing operations are applied.
-            builder:
-                Callable signature ``builder(inst, item) -> inst`` that
-                constructs a new class instance with the indexing specified from
-                ``item`` applied.
-
-
-        The resulting indexer supports indexing and slicing (depending on the
-        subclass implementation), as well as iteration, where instances holding
-        individual items are yielded.
-        """
-        self._inst = inst
-        self._builder = builder
-        self._iter_loc = 0
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}({self._inst.__class__.__name__})"
-
-    def __getitem__(self, item: _TK) -> _TV:
-        return self._builder(self._inst, item)
-
-    def __next__(self) -> _TV:
-        """Returns the next value and increments the iterator location index."""
-        try:
-            val = self[self._iter_loc]
-        except IndexError:
-            raise StopIteration
-        else:
-            self._iter_loc += 1
-            return val
+    Contains the redshift binning, estimated fraction of galaxies at the given
+    redshift (**not** a density), and resampled fractions (e.g. from jackknife
+    or bootstrap). The resampled values are used to compute error estimates and
+    covariance/correlation matrices. Provides some plotting methods for
+    convenience.
 
-    def __iter__(self) -> Iterator[_TV]:
-        """Returns a new instance of this class to have an independent iterator
-        location index"""
-        return self.__class__(inst=self._inst, builder=self._builder)
+    This container holds data in the form of
+    :math:`\\frac{w_\\rm{sp}(z)}{\\sqrt{\\Delta z \\, w_\\rm{ss}(z) \\, w_\\rm{pp}(z)}}`,
+    where :math:`w_\\rm{sp}` is the crosscorrelation function, and
+    :math:`w_\\rm{ss}` and :math:`w_\\rm{pp}` are autocorrelation functions that
+    account for the evolving galaxy bias. If no autocorrelation is provided, the
+    data is still scaled by :math:`1/\\Delta z` compared to the crosscorrelation
+    data in :obj:`~yaw.correlation.CorrData`.
 
+    .. Note::
+        This container should be constructed from a crosscorrelation measurement
+        with one of the preferred methods :meth:`from_corrdata` or
+        :meth:`from_corrfuncs`. These additionally allow galaxy bias mitigation
+        by specifying any additionally measured autocorrelation functions.
 
-class PatchIDs(NamedTuple):
-    """Named tuple that can hold a pair of patch indices."""
+    The comparison, addition and subtraction and indexing rules are inherited
+    from :obj:`~yaw.core.containers.SampledData`, check the examples there.
 
-    id1: int
-    """First patch index."""
-    id2: int
-    """Second patch index."""
+    .. rubric:: Examples
 
+    Create a redshift estimate from a crosscorrelation function and correct for
+    the evolving bias of the reference sample using its autocorrelation
+    function:
 
-@dataclass(frozen=True)
-class PatchCorrelationData:
-    """Container to hold the result of a pair counting operation between two
-    spatial patches.
+    >>> from yaw.examples import w_sp  # crosscorrelation
+    >>> from yaw.examples import w_ss  # reference sample autocorrelation
+    >>> nz = yaw.yaw.RedshiftData.from_corrfuncs(w_sp, ref_corr=w_ss)
+    RedshiftData(n_bins=30, z='0.070...1.420', n_samples=64, method='jackknife')
 
-    Args:
-        patches (:obj:`PatchIDs`):
-            The indices of used the patches.
-        totals1 (:obj:`NDArray`):
-            Total number of objects after binning by redshift in first patch.
-        totals1 (:obj:`NDArray`):
-            Total number of objects after binning by redshift in second patch.
-        counts (:obj:`dict`):
-            Dictionary listing the number of counted pairs after binning by
-            redshift. Each item represents results from a different scale.
-    """
+    Use a different estimator when sampling the autocorrelation function, e.g.
+    the Peebles-Hauser estimator:
 
-    patches: PatchIDs
-    totals1: NDArray
-    totals2: NDArray
-    counts: dict[str, NDArray]
+    >>> nz = yaw.RedshiftData.from_corrfuncs(w_sp, ref_corr=w_ss, ref_est="PH")
+    RedshiftData(n_bins=30, z='0.070...1.420', n_samples=64, method='jackknife')
 
+    View the data for a subset of the redshift bins:
 
-_Tscalar = TypeVar("_Tscalar", bound=np.number)
+    >>> nz.bins[5:9].data
+    array([2.5234212 , 1.96617211, 1.05342   , 0.67866257])
 
+    View the same subset as series:
 
-@dataclass(frozen=True)
-class SampledValue(Generic[_Tscalar]):
-    """Container to hold a scalar value with an empirically estimated
-    uncertainty from resampling.
+    >>> nz.bins[5:9].get_data()
+    (0.295, 0.34]    2.523421
+    (0.34, 0.385]    1.966172
+    (0.385, 0.43]    1.053420
+    (0.43, 0.475]    0.678663
+    dtype: float64
 
-    Supports comparison of the values and samples with ``==`` and ``!=``.
+    Get the redshift bin centers for these bins:
 
-    .. rubric:: Examples
+    >>> nz.bins[5:9].mids
+    array([0.3175, 0.3625, 0.4075, 0.4525])
+
+    Plot the redshift distribution, indicating a zero-line
 
-    Create a value container with 100 assumed jackknife samples that scatter
-    around zero with a standard deviation of 0.1:
+    >>> nz.plot(zero_line=True)
+    <Axes: >
 
-    >>> from numpy.random import normal
-    >>> samples = normal(loc=0.0, scale=0.01, size=101)
-    >>> value = yaw.core.SampledValue(0.0, samples, method="jackknife")
-    >>> value
-    SampledValue(value=0, error=0.963, n_samples=100, method='jackknife')
+    .. figure:: ../../_static/ncc_example.png
+        :width: 400
+        :alt: example clustering redshfit estimate
 
     Args:
-        value:
-            Numerical, scalar value.
+        binning (:obj:`pandas.IntervalIndex`):
+            The redshift bin edges used for this correlation function.
+        data (:obj:`NDArray`):
+            The correlation function values.
         samples (:obj:`NDArray`):
-            Samples of ``value`` obtained from resampling methods.
+            The resampled correlation function values.
         method (:obj:`str`):
-            Resampling method used to obtain the data samples, see
-            :class:`~yaw.ResamplingConfig` for available options.
+            The resampling method used, see :class:`~yaw.ResamplingConfig` for
+            available options.
+        info (:obj:`str`, optional):
+            Descriptive text included in the headers of output files produced
+            by :func:`CorrData.to_files`.
     """
 
-    value: _Tscalar
-    """Numerical, scalar value."""
-    samples: NDArray[_Tscalar]
-    """Samples of ``value`` obtained from resampling methods."""
-    method: str
-    """Resampling method used to obtain the data samples, see
-    :class:`~yaw.ResamplingConfig` for available options."""
-    error: _Tscalar = field(init=False)
-    """The uncertainty (standard error) of the value."""
-
-    def __post_init__(self) -> None:
-        if self.method not in OPTIONS.method:
-            raise ValueError(f"unknown sampling method '{self.method}'")
-        if self.method == "bootstrap":
-            error = np.std(self.samples, ddof=1, axis=0)
-        else:  # jackknife
-            error = np.std(self.samples, ddof=0, axis=0) * (self.n_samples - 1)
-        object.__setattr__(self, "error", error)
-
-    def __repr__(self) -> str:
-        string = self.__class__.__name__
-        value = self.value
-        error = self.error
-        n_samples = self.n_samples
-        method = self.method
-        return f"{string}({value=:.3g}, {error=:.3g}, {n_samples=}, {method=})"
-
-    def __str__(self) -> str:
-        return f"{self.value:+.3g}+/-{self.error:.3g}"
-
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, SampledValue):
-            return (
-                self.samples.shape == other.samples.shape
-                and self.method == other.method
-                and self.value == other.value
-                and np.all(self.samples == other.samples)
-            )
-        return NotImplemented
+    @classmethod
+    @deprecated(reason="renamed to RedshiftData.from_corrdata", version="2.3.2")
+    def from_correlation_data(cls, *args, **kwargs):
+        """
+        .. deprecated:: 2.3.2
+            Renamed to :meth:`from_corrdata`.
+        """
+        return cls.from_corrdata(*args, **kwargs)
 
-    @property
-    def n_samples(self) -> int:
-        """Number of samples used for error estimate."""
-        return len(self.samples)
+    @classmethod
+    def from_corrdata(
+        cls,
+        cross_data: CorrData,
+        ref_data: CorrData | None = None,
+        unk_data: CorrData | None = None,
+        info: str | None = None,
+    ) -> RedshiftData:
+        """Compute redshift estimate from readily sampled function data.
+
+        The required argument is a crosscorrelation measurement, additional
+        parameters can specify sample autocorrelation measurements that are used
+        to mitigate the evolving galaxy bias.
 
+        Args:
+            cross_corr (:obj:`CorrData`):
+                Data from the sampled cross-correlation function.
+            ref_corr (:obj:`CorrData`, optional):
+                Data from the sampled reference sample autocorrelation function.
+                Used to mitigate reference bias evolution.
+            unk_corr (:obj:`CorrData`, optional):
+                Data from the sampled unknown sample autocorrelation function.
+                Used to mitigate unknown bias evolution.
 
-_Tdata = TypeVar("_Tdata", bound="SampledData")
+        Returns:
+            :obj:`RedshiftData`
+        """
+        logger.debug("computing clustering redshifts from correlation function samples")
+        w_sp_data = cross_data.data
+        w_sp_samp = cross_data.samples
+        mitigate = []
+
+        if ref_data is None:
+            w_ss_data = np.float64(1.0)
+            w_ss_samp = np.float64(1.0)
+        else:
+            try:
+                ref_data.is_compatible(cross_data, require=True)
+            except ValueError as e:
+                raise ValueError(
+                    "'ref_corr' correlation data is not compatible with 'cross_data'"
+                ) from e
+            w_ss_data = ref_data.data
+            w_ss_samp = ref_data.samples
+            mitigate.append("reference")
+
+        if unk_data is None:
+            w_pp_data = np.float64(1.0)
+            w_pp_samp = np.float64(1.0)
+        else:
+            try:
+                unk_data.is_compatible(cross_data, require=True)
+            except ValueError as e:
+                raise ValueError(
+                    "'unk_data' correlation data is not compatible with " "'cross_data'"
+                ) from e
+            w_pp_data = unk_data.data
+            w_pp_samp = unk_data.samples
+            mitigate.append("unknown")
+
+        if len(mitigate) > 0:
+            logger.debug(f"mitigating {' and '.join(mitigate)} sample bias")
+        N = cross_data.n_samples
+        dzsq_data = cross_data.dz**2
+        dzsq_samp = np.tile(dzsq_data, N).reshape((N, -1))
+        with LogCustomWarning(
+            logger, "invalid values encountered in redshift estimate"
+        ):
+            nz_data = w_sp_data / np.sqrt(dzsq_data * w_ss_data * w_pp_data)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            nz_samp = w_sp_samp / np.sqrt(dzsq_samp * w_ss_samp * w_pp_samp)
+        return cls(
+            binning=cross_data.binning,
+            data=nz_data,
+            samples=nz_samp,
+            method=cross_data.method,
+            info=info,
+        )
 
+    @classmethod
+    @deprecated(reason="renamed to RedshiftData.from_corrfuncs", version="2.3.2")
+    def from_correlation_functions(cls, *args, **kwargs):
+        """
+        .. deprecated:: 2.3.2
+            Renamed to :meth:`from_corrfuncs`.
+        """
+        return cls.from_corrfuncs(*args, **kwargs)
 
-@dataclass(frozen=True, repr=False)
-class SampledData(BinnedQuantity):
-    """Container for data and resampled data with redshift binning.
+    @classmethod
+    def from_corrfuncs(
+        cls,
+        cross_corr: CorrFunc,
+        ref_corr: CorrFunc | None = None,
+        unk_corr: CorrFunc | None = None,
+        *,
+        cross_est: str | None = None,
+        ref_est: str | None = None,
+        unk_est: str | None = None,
+        config: ResamplingConfig | None = None,
+        info: str | None = None,
+    ) -> RedshiftData:
+        """Sample correlation functions to compute a redshift estimate.
+
+        The required argument is a crosscorrelation measurement, additional
+        parameters can specify sample autocorrelation measurements that are used
+        to mitigate the evolving galaxy bias.
 
-    Contains the redshift binning, data vector, and resampled data vector (e.g.
-    jackknife or bootstrap samples). The resampled values are used to compute
-    error estimates and covariance/correlation matrices.
+        Args:
+            cross_corr (:obj:`CorrFunc`):
+                The measured cross-correlation function.
+            ref_corr (:obj:`CorrFunc`, optional):
+                The measured reference sample autocorrelation function. Used to
+                mitigate reference bias evolution.
+            unk_corr (:obj:`CorrFunc`, optional):
+                The measured unknown sample autocorrelation function. Used to
+                mitigate unknown bias evolution.
 
-    Args:
-        binning (:obj:`pandas.IntervalIndex`):
-            The redshift binning applied to the data.
-        data (:obj:`NDArray`):
-            The data values, one for each redshift bin.
-        samples (:obj:`NDArray`):
-            The resampled data values (e.g. jackknife or bootstrap samples).
-        method (:obj:`str`):
-            The resampling method used, see :class:`~yaw.ResamplingConfig` for
-            available options.
+        Returns:
+            :obj:`RedshiftData`
+        """
+        if config is None:
+            config = ResamplingConfig()
+        with TimedLog(
+            logger.debug,
+            f"estimating clustering redshifts with method '{config.method}'",
+        ):
+            # check compatibilty before sampling anything
+            if ref_corr is not None:
+                try:
+                    cross_corr.is_compatible(ref_corr, require=True)
+                except ValueError as e:
+                    raise ValueError(
+                        "'ref_corr' correlation function is not compatible "
+                        "with 'cross_corr'"
+                    ) from e
+            if unk_corr is not None:
+                try:
+                    cross_corr.is_compatible(unk_corr, require=True)
+                except ValueError as e:
+                    raise ValueError(
+                        "'unk_corr' correlation function is not compatible "
+                        "with 'cross_corr'"
+                    ) from e
+            # sample pair counts and evaluate estimator
+            cross_data = cross_corr.sample(config, estimator=cross_est)
+            if ref_corr is not None:
+                ref_data = ref_corr.sample(config, estimator=ref_est)
+            else:
+                ref_data = None
+            if unk_corr is not None:
+                unk_data = unk_corr.sample(config, estimator=unk_est)
+            else:
+                unk_data = None
+            return cls.from_correlation_data(
+                cross_data=cross_data, ref_data=ref_data, unk_data=unk_data, info=info
+            )
 
-    The container supports addition and subtraction, which return a new instance
-    of the container, holding the modified data. This requires that both
-    operands are compatible (same binning and same sampling). The operands are
-    applied to the ``data`` and ``samples`` attribtes.
-
-    Furthermore, the container supports indexing and iteration over the redshift
-    bins using the :obj:`SampledData.bins` attribute. This attribute yields
-    instances of :obj:`SampledData` containing a single bin when iterating.
-    Slicing and indexing follows the same rules as the underlying ``data``
-    :obj:`NDArray`. Refer to :obj:`~yaw.correlation.CorrData` for some indexing
-    and iteration examples.
+    @property
+    def _dat_desc(self) -> str:
+        return "# n(z) estimate with symmetric 68% percentile confidence"
 
-    .. rubric:: Examples
+    @property
+    def _smp_desc(self) -> str:
+        return f"# {self.n_samples} {self.method} n(z) samples"
+
+    @property
+    def _cov_desc(self) -> str:
+        return f"# n(z) estimate covariance matrix ({self.n_bins}x{self.n_bins})"
+
+    def normalised(self, to: CorrData | None = None) -> RedshiftData:
+        """Obtain a normalised copy of the data.
+
+        Either attempts to normalise the data by integration along the redshift
+        axis or by fitting it to a provided reference data container (e.g. a
+        known redshift distribution in a :obj:`HistData` container).
+
+        .. Note::
+            The fit does not use the uncertainties but weights the data points
+            inversely to their amplitude.
 
-    Create a redshift binning:
+        Args:
+            to (:obj:`CorrData`, optional):
+                Reference data to which the stored values are normalised by
+                fitting.
 
-    >>> import pandas as pd
-    >>> bins = pd.IntervalIndex.from_breaks([0.1, 0.2, 0.3])
-    >>> bins
-    IntervalIndex([(0.1, 0.2], (0.2, 0.3]], dtype='interval[float64, right]')
+        Returns:
+            :obj:`RedshiftData`
+        """
+        if to is None:
+            norm = np.nansum(self.dz * self.data)
+        else:
+            y_from = self.data
+            y_to = to.data
+            mask = np.isfinite(y_from) & np.isfinite(y_to) & (y_to > 0.0)
+            norm = scipy.optimize.curve_fit(
+                lambda x, norm: y_from[mask] / norm,  # x is a dummy variable
+                xdata=to.mids[mask],
+                ydata=y_to[mask],
+                p0=[1.0],
+                sigma=1 / y_to[mask],
+            )[0][0]
+        return self.__class__(
+            binning=self.get_binning(),
+            data=self.data / norm,
+            samples=self.samples / norm,
+            method=self.method,
+            info=self.info,
+        )
 
-    Create some sample data for the bins with value 1 and five assumed jackknife
-    samples normal-distributed around 1.
+    def mean(self):
+        """Attempts to compute a mean redshift.
 
-    >>> import numpy as np
-    >>> n_bins, n_samples = len(bins), 5
-    >>> data = np.ones(n_bins)
-    >>> samples = np.random.normal(1.0, size=(n_samples, n_bins))
+        .. Warning::
+            This should be just considered an estimate since the redshift
+            estimate is not a true probability density, due to residual negative
+            correlation amplitudes.
 
-    Create the container:
+        Returns:
+            :obj:`~yaw.core.SampledValue`:
+                Mean redshift for the redshift data and its samples in a data
+                container.
+        """
+        norm = np.nansum(self.data)
+        mean = np.nansum(self.data * self.mids) / norm
+        samples = np.nansum(self.samples * self.mids, axis=1) / norm
+        return SampledValue(value=mean, samples=samples, method=self.method)
+
+    def rebin(self, bins: NDArray) -> RedshiftData:
+        """Attempts recomute the data for a different redshift binning.
+
+        .. Warning::
+            The result may be inaccurate since the redshift estimate is not a
+            true probability density, due to residual negative correlation
+            amplitudes.
 
-    >>> values = yaw.core.SampledData(bins, data, samples, method="jackknife")
-    >>> values
-    SampledData(n_bins=2, z='0.100...0.300', n_samples=10, method='jackknife')
+        Args:
+            bins (:obj:`NDArray`):
+                Edges of the new redshift bins. May exceed or cover just a
+                fraction of the original redshift range.
 
-    Add the container to itself and verify that the values are doubled:
+        Returns:
+            :obj:`RedshiftData`:
+        """
+        old_bins = self.edges
+        # shift main values
+        data = rebin(bins, old_bins, self.data)
+        # shift the value samples
+        samples = np.empty([self.n_samples, len(bins) - 1], data.dtype)
+        for i, sample in enumerate(self.samples):
+            samples[i] = rebin(bins, old_bins, sample)
+
+        return self.__class__(
+            binning=pd.IntervalIndex.from_breaks(bins),
+            data=data,
+            samples=samples,
+            method=self.method,
+            info=self.info,
+        )
 
-    >>> summed = values + values
-    >>> summed.data
-    array([2., 2.])
+    def shift(
+        self, dz: float | SampledValue = 0.0, *, amplitude: float | SampledValue = 1.0
+    ) -> RedshiftData:
+        """Attempts shift the data along the redshift axis.
+
+        The shifting is performed by recomputing the redshift estimate with its
+        original redshift bins which are shifted by some amount.
+
+        .. Warning::
+            The result may be inaccurate since the redshift estimate is not a
+            true probability density, due to residual negative correlation
+            amplitudes.
 
-    The same applies to the samples:
+        Args:
+            dz (:obj:`SampledValue` or :obj:`float`):
+                The amplitude of the shift along the redshift axis. If the input
+                provides samples of the shift, each redshift estimate sample is
+                shifted individually to obtain a more accurate error estimate.
+            amplitude (:obj:`SampledValue` or :obj:`float`):
+                An optional ampltude factor applied to the redshift estimate.
+                Same rules as for the ``dz`` parameter.
 
-    >>> summed.samples / values.samples
-    array([[2., 2.],
-           [2., 2.],
-           [2., 2.],
-           [2., 2.],
-           [2., 2.]])
-    """
+        Returns:
+            :obj:`RedshiftData`:
+        """
+        if isinstance(amplitude, SampledValue):
+            A_samples = amplitude.samples
+            amplitude = amplitude.value
+        else:
+            A_samples = [amplitude] * self.n_samples
+        if isinstance(dz, SampledValue):
+            dz_samples = dz.samples
+            dz = dz.value
+        else:
+            dz_samples = [dz] * self.n_samples
 
-    binning: IntervalIndex
-    """The redshift bin intervals."""
-    data: NDArray
-    """The data values, one for each redshift bin."""
-    samples: NDArray
-    """Samples of the data values, shape (# samples, # bins)."""
-    method: str
-    """The resampling method used."""
-    covariance: NDArray = field(init=False)
-    """Covariance matrix automatically computed from the resampled values."""
-
-    def __post_init__(self) -> None:
-        if self.data.shape != (self.n_bins,):
-            raise ValueError("unexpected shape of 'data' array")
-        if not self.samples.shape[1] == self.n_bins:
-            raise ValueError("number of bins for 'data' and 'samples' do not match")
-        if self.method not in OPTIONS.method:
-            raise ValueError(f"unknown sampling method '{self.method}'")
-
-        covmat = cov_from_samples(self.samples, self.method)
-        object.__setattr__(self, "covariance", np.atleast_2d(covmat))
-
-    def __repr__(self) -> str:
-        string = super().__repr__()[:-1]
-        n_samples = self.n_samples
-        method = self.method
-        return f"{string}, {n_samples=}, {method=})"
-
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, self.__class__):
-            return (
-                self.samples.shape == other.samples.shape
-                and self.method == other.method
-                and np.all(self.data == other.data)
-                and np.all(self.samples == other.samples)
-                and (self.binning == other.binning).all()
-            )
-        return NotImplemented
+        bins = self.edges
+        # shift main values
+        data = shift_histogram(bins, self.data, A=amplitude, dx=dz)
+        # shift the value samples
+        samples = np.empty_like(self.samples)
+        iter_samples = zip(self.samples, A_samples, dz_samples)
+        for i, (sample, amplitude, dz) in enumerate(iter_samples):
+            samples[i] = shift_histogram(bins, sample, A=amplitude, dx=dz)
+
+        return self.__class__(
+            binning=self.get_binning(),
+            data=data,
+            samples=samples,
+            method=self.method,
+            info=self.info,
+        )
 
-    def __add__(self, other: object) -> _Tdata:
-        if not isinstance(other, self.__class__):
-            self.is_compatible(other, require=True)
-            return self.__class__(
-                binning=self.get_binning(),
-                data=self.data + other.data,
-                samples=self.samples + other.samples,
-                method=self.method,
-            )
-        return NotImplemented
 
-    def __sub__(self, other: object) -> _Tdata:
-        if not isinstance(other, self.__class__):
-            self.is_compatible(other, require=True)
-            return self.__class__(
-                binning=self.get_binning(),
-                data=self.data - other.data,
-                samples=self.samples - other.samples,
-                method=self.method,
-            )
-        return NotImplemented
+@dataclass(frozen=True, repr=False, eq=False)
+class HistData(RedshiftData):
+    """Container for histogram data.
+
+    Contains the redshift binning, histogram counts, and resampled counts (e.g.
+    from jackknife or bootstrap). The resampled values are used to compute error
+    estimates and covariance/correlation matrices. Provides some plotting
+    methods for convenience.
 
-    @property
-    def bins(self: _Tdata) -> Indexer[int | slice | Sequence, _Tdata]:
-        def builder(inst: _Tdata, item: int | slice | Sequence) -> _Tdata:
-            if isinstance(item, int):
-                item = [item]
-            # try to take subsets along bin axis
-            binning = inst.get_binning()[item]
-            data = inst.data[item]
-            samples = inst.samples[:, item]
-            # determine which extra attributes need to be copied
-            init_attrs = {field.name for field in fields(inst) if field.init}
-            copy_attrs = init_attrs - {"binning", "data", "samples"}
-
-            kwargs = dict(binning=binning, data=data, samples=samples)
-            kwargs.update({attr: getattr(inst, attr) for attr in copy_attrs})
-            return inst.__class__(**kwargs)
+    Args:
+        binning (:obj:`pandas.IntervalIndex`):
+            The redshift bin edges used for this correlation function.
+        data (:obj:`NDArray`):
+            The correlation function values.
+        samples (:obj:`NDArray`):
+            The resampled correlation function values.
+        method (:obj:`str`):
+            The resampling method used, see :class:`~yaw.ResamplingConfig` for
+            available options.
+        info (:obj:`str`, optional):
+            Descriptive text included in the headers of output files produced
+            by :func:`CorrData.to_files`.
+        density (:obj:`bool`):
+            Whether the data is normalised, i.e. a density estimate.
+    """
 
-        return Indexer(self, builder)
+    density: bool = field(default=False)
+    """Whether the data is normalised, i.e. a density estimate."""
 
     @property
-    def n_samples(self) -> int:
-        """Number of samples used for error estimate."""
-        return len(self.samples)
+    def _dat_desc(self) -> str:
+        n = "normalised " if self.density else " "
+        return f"# n(z) {n}histogram with symmetric 68% percentile confidence"
 
     @property
-    def error(self) -> NDArray:
-        """The uncertainty (standard error) of the data.
-
-        Returns:
-            :obj:`NDArray`
-        """
-        return np.sqrt(np.diag(self.covariance))
-
-    def get_binning(self) -> IntervalIndex:
-        return self.binning
+    def _smp_desc(self) -> str:
+        n = "normalised " if self.density else " "
+        return f"# {self.n_samples} {self.method} n(z) {n}histogram samples"
 
-    def is_compatible(self, other: SampledData, require: bool = False) -> bool:
-        """Check whether this instance is compatible with another instance.
+    @property
+    def _cov_desc(self) -> str:
+        n = "normalised " if self.density else " "
+        return f"# n(z) {n}histogram covariance matrix ({self.n_bins}x{self.n_bins})"
+
+    @classmethod
+    def from_files(cls, path_prefix: TypePathStr) -> HistData:
+        new = super().from_files(path_prefix)
+        with open(f"{path_prefix}.dat") as f:
+            line = f.readline()
+            density = "normalised" in line
+        return cls(
+            binning=new.get_binning(),
+            data=new.data,
+            samples=new.samples,
+            method=new.method,
+            density=density,
+        )
 
-        Ensures that both objects are instances of the same class, that the
-        redshift binning is identical, that the number of samples agree, and
-        that the resampling method is identical.
+    def normalised(self, *args, **kwargs) -> HistData:
+        """Obtain a normalised copy of the data.
 
-        Args:
-            other (:obj:`BinnedQuantity`):
-                Object instance to compare to.
-            require (:obj:`bool`, optional)
-                Raise a ValueError if any of the checks fail.
+        Normalises the data by integration along the redshift axis. This sets
+        the containers :obj:`density` flag to ``True``.
 
         Returns:
-            :obj:`bool`
+            :obj:`HistData`
         """
-        if not super().is_compatible(other, require):
-            return False
-        if self.n_samples != other.n_samples:
-            if require:
-                raise ValueError("number of samples do not agree")
-            return False
-        if self.method != other.method:
-            if require:
-                raise ValueError("resampling method does not agree")
-            return False
-        return True
-
-    def concatenate_bins(self: _Tdata, *data: _Tdata) -> _Tdata:
-        for other in data:
-            self.is_compatible(other, require=True)
-        all_data: list[_Tdata] = [self, *data]
-        binning = concatenate_bin_edges(*all_data)
-        # concatenate data
-        data = np.concatenate([d.data for d in all_data])
-        samples = np.concatenate([d.samples for d in all_data], axis=1)
-        # determine which extra attributes need to be copied
-        init_attrs = {field.name for field in fields(self) if field.init}
-        copy_attrs = init_attrs - {"binning", "data", "samples"}
-
-        kwargs = dict(binning=binning, data=data, samples=samples)
-        kwargs.update({attr: getattr(self, attr) for attr in copy_attrs})
-        return self.__class__(**kwargs)
-
-    def get_data(self) -> Series:
-        """Get the data as :obj:`pandas.Series` with the binning as index."""
-        return pd.Series(self.data, index=self.binning)
-
-    def get_samples(self) -> DataFrame:
-        """Get the data as :obj:`pandas.DataFrame` with the binning as index.
-        The columns are labelled numerically and each represent one of the
-        samples."""
-        return pd.DataFrame(self.samples.T, index=self.binning)
-
-    def get_error(self) -> Series:
-        """Get value error estimate (diagonal of covariance matrix) as series
-        with its corresponding redshift bin intervals as index.
+        if self.density:  # guard from repeatedly altering the data
+            return self
+        zmin, zmax = self.edges[[0, -1]]
+        width_correction = (zmax - zmin) / (self.n_bins * self.dz)
+        data = self.data * width_correction
+        samples = self.samples * width_correction
+        norm = np.nansum(self.dz * data)
+        return self.__class__(
+            binning=self.get_binning(),
+            data=data / norm,
+            samples=samples / norm,
+            method=self.method,
+            info=self.info,
+            density=True,
+        )
+
+    def mean(self) -> SampledValue:
+        """Compute the mean redshift.
 
         Returns:
-            :obj:`pandas.Series`
+            :obj:`~yaw.core.SampledValue`:
+                Mean redshift for the redshift data and its samples in a data
+                container.
         """
-        return pd.Series(self.error, index=self.binning)
+        normed = self.normalised()
+        norm = np.nansum(normed.data)
+        mean = np.nansum(normed.data * normed.mids) / norm
+        samples = np.nansum(normed.samples * normed.mids, axis=1) / norm
+        return SampledValue(value=mean, samples=samples, method=normed.method)
+
+    def rebin(self, bins: NDArray) -> HistData:
+        """Recomute the data for a different redshift binning.
+
+        .. Warning::
+            The result may be inaccurate since the result is interpolated
+            step-wise.
 
-    def get_covariance(self) -> DataFrame:
-        """Get value covariance matrix as data frame with its corresponding
-        redshift bin intervals as index and column labels.
+        Args:
+            bins (:obj:`NDArray`):
+                Edges of the new redshift bins. May exceed or cover just a
+                fraction of the original redshift range.
 
         Returns:
-            :obj:`pandas.DataFrame`
+            :obj:`HistData`:
         """
-        return pd.DataFrame(
-            data=self.covariance, index=self.binning, columns=self.binning
-        )
+        result = super().rebin(bins)
+        object.__setattr__(self, "density", self.density)
+        return result
+
+    def shift(
+        self, dz: float | SampledValue = 0.0, *, amplitude: float | SampledValue = 1.0
+    ) -> HistData:
+        """Shifts the data along the redshift axis.
+
+        The shifting is performed by recomputing the histogram with its original
+        redshift bins which are shifted by some amount.
+
+        .. Warning::
+            The result may be inaccurate since the result is interpolated
+            step-wise.
 
-    def get_correlation(self) -> DataFrame:
-        """Get value correlation matrix as data frame with its corresponding
-        redshift bin intervals as index and column labels.
+        Args:
+            dz (:obj:`SampledValue` or :obj:`float`):
+                The amplitude of the shift along the redshift axis. If the input
+                provides samples of the shift, each redshift estimate sample is
+                shifted individually to obtain a more accurate error estimate.
+            amplitude (:obj:`SampledValue` or :obj:`float`):
+                An optional ampltude factor applied to the redshift estimate.
+                Same rules as for the ``dz`` parameter.
 
         Returns:
-            :obj:`pandas.DataFrame`
+            :obj:`HistData`:
         """
-        stdev = np.sqrt(np.diag(self.covariance))
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            corr = self.covariance / np.outer(stdev, stdev)
-        corr[self.covariance == 0] = 0
-        return pd.DataFrame(data=corr, index=self.binning, columns=self.binning)
+        result = super().shift(dz, amplitude=amplitude)
+        if amplitude == 1.0:
+            object.__setattr__(self, "density", self.density)
+        else:
+            object.__setattr__(self, "density", False)
+        return result
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/core/coordinates.py` & `yet_another_wizz-2.5.post0/src/yaw/core/coordinates.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module defines simple containers for coordiantes and distances. There
 are currently two flavours, 3-dim Euclidean coordinates and distances, as well
 as angular coordinates and distances in radian.
 """
 
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
+from abc import ABC, abstractclassmethod, abstractmethod, abstractproperty
 from collections.abc import Iterator, Sequence
 from functools import total_ordering
 from typing import TYPE_CHECKING, TypeVar
 
 import numpy as np
 
 from yaw.core.math import sgn
@@ -23,42 +23,38 @@
 class Coordinate(ABC):
     """Base class for a vector of coordinates."""
 
     @abstractmethod
     def __init__(self, coords: dict[str, ArrayLike]) -> None:
         pass
 
-    @classmethod
-    @abstractmethod
+    @abstractclassmethod
     def from_array(cls, array) -> Coordinate:
         pass
 
-    @classmethod
-    @abstractmethod
+    @abstractclassmethod
     def from_coords(cls, coords: Sequence[Coordinate]) -> Coordinate:
         """Concatenate a sequence of coordinates into a new vector of
         coordates."""
         pass
 
     def __repr__(self) -> str:
         pass
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def dim(self) -> tuple[str]:
         """A list of names of coordinates in the coordinate system."""
         pass
 
     @property
     def ndim(self) -> int:
         """The number of coordinates in the coordinate system."""
         return len(self.dim)
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def values(self) -> NDArray[np.float_]:
         """The coordinate values cast into a numpy array with shape
         `(N, ndim)` or `(ndim,)` if there is only a single entry."""
         pass
 
     @abstractmethod
     def mean(self) -> Coordinate:
@@ -160,17 +156,16 @@
     def to_sky(self) -> CoordSky:
         x = self.x
         y = self.y
         z = self.z
         r_d2 = np.sqrt(x * x + y * y)
         r_d3 = np.sqrt(x * x + y * y + z * z)
         # transform
-        x_normed = np.ones_like(x)  # fallback for zero-division, arccos(1)=0.0
-        np.divide(x, r_d2, where=r_d2 > 0.0, out=x_normed)
-        ra = np.arccos(x_normed) * sgn(y) % (2.0 * np.pi)
+        ra = np.arccos(x / r_d2) * sgn(y) % (2.0 * np.pi)
+        ra[np.isnan(ra)] = 0.0
         dec = np.arcsin(self.z / r_d3)
         return CoordSky(ra, dec)
 
     def distance(self, other: Coordinate) -> Dist3D:
         """Compute the Euclidean distance between two coordinate vectors.
 
         Coordinates are automatically converted before distance calculation.
@@ -335,30 +330,26 @@
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.values})"
 
     def __format__(self, __format_spec: str) -> str:
         return self.values.__format__(__format_spec)
 
-    def __eq__(self, other: object) -> ArrayLike[np.bool_]:
-        if isinstance(other, self.__class__):
-            return self.values == other.values
-        return NotImplemented
+    def __eq__(self, other: Distance) -> ArrayLike[np.bool_]:
+        return self.values == other.values
 
     def __lt__(self, other: Distance) -> ArrayLike[np.bool_]:
-        if isinstance(other, self.__class__):
-            return self.values < other.values
-        return NotImplemented
+        return self.values < other.values
 
     @abstractmethod
-    def __add__(self, other: object) -> _Tdist:
+    def __add__(self: _Tdist, other: _Tdist) -> _Tdist:
         pass
 
     @abstractmethod
-    def __sub__(self, other: object) -> _Tdist:
+    def __sub__(self: _Tdist, other: _Tdist) -> _Tdist:
         pass
 
     def min(self) -> _Tdist:
         """Compute the minimum value and return it as new `Distance`
         instance."""
         return self.__class__(self.values.min())
 
@@ -377,46 +368,38 @@
         """Convert the distance to an angular separation in radian."""
         pass
 
 
 class Dist3D(Distance):
     """Implements a vector of Euclidean distances."""
 
-    def __add__(self, other: object) -> DistSky:
-        if isinstance(other, Dist3D):
-            dist_sky = self.to_sky() + other.to_sky()
-            return dist_sky.to_3d()
-        return NotImplemented
-
-    def __sub__(self, other: object) -> DistSky:
-        if isinstance(other, Dist3D):
-            dist_sky = self.to_sky() - other.to_sky()
-            return dist_sky.to_3d()
-        return NotImplemented
+    def __add__(self, other: Dist3D) -> DistSky:
+        dist_sky = self.to_sky() + other.to_sky()
+        return dist_sky.to_3d()
+
+    def __sub__(self, other: Dist3D) -> DistSky:
+        dist_sky = self.to_sky() - other.to_sky()
+        return dist_sky.to_3d()
 
     def to_3d(self) -> Dist3D:
         return self
 
     def to_sky(self) -> DistSky:
         if np.any(self._values > 2.0):
             raise ValueError("distance exceeds size of unit sphere")
         return DistSky(2.0 * np.arcsin(self.values / 2.0))
 
 
 class DistSky(Distance):
     """Implements a vector of angular distances in radian."""
 
-    def __add__(self, other: object) -> DistSky:
-        if isinstance(other, DistSky):
-            return DistSky(self.values + other.values)
-        return NotImplemented
-
-    def __sub__(self, other: object) -> DistSky:
-        if isinstance(other, DistSky):
-            return DistSky(self.values - other.values)
-        return NotImplemented
+    def __add__(self, other: DistSky) -> DistSky:
+        return DistSky(self.values + other.values)
+
+    def __sub__(self, other: DistSky) -> DistSky:
+        return DistSky(self.values - other.values)
 
     def to_3d(self) -> Dist3D:
         return Dist3D(2.0 * np.sin(self.values / 2.0))
 
     def to_sky(self) -> DistSky:
         return self
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/core/cosmology.py` & `yet_another_wizz-2.5.post0/src/yaw/core/cosmology.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             z (Quantity-like ``redshift``, :obj:`NDArray`, or scalar number):
                 Input redshift.
 
         Returns:
             :obj:`astropy.units.Quantity`:
                 Comoving distance in Mpc to each input redshift.
         """
-        pass
+        NotImplemented
 
     @abstractmethod
     def comoving_transverse_distance(self, z: ArrayLike) -> ArrayLike:
         """Comoving transverse distance in Mpc at a given redshift.
 
         This value is the transverse comoving distance at redshift :math:`z`
         corresponding to an angular separation of 1 radian. This is the same as
@@ -71,15 +71,15 @@
             z (Quantity-like ``redshift``, :obj:`NDArray`, or scalar number):
                 Input redshift.
 
         Returns:
             :obj:`astropy.units.Quantity`:
                 Comoving transverse distance in Mpc at each input redshift.
         """
-        pass
+        NotImplemented
 
 
 TypeCosmology: TypeAlias = Union[FLRW, CustomCosmology]
 
 
 def r_kpc_to_angle(
     r_kpc: NDArray[np.float_] | Sequence[float], z: float, cosmology: TypeCosmology
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/core/docs.py` & `yet_another_wizz-2.5.post0/src/yaw/core/docs.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/core/math.c` & `yet_another_wizz-2.5.post0/src/yaw/core/math.c`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/core/math.py` & `yet_another_wizz-2.5.post0/src/yaw/core/math.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/core/utils.py` & `yet_another_wizz-2.5.post0/src/yaw/core/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/correlation/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/correlation/corrfuncs.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/corrfuncs.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import pandas as pd
 from deprecated import deprecated
 
 from yaw.catalogs import PatchLinkage
 from yaw.config import OPTIONS, ResamplingConfig
 from yaw.core.abc import BinnedQuantity, HDFSerializable, PatchedQuantity
 from yaw.core.containers import Indexer, SampledData
-from yaw.core.logging import TimedLog
+from yaw.core.logging import LogCustomWarning, TimedLog
 from yaw.core.utils import TypePathStr
 from yaw.core.utils import format_float_fixed_width as fmt_num
 from yaw.correlation.estimators import (
     CorrelationEstimator,
     CtsMix,
     EstimatorError,
     cts_from_code,
@@ -102,15 +102,18 @@
             by :func:`CorrData.to_files`.
     """
 
     info: str | None = None
     """Optional descriptive text for the contained data."""
 
     def __post_init__(self) -> None:
-        super().__post_init__()
+        with LogCustomWarning(
+            logger, "invalid values encountered in correlation samples"
+        ):
+            super().__post_init__()
 
     @classmethod
     def from_files(cls: Type[_Tdata], path_prefix: TypePathStr) -> _Tdata:
         """Create a new instance by loading the data from ASCII files.
 
         The data is restored from a set of three input files produced by
         :meth:`to_files`.
@@ -124,15 +127,15 @@
             path_prefix (:obj:`str`):
                 The base name of the input files without any file extension.
 
         Returns:
             :obj:`CorrData`
         """
         name = cls.__name__.lower()[:-4]
-        logger.debug("reading %s data from '%s.*'", name, path_prefix)
+        logger.debug(f"reading {name} data from '{path_prefix}.*'")
         # load data and errors
         ext = "dat"
         data_error = np.loadtxt(f"{path_prefix}.{ext}")
         # restore index
         binning = pd.IntervalIndex.from_arrays(data_error[:, 0], data_error[:, 1])
         # load samples
         ext = "smp"
@@ -208,15 +211,15 @@
         the :obj:`info` attribute.
 
         Args:
             path_prefix (:obj:`str`):
                 The base name of the output files without any file extension.
         """
         name = self.__class__.__name__.lower()[:-4]
-        logger.info("writing %s data to '%s.*'", name, path_prefix)
+        logger.info(f"writing {name} data to '{path_prefix}.*'")
         PREC = 10
         DELIM = " "
 
         def comment(string: str) -> str:
             if self.info is not None:
                 string = f"{string}\n# extra info: {self.info}"
             return string
@@ -302,15 +305,15 @@
         label: str | None = None,
         error_bars: bool = True,
         ax: Axis | None = None,
         xoffset: float = 0.0,
         plot_kwargs: dict[str, Any] | None = None,
         zero_line: bool = False,
         scale_by_dz: bool = False,
-    ) -> Axis:
+    ) -> Axis:  # pragma: no cover
         """Create a plot of the correlation data as a function of redshift.
 
         Create a new axis or plot to an existing one, add x-axis offsets, if
         plotting multiple instances, or specify if the values should be
         represented as points with errorbars (default) or as line plot with
         shaded area to represent uncertainties.
 
@@ -333,16 +336,16 @@
             zero_lilne (:obj:`bool`, optional):
                 Wether to draw a thin black line that indicates ``y=0``.
             scale_by_dz (:obj:`bool`, optional):
                 Whether to multiply the y-values by the redshift bin width
                 :obj:`dz`.
         """
         x = self.mids + xoffset
-        y = self.data.astype(np.float_)
-        yerr = self.error.astype(np.float_)
+        y = self.data
+        yerr = self.error
         if scale_by_dz:
             y *= self.dz
             yerr *= self.dz
         return self._make_plot(
             x,
             y,
             yerr,
@@ -489,73 +492,68 @@
         # check that the pair counts are compatible
         for kind in ("dr", "rd", "rr"):
             pairs: NormalisedCounts | None = getattr(self, kind)
             if pairs is None:
                 continue
             try:
                 self.dd.is_compatible(pairs, require=True)
-                assert self.dd.n_patches == pairs.n_patches
-            except (ValueError, AssertionError) as e:
+            except ValueError as e:
                 raise ValueError(
                     f"pair counts '{kind}' and 'dd' are not compatible"
                 ) from e
 
     def __repr__(self) -> str:
         string = super().__repr__()[:-1]
         pairs = f"dd=True, dr={self.dr is not None}, "
         pairs += f"rd={self.rd is not None}, rr={self.rr is not None}"
         other = f"n_patches={self.n_patches}"
         return f"{string}, {pairs}, {other})"
 
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, self.__class__):
-            for cfield in fields(self):
-                kind = cfield.name
-                if getattr(self, kind) != getattr(other, kind):
-                    return False
-            return True
-        return NotImplemented
-
-    def __add__(self, other: object) -> CorrFunc:
-        if isinstance(other, self.__class__):
-            # check that the pair counts are set consistently
-            kinds = []
-            for cfield in fields(self):
-                kind = cfield.name
-                self_set = getattr(self, kind) is not None
-                other_set = getattr(other, kind) is not None
-                if (self_set and not other_set) or (not self_set and other_set):
-                    raise ValueError(
-                        f"pair counts for '{kind}' not set for both operands"
-                    )
-                elif self_set and other_set:
-                    kinds.append(kind)
-
-            kwargs = {
-                kind: getattr(self, kind) + getattr(other, kind) for kind in kinds
-            }
-            return self.__class__(**kwargs)
-        return NotImplemented
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, self.__class__):
+            return False
+        for cfield in fields(self):
+            kind = cfield.name
+            if getattr(self, kind) != getattr(other, kind):
+                return False
+        return True
+
+    def __neq__(self, other) -> bool:
+        return not self == other
+
+    def __add__(self, other: CorrFunc) -> CorrFunc:
+        # check that the pair counts are set consistently
+        kinds = []
+        for cfield in fields(self):
+            kind = cfield.name
+            self_set = getattr(self, kind) is not None
+            other_set = getattr(other, kind) is not None
+            if (self_set and not other_set) or (not self_set and other_set):
+                raise ValueError(f"pair counts for '{kind}' not set for both operands")
+            elif self_set and other_set:
+                kinds.append(kind)
 
-    def __radd__(self, other: object) -> CorrFunc:
-        if np.isscalar(other) and other == 0:
+        kwargs = {kind: getattr(self, kind) + getattr(other, kind) for kind in kinds}
+        return self.__class__(**kwargs)
+
+    def __radd__(self, other: CorrFunc | int | float) -> CorrFunc:
+        if other == 0:
             return self
-        return other.__add__(self)
+        else:
+            return self.__add__(other)
 
-    def __mul__(self, other: object) -> CorrFunc:
-        if np.isscalar(other) and not isinstance(other, (bool, np.bool_)):
-            # check that the pair counts are set consistently
-            kwargs = {}
-            for cfield in fields(self):
-                kind = cfield.name
-                counts = getattr(self, kind)
-                if counts is not None:
-                    kwargs[kind] = counts * other
-            return self.__class__(**kwargs)
-        return NotImplemented
+    def __mul__(self, other: np.number) -> CorrFunc:
+        # check that the pair counts are set consistently
+        kwargs = {}
+        for cfield in fields(self):
+            kind = cfield.name
+            counts = getattr(self, kind)
+            if counts is not None:
+                kwargs[kind] = counts * other
+        return self.__class__(**kwargs)
 
     @property
     def auto(self) -> bool:
         """Whether the stored data are from an autocorrelation measurement."""
         return self.dd.auto
 
     @property
@@ -590,15 +588,15 @@
     def get_binning(self) -> IntervalIndex:
         return self.dd.get_binning()
 
     @property
     def n_patches(self) -> int:
         return self.dd.n_patches
 
-    def is_compatible(self, other: CorrFunc, require: bool = False) -> bool:
+    def is_compatible(self, other: CorrFunc, require: bool = True) -> bool:
         """Check whether this instance is compatible with another instance.
 
         Ensures that the redshift binning and the number of patches are
         identical.
 
         Args:
             other (:obj:`BinnedQuantity`):
@@ -624,25 +622,27 @@
             :obj:`dict`: Mapping from correlation estimator name abbreviation to
             correlation function class.
         """
         # figure out which of dd, dr, ... are not None
         available = set()
         # iterate all dataclass attributes that are in __init__
         for attr in fields(self):
+            if not attr.init:
+                continue
             if getattr(self, attr.name) is not None:
                 available.add(cts_from_code(attr.name))
         # check which estimators are supported
         estimators = {}
         for estimator in CorrelationEstimator.variants:  # registered estimators
             if set(estimator.requires) <= available:
                 estimators[estimator.short] = estimator
         return estimators
 
     def _check_and_select_estimator(
-        self, estimator: str | None = None
+        self, estimator: str | None
     ) -> type[CorrelationEstimator]:
         options = self.estimators
         if estimator is None:
             for shortname in ["LS", "DP", "PH"]:  # preferred hierarchy
                 if shortname in options:
                     estimator = shortname
                     break
@@ -654,21 +654,25 @@
                 )
                 est_class = CorrelationEstimator.variants[index]
             except ValueError as e:
                 raise ValueError(f"invalid estimator '{estimator}'") from e
             # determine which pair counts are missing
             for attr in fields(self):
                 name = attr.name
+                if not attr.init:
+                    continue
                 cts = cts_from_code(name)
                 if getattr(self, name) is None and cts in est_class.requires:
                     raise EstimatorError(f"estimator requires {name}")
+            else:
+                raise RuntimeError()
         # select the correct estimator
         cls = options[estimator]
         logger.debug(
-            "selecting estimator '%s' from %s", cls.short, "/".join(self.estimators)
+            f"selecting estimator '{cls.short}' from {'/'.join(self.estimators)}"
         )
         return cls
 
     def _getattr_from_cts(self, cts: Cts) -> NormalisedCounts | None:
         if isinstance(cts, CtsMix):
             for code in str(cts).split("_"):
                 value = getattr(self, code)
@@ -680,15 +684,15 @@
 
     @deprecated(reason="renamed to CorrFunc.sample", version="2.3.1")
     def get(self, *args, **kwargs):
         """
         .. deprecated:: 2.3.1
             Renamed to :meth:`sample`.
         """
-        return self.sample(*args, **kwargs)  # pragma: no cover
+        return self.sample(*args, **kwargs)
 
     def sample(
         self,
         config: ResamplingConfig | None = None,
         *,
         estimator: str | None = None,
         info: str | None = None,
@@ -713,15 +717,15 @@
             :obj:`CorrData`:
                 Correlation function data, including redshift binning, function
                 values and samples.
         """
         if config is None:
             config = ResamplingConfig()
         est_fun = self._check_and_select_estimator(estimator)
-        logger.debug("computing correlation and %s samples", config.method)
+        logger.debug(f"computing correlation and {config.method} samples")
         # get the pair counts for the required terms (DD, maybe DR and/or RR)
         required_data = {}
         required_samples = {}
         for cts in est_fun.requires:
             try:  # if pairs are None, estimator with throw error
                 pairs = self._getattr_from_cts(cts).sample(config)
                 required_data[str(cts)] = pairs.data
@@ -774,20 +778,20 @@
             if data is not None:
                 group = dest.create_group(name)
                 data.to_hdf(group)
         dest.create_dataset("n_patches", data=self.n_patches)
 
     @classmethod
     def from_file(cls, path: TypePathStr) -> CorrFunc:
-        logger.debug("reading pair counts from '%s'", path)
+        logger.debug(f"reading pair counts from '{path}'")
         with h5py.File(str(path)) as f:
             return cls.from_hdf(f)
 
     def to_file(self, path: TypePathStr) -> None:
-        logger.info("writing pair counts to '%s'", path)
+        logger.info(f"writing pair counts to '{path}'")
         with h5py.File(str(path), mode="w") as f:
             self.to_hdf(f)
 
     def concatenate_patches(self, *cfs: CorrFunc) -> CorrFunc:
         check_mergable([self, *cfs])
         merged = {}
         for kind in ("dd", "dr", "rd", "rr"):
@@ -923,18 +927,16 @@
             containers if multiple scales are configured. Dictionary keys have a
             ``kpcXXtXX`` pattern, where ``XX`` are the lower and upper scale
             limit as integers, in kpc (see :obj:`yaw.core.cosmology.Scale`).
     """
     _check_patch_centers([data, random])
     scales = config.scales.as_array()
     logger.info(
-        "running autocorrelation (%i scales, %.0f<r<=%.0fkpc)",
-        len(scales),
-        scales.min(),
-        scales.max(),
+        f"running autocorrelation ({len(scales)} scales, "
+        f"{scales.min():.0f}<r<={scales.max():.0f}kpc)"
     )
     if linkage is None:
         linkage = PatchLinkage.from_setup(config, random)
     kwargs = dict(linkage=linkage, progress=progress)
     logger.debug("scheduling DD, DR" + (", RR" if compute_rr else ""))
     with TimedLog(logger.info, "counting data-data pairs"):
         DD = data.correlate(config, binned=True, **kwargs)
@@ -1020,18 +1022,16 @@
         all_cats.append(unk_rand)
     if compute_rd:
         all_cats.append(ref_rand)
     _check_patch_centers(all_cats)
 
     scales = config.scales.as_array()
     logger.info(
-        "running crosscorrelation (%i scales, %.0f<r<=%.0fkpc)",
-        len(scales),
-        scales.min(),
-        scales.max(),
+        f"running crosscorrelation ({len(scales)} scales, "
+        f"{scales.min():.0f}<r<={scales.max():.0f}kpc)"
     )
     if linkage is None:
         linkage = PatchLinkage.from_setup(config, unknown)
     logger.debug(
         "scheduling DD"
         + (", DR" if compute_dr else "")
         + (", RD" if compute_rd else "")
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/correlation/estimators.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 True
 >>> CtsMix() == CtsRD()
 True
 """
 
 from __future__ import annotations
 
-import warnings
-from abc import ABC, abstractmethod
+import logging
+from abc import ABC, abstractclassmethod, abstractproperty
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
@@ -36,50 +36,51 @@
     "PeeblesHauser",
     "DavisPeebles",
     "Hamilton",
     "LandySzalay",
 ]
 
 
+logger = logging.getLogger(__name__)
+
+
 class EstimatorError(Exception):
     pass
 
 
 class Cts(ABC):
     """Base class to symbolically represent pair counts."""
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def _hash(self) -> int:
         """Used for comparison.
 
         Equivalent pair counts types should have the same hash value, see
         :obj:`CtsMix`."""
         pass
 
-    @property
-    @abstractmethod
+    @abstractproperty
     def _str(self) -> str:
         pass
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}>"
 
     def __str__(self) -> str:
         return self._str
 
     def __hash__(self) -> int:
         return self._hash
 
     def __eq__(self, other: object) -> bool:
-        if isinstance(other, Cts):
-            var1 = set(self._str.split("_"))
-            var2 = set(other._str.split("_"))
-            return not var1.isdisjoint(var2)
-        return NotImplemented
+        if not isinstance(other, Cts):
+            return False
+        var1 = set(self._str.split("_"))
+        var2 = set(other._str.split("_"))
+        return not var1.isdisjoint(var2)
 
 
 class CtsDD(Cts):
     """Symbolic representation of data-data paircounts."""
 
     _str = "dd"
     _hash = 1
@@ -154,26 +155,25 @@
         super().__init_subclass__(**kwargs)
         cls.variants.append(cls)
 
     @classmethod
     def _warn_enum_zero(cls, counts: NDArray):
         """Raise a warning if any value in the expression enumerator is zero"""
         if np.any(counts == 0.0):
-            warnings.warn(f"estimator {cls.short} encontered zeros in enumerator")
+            logger.warn(f"estimator {cls.short} encontered zeros in enumerator")
 
-    @classmethod
-    @abstractmethod
+    @abstractclassmethod
     def eval(
         cls, *, dd: NDArray, dr: NDArray, rr: NDArray, rd: NDArray | None = None
     ) -> NDArray:
         """Method that implements the estimator.
 
         Should call :meth:`_warn_enum_zero` to raise warnings on zero-division.
         """
-        pass
+        NotImplemented
 
 
 class PeeblesHauser(CorrelationEstimator):
     """Implementation of the Peebles-Hauser correlation estimator
     :math:`\\frac{DD}{RR} - 1`.
     """
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/correlation/paircounts.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/paircounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 both a :obj:`PatchedCount` and :obj:`PatchedTotal` container. Its
 :meth:`NormalisedCounts.sample` method computes the ratio of
 counts-to-total-objects and samples thereof.
 """
 
 from __future__ import annotations
 
+import logging
 from abc import abstractmethod
 from collections.abc import Iterable, Sequence
 from dataclasses import dataclass
 from itertools import accumulate
-from typing import TYPE_CHECKING, NoReturn, Type, Union
+from typing import TYPE_CHECKING, NoReturn, Union
 
 try:  # pragma: no cover
     from typing import TypeAlias
 except ImportError:  # pragma: no cover
     from typing_extensions import TypeAlias
 
 import h5py
@@ -33,36 +34,34 @@
 from yaw.core.abc import (
     BinnedQuantity,
     HDFSerializable,
     PatchedQuantity,
     concatenate_bin_edges,
 )
 from yaw.core.containers import Indexer, PatchIDs, SampledData
+from yaw.core.logging import LogCustomWarning
 from yaw.core.math import apply_slice_ndim, outer_triu_sum
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import DTypeLike, NDArray
     from pandas import IntervalIndex
 
 __all__ = ["PatchedTotal", "PatchedCount", "NormalisedCounts"]
 
+
+logger = logging.getLogger(__name__)
+
 _compression = dict(fletcher32=True, compression="gzip", shuffle=True)
 """default compression settings for :obj:`h5py.Dataset`."""
 
 
 TypeSlice: TypeAlias = Union[slice, int, None]
 TypeIndex: TypeAlias = Union[int, slice, Sequence]
 
 
-def sequence_require_type(items: Sequence, class_or_inst: Type | object) -> None:
-    for item in items:
-        if not isinstance(item, class_or_inst):
-            raise TypeError(f"invalid type '{type(item)}' for concatenation")
-
-
 def check_mergable(patched_arrays: Sequence[PatchedArray], *, patches: bool) -> None:
     """Check if two instaces of PatchedArray can be merged along the patch
     or binning axis.
 
     Args:
         patched_arrays (:obj:`Sequence[PatchedArray]`):
             Instances to merge
@@ -73,16 +72,19 @@
     """
     reference = patched_arrays[0]
     for patched in patched_arrays[1:]:
         if reference.auto != patched.auto:
             raise ValueError("cannot merge mixed cross- and autocorrelations")
         if patches:
             reference.is_compatible(patched, require=True)
-        elif reference.n_patches != patched.n_patches:
-            raise ValueError("cannot merge, patch numbers do not match")
+        else:
+            if reference.auto != patched.auto:
+                raise ValueError("cannot merge mixed cross- and autocorrelations")
+            if reference.n_patches != patched.n_patches:
+                raise ValueError("cannot merge, patch numbers do not match")
 
 
 def binning_from_hdf(source: h5py.Group) -> IntervalIndex:
     """Construct a :obj:`pandas.IntervalIndex` from a group in an HDF5 file."""
     dset = source["binning"]
     left, right = dset[:].T
     closed = dset.attrs["closed"]
@@ -121,16 +123,26 @@
 
     def __repr__(self) -> str:
         string = super().__repr__()[:-1]
         shape = self.shape
         return f"{string}, {shape=})"
 
     @abstractmethod
-    def __eq__(self, other: object) -> bool:
-        pass
+    def __eq__(self, other) -> bool:
+        if isinstance(other, self.__class__):
+            if self.n_bins != other.n_bins:
+                return False
+            elif self.n_patches != other.n_patches:
+                return False
+            elif not (self.get_binning() == other.get_binning()).all():
+                return False
+        return True
+
+    def __neq__(self, other) -> bool:
+        return not self == other
 
     @property
     def dtype(self) -> DTypeLike:
         """The numpy data type of the underlying data."""
         return np.float_
 
     @property
@@ -150,47 +162,47 @@
 
     @abstractmethod
     def as_array(self) -> NDArray:
         """Get the underlying data as contiguous array.
 
         The array 3-dimensional with shape (N, N, K), where N is the number of
         spatial patches, and K is the number of redshift bins."""
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def _sum(self, config: ResamplingConfig) -> NDArray:
         """Method that implements the sum over all patches."""
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def _jackknife(self, config: ResamplingConfig, signal: NDArray) -> NDArray:
         """Method that implements generating jackknife samples of the sum over
         all patches.
 
         For N patches, draw N realisations by leaving out one of the N patches.
         """
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def _bootstrap(self, config: ResamplingConfig) -> NDArray:
         """Method that implements generating bootstrap samples of the sum over
         all patches.
 
         For N patches, draw M realisations each containing N randomly chosen
         patches.
         """
-        pass
+        raise NotImplementedError
 
     @deprecated(reason="renamed to CorrFunc.sample_sum", version="2.3.1")
     def get_sum(self, *args, **kwargs):
         """
         .. deprecated:: 2.3.1
             Renamed to :meth:`sample_sum`.
         """
-        return self.sample_sum(*args, **kwargs)  # pragma: no cover
+        return self.sample_sum(*args, **kwargs)
 
     def sample_sum(self, config: ResamplingConfig | None = None) -> SampledData:
         """Compute the sum of the data over all patches and samples thereof.
 
         Returns a data container with the sum in each redshift bin and samples
         generated from the patches using the resampling method specified in the
         configuration parameter.
@@ -317,25 +329,22 @@
                 f"number of patches and bins do not match: "
                 f"{totals1.shape} != {totals2.shape}"
             )
         self.totals1 = totals1
         self.totals2 = totals2
         self.auto = auto
 
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, self.__class__):
-            return (
-                self.n_bins == other.n_bins
-                and self.n_patches == other.n_patches
-                and (self.get_binning() == other.get_binning()).all()
-                and np.all(self.totals1 == other.totals1)
-                and np.all(self.totals2 == other.totals2)
-                and self.auto == other.auto
-            )
-        return NotImplemented
+    def __eq__(self, other) -> bool:
+        if not super().__eq__(other):
+            return False  # checks type
+        return (
+            np.all(self.totals1 == other.totals1)
+            and np.all(self.totals2 == other.totals2)
+            and self.auto == other.auto
+        )
 
     def as_array(self) -> NDArray:
         return np.einsum("i...,j...->ij...", self.totals1, self.totals2)
 
     @property
     def bins(self) -> Indexer[TypeIndex, PatchedTotal]:
         def builder(inst: PatchedTotal, item: TypeIndex) -> PatchedTotal:
@@ -386,26 +395,24 @@
         binning_to_hdf(self.get_binning(), dest)
         # store the data
         dest.create_dataset("totals1", data=self.totals1, **_compression)
         dest.create_dataset("totals2", data=self.totals2, **_compression)
         dest.create_dataset("auto", data=self.auto)
 
     def concatenate_patches(self, *data: PatchedTotal) -> PatchedTotal:
-        sequence_require_type(data, self.__class__)
         all_totals: list[PatchedTotal] = [self, *data]
         check_mergable(all_totals, patches=True)
         return self.__class__(
             binning=self.get_binning().copy(),
             totals1=np.concatenate([t.totals1 for t in all_totals], axis=0),
             totals2=np.concatenate([t.totals2 for t in all_totals], axis=0),
             auto=self.auto,
         )
 
     def concatenate_bins(self, *data: PatchedTotal) -> PatchedTotal:
-        sequence_require_type(data, self.__class__)
         all_totals: list[PatchedTotal] = [self, *data]
         check_mergable(all_totals, patches=False)
         binning = concatenate_bin_edges(*all_totals)
         return self.__class__(
             binning=binning,
             totals1=np.concatenate([t.totals1 for t in all_totals], axis=1),
             totals2=np.concatenate([t.totals2 for t in all_totals], axis=1),
@@ -634,46 +641,35 @@
             dtype (:obj:`DTypeLike`, optional):
                 Data type to use for the internal data array.
 
         """
         counts = np.zeros((n_patches, n_patches, len(binning)), dtype=dtype)
         return cls(binning, counts, auto=auto)
 
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, self.__class__):
-            return (
-                self.n_bins == other.n_bins
-                and self.n_patches == other.n_patches
-                and (self.get_binning() == other.get_binning()).all()
-                and np.all(self.counts == other.counts)
-                and (self.auto == other.auto)
-            )
-        return NotImplemented
-
-    def __add__(self, other: object) -> PatchedCount:
-        if isinstance(other, self.__class__):
-            self.is_compatible(other, require=True)
-            if self.n_patches != other.n_patches:
-                raise ValueError("number of patches does not agree")
-            return self.__class__(
-                self.get_binning(), self.counts + other.counts, auto=self.auto
-            )
-        return NotImplemented
+    def __eq__(self, other) -> bool:
+        if not super().__eq__(other):
+            return False  # checks type
+        return np.all(self.counts == other.counts) and (self.auto == other.auto)
+
+    def __add__(self, other: PatchedCount) -> PatchedCount:
+        self.is_compatible(other, require=True)
+        if self.n_patches != other.n_patches:
+            raise ValueError("number of patches does not agree")
+        return self.__class__(
+            self.get_binning(), self.counts + other.counts, auto=self.auto
+        )
 
-    def __radd__(self, other: object) -> PatchedCount:
-        if np.isscalar(other) and other == 0:
+    def __radd__(self, other: PatchedCount | int | float) -> PatchedCount:
+        if other == 0:
             return self
-        return other.__add__(self)
+        else:
+            return self.__add__(other)
 
-    def __mul__(self, other: object) -> PatchedCount:
-        if np.isscalar(other) and not isinstance(other, (bool, np.bool_)):
-            return self.__class__(
-                self.get_binning(), self.counts * other, auto=self.auto
-            )
-        return NotImplemented
+    def __mul__(self, other: np.number) -> PatchedCount:
+        return self.__class__(self.get_binning(), self.counts * other, auto=self.auto)
 
     def set_measurement(self, key: PatchIDs | tuple[int, int], item: NDArray):
         """Set the counts value in all redshift bins for a pair of patch
         indices.
 
         Args:
             key (:obj:`yaw.core.containers.PatchIDs`, tuple):
@@ -788,35 +784,30 @@
         # store the data
         dest.create_dataset("keys", data=self.keys(), **_compression)
         dest.create_dataset("data", data=self.values(), **_compression)
         dest.create_dataset("n_patches", data=self.n_patches)
         dest.create_dataset("auto", data=self.auto)
 
     def concatenate_patches(self, *data: PatchedCount) -> PatchedCount:
-        sequence_require_type(data, self.__class__)
         all_counts: list[PatchedCount] = [self, *data]
         check_mergable(all_counts, patches=True)
         offsets = patch_idx_offset(all_counts)
-        n_patches = [count.n_patches for count in all_counts]
         merged = self.__class__.zeros(
             binning=self.get_binning(),
-            n_patches=sum(n_patches),
+            n_patches=sum(count.n_patches for count in all_counts),
             auto=self.auto,
         )
         # insert the blocks of counts into the merged counts array
         loc = 0
-        for count, offset, n in zip(all_counts, offsets, n_patches):
-            i_start = offset
-            i_end = i_start + n
-            merged.counts[i_start:i_end, i_start:i_end] = count.counts
+        for count, offset in zip(all_counts, offsets):
+            merged.counts[loc : loc + offset, loc : loc + offset] = count.counts
             loc += offset
         return merged
 
     def concatenate_bins(self, *data: PatchedCount) -> PatchedCount:
-        sequence_require_type(data, self.__class__)
         all_counts: list[PatchedCount] = [self, *data]
         check_mergable(all_counts, patches=False)
         binning = concatenate_bin_edges(*all_counts)
         merged = self.__class__.zeros(
             binning=binning, n_patches=self.n_patches, auto=self.auto, dtype=self.dtype
         )
         merged.counts = np.concatenate([count.counts for count in all_counts], axis=2)
@@ -962,38 +953,41 @@
             raise ValueError("number of bins of 'count' and total' do not match")
 
     def __repr__(self) -> str:
         string = super().__repr__()[:-1]
         n_patches = self.n_patches
         return f"{string}, {n_patches=})"
 
-    def __eq__(self, other: object) -> bool:
+    def __eq__(self, other) -> bool:
         if isinstance(other, self.__class__):
-            return self.count == other.count and self.total == other.total
-        return NotImplemented
+            return np.all(self.count == other.count) and np.all(
+                self.total == other.total
+            )
+        else:
+            return False
 
-    def __add__(self, other: object) -> NormalisedCounts:
-        if isinstance(other, self.__class__):
-            count = self.count + other.count
-            if np.any(self.total.totals1 != other.total.totals1) or np.any(
-                self.total.totals2 != other.total.totals2
-            ):
-                raise ValueError("total number of objects do not agree for operands")
-            return self.__class__(count, self.total)
-        return NotImplemented
+    def __neq__(self, other) -> bool:
+        return not self == other
 
-    def __radd__(self, other: object) -> NormalisedCounts:
-        if np.isscalar(other) and other == 0:
+    def __add__(self, other: NormalisedCounts) -> NormalisedCounts:
+        count = self.count + other.count
+        if np.any(self.total.totals1 != other.total.totals1) or np.any(
+            self.total.totals2 != other.total.totals2
+        ):
+            raise ValueError("total number of objects do not agree for operands")
+        return self.__class__(count, self.total)
+
+    def __radd__(self, other: NormalisedCounts | int | float) -> NormalisedCounts:
+        if other == 0:
             return self
-        return other.__add__(self)
+        else:
+            return self.__add__(other)
 
-    def __mul__(self, other: object) -> NormalisedCounts:
-        if np.isscalar(other) and not isinstance(other, (bool, np.bool_)):
-            return self.__class__(self.count * other, self.total)
-        return NotImplemented
+    def __mul__(self, other: np.number) -> NormalisedCounts:
+        return self.__class__(self.count * other, self.total)
 
     @property
     def auto(self) -> bool:
         """Whether the stored data are from an autocorrelation measurement."""
         return self.count.auto
 
     @property
@@ -1040,20 +1034,23 @@
                 parameters.
 
         Returns:
             :obj:`~yaw.core.SampledData`
         """
         counts = self.count.sample_sum(config)
         totals = self.total.sample_sum(config)
-        samples = SampledData(
-            binning=self.get_binning(),
-            data=(counts.data / totals.data),
-            samples=(counts.samples / totals.samples),
-            method=config.method,
-        )
+        with LogCustomWarning(
+            logger, "some patches contain no data after binning by redshift"
+        ):
+            samples = SampledData(
+                binning=self.get_binning(),
+                data=(counts.data / totals.data),
+                samples=(counts.samples / totals.samples),
+                method=config.method,
+            )
         return samples
 
     @classmethod
     def from_hdf(cls, source: h5py.Group) -> NormalisedCounts:
         count = PatchedCount.from_hdf(source["count"])
         total = PatchedTotal.from_hdf(source["total"])
         return cls(count=count, total=total)
@@ -1061,24 +1058,22 @@
     def to_hdf(self, dest: h5py.Group) -> None:
         group = dest.create_group("count")
         self.count.to_hdf(group)
         group = dest.create_group("total")
         self.total.to_hdf(group)
 
     def concatenate_patches(self, *pcounts: NormalisedCounts) -> NormalisedCounts:
-        sequence_require_type(pcounts, self.__class__)
         counts = [pc.count for pc in pcounts]
         totals = [pc.total for pc in pcounts]
         return self.__class__(
             count=self.count.concatenate_patches(*counts),
             total=self.total.concatenate_patches(*totals),
         )
 
     def concatenate_bins(self, *pcounts: NormalisedCounts) -> NormalisedCounts:
-        sequence_require_type(pcounts, self.__class__)
         counts = [pc.count for pc in pcounts]
         totals = [pc.total for pc in pcounts]
         return self.__class__(
             count=self.count.concatenate_bins(*counts),
             total=self.total.concatenate_bins(*totals),
         )
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/deprecated/correlation/corrfuncs.py` & `yet_another_wizz-2.5.post0/src/yaw/deprecated.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 from deprecated import deprecated
 
 from yaw.correlation import CorrData, CorrFunc
+from yaw.correlation.paircounts import NormalisedCounts
+from yaw.redshifts import HistData
 
-__all__ = ["CorrelationData", "CorrelationFunction"]
+__all__ = ["CorrelationData", "CorrelationFunction", "HistogramData", "PairCountResult"]
 
 
 @deprecated(reason="renamed to yaw.CorrData", action="module", version="2.3.2")
 class CorrelationData(CorrData):
     """
     .. deprecated:: 2.3.2
         Renamed to :meth:`yaw.CorrData`.
@@ -21,7 +23,31 @@
 class CorrelationFunction(CorrFunc):
     """
     .. deprecated:: 2.3.2
         Renamed to :meth:`yaw.CorrFunc`.
     """
 
     pass
+
+
+@deprecated(reason="renamed to yaw.HistData", action="module", version="2.3.2")
+class HistogramData(HistData):
+    """
+    .. deprecated:: 2.3.2
+        Renamed to :meth:`yaw.HistData`.
+    """
+
+    pass
+
+
+@deprecated(
+    reason="renamed to yaw.correlation.paircounts.NormalisedCounts",
+    action="module",
+    version="2.3.2",
+)
+class PairCountResult(NormalisedCounts):
+    """
+    .. deprecated:: 2.3.2
+        Renamed to :obj:`yaw.correlation.paircounts.NormalisedCounts`.
+    """
+
+    pass
```

### Comparing `yet_another_wizz-2.5.7/src/yaw/examples/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/examples/auto_reference.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/auto_reference.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/examples/auto_unknown_1.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/auto_unknown_1.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/examples/cross_1.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/cross_1.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.7/src/yaw/randoms.py` & `yet_another_wizz-2.5.post0/src/yaw/randoms.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 
 from yaw.core.logging import TimedLog
+from yaw.core.parallel import POOL_SHARE, ParallelHelper, SharedArray
 from yaw.core.utils import long_num_format
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
     from pandas import DataFrame
 
     from yaw.catalogs import BaseCatalog
@@ -159,40 +160,85 @@
                     version.
 
         Returns:
             :obj:`pandas.DataFrame`:
                 Data frame with uniform random coordinates and optionally
                 additional features draw from input data.
         """
-        if n_threads != 1:
-            DeprecationWarning("'n_threads' is deprecated")
-        seed = self.rng.spawn(1)[0]  # backwards compatibility
+        # seeds for threads
+        if size <= 100 * n_threads:  # there is some kind of floor
+            n_threads = 1
+        seeds = self.rng.spawn(n_threads)
+        # distribute load
+        idx_break = np.linspace(0, size, n_threads + 1).astype(np.int_)
+        start = idx_break[:-1]
+        end = idx_break[1:]
+
+        # create output arrays
+        shares = dict(
+            ra=SharedArray.empty((size,), "f8"), dec=SharedArray.empty((size,), "f8")
+        )
+        if draw_from is not None:
+            shares["in"] = {
+                key: SharedArray.from_numpy(array) for key, array in draw_from.items()
+            }
+            shares["out"] = {
+                key: SharedArray.empty((size,), array.dtype)
+                for key, array in draw_from.items()
+            }
+        if names is None:
+            names = ["ra", "dec"]
+
+        # process
         msg = f"generate ({long_num_format(size)} uniform randoms)"
         with TimedLog(logger.info, msg):
-            # build the output dataframe
-            columns = ["ra", "dec"] if names is None else names
-            if draw_from is not None:
-                columns.extend(draw_from.keys())
-            rand = pd.DataFrame(
-                columns=["ra", "dec"] if names is None else names,
-                index=pd.RangeIndex(0, size),
-            )
-            # generate the positions
-            rng = np.random.default_rng(seed)
-            x = rng.uniform(self.x_min, self.x_max, size)
-            y = rng.uniform(self.y_min, self.y_max, size)
-            ra_dec = UniformRandoms.cylinder2sky(x, y)
-            rand["ra"] = ra_dec[:, 0]
-            rand["dec"] = ra_dec[:, 1]
-            # draw extra data
-            if draw_from is not None:
-                N = len(next(iter(draw_from.values())))
-                draw_idx = rng.integers(0, N, size=size)
-                for key, values in draw_from.items():
-                    if not isinstance(values, np.ndarray):
-                        raise TypeError(f"expected a numpy array for property '{key}")
-                    if len(values) != N:
-                        raise ValueError(
-                            f"expected a {N} values to draw from for property '{key}'"
-                        )
-                    rand[key] = values[draw_idx]
+            with ParallelHelper(_generate_uniform_randoms, n_threads) as pool:
+                pool.shares = shares  # assign in bulk
+                pool.add_constant(self)
+                pool.add_iterable(seeds)
+                pool.add_iterable(start)
+                pool.add_iterable(end)
+                pool.result()  # output direclty pasted into shared arrays
+                # convert to dataframe
+                rand = pd.DataFrame(
+                    {
+                        names[0]: pool.shares["ra"].to_numpy(copy=True),
+                        names[1]: pool.shares["dec"].to_numpy(copy=True),
+                    }
+                )
+                if draw_from is not None:
+                    for col, data in pool.shares["out"].items():
+                        rand[col] = data.to_numpy(copy=True)
+                # will delete shared arrays after this
         return rand
+
+
+def _generate_uniform_randoms(
+    inst: UniformRandoms, seed: np.random.SeedSequence, start: int, end: int
+) -> int:
+    rng = np.random.default_rng(seed)
+    size = end - start
+    ra = POOL_SHARE["ra"].to_numpy()
+    dec = POOL_SHARE["dec"].to_numpy()
+    # generate positions
+    x = rng.uniform(inst.x_min, inst.x_max, size)
+    y = rng.uniform(inst.y_min, inst.y_max, size)
+    ra_dec = UniformRandoms.cylinder2sky(x, y)
+    ra[start:end] = ra_dec[:, 0]
+    dec[start:end] = ra_dec[:, 1]
+    # generate random draw
+    if "in" in POOL_SHARE:
+        N = None
+        for col, data in POOL_SHARE["in"].items():
+            if N is None:
+                if len(data.shape) > 1:
+                    raise ValueError("data to draw from must be 1-dimensional")
+                N = len(data)
+            else:
+                if len(data) != N:
+                    raise ValueError("length of columns to draw from does not match")
+        draw_idx = rng.integers(0, N, size=size)
+        # draw and insert data
+        for col, data in POOL_SHARE["in"].items():
+            rand = POOL_SHARE["out"][col].to_numpy()
+            rand[start:end] = data.to_numpy()[draw_idx]
+    return size
```

