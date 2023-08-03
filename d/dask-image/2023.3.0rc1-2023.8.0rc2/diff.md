# Comparing `tmp/dask-image-2023.3.0rc1.tar.gz` & `tmp/dask-image-2023.8.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-image-2023.3.0rc1.tar", last modified: Mon Mar 27 04:07:44 2023, max compression
+gzip compressed data, was "dask-image-2023.8.0rc2.tar", last modified: Thu Aug  3 14:14:38 2023, max compression
```

## Comparing `dask-image-2023.3.0rc1.tar` & `dask-image-2023.8.0rc2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20073 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/dask_image/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/dask_image/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndinterp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/dispatch/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/imread/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/imread/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndfilters/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfilters/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndfourier/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndfourier/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndinterp/
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndinterp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndmeasure/
--rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmeasure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/_find_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image/ndmorph/
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmorph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmorph/_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/dask_image/ndmorph/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.791502 dask-image-2023.3.0rc1/dask_image.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20073 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 04:07:44.000000 dask-image-2023.3.0rc1/dask_image.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9202 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/coverage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/docs/release/
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/docs/release/release_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.787502 dask-image-2023.3.0rc1/tests/test_dask_image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/test_cupy_imread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfourier/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfourier/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfourier/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndinterp/
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndinterp/test_affine_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndinterp/test_spline_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test_find_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 04:07:44.795502 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test__utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test_ndmorph.py
--rw-r--r--   0 runner    (1001) docker     (123)    68567 2023-03-27 04:07:32.000000 dask-image-2023.3.0rc1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.061274 dask-image-2023.8.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20666 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22464 2023-08-03 14:14:38.061274 dask-image-2023.8.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.061274 dask-image-2023.8.0rc2/dask_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-03 14:14:38.061274 dask-image-2023.8.0rc2/dask_image/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.053274 dask-image-2023.8.0rc2/dask_image/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/dispatch/_dispatch_ndfilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/dispatch/_dispatch_ndinterp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/dispatch/_dispatch_ndmorph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/dispatch/_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/dispatch/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.053274 dask-image-2023.8.0rc2/dask_image/imread/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/imread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.053274 dask-image-2023.8.0rc2/dask_image/ndfilters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfilters/_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfilters/_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfilters/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfilters/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfilters/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfilters/_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfilters/_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfilters/_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfilters/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.053274 dask-image-2023.8.0rc2/dask_image/ndfourier/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndfourier/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.053274 dask-image-2023.8.0rc2/dask_image/ndinterp/
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndinterp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.053274 dask-image-2023.8.0rc2/dask_image/ndmeasure/
+-rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndmeasure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.053274 dask-image-2023.8.0rc2/dask_image/ndmeasure/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndmeasure/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndmeasure/_utils/_find_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndmeasure/_utils/_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.053274 dask-image-2023.8.0rc2/dask_image/ndmorph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndmorph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndmorph/_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/dask_image/ndmorph/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.049274 dask-image-2023.8.0rc2/dask_image.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22464 2023-08-03 14:14:37.000000 dask-image-2023.8.0rc2/dask_image.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-08-03 14:14:38.000000 dask-image-2023.8.0rc2/dask_image.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:14:37.000000 dask-image-2023.8.0rc2/dask_image.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:14:37.000000 dask-image-2023.8.0rc2/dask_image.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 14:14:37.000000 dask-image-2023.8.0rc2/dask_image.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 14:14:37.000000 dask-image-2023.8.0rc2/dask_image.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.057274 dask-image-2023.8.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9202 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/coverage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.057274 dask-image-2023.8.0rc2/docs/release/
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/docs/release/release_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-03 14:14:38.061274 dask-image-2023.8.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.057274 dask-image-2023.8.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.049274 dask-image-2023.8.0rc2/tests/test_dask_image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.057274 dask-image-2023.8.0rc2/tests/test_dask_image/test_imread/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_imread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_imread/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_imread/test_cupy_imread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.061274 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.061274 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfourier/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfourier/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfourier/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.061274 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndinterp/
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndinterp/test_affine_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndinterp/test_spline_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.061274 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmeasure/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmeasure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmeasure/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmeasure/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmeasure/test_find_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:14:38.061274 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmorph/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmorph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmorph/test__utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmorph/test_ndmorph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68567 2023-08-03 14:14:23.000000 dask-image-2023.8.0rc2/versioneer.py
```

### Comparing `dask-image-2023.3.0rc1/CONTRIBUTING.rst` & `dask-image-2023.8.0rc2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/HISTORY.rst` & `dask-image-2023.8.0rc2/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,71 @@
 =======
 History
 =======
 
+2023.08.0 (2023-08-03)
+----------------------
+
+We're pleased to announce the release of dask-image 2023.08.0!
+
+Highlights
+
+This version fixes bugs related to processing CuPy backed dask arrays
+and improves testing on GPU CI. It drops support for python 3.8 and
+adds pandas as a dependency. As a feature improvement, the dask-image
+equivalent of ``scipy.ndimage.label`` now supports arbitrary
+structuring elements.
+
+For full support of all GPU functionality in dask-image we recommend
+using CuPy version 9.0.0 or higher.
+
+Improvements
+
+* Generalised ndmeasure.label to arbitrary structuring elements (#321)
+
+Bug Fixes
+
+* Added missing cupy test mark and fixed cupy threshold (#329)
+* Moved functions from ndimage submodules to ndimage namespace (#325)
+
+Updated requirements
+
+* Drop Python 3.8, in accordance with NEP29 recommendation (#315)
+* Require NumPy 1.18+ (#304)
+* Add pandas requirement for find_objs function (#309)
+
+Build Tools
+
+* Continuous integration
+   * Update GPU conda environment before running tests (#318)
+   * Fix GitHub actions README badge (#323)
+* Dependabot updates
+   * Bump coverallsapp/github-action from 2.0.0 to 2.1.2 (#313)
+   * Bump coverallsapp/github-action from 2.1.2 to 2.2.0 (#322)
+   * Bump coverallsapp/github-action from 2.2.0 to 2.2.1 (#326)
+
+
+6 authors added to this release (alphabetical)
+
+* `Charles Blackmon-Luca <https://github.com/dask/dask-image/commits?author=charlesbluca>`_ - @charlesbluca
+* `David Stansby <https://github.com/dask/dask-image/commits?author=dstansby>`_ - @dstansby
+* `dependabot[bot] <https://github.com/dask/dask-image/commits?author=dependabot[bot]>`_ - @dependabot[bot]
+* `Genevieve Buckley <https://github.com/dask/dask-image/commits?author=GenevieveBuckley>`_ - @GenevieveBuckley
+* `jakirkham <https://github.com/dask/dask-image/commits?author=jakirkham>`_ - @jakirkham
+* `Marvin Albert <https://github.com/dask/dask-image/commits?author=m-albert>`_ - @m-albert
+
+
+4 reviewers added to this release (alphabetical)
+
+* `Charles Blackmon-Luca <https://github.com/dask/dask-image/commits?author=charlesbluca>`_ - @charlesbluca
+* `Genevieve Buckley <https://github.com/dask/dask-image/commits?author=GenevieveBuckley>`_ - @GenevieveBuckley
+* `jakirkham <https://github.com/dask/dask-image/commits?author=jakirkham>`_ - @jakirkham
+* `Juan Nunez-Iglesias <https://github.com/dask/dask-image/commits?author=jni>`_ - @jni
+
+
 v2023.03.0 (2023-03-27)
 -----------------------
 
 We're pleased to announce the release of dask-image v2023.03.0!
 
 Highlights
```

### Comparing `dask-image-2023.3.0rc1/LICENSE.txt` & `dask-image-2023.8.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/PKG-INFO` & `dask-image-2023.8.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: dask-image
-Version: 2023.3.0rc1
+Version: 2023.8.0rc2
 Summary: Distributed image processing
 Home-page: https://github.com/dask/dask-image
 Author: dask-image contributors
 License: BSD 3-Clause
 Keywords: dask-image
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
@@ -28,16 +27,16 @@
         :target: https://pypi.python.org/pypi/dask-image
         :alt: PyPI
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/dask-image.svg
         :target: https://anaconda.org/conda-forge/dask-image
         :alt: conda-forge
 
-.. image:: https://github.com/dask/dask-image/workflows/CI/badge.svg
-        :target: https://github.com/dask/dask-image/actions
+.. image:: https://github.com/dask/dask-image/actions/workflows/test_and_deploy.yml/badge.svg
+        :target: https://github.com/dask/dask-image/actions/workflows/test_and_deploy.yml
         :alt: GitHub Actions CI
 
 .. image:: https://readthedocs.org/projects/dask-image/badge/?version=latest
         :target: https://dask-image.readthedocs.io/en/latest/?badge=latest
         :alt: Read the Docs
 
 .. image:: https://coveralls.io/repos/github/dask/dask-image/badge.svg
@@ -56,14 +55,74 @@
 * Documentation: https://dask-image.readthedocs.io.
 
 
 =======
 History
 =======
 
+2023.08.0 (2023-08-03)
+----------------------
+
+We're pleased to announce the release of dask-image 2023.08.0!
+
+Highlights
+
+This version fixes bugs related to processing CuPy backed dask arrays
+and improves testing on GPU CI. It drops support for python 3.8 and
+adds pandas as a dependency. As a feature improvement, the dask-image
+equivalent of ``scipy.ndimage.label`` now supports arbitrary
+structuring elements.
+
+For full support of all GPU functionality in dask-image we recommend
+using CuPy version 9.0.0 or higher.
+
+Improvements
+
+* Generalised ndmeasure.label to arbitrary structuring elements (#321)
+
+Bug Fixes
+
+* Added missing cupy test mark and fixed cupy threshold (#329)
+* Moved functions from ndimage submodules to ndimage namespace (#325)
+
+Updated requirements
+
+* Drop Python 3.8, in accordance with NEP29 recommendation (#315)
+* Require NumPy 1.18+ (#304)
+* Add pandas requirement for find_objs function (#309)
+
+Build Tools
+
+* Continuous integration
+   * Update GPU conda environment before running tests (#318)
+   * Fix GitHub actions README badge (#323)
+* Dependabot updates
+   * Bump coverallsapp/github-action from 2.0.0 to 2.1.2 (#313)
+   * Bump coverallsapp/github-action from 2.1.2 to 2.2.0 (#322)
+   * Bump coverallsapp/github-action from 2.2.0 to 2.2.1 (#326)
+
+
+6 authors added to this release (alphabetical)
+
+* `Charles Blackmon-Luca <https://github.com/dask/dask-image/commits?author=charlesbluca>`_ - @charlesbluca
+* `David Stansby <https://github.com/dask/dask-image/commits?author=dstansby>`_ - @dstansby
+* `dependabot[bot] <https://github.com/dask/dask-image/commits?author=dependabot[bot]>`_ - @dependabot[bot]
+* `Genevieve Buckley <https://github.com/dask/dask-image/commits?author=GenevieveBuckley>`_ - @GenevieveBuckley
+* `jakirkham <https://github.com/dask/dask-image/commits?author=jakirkham>`_ - @jakirkham
+* `Marvin Albert <https://github.com/dask/dask-image/commits?author=m-albert>`_ - @m-albert
+
+
+4 reviewers added to this release (alphabetical)
+
+* `Charles Blackmon-Luca <https://github.com/dask/dask-image/commits?author=charlesbluca>`_ - @charlesbluca
+* `Genevieve Buckley <https://github.com/dask/dask-image/commits?author=GenevieveBuckley>`_ - @GenevieveBuckley
+* `jakirkham <https://github.com/dask/dask-image/commits?author=jakirkham>`_ - @jakirkham
+* `Juan Nunez-Iglesias <https://github.com/dask/dask-image/commits?author=jni>`_ - @jni
+
+
 v2023.03.0 (2023-03-27)
 -----------------------
 
 We're pleased to announce the release of dask-image v2023.03.0!
 
 Highlights
```

### Comparing `dask-image-2023.3.0rc1/README.rst` & `dask-image-2023.8.0rc2/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         :target: https://pypi.python.org/pypi/dask-image
         :alt: PyPI
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/dask-image.svg
         :target: https://anaconda.org/conda-forge/dask-image
         :alt: conda-forge
 
-.. image:: https://github.com/dask/dask-image/workflows/CI/badge.svg
-        :target: https://github.com/dask/dask-image/actions
+.. image:: https://github.com/dask/dask-image/actions/workflows/test_and_deploy.yml/badge.svg
+        :target: https://github.com/dask/dask-image/actions/workflows/test_and_deploy.yml
         :alt: GitHub Actions CI
 
 .. image:: https://readthedocs.org/projects/dask-image/badge/?version=latest
         :target: https://dask-image.readthedocs.io/en/latest/?badge=latest
         :alt: Read the Docs
 
 .. image:: https://coveralls.io/repos/github/dask/dask-image/badge.svg
```

### Comparing `dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndfilters.py` & `dask-image-2023.8.0rc2/dask_image/dispatch/_dispatch_ndfilters.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 @dispatch_convolve.register_lazy("cupy")
 def register_cupy_convolve():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_convolve.register(cupy.ndarray)
     def cupy_convolve(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.convolve
+        return cupyx.scipy.ndimage.convolve
 
 
 # ================== correlate ==================
 @dispatch_correlate.register(np.ndarray)
 def numpy_correlate(*args, **kwargs):
     return scipy.ndimage.correlate
 
@@ -68,15 +68,15 @@
 @dispatch_correlate.register_lazy("cupy")
 def register_cupy_correlate():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_correlate.register(cupy.ndarray)
     def cupy_correlate(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.correlate
+        return cupyx.scipy.ndimage.correlate
 
 
 # ================== laplace ==================
 @dispatch_laplace.register(np.ndarray)
 def numpy_laplace(*args, **kwargs):
     return scipy.ndimage.laplace
 
@@ -84,15 +84,15 @@
 @dispatch_laplace.register_lazy("cupy")
 def register_cupy_laplace():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_laplace.register(cupy.ndarray)
     def cupy_laplace(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.laplace
+        return cupyx.scipy.ndimage.laplace
 
 
 # ================== prewitt ==================
 @dispatch_prewitt.register(np.ndarray)
 def numpy_prewitt(*args, **kwargs):
     return scipy.ndimage.prewitt
 
@@ -100,15 +100,15 @@
 @dispatch_prewitt.register_lazy("cupy")
 def register_cupy_prewitt():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_prewitt.register(cupy.ndarray)
     def cupy_prewitt(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.prewitt
+        return cupyx.scipy.ndimage.prewitt
 
 
 # ================== sobel ==================
 @dispatch_sobel.register(np.ndarray)
 def numpy_sobel(*args, **kwargs):
     return scipy.ndimage.sobel
 
@@ -116,15 +116,15 @@
 @dispatch_sobel.register_lazy("cupy")
 def register_cupy_sobel():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_sobel.register(cupy.ndarray)
     def cupy_sobel(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.sobel
+        return cupyx.scipy.ndimage.sobel
 
 
 # ================== gaussian_filter ==================
 @dispatch_gaussian_filter.register(np.ndarray)
 def numpy_gaussian_filter(*args, **kwargs):
     return scipy.ndimage.gaussian_filter
 
@@ -132,15 +132,15 @@
 @dispatch_gaussian_filter.register_lazy("cupy")
 def register_cupy_gaussian_filter():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_gaussian_filter.register(cupy.ndarray)
     def cupy_gaussian_filter(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.gaussian_filter
+        return cupyx.scipy.ndimage.gaussian_filter
 
 
 # ================== gaussian_gradient_magnitude ==================
 @dispatch_gaussian_gradient_magnitude.register(np.ndarray)
 def numpy_gaussian_gradient_magnitude(*args, **kwargs):
     return scipy.ndimage.gaussian_gradient_magnitude
 
@@ -148,15 +148,15 @@
 @dispatch_gaussian_gradient_magnitude.register_lazy("cupy")
 def register_cupy_gaussian_gradient_magnitude():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_gaussian_gradient_magnitude.register(cupy.ndarray)
     def cupy_gaussian_gradient_magnitude(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.gaussian_gradient_magnitude
+        return cupyx.scipy.ndimage.gaussian_gradient_magnitude
 
 
 # ================== gaussian_laplace ==================
 @dispatch_gaussian_laplace.register(np.ndarray)
 def numpy_gaussian_laplace(*args, **kwargs):
     return scipy.ndimage.gaussian_laplace
 
@@ -164,15 +164,15 @@
 @dispatch_gaussian_laplace.register_lazy("cupy")
 def register_cupy_gaussian_laplace():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_gaussian_laplace.register(cupy.ndarray)
     def cupy_gaussian_laplace(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.gaussian_laplace
+        return cupyx.scipy.ndimage.gaussian_laplace
 
 
 # ================== generic_filter ==================
 @dispatch_generic_filter.register(np.ndarray)
 def numpy_generic_filter(*args, **kwargs):
     return scipy.ndimage.generic_filter
 
@@ -180,15 +180,15 @@
 @dispatch_generic_filter.register_lazy("cupy")
 def register_cupy_generic_filter():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_generic_filter.register(cupy.ndarray)
     def cupy_generic_filter(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.generic_filter
+        return cupyx.scipy.ndimage.generic_filter
 
 
 # ================== minimum_filter ==================
 @dispatch_minimum_filter.register(np.ndarray)
 def numpy_minimum_filter(*args, **kwargs):
     return scipy.ndimage.minimum_filter
 
@@ -196,15 +196,15 @@
 @dispatch_minimum_filter.register_lazy("cupy")
 def register_cupy_minimum_filter():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_minimum_filter.register(cupy.ndarray)
     def cupy_minimum_filter(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.minimum_filter
+        return cupyx.scipy.ndimage.minimum_filter
 
 
 # ================== median_filter ==================
 @dispatch_median_filter.register(np.ndarray)
 def numpy_median_filter(*args, **kwargs):
     return scipy.ndimage.median_filter
 
@@ -212,15 +212,15 @@
 @dispatch_median_filter.register_lazy("cupy")
 def register_cupy_median_filter():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_median_filter.register(cupy.ndarray)
     def cupy_median_filter(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.median_filter
+        return cupyx.scipy.ndimage.median_filter
 
 
 # ================== maximum_filter ==================
 @dispatch_maximum_filter.register(np.ndarray)
 def numpy_maximum_filter(*args, **kwargs):
     return scipy.ndimage.maximum_filter
 
@@ -228,15 +228,15 @@
 @dispatch_maximum_filter.register_lazy("cupy")
 def register_cupy_maximum_filter():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_maximum_filter.register(cupy.ndarray)
     def cupy_maximum_filter(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.maximum_filter
+        return cupyx.scipy.ndimage.maximum_filter
 
 
 # ================== rank_filter ==================
 @dispatch_rank_filter.register(np.ndarray)
 def numpy_rank_filter(*args, **kwargs):
     return scipy.ndimage.rank_filter
 
@@ -244,15 +244,15 @@
 @dispatch_rank_filter.register_lazy("cupy")
 def register_cupy_rank_filter():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_rank_filter.register(cupy.ndarray)
     def cupy_rank_filter(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.rank_filter
+        return cupyx.scipy.ndimage.rank_filter
 
 
 # ================== percentile_filter ==================
 @dispatch_percentile_filter.register(np.ndarray)
 def numpy_percentile_filter(*args, **kwargs):
     return scipy.ndimage.percentile_filter
 
@@ -260,15 +260,15 @@
 @dispatch_percentile_filter.register_lazy("cupy")
 def register_cupy_percentile_filter():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_percentile_filter.register(cupy.ndarray)
     def cupy_percentile_filter(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.percentile_filter
+        return cupyx.scipy.ndimage.percentile_filter
 
 
 # ================== uniform_filter ==================
 @dispatch_uniform_filter.register(np.ndarray)
 def numpy_uniform_filter(*args, **kwargs):
     return scipy.ndimage.uniform_filter
 
@@ -276,15 +276,15 @@
 @dispatch_uniform_filter.register_lazy("cupy")
 def register_cupy_uniform_filter():
     import cupy
     import cupyx.scipy.ndimage
 
     @dispatch_uniform_filter.register(cupy.ndarray)
     def cupy_uniform_filter(*args, **kwargs):
-        return cupyx.scipy.ndimage.filters.uniform_filter
+        return cupyx.scipy.ndimage.uniform_filter
 
 
 # ================== threshold_local_mean ==================
 @dispatch_threshold_local_mean.register(np.ndarray)
 def numpy_threshold_local_mean(*args, **kwargs):
     return np.mean
```

### Comparing `dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndinterp.py` & `dask-image-2023.8.0rc2/dask_image/dispatch/_dispatch_ndinterp.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/dispatch/_dispatch_ndmorph.py` & `dask-image-2023.8.0rc2/dask_image/dispatch/_dispatch_ndmorph.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/dispatch/_dispatcher.py` & `dask-image-2023.8.0rc2/dask_image/dispatch/_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/dispatch/_utils.py` & `dask-image-2023.8.0rc2/dask_image/dispatch/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/imread/__init__.py` & `dask-image-2023.8.0rc2/dask_image/imread/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfilters/__init__.py` & `dask-image-2023.8.0rc2/dask_image/ndfilters/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfilters/_conv.py` & `dask-image-2023.8.0rc2/dask_image/ndfilters/_conv.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfilters/_edge.py` & `dask-image-2023.8.0rc2/dask_image/ndfilters/_edge.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfilters/_gaussian.py` & `dask-image-2023.8.0rc2/dask_image/ndfilters/_gaussian.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfilters/_generic.py` & `dask-image-2023.8.0rc2/dask_image/ndfilters/_generic.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfilters/_order.py` & `dask-image-2023.8.0rc2/dask_image/ndfilters/_order.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfilters/_smooth.py` & `dask-image-2023.8.0rc2/dask_image/ndfilters/_smooth.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfilters/_threshold.py` & `dask-image-2023.8.0rc2/dask_image/ndfilters/_threshold.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         if not callable(param):
             raise ValueError("Must include a valid function to use as the "
                              "'param' keyword argument.")
         thresh_image = _generic.generic_filter(image, param, block_size,
                                                mode=mode, cval=cval)
     elif method == 'gaussian':
         if param is None:
-            sigma = (da.asarray(block_size, like=image._meta) - 1) / 6.0
+            sigma = (np.array(block_size).astype(float) - 1) / 6.0
         else:
             sigma = param
         thresh_image = _gaussian.gaussian_filter(image, sigma, mode=mode,
                                                  cval=cval)
     elif method == 'mean':
         thresh_image = _generic.generic_filter(
             image, dispatch_threshold_local_mean(image), block_size, mode=mode,
```

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfilters/_utils.py` & `dask-image-2023.8.0rc2/dask_image/ndfilters/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfourier/__init__.py` & `dask-image-2023.8.0rc2/dask_image/ndfourier/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndfourier/_utils.py` & `dask-image-2023.8.0rc2/dask_image/ndfourier/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndinterp/__init__.py` & `dask-image-2023.8.0rc2/dask_image/ndinterp/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndmeasure/__init__.py` & `dask-image-2023.8.0rc2/dask_image/ndmeasure/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/__init__.py` & `dask-image-2023.8.0rc2/dask_image/ndmeasure/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/_find_objects.py` & `dask-image-2023.8.0rc2/dask_image/ndmeasure/_utils/_find_objects.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndmeasure/_utils/_label.py` & `dask-image-2023.8.0rc2/dask_image/ndmeasure/_utils/_label.py`

 * *Files 13% similar despite different names*

```diff
@@ -147,65 +147,102 @@
 
     Returns
     -------
     mat : delayed scipy.sparse.csr_matrix
         This matrix has value 1 at (i, j) if label i is connected to
         label j in the global volume, 0 everywhere else.
     """
-    faces = _chunk_faces(labels.chunks, labels.shape)
+
+    if structure is None:
+        structure = scipy.ndimage.generate_binary_structure(labels.ndim, 1)
+
+    faces = _chunk_faces(labels.chunks, labels.shape, structure)
     all_mappings = [da.empty((2, 0), dtype=LABEL_DTYPE, chunks=1)]
     for face_slice in faces:
         face = labels[face_slice]
         mapped = _across_block_label_grouping_delayed(face, structure)
         all_mappings.append(mapped)
     all_mappings = da.concatenate(all_mappings, axis=1)
     i, j = all_mappings
     mat = _to_csr_matrix(i, j, nlabels + 1)
     return mat
 
 
-def _chunk_faces(chunks, shape):
+def _chunk_faces(chunks, shape, structure):
     """
     Return slices for two-pixel-wide boundaries between chunks.
 
     Parameters
     ----------
     chunks : tuple of tuple of int
         The chunk specification of the array.
     shape : tuple of int
         The shape of the array.
+    structure: array of bool
+        Structuring element, shape (3,) * ndim.
 
     Returns
     -------
     faces : list of tuple of slices
         Each element in this list indexes a face between two chunks.
 
     Examples
     --------
     >>> import dask.array as da
+    >>> import scipy.ndimage as ndi
     >>> a = da.arange(110, chunks=110).reshape((10, 11)).rechunk(5)
-    >>> chunk_faces(a.chunks, a.shape)
+    >>> structure = ndi.generate_binary_structure(2, 1)
+    >>> chunk_faces(a.chunks, a.shape, structure)
     [(slice(4, 6, None), slice(0, 5, None)),
      (slice(4, 6, None), slice(5, 10, None)),
      (slice(4, 6, None), slice(10, 11, None)),
      (slice(0, 5, None), slice(4, 6, None)),
      (slice(0, 5, None), slice(9, 11, None)),
      (slice(5, 10, None), slice(4, 6, None)),
      (slice(5, 10, None), slice(9, 11, None))]
     """
-    slices = da.core.slices_from_chunks(chunks)
+
     ndim = len(shape)
+    numblocks = tuple(list(len(c) for c in chunks))
+    
+    slices = da.core.slices_from_chunks(chunks)
+    
+    # arrange block/chunk indices on grid
+    block_summary = np.arange(len(slices)).reshape(numblocks)
+    
     faces = []
-    for ax in range(ndim):
-        for sl in slices:
-            if sl[ax].stop == shape[ax]:
-                continue
-            slice_to_append = list(sl)
-            slice_to_append[ax] = slice(sl[ax].stop - 1, sl[ax].stop + 1)
-            faces.append(tuple(slice_to_append))
+    for ind_curr_block, curr_block in enumerate(np.ndindex(numblocks)):
+        
+        for pos_structure_coord in np.array(np.where(structure)).T:
+                        
+            # only consider forward neighbors
+            if min(pos_structure_coord) < 1 or \
+               max(pos_structure_coord) < 2: continue
+
+            neigh_block = [curr_block[dim] + pos_structure_coord[dim] - 1
+                           for dim in range(ndim)]
+
+            if max([neigh_block[dim] >= numblocks[dim] for dim in range(ndim)]): continue
+
+            # get neighbor slice index
+            ind_neigh_block = block_summary[tuple(neigh_block)]
+
+            curr_slice = []
+            for dim in range(ndim):
+                # keep slice if not on boundary
+                if slices[ind_curr_block][dim] == slices[ind_neigh_block][dim]:
+                    curr_slice.append(slices[ind_curr_block][dim])
+                # otherwise, add two-pixel-wide boundary
+                else:
+                    curr_slice.append(slice(
+                        slices[ind_curr_block][dim].stop - 1,
+                        slices[ind_curr_block][dim].stop + 1))
+                    
+            faces.append(tuple(curr_slice))
+            
     return faces
 
 
 def block_ndi_label_delayed(block, structure):
     """
     Delayed version of ``scipy.ndimage.label``.
```

### Comparing `dask-image-2023.3.0rc1/dask_image/ndmorph/__init__.py` & `dask-image-2023.8.0rc2/dask_image/ndmorph/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndmorph/_ops.py` & `dask-image-2023.8.0rc2/dask_image/ndmorph/_ops.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image/ndmorph/_utils.py` & `dask-image-2023.8.0rc2/dask_image/ndmorph/_utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/dask_image.egg-info/PKG-INFO` & `dask-image-2023.8.0rc2/dask_image.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: dask-image
-Version: 2023.3.0rc1
+Version: 2023.8.0rc2
 Summary: Distributed image processing
 Home-page: https://github.com/dask/dask-image
 Author: dask-image contributors
 License: BSD 3-Clause
 Keywords: dask-image
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
@@ -28,16 +27,16 @@
         :target: https://pypi.python.org/pypi/dask-image
         :alt: PyPI
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/dask-image.svg
         :target: https://anaconda.org/conda-forge/dask-image
         :alt: conda-forge
 
-.. image:: https://github.com/dask/dask-image/workflows/CI/badge.svg
-        :target: https://github.com/dask/dask-image/actions
+.. image:: https://github.com/dask/dask-image/actions/workflows/test_and_deploy.yml/badge.svg
+        :target: https://github.com/dask/dask-image/actions/workflows/test_and_deploy.yml
         :alt: GitHub Actions CI
 
 .. image:: https://readthedocs.org/projects/dask-image/badge/?version=latest
         :target: https://dask-image.readthedocs.io/en/latest/?badge=latest
         :alt: Read the Docs
 
 .. image:: https://coveralls.io/repos/github/dask/dask-image/badge.svg
@@ -56,14 +55,74 @@
 * Documentation: https://dask-image.readthedocs.io.
 
 
 =======
 History
 =======
 
+2023.08.0 (2023-08-03)
+----------------------
+
+We're pleased to announce the release of dask-image 2023.08.0!
+
+Highlights
+
+This version fixes bugs related to processing CuPy backed dask arrays
+and improves testing on GPU CI. It drops support for python 3.8 and
+adds pandas as a dependency. As a feature improvement, the dask-image
+equivalent of ``scipy.ndimage.label`` now supports arbitrary
+structuring elements.
+
+For full support of all GPU functionality in dask-image we recommend
+using CuPy version 9.0.0 or higher.
+
+Improvements
+
+* Generalised ndmeasure.label to arbitrary structuring elements (#321)
+
+Bug Fixes
+
+* Added missing cupy test mark and fixed cupy threshold (#329)
+* Moved functions from ndimage submodules to ndimage namespace (#325)
+
+Updated requirements
+
+* Drop Python 3.8, in accordance with NEP29 recommendation (#315)
+* Require NumPy 1.18+ (#304)
+* Add pandas requirement for find_objs function (#309)
+
+Build Tools
+
+* Continuous integration
+   * Update GPU conda environment before running tests (#318)
+   * Fix GitHub actions README badge (#323)
+* Dependabot updates
+   * Bump coverallsapp/github-action from 2.0.0 to 2.1.2 (#313)
+   * Bump coverallsapp/github-action from 2.1.2 to 2.2.0 (#322)
+   * Bump coverallsapp/github-action from 2.2.0 to 2.2.1 (#326)
+
+
+6 authors added to this release (alphabetical)
+
+* `Charles Blackmon-Luca <https://github.com/dask/dask-image/commits?author=charlesbluca>`_ - @charlesbluca
+* `David Stansby <https://github.com/dask/dask-image/commits?author=dstansby>`_ - @dstansby
+* `dependabot[bot] <https://github.com/dask/dask-image/commits?author=dependabot[bot]>`_ - @dependabot[bot]
+* `Genevieve Buckley <https://github.com/dask/dask-image/commits?author=GenevieveBuckley>`_ - @GenevieveBuckley
+* `jakirkham <https://github.com/dask/dask-image/commits?author=jakirkham>`_ - @jakirkham
+* `Marvin Albert <https://github.com/dask/dask-image/commits?author=m-albert>`_ - @m-albert
+
+
+4 reviewers added to this release (alphabetical)
+
+* `Charles Blackmon-Luca <https://github.com/dask/dask-image/commits?author=charlesbluca>`_ - @charlesbluca
+* `Genevieve Buckley <https://github.com/dask/dask-image/commits?author=GenevieveBuckley>`_ - @GenevieveBuckley
+* `jakirkham <https://github.com/dask/dask-image/commits?author=jakirkham>`_ - @jakirkham
+* `Juan Nunez-Iglesias <https://github.com/dask/dask-image/commits?author=jni>`_ - @jni
+
+
 v2023.03.0 (2023-03-27)
 -----------------------
 
 We're pleased to announce the release of dask-image v2023.03.0!
 
 Highlights
```

### Comparing `dask-image-2023.3.0rc1/dask_image.egg-info/SOURCES.txt` & `dask-image-2023.8.0rc2/dask_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/docs/Makefile` & `dask-image-2023.8.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/docs/conf.py` & `dask-image-2023.8.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/docs/coverage.rst` & `dask-image-2023.8.0rc2/docs/coverage.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/docs/index.rst` & `dask-image-2023.8.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/docs/installation.rst` & `dask-image-2023.8.0rc2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/docs/make.bat` & `dask-image-2023.8.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/docs/quickstart.rst` & `dask-image-2023.8.0rc2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/docs/release/release_guide.rst` & `dask-image-2023.8.0rc2/docs/release/release_guide.rst`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/setup.py` & `dask-image-2023.8.0rc2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
 requirements = [
-    "dask[array] >=2021.10.0",
-    "numpy >=1.11.3",
+    "dask[array] >=2023.2.0",
+    "dask[dataframe] >=2023.2.0",
+    "numpy >=1.18",
     "scipy >=0.19.1",
     "pims >=0.4.1",
     "tifffile >=2018.10.18",
+    "pandas >=2.0.0",
 ]
 
 test_requirements = [
     "flake8 >=3.4.1",
     "pytest >=3.0.5",
     "pytest-flake8 >=0.8.1",
     "pytest-timeout >=1.0.0",
@@ -66,14 +68,13 @@
     keywords="dask-image",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     tests_require=test_requirements
 )
```

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/test_core.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_imread/test_core.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_imread/test_cupy_imread.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_imread/test_cupy_imread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import tifffile
 import pytest
 
 import dask_image.imread
 
-cupy = pytest.importorskip("cupy", minversion="7.7.0")
+cupy = pytest.importorskip("cupy", minversion="6.0.0")
 
 
 @pytest.mark.cupy
 def test_cupy_imread(tmp_path):
     a = np.random.uniform(low=0.0, high=1.0, size=(1, 4, 3)).astype(np.float32)
 
     fn = str(tmp_path/"test.tiff")
```

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__conv.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__conv.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__diff.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__diff.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__edge.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__edge.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__gaussian.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__gaussian.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__generic.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__generic.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__order.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__order.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__smooth.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__smooth.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__threshold.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__threshold.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test__utils.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test_cupy_ndfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import dask.array as da
 import numpy as np
 import pytest
 
 import dask_image.ndfilters
 
-cupy = pytest.importorskip("cupy", minversion="7.7.0")
+cupy = pytest.importorskip("cupy", minversion="8.0.0")
 
 
 @pytest.fixture
 def array():
     s = (10, 10)
     a = da.from_array(cupy.arange(int(np.prod(s)),
                       dtype=cupy.float32).reshape(s), chunks=5)
```

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfilters/test_cupy_threshold.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 import dask.array as da
 import numpy as np
 import pytest
 
 from dask_image.ndfilters import threshold_local
 
-cupy = pytest.importorskip("cupy", minversion="7.7.0")
+cupy = pytest.importorskip("cupy", minversion="5.0.0")
 
 
+@pytest.mark.cupy
 @pytest.mark.parametrize('block_size', [
     3,
     [3, 3],
     np.array([3, 3]),
     da.from_array(np.array([3, 3]), chunks=1),
     da.from_array(np.array([3, 3]), chunks=2),
 ])
```

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfourier/test__utils.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfourier/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndfourier/test_core.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndfourier/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     [
         "fourier_shift",
         "fourier_gaussian",
     ]
 )
 def test_fourier_filter_identity(funcname, s):
     da_func = getattr(dask_image.ndfourier, funcname)
-    sp_func = getattr(scipy.ndimage.fourier, funcname)
+    sp_func = getattr(scipy.ndimage, funcname)
 
     a = np.arange(140.0).reshape(10, 14).astype(complex)
     d = da.from_array(a, chunks=(5, 7))
 
     r_a = sp_func(a, s)
     r_d = da_func(d, s)
 
@@ -101,15 +101,15 @@
         )
 
     dtype = np.dtype(dtype).type
 
     s = 1
 
     da_func = getattr(dask_image.ndfourier, funcname)
-    sp_func = getattr(scipy.ndimage.fourier, funcname)
+    sp_func = getattr(scipy.ndimage, funcname)
 
     a = np.arange(140.0).reshape(10, 14).astype(dtype)
     d = da.from_array(a, chunks=(5, 7))
 
     r_a = sp_func(a, s)
     r_d = da_func(d, s)
 
@@ -143,15 +143,15 @@
 )
 def test_fourier_filter_chunks(funcname, shape, chunks):
     dtype = np.dtype(complex).type
 
     s = 1
 
     da_func = getattr(dask_image.ndfourier, funcname)
-    sp_func = getattr(scipy.ndimage.fourier, funcname)
+    sp_func = getattr(scipy.ndimage, funcname)
 
     a = np.arange(np.prod(shape)).reshape(shape).astype(dtype)
     d = da.from_array(a, chunks=chunks)
 
     r_a = sp_func(a, s)
     r_d = da_func(d, s)
 
@@ -176,15 +176,15 @@
     [
         "fourier_shift",
         "fourier_gaussian",
     ]
 )
 def test_fourier_filter_non_positive(funcname, s):
     da_func = getattr(dask_image.ndfourier, funcname)
-    sp_func = getattr(scipy.ndimage.fourier, funcname)
+    sp_func = getattr(scipy.ndimage, funcname)
 
     a = np.arange(140.0).reshape(10, 14).astype(complex)
     d = da.from_array(a, chunks=(5, 7))
 
     r_a = sp_func(a, s)
     r_d = da_func(d, s)
 
@@ -221,15 +221,15 @@
         (True, -1),
         (True, 0),
         (False, -1),
     ]
 )
 def test_fourier_filter(funcname, s, real_fft, axis):
     da_func = getattr(dask_image.ndfourier, funcname)
-    sp_func = getattr(scipy.ndimage.fourier, funcname)
+    sp_func = getattr(scipy.ndimage, funcname)
 
     shape = (10, 14)
     n = 2 * shape[axis] - 1 if real_fft else -1
     dtype = np.float64 if real_fft else np.complex128
 
     a = np.arange(140.0).reshape(shape).astype(dtype)
     d = da.from_array(a, chunks=(5, 7))
```

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndinterp/test_affine_transformation.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndinterp/test_affine_transformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 @pytest.mark.parametrize("random_seed",
                          [0])
 def test_affine_transform_cupy(n,
                                input_output_shape_per_dim,
                                interp_order,
                                input_output_chunksize_per_dim,
                                random_seed):
-    pytest.importorskip("cupy", minversion="6.0.0")
+    pytest.importorskip("cupy", minversion="5.0.0")
 
     kwargs = dict()
     kwargs['n'] = n
     kwargs['input_output_shape_per_dim'] = input_output_shape_per_dim
     kwargs['interp_order'] = interp_order
     kwargs['input_output_chunksize_per_dim'] = input_output_chunksize_per_dim
     kwargs['random_seed'] = random_seed
@@ -260,15 +260,15 @@
     assert isinstance(image, type(image_t))
     assert isinstance(image[0, 0].compute(), type(image_t[0, 0].compute()))
 
 
 @pytest.mark.cupy
 def test_affine_transform_type_consistency_gpu():
 
-    cupy = pytest.importorskip("cupy", minversion="6.0.0")
+    cupy = pytest.importorskip("cupy", minversion="5.0.0")
 
     image = da.ones((3, 3))
     image_t = dask_image.ndinterp.affine_transform(image, np.eye(2), [0, 0])
 
     image.map_blocks(cupy.asarray)
 
     assert isinstance(image, type(image_t))
@@ -310,15 +310,15 @@
 
 @pytest.mark.cupy
 @pytest.mark.timeout(15)
 def test_affine_transform_large_input_small_output_gpu():
     """
     Make sure input array does not need to be computed entirely
     """
-    cupy = pytest.importorskip("cupy", minversion="6.0.0")
+    cupy = pytest.importorskip("cupy", minversion="5.0.0")
 
     # this array would occupy more than 24GB on a GPU
     image = da.random.random([2000] * 3, chunks=(50, 50, 50))
     image.map_blocks(cupy.asarray)
 
     image_t = dask_image.ndinterp.affine_transform(image, np.eye(3), [0, 0, 0],
                                                    output_chunks=[1, 1, 1],
```

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndinterp/test_spline_filter.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndinterp/test_spline_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     interp_order,
     interp_mode,
     chunksize,
     axis,
     input_as_non_dask_array,
 ):
 
-    pytest.importorskip("cupy", minversion="6.0.0")
+    pytest.importorskip("cupy", minversion="9.0.0")
 
     validate_spline_filter(
         n=n,
         axis_size=axis_size,
         interp_order=interp_order,
         interp_mode=interp_mode,
         chunksize=chunksize,
```

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test__utils.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmeasure/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test_core.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmeasure/test_core.py`

 * *Files 9% similar despite different names*

```diff
@@ -333,40 +333,74 @@
 
 
 @pytest.mark.parametrize(
     "seed, prob, shape, chunks, connectivity", [
         (42, 0.4, (15, 16), (15, 16), 1),
         (42, 0.4, (15, 16), (4, 5), 1),
         (42, 0.4, (15, 16), (4, 5), 2),
+        (42, 0.4, (15, 16), (4, 5), None),
         (42, 0.4, (15, 16), (8, 5), 1),
         (42, 0.4, (15, 16), (8, 5), 2),
         (42, 0.3, (10, 8, 6), (5, 4, 3), 1),
         (42, 0.3, (10, 8, 6), (5, 4, 3), 2),
         (42, 0.3, (10, 8, 6), (5, 4, 3), 3),
     ]
 )
 def test_label(seed, prob, shape, chunks, connectivity):
     np.random.seed(seed)
 
     a = np.random.random(shape) < prob
     d = da.from_array(a, chunks=chunks)
 
-    s = scipy.ndimage.generate_binary_structure(a.ndim, connectivity)
+    if connectivity is None:
+        s = None
+    else:
+        s = scipy.ndimage.generate_binary_structure(a.ndim, connectivity)
 
     a_l, a_nl = scipy.ndimage.label(a, s)
     d_l, d_nl = dask_image.ndmeasure.label(d, s)
 
     assert a_nl == d_nl.compute()
 
     assert a_l.dtype == d_l.dtype
     assert a_l.shape == d_l.shape
     _assert_equivalent_labeling(a_l, d_l.compute())
 
 
 @pytest.mark.parametrize(
+    "ndim", (2, 3, 4, 5)
+)
+def test_label_full_struct_element(ndim):
+
+    full_s = scipy.ndimage.generate_binary_structure(ndim, ndim)
+    orth_s = scipy.ndimage.generate_binary_structure(ndim, ndim - 1)
+
+    # create a mask that represents a single connected component
+    # under the full (highest rank) structuring element
+    # but several connected components under the orthogonal
+    # structuring element
+    mask = full_s ^ orth_s
+    mask[tuple([1] * ndim)] = True
+
+    # create dask array with chunk boundary
+    # that passes through the mask
+    mask_da = da.from_array(mask, chunks=[2] * ndim)
+
+    labels_ndi, N_ndi = scipy.ndimage.label(mask, structure=full_s)
+    labels_di_da, N_di_da = dask_image.ndmeasure.label(
+        mask_da, structure=full_s)
+    
+    assert N_ndi == N_di_da.compute()
+
+    _assert_equivalent_labeling(
+        labels_ndi,
+        labels_di_da.compute())
+
+
+@pytest.mark.parametrize(
     "shape, chunks, ind", [
         ((15, 16), (4, 5), None),
         ((5, 6, 4), (2, 3, 2), None),
         ((15, 16), (4, 5), 0),
         ((15, 16), (4, 5), 1),
         ((15, 16), (4, 5), [1]),
         ((15, 16), (4, 5), [1, 2]),
```

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmeasure/test_find_objects.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmeasure/test_find_objects.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test__utils.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmorph/test__utils.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmorph/test_cupy_ndmorph.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import dask.array as da
 import numpy as np
 import pytest
 
 import dask_image.ndmorph
 
-cupy = pytest.importorskip("cupy", minversion="7.7.0")
+cupy = pytest.importorskip("cupy", minversion="9.0.0")
 
 
 @pytest.fixture
 def array():
     s = (10, 10)
     a = da.from_array(cupy.arange(int(np.prod(s)),
                       dtype=cupy.float32).reshape(s), chunks=5)
```

### Comparing `dask-image-2023.3.0rc1/tests/test_dask_image/test_ndmorph/test_ndmorph.py` & `dask-image-2023.8.0rc2/tests/test_dask_image/test_ndmorph/test_ndmorph.py`

 * *Files identical despite different names*

### Comparing `dask-image-2023.3.0rc1/versioneer.py` & `dask-image-2023.8.0rc2/versioneer.py`

 * *Files identical despite different names*

