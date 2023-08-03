# Comparing `tmp/dask-image-2023.3.0.tar.gz` & `tmp/dask-image-2023.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-image-2023.3.0.tar", last modified: Mon Mar 27 05:17:44 2023, max compression
+gzip compressed data, was "dask-image-2023.3.0rc1.tar", last modified: Mon Mar 27 04:07:44 2023, max compression
```

## Comparing `dask-image-2023.3.0.tar` & `dask-image-2023.3.0rc1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.972236 dask-image-2023.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-27 05:17:30.000000 dask-image-2023.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-03-27 05:17:30.000000 dask-image-2023.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-03-27 05:17:30.000000 dask-image-2023.3.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-27 05:17:30.000000 dask-image-2023.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-27 05:17:30.000000 dask-image-2023.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-03-27 05:17:44.972236 dask-image-2023.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-27 05:17:30.000000 dask-image-2023.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.976236 dask-image-2023.3.0/dask_image/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-27 05:17:44.976236 dask-image-2023.3.0/dask_image/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.960235 dask-image-2023.3.0/dask_image/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/dispatch/_dispatch_ndfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/dispatch/_dispatch_ndinterp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/dispatch/_dispatch_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/dispatch/_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/dispatch/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.960235 dask-image-2023.3.0/dask_image/imread/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/imread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.964236 dask-image-2023.3.0/dask_image/ndfilters/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfilters/_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfilters/_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfilters/_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfilters/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfilters/_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfilters/_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfilters/_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfilters/_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfilters/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.964236 dask-image-2023.3.0/dask_image/ndfourier/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndfourier/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.964236 dask-image-2023.3.0/dask_image/ndinterp/
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndinterp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.964236 dask-image-2023.3.0/dask_image/ndmeasure/
--rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndmeasure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.964236 dask-image-2023.3.0/dask_image/ndmeasure/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndmeasure/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndmeasure/_utils/_find_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndmeasure/_utils/_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.968236 dask-image-2023.3.0/dask_image/ndmorph/
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndmorph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndmorph/_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-27 05:17:30.000000 dask-image-2023.3.0/dask_image/ndmorph/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.960235 dask-image-2023.3.0/dask_image.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-03-27 05:17:44.000000 dask-image-2023.3.0/dask_image.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-27 05:17:44.000000 dask-image-2023.3.0/dask_image.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 05:17:44.000000 dask-image-2023.3.0/dask_image.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 05:17:44.000000 dask-image-2023.3.0/dask_image.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-27 05:17:44.000000 dask-image-2023.3.0/dask_image.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 05:17:44.000000 dask-image-2023.3.0/dask_image.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.968236 dask-image-2023.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9202 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/coverage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.968236 dask-image-2023.3.0/docs/release/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-03-27 05:17:30.000000 dask-image-2023.3.0/docs/release/release_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-27 05:17:44.972236 dask-image-2023.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-27 05:17:30.000000 dask-image-2023.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.968236 dask-image-2023.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.952235 dask-image-2023.3.0/tests/test_dask_image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.972236 dask-image-2023.3.0/tests/test_dask_image/test_imread/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_imread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_imread/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_imread/test_cupy_imread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.972236 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.972236 dask-image-2023.3.0/tests/test_dask_image/test_ndfourier/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfourier/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndfourier/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.972236 dask-image-2023.3.0/tests/test_dask_image/test_ndinterp/
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndinterp/test_affine_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndinterp/test_spline_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.972236 dask-image-2023.3.0/tests/test_dask_image/test_ndmeasure/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndmeasure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndmeasure/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndmeasure/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndmeasure/test_find_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:17:44.972236 dask-image-2023.3.0/tests/test_dask_image/test_ndmorph/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndmorph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndmorph/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-03-27 05:17:30.000000 dask-image-2023.3.0/tests/test_dask_image/test_ndmorph/test_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (123)    68567 2023-03-27 05:17:30.000000 dask-image-2023.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20073 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/dask_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/dask_image/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndfilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndinterp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndmorph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/imread/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/imread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndfilters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndfourier/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfourier/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndinterp/
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndinterp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndmeasure/
+-rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmeasure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/_find_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndmorph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmorph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmorph/_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmorph/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20073 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9202 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/coverage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/docs/release/
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/release/release_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.787502 dask-image-2023.3.0rc1/tests/test_dask_image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/test_cupy_imread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfourier/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfourier/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfourier/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndinterp/
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndinterp/test_affine_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndinterp/test_spline_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test_find_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test_ndmorph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68567 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/versioneer.py
```

### Comparing `dask-image-2023.3.0/CONTRIBUTING.rst` & `dask-image-2023.3.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/HISTORY.rst` & `dask-image-2023.3.0rc1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/LICENSE.txt` & `dask-image-2023.3.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/PKG-INFO` & `dask-image-2023.3.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-image
-Version: 2023.3.0
+Version: 2023.3.0rc1
 Summary: Distributed image processing
 Home-page: https://github.com/dask/dask-image
 Author: dask-image contributors
 License: BSD 3-Clause
 Keywords: dask-image
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-image-2023.3.0/README.rst` & `dask-image-2023.3.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/dispatch/_dispatch_ndfilters.py` & `dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndfilters.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/dispatch/_dispatch_ndinterp.py` & `dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndinterp.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/dispatch/_dispatch_ndmorph.py` & `dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndmorph.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/dispatch/_dispatcher.py` & `dask-image-2023.3.0rc1/dask_image/dispatch/_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/dispatch/_utils.py` & `dask-image-2023.3.0rc1/dask_image/dispatch/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/imread/__init__.py` & `dask-image-2023.3.0rc1/dask_image/imread/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfilters/__init__.py` & `dask-image-2023.3.0rc1/dask_image/ndfilters/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfilters/_conv.py` & `dask-image-2023.3.0rc1/dask_image/ndfilters/_conv.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfilters/_edge.py` & `dask-image-2023.3.0rc1/dask_image/ndfilters/_edge.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfilters/_gaussian.py` & `dask-image-2023.3.0rc1/dask_image/ndfilters/_gaussian.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfilters/_generic.py` & `dask-image-2023.3.0rc1/dask_image/ndfilters/_generic.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfilters/_order.py` & `dask-image-2023.3.0rc1/dask_image/ndfilters/_order.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfilters/_smooth.py` & `dask-image-2023.3.0rc1/dask_image/ndfilters/_smooth.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfilters/_threshold.py` & `dask-image-2023.3.0rc1/dask_image/ndfilters/_threshold.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfilters/_utils.py` & `dask-image-2023.3.0rc1/dask_image/ndfilters/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfourier/__init__.py` & `dask-image-2023.3.0rc1/dask_image/ndfourier/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndfourier/_utils.py` & `dask-image-2023.3.0rc1/dask_image/ndfourier/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndinterp/__init__.py` & `dask-image-2023.3.0rc1/dask_image/ndinterp/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndmeasure/__init__.py` & `dask-image-2023.3.0rc1/dask_image/ndmeasure/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndmeasure/_utils/__init__.py` & `dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndmeasure/_utils/_find_objects.py` & `dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/_find_objects.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndmeasure/_utils/_label.py` & `dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/_label.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndmorph/__init__.py` & `dask-image-2023.3.0rc1/dask_image/ndmorph/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndmorph/_ops.py` & `dask-image-2023.3.0rc1/dask_image/ndmorph/_ops.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image/ndmorph/_utils.py` & `dask-image-2023.3.0rc1/dask_image/ndmorph/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/dask_image.egg-info/PKG-INFO` & `dask-image-2023.3.0rc1/dask_image.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-image
-Version: 2023.3.0
+Version: 2023.3.0rc1
 Summary: Distributed image processing
 Home-page: https://github.com/dask/dask-image
 Author: dask-image contributors
 License: BSD 3-Clause
 Keywords: dask-image
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-image-2023.3.0/dask_image.egg-info/SOURCES.txt` & `dask-image-2023.3.0rc1/dask_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/docs/Makefile` & `dask-image-2023.3.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/docs/conf.py` & `dask-image-2023.3.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/docs/coverage.rst` & `dask-image-2023.3.0rc1/docs/coverage.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/docs/index.rst` & `dask-image-2023.3.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/docs/installation.rst` & `dask-image-2023.3.0rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/docs/make.bat` & `dask-image-2023.3.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/docs/quickstart.rst` & `dask-image-2023.3.0rc1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/docs/release/release_guide.rst` & `dask-image-2023.3.0rc1/docs/release/release_guide.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/setup.py` & `dask-image-2023.3.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_imread/test_core.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/test_core.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_imread/test_cupy_imread.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/test_cupy_imread.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__conv.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__conv.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__diff.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__diff.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__edge.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__edge.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__gaussian.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__gaussian.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__generic.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__generic.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__order.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__order.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__smooth.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__smooth.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__threshold.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__threshold.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test__utils.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfourier/test__utils.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfourier/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndfourier/test_core.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfourier/test_core.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndinterp/test_affine_transformation.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndinterp/test_affine_transformation.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndinterp/test_spline_filter.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndinterp/test_spline_filter.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndmeasure/test__utils.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndmeasure/test_core.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test_core.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndmeasure/test_find_objects.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test_find_objects.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndmorph/test__utils.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/tests/test_dask_image/test_ndmorph/test_ndmorph.py` & `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test_ndmorph.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0/versioneer.py` & `dask-image-2023.3.0rc1/versioneer.py`

 * *Files identical despite different names*

