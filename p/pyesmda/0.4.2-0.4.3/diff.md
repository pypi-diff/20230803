# Comparing `tmp/pyesmda-0.4.2.tar.gz` & `tmp/pyesmda-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyesmda-0.4.2.tar", last modified: Wed Aug  2 09:25:17 2023, max compression
+gzip compressed data, was "pyesmda-0.4.3.tar", last modified: Thu Aug  3 17:13:20 2023, max compression
```

## Comparing `pyesmda-0.4.2.tar` & `pyesmda-0.4.3.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.689232 pyesmda-0.4.2/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      197 2022-03-01 14:30:06.000000 pyesmda-0.4.2/AUTHORS.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     4702 2023-08-02 09:24:23.000000 pyesmda-0.4.2/CHANGELOG.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     6428 2023-08-02 09:24:23.000000 pyesmda-0.4.2/CONTRIBUTING.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1072 2022-03-01 14:30:06.000000 pyesmda-0.4.2/LICENSE
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      264 2022-03-01 14:30:06.000000 pyesmda-0.4.2/MANIFEST.in
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    10247 2023-08-02 09:25:17.689232 pyesmda-0.4.2/PKG-INFO
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     3537 2023-08-02 09:24:23.000000 pyesmda-0.4.2/README.rst
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.669232 pyesmda-0.4.2/docs/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      612 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/Makefile
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.649232 pyesmda-0.4.2/docs/build/
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.645232 pyesmda-0.4.2/docs/build/doctrees/
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.673232 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    71733 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_12_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28238 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_15_2.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28594 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_20_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21296 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_24_2.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    19817 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_28_2.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    23144 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_30_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21943 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_33_2.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24483 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_35_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24951 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_37_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21251 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_7_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    72926 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_9_1.png
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.649232 pyesmda-0.4.2/docs/build/html/
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.677232 pyesmda-0.4.2/docs/build/html/_images/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    71733 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_12_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28238 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_15_2.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28594 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_20_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21296 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_24_2.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    19817 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_28_2.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    23144 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_30_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21943 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_33_2.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24483 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_35_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24951 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_37_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21251 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_7_1.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    72926 2023-08-02 09:07:26.000000 pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_9_1.png
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.677232 pyesmda-0.4.2/docs/build/html/_static/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      286 2022-12-06 09:06:20.000000 pyesmda-0.4.2/docs/build/html/_static/file.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       90 2022-12-06 09:06:20.000000 pyesmda-0.4.2/docs/build/html/_static/minus.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       90 2022-12-06 09:06:20.000000 pyesmda-0.4.2/docs/build/html/_static/plus.png
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      773 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/make.bat
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.677232 pyesmda-0.4.2/docs/source/
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.681232 pyesmda-0.4.2/docs/source/_autosummary/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1326 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.ESMDA.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1563 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.ESMDA_RS.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      126 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.approximate_cov_mm.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      208 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.approximate_covariance_matrix_from_ensembles.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      149 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.check_nans_in_predictions.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      240 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.compute_ensemble_average_normalized_objective_function.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      185 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.compute_normalized_objective_function.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      184 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.distances_to_weights_beta_cumulative.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      172 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.distances_to_weights_fifth_order.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      135 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.get_ensemble_variance.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      172 2023-08-02 09:07:23.000000 pyesmda-0.4.2/docs/source/_autosummary/pyesmda.inflate_ensemble_around_its_mean.rst
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.681232 pyesmda-0.4.2/docs/source/_templates/
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.681232 pyesmda-0.4.2/docs/source/_templates/autosummary/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      106 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      735 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1098 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      735 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/source/_templates/class.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1079 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1098 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/source/_templates/module.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      113 2023-08-02 09:24:23.000000 pyesmda-0.4.2/docs/source/api_reference.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       31 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/source/authors.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       76 2023-08-02 09:24:23.000000 pyesmda-0.4.2/docs/source/bibliography.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       33 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/source/changelog.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    14867 2023-06-28 13:57:41.000000 pyesmda-0.4.2/docs/source/conf.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       36 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/source/contributing.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      458 2022-08-11 22:32:41.000000 pyesmda-0.4.2/docs/source/index.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1138 2022-08-11 22:32:41.000000 pyesmda-0.4.2/docs/source/installation.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       30 2022-08-11 22:03:08.000000 pyesmda-0.4.2/docs/source/readme.rst
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      288 2022-08-12 09:15:56.000000 pyesmda-0.4.2/docs/source/usage.rst
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.685232 pyesmda-0.4.2/pyesmda/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       96 2023-08-02 09:24:23.000000 pyesmda-0.4.2/pyesmda/__about__.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     2165 2023-08-02 09:24:23.000000 pyesmda-0.4.2/pyesmda/__init__.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    31964 2023-08-02 07:06:07.000000 pyesmda-0.4.2/pyesmda/esmda.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    16165 2023-06-28 13:57:41.000000 pyesmda-0.4.2/pyesmda/esmda_rs.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     4201 2023-08-02 09:24:23.000000 pyesmda-0.4.2/pyesmda/localization.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     7805 2023-06-28 13:57:41.000000 pyesmda-0.4.2/pyesmda/utils.py
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.685232 pyesmda-0.4.2/pyesmda.egg-info/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    10247 2023-08-02 09:25:17.000000 pyesmda-0.4.2/pyesmda.egg-info/PKG-INFO
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     3530 2023-08-02 09:25:17.000000 pyesmda-0.4.2/pyesmda.egg-info/SOURCES.txt
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        1 2023-08-02 09:25:17.000000 pyesmda-0.4.2/pyesmda.egg-info/dependency_links.txt
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        1 2023-08-02 09:25:17.000000 pyesmda-0.4.2/pyesmda.egg-info/not-zip-safe
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       25 2023-08-02 09:25:17.000000 pyesmda-0.4.2/pyesmda.egg-info/requires.txt
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       14 2023-08-02 09:25:17.000000 pyesmda-0.4.2/pyesmda.egg-info/top_level.txt
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      172 2023-08-02 09:24:23.000000 pyesmda-0.4.2/pyproject.toml
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1481 2023-08-02 09:25:17.689232 pyesmda-0.4.2/setup.cfg
-drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-02 09:25:17.689232 pyesmda-0.4.2/tests/
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        0 2022-03-01 14:30:06.000000 pyesmda-0.4.2/tests/__init__.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    14545 2023-06-28 13:57:41.000000 pyesmda-0.4.2/tests/test_esmda.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     2172 2023-06-28 07:47:34.000000 pyesmda-0.4.2/tests/test_esmda_rs.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     2791 2023-08-02 09:24:23.000000 pyesmda-0.4.2/tests/test_localization.py
--rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     5136 2023-06-28 13:57:41.000000 pyesmda-0.4.2/tests/test_utils.py
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.527152 pyesmda-0.4.3/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      197 2022-03-01 14:30:06.000000 pyesmda-0.4.3/AUTHORS.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     5458 2023-08-03 17:09:47.000000 pyesmda-0.4.3/CHANGELOG.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     6428 2023-08-03 17:09:47.000000 pyesmda-0.4.3/CONTRIBUTING.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1072 2022-03-01 14:30:06.000000 pyesmda-0.4.3/LICENSE
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      264 2022-03-01 14:30:06.000000 pyesmda-0.4.3/MANIFEST.in
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    11003 2023-08-03 17:13:20.527152 pyesmda-0.4.3/PKG-INFO
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     3537 2023-08-03 17:09:47.000000 pyesmda-0.4.3/README.rst
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.511152 pyesmda-0.4.3/docs/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      612 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/Makefile
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.499152 pyesmda-0.4.3/docs/build/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.499152 pyesmda-0.4.3/docs/build/doctrees/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.515152 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    71733 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_12_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28238 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_15_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28594 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_20_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21296 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_24_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    19817 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_28_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    23144 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_30_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21943 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_33_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24483 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_35_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24951 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_37_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21251 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_7_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    72926 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_9_1.png
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.499152 pyesmda-0.4.3/docs/build/html/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.519152 pyesmda-0.4.3/docs/build/html/_images/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    71733 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_12_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28238 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_15_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    28594 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_20_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21296 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_24_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    19817 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_28_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    23144 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_30_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21943 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_33_2.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24483 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_35_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    24951 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_37_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    21251 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_7_1.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    72926 2023-08-03 16:43:58.000000 pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_9_1.png
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.519152 pyesmda-0.4.3/docs/build/html/_static/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      286 2022-12-06 09:06:20.000000 pyesmda-0.4.3/docs/build/html/_static/file.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       90 2022-12-06 09:06:20.000000 pyesmda-0.4.3/docs/build/html/_static/minus.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       90 2022-12-06 09:06:20.000000 pyesmda-0.4.3/docs/build/html/_static/plus.png
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      773 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/make.bat
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.523152 pyesmda-0.4.3/docs/source/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.523152 pyesmda-0.4.3/docs/source/_autosummary/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1278 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.ESMDA.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1463 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.ESMDA_RS.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      126 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.approximate_cov_mm.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      208 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.approximate_covariance_matrix_from_ensembles.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      149 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.check_nans_in_predictions.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      240 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.compute_ensemble_average_normalized_objective_function.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      185 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.compute_normalized_objective_function.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      184 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.distances_to_weights_beta_cumulative.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      172 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.distances_to_weights_fifth_order.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      135 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.get_ensemble_variance.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      172 2023-08-03 16:43:55.000000 pyesmda-0.4.3/docs/source/_autosummary/pyesmda.inflate_ensemble_around_its_mean.rst
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.523152 pyesmda-0.4.3/docs/source/_templates/
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.523152 pyesmda-0.4.3/docs/source/_templates/autosummary/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      106 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      735 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1098 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      735 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/source/_templates/class.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1079 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1098 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/source/_templates/module.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      113 2023-08-03 17:09:47.000000 pyesmda-0.4.3/docs/source/api_reference.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       31 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/source/authors.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       76 2023-08-03 17:09:47.000000 pyesmda-0.4.3/docs/source/bibliography.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       33 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/source/changelog.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    14867 2023-06-28 13:57:41.000000 pyesmda-0.4.3/docs/source/conf.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       36 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/source/contributing.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      458 2022-08-11 22:32:41.000000 pyesmda-0.4.3/docs/source/index.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1138 2022-08-11 22:32:41.000000 pyesmda-0.4.3/docs/source/installation.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       30 2022-08-11 22:03:08.000000 pyesmda-0.4.3/docs/source/readme.rst
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      288 2022-08-12 09:15:56.000000 pyesmda-0.4.3/docs/source/usage.rst
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.527152 pyesmda-0.4.3/pyesmda/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       96 2023-08-03 17:09:47.000000 pyesmda-0.4.3/pyesmda/__about__.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     2165 2023-08-03 17:09:47.000000 pyesmda-0.4.3/pyesmda/__init__.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    26034 2023-08-03 17:09:47.000000 pyesmda-0.4.3/pyesmda/base.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    17412 2023-08-03 17:09:47.000000 pyesmda-0.4.3/pyesmda/esmda.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    18467 2023-08-03 17:09:47.000000 pyesmda-0.4.3/pyesmda/esmda_rs.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     4201 2023-08-03 17:09:47.000000 pyesmda-0.4.3/pyesmda/localization.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     7865 2023-08-03 17:09:47.000000 pyesmda-0.4.3/pyesmda/utils.py
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.527152 pyesmda-0.4.3/pyesmda.egg-info/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    11003 2023-08-03 17:13:20.000000 pyesmda-0.4.3/pyesmda.egg-info/PKG-INFO
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     3546 2023-08-03 17:13:20.000000 pyesmda-0.4.3/pyesmda.egg-info/SOURCES.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        1 2023-08-03 17:13:20.000000 pyesmda-0.4.3/pyesmda.egg-info/dependency_links.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        1 2023-08-03 17:13:20.000000 pyesmda-0.4.3/pyesmda.egg-info/not-zip-safe
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       25 2023-08-03 17:13:20.000000 pyesmda-0.4.3/pyesmda.egg-info/requires.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)       14 2023-08-03 17:13:20.000000 pyesmda-0.4.3/pyesmda.egg-info/top_level.txt
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)      172 2023-08-03 17:09:47.000000 pyesmda-0.4.3/pyproject.toml
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     1481 2023-08-03 17:13:20.527152 pyesmda-0.4.3/setup.cfg
+drwxr-xr-x   0 acollet  (27416) GEOSCIENCES (20042)        0 2023-08-03 17:13:20.527152 pyesmda-0.4.3/tests/
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)        0 2022-03-01 14:30:06.000000 pyesmda-0.4.3/tests/__init__.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)    14543 2023-08-03 17:09:47.000000 pyesmda-0.4.3/tests/test_esmda.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     5122 2023-08-03 17:09:47.000000 pyesmda-0.4.3/tests/test_esmda_rs.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     2791 2023-08-03 17:09:47.000000 pyesmda-0.4.3/tests/test_localization.py
+-rw-r--r--   0 acollet  (27416) GEOSCIENCES (20042)     5136 2023-06-28 13:57:41.000000 pyesmda-0.4.3/tests/test_utils.py
```

### Comparing `pyesmda-0.4.2/CHANGELOG.rst` & `pyesmda-0.4.3/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 ==============
 Changelog
 ==============
 
+0.4.3 (2023-08-03)
+------------------
+
+* `!PR39 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/39>`_ ENH: introduce abstraction through a base class and remove some code duplication (see solve methods) and remove some conflicts around the inflation parameters.
+  ESMDA-RS now supports local update (**batch_size** and **is_parallel_analyse_step**) and initial inflation of the ensemble (**cov_mm_inflation_factor**). The keyword `seed` has been replaced by a more flexible `random_state`, that accepts
+  **np.random.RandomState** and **Generator** in addition to classic seeds. In ESMDA-RS, the **std_m_prior** is no longer mandatory and can be omitted. In that case,
+  the initial adjusted parameter variance is estimated from the ensemble.
+
 0.4.2 (2023-08-02)
 ------------------
 
 * `!PR36 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/36>`_ ENH: add some correlation functions.
 * Also add new hooks in pre-commit.
 
 0.4.1 (2023-07-31)
```

### Comparing `pyesmda-0.4.2/CONTRIBUTING.rst` & `pyesmda-0.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/LICENSE` & `pyesmda-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/PKG-INFO` & `pyesmda-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesmda
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python Ensemble Smoother with Multiple Data Assimilation.
 Home-page: https://gitlab.com/antoinecollet5/pyesmda
 Author: attr: pyesmda.__author__
 Author-email: antoinecollet5@gmail.com
 License: MIT license
 Keywords: esmda,es-mda,inversion,inverse problem,parameter estimation,stochastic-optimization,ensemble smoother
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -91,15 +91,15 @@
 * Documentation: https://pyesmda.readthedocs.io.
 
 How to Cite
 -----------
 
 **Software/Code citation for pyESMDA:**
 
-Antoine Collet. (2023). pyESMDA - Python Ensemble Smoother with Multiple Data Assimilation (v0.4.2). Zenodo. https://doi.org/10.5281/zenodo.7425670
+Antoine Collet. (2023). pyESMDA - Python Ensemble Smoother with Multiple Data Assimilation (v0.4.3). Zenodo. https://doi.org/10.5281/zenodo.7425670
 
 
 References
 ----------
 
 * [1] Emerick, A. A. and A. C. Reynolds, Ensemble smoother with multiple
   data assimilation, Computers & Geosciences, 2012.
@@ -109,14 +109,22 @@
   Engineers - SPE Reservoir Simulation Symposium
   1.    2. 10.2118/163675-MS.
 
 ==============
 Changelog
 ==============
 
+0.4.3 (2023-08-03)
+------------------
+
+* `!PR39 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/39>`_ ENH: introduce abstraction through a base class and remove some code duplication (see solve methods) and remove some conflicts around the inflation parameters.
+  ESMDA-RS now supports local update (**batch_size** and **is_parallel_analyse_step**) and initial inflation of the ensemble (**cov_mm_inflation_factor**). The keyword `seed` has been replaced by a more flexible `random_state`, that accepts
+  **np.random.RandomState** and **Generator** in addition to classic seeds. In ESMDA-RS, the **std_m_prior** is no longer mandatory and can be omitted. In that case,
+  the initial adjusted parameter variance is estimated from the ensemble.
+
 0.4.2 (2023-08-02)
 ------------------
 
 * `!PR36 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/36>`_ ENH: add some correlation functions.
 * Also add new hooks in pre-commit.
 
 0.4.1 (2023-07-31)
```

### Comparing `pyesmda-0.4.2/README.rst` & `pyesmda-0.4.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 * Documentation: https://pyesmda.readthedocs.io.
 
 How to Cite
 -----------
 
 **Software/Code citation for pyESMDA:**
 
-Antoine Collet. (2023). pyESMDA - Python Ensemble Smoother with Multiple Data Assimilation (v0.4.2). Zenodo. https://doi.org/10.5281/zenodo.7425670
+Antoine Collet. (2023). pyESMDA - Python Ensemble Smoother with Multiple Data Assimilation (v0.4.3). Zenodo. https://doi.org/10.5281/zenodo.7425670
 
 
 References
 ----------
 
 * [1] Emerick, A. A. and A. C. Reynolds, Ensemble smoother with multiple
   data assimilation, Computers & Geosciences, 2012.
```

### Comparing `pyesmda-0.4.2/docs/Makefile` & `pyesmda-0.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_12_1.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_12_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_15_2.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_15_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_20_1.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_20_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_24_2.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_24_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_28_2.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_28_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_30_1.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_30_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_33_2.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_33_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_35_1.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_35_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_37_1.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_37_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_7_1.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_7_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_9_1.png` & `pyesmda-0.4.3/docs/build/doctrees/nbsphinx/tutorials_correlation_matrices_building_9_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_12_1.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_12_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_15_2.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_15_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_20_1.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_20_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_24_2.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_24_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_28_2.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_28_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_30_1.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_30_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_33_2.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_33_2.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_35_1.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_35_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_37_1.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_37_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_7_1.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_7_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/build/html/_images/tutorials_correlation_matrices_building_9_1.png` & `pyesmda-0.4.3/docs/build/html/_images/tutorials_correlation_matrices_building_9_1.png`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/make.bat` & `pyesmda-0.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/source/_autosummary/pyesmda.ESMDA.rst` & `pyesmda-0.4.3/docs/source/_autosummary/pyesmda.ESMDA.rst`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,14 @@
       ~ESMDA._apply_bounds
       ~ESMDA._approximate_covariance_matrices
       ~ESMDA._forecast
       ~ESMDA._get_batch_m_update
       ~ESMDA._local_analyse
       ~ESMDA._pertrub
       ~ESMDA._set_n_assimilations
-      ~ESMDA._solve
-      ~ESMDA._solve_locally
       ~ESMDA.set_cov_obs_inflation_factors
       ~ESMDA.solve
    
    
    
 
    .. rubric:: Methods definition
```

### Comparing `pyesmda-0.4.2/docs/source/_autosummary/pyesmda.ESMDA_RS.rst` & `pyesmda-0.4.3/docs/source/_autosummary/pyesmda.ESMDA_RS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,13 @@
       ~ESMDA_RS._forecast
       ~ESMDA_RS._get_batch_m_update
       ~ESMDA_RS._is_unity_reached
       ~ESMDA_RS._is_valid_parameter_change
       ~ESMDA_RS._local_analyse
       ~ESMDA_RS._pertrub
       ~ESMDA_RS._set_n_assimilations
-      ~ESMDA_RS._solve
-      ~ESMDA_RS._solve_locally
-      ~ESMDA_RS.set_cov_obs_inflation_factors
       ~ESMDA_RS.solve
    
    
    
 
    .. rubric:: Methods definition
```

### Comparing `pyesmda-0.4.2/docs/source/_templates/autosummary/class.rst` & `pyesmda-0.4.3/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/source/_templates/autosummary/module.rst` & `pyesmda-0.4.3/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/source/_templates/class.rst` & `pyesmda-0.4.3/docs/source/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/source/_templates/custom-module-template.rst` & `pyesmda-0.4.3/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/source/_templates/module.rst` & `pyesmda-0.4.3/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/source/conf.py` & `pyesmda-0.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/docs/source/installation.rst` & `pyesmda-0.4.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/pyesmda/__init__.py` & `pyesmda-0.4.3/pyesmda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/pyesmda/esmda.py` & `pyesmda-0.4.3/pyesmda/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
-Implement the ES-MDA algorithms.
+Implement a base class for the ES-MDA algorithms and variants.
 
 @author: acollet
 """
+import warnings
+from abc import ABC, abstractmethod
 from concurrent.futures import ProcessPoolExecutor
 from typing import Any, Callable, Dict, Iterator, List, Optional, Sequence, Union
 
 import numpy as np
+from scipy._lib._util import check_random_state  # To handle random_state
 from scipy.sparse import csr_matrix
 
 from pyesmda.utils import (
     NDArrayFloat,
     approximate_cov_mm,
     approximate_covariance_matrix_from_ensembles,
     check_nans_in_predictions,
-    inflate_ensemble_around_its_mean,
 )
 
 # pylint: disable=C0103 # Does not conform to snake_case naming style
 
 
-class ESMDA:
+class ESMDABase(ABC):
     r"""
     Ensemble Smoother with Multiple Data Assimilation.
 
     Implement the ES-MDA as proposed by  Emerick, A. A. and A. C. Reynolds
     :cite:p:`emerickEnsembleSmootherMultiple2013,
     emerickHistoryMatchingProductionSeismic2013`.
 
@@ -130,16 +132,14 @@
         "cov_md",
         "cov_dd",
         "forward_model",
         "forward_model_args",
         "forward_model_kwargs",
         "_n_assimilations",
         "_assimilation_step",
-        "_cov_obs_inflation_factors",
-        "_cov_mm_inflation_factors",
         "_dd_correlation_matrix",
         "_md_correlation_matrix",
         "save_ensembles_history",
         "rng",
         "is_forecast_for_last_assimilation",
         "batch_size",
         "is_parallel_analyse_step",
@@ -150,22 +150,23 @@
         obs: NDArrayFloat,
         m_init: NDArrayFloat,
         cov_obs: Union[NDArrayFloat, csr_matrix],
         forward_model: Callable[..., NDArrayFloat],
         forward_model_args: Sequence[Any] = (),
         forward_model_kwargs: Optional[Dict[str, Any]] = None,
         n_assimilations: int = 4,
-        cov_obs_inflation_factors: Optional[Sequence[float]] = None,
-        cov_mm_inflation_factors: Optional[Sequence[float]] = None,
         dd_correlation_matrix: Optional[Union[NDArrayFloat, csr_matrix]] = None,
         md_correlation_matrix: Optional[Union[NDArrayFloat, csr_matrix]] = None,
         m_bounds: Optional[NDArrayFloat] = None,
         save_ensembles_history: bool = False,
         seed: Optional[int] = None,
         is_forecast_for_last_assimilation: bool = True,
+        random_state: Optional[
+            Union[int, np.random.Generator, np.random.RandomState]
+        ] = 198873,
         batch_size: int = 5000,
         is_parallel_analyse_step: bool = True,
     ) -> None:
         # pylint: disable=R0913 # Too many arguments
         # pylint: disable=R0914 # Too many local variables
         r"""Construct the instance.
 
@@ -186,28 +187,14 @@
             each ensemble member.
         forward_model_args: Optional[Tuple[Any]]
             Additional args for the callable forward_model. The default is None.
         forward_model_kwargs: Optional[Dict[str, Any]]
             Additional kwargs for the callable forward_model. The default is None.
         n_assimilations : int, optional
             Number of data assimilations (:math:`N_{a}`). The default is 4.
-        cov_obs_inflation_factors : Optional[Sequence[float]]
-            Multiplication factor used to inflate the covariance matrix of the
-            measurement errors.
-            Must match the number of data assimilations (:math:`N_{a}`).
-            The default is None.
-        cov_mm_inflation_factors: Optional[Sequence[float]]
-            List of factors used to inflate the adjusted parameters covariance
-            among iterations:
-            Each realization of the ensemble at the end of each update step i,
-            is linearly inflated around its mean.
-            Must match the number of data assimilations (:math:`N_{a}`).
-            See :cite:p:`andersonExploringNeedLocalization2007`.
-            If None, the default is 1.0. at each iteration (no inflation).
-            The default is None.
         dd_correlation_matrix : Optional[NDArrayFloat]
             Correlation matrix based on spatial and temporal distances between
             observations and observations :math:`\rho_{DD}`. It is used to localize the
             autocovariance matrix of predicted data by applying an elementwise
             multiplication by this matrix.
             Expected dimensions are (:math:`N_{obs}`, :math:`N_{obs}`).
             The default is None.
@@ -223,20 +210,27 @@
             Lower and upper bounds for the :math:`N_{m}` parameter values.
             Expected dimensions are (:math:`N_{m}`, 2) with lower bounds on the first
             column and upper on the second one. The default is None.
         save_ensembles_history: bool, optional
             Whether to save the history predictions and parameters over
             the assimilations. The default is False.
         seed: Optional[int]
-            Seed for the white noise generator used in the perturbation step.
-            If None, the default :func:`numpy.random.default_rng()` is used.
-            The default is None.
+            .. deprecated:: 0.4.2
+            Since 0.4.2, you can use the parameter `random_state` instead.
         is_forecast_for_last_assimilation: bool, optional
             Whether to compute the predictions for the ensemble obtained at the
             last assimilation step. The default is True.
+        random_state: Optional[Union[int, np.random.Generator, np.random.RandomState]]
+            Pseudorandom number generator state used to generate resamples.
+            If `random_state` is ``None`` (or `np.random`), the
+            `numpy.random.RandomState` singleton is used.
+            If `random_state` is an int, a new ``RandomState`` instance is used,
+            seeded with `random_state`.
+            If `random_state` is already a ``Generator`` or ``RandomState``
+            instance then that instance is used.
         batch_size: int
             Number of parameters that are assimilated at once. This option is
             available to overcome memory limitations when the number of parameters is
             large. In that case, the size of the covariance matrices tends to explode
             and the update step must be performed by chunks of parameters.
             The default is 5000.
         is_parallel_analyse_step: bool, optional
@@ -258,20 +252,25 @@
         self.forward_model: Callable = forward_model
         self.forward_model_args: Sequence[Any] = forward_model_args
         if forward_model_kwargs is None:
             forward_model_kwargs = {}
         self.forward_model_kwargs: Dict[str, Any] = forward_model_kwargs
         self._set_n_assimilations(n_assimilations)
         self._assimilation_step: int = 0
-        self.set_cov_obs_inflation_factors(cov_obs_inflation_factors)
-        self.cov_mm_inflation_factors = cov_mm_inflation_factors
         self.dd_correlation_matrix = dd_correlation_matrix
         self.md_correlation_matrix = md_correlation_matrix
         self.m_bounds = m_bounds
-        self.rng: np.random.Generator = np.random.default_rng(seed)
+        if seed is not None:
+            warnings.warn(
+                DeprecationWarning(
+                    "The keyword `seed` is now replaced by `random_state` "
+                    "and will be dropped in 0.5.x."
+                )
+            )
+        self.rng: np.random.RandomState = check_random_state(random_state)
         self.is_forecast_for_last_assimilation = is_forecast_for_last_assimilation
         self.batch_size = batch_size
         self.is_parallel_analyse_step = is_parallel_analyse_step
 
     @property
     def n_assimilations(self) -> int:
         """Return the number of assimilations to perform. Read-only attribute."""
@@ -357,83 +356,14 @@
                 f"m_bounds is of shape {mb.shape} while it "
                 f"should be of shape ({self.m_dim}, 2)"
             )
         else:
             self._m_bounds = mb
 
     @property
-    def cov_obs_inflation_factors(self) -> List[float]:
-        r"""
-        Get the inlfation factors for the covariance matrix of the measurement errors.
-
-        Single and multiple data assimilation are equivalent for the
-        linear-Gaussian case as long as the factor :math:`\alpha_{l}` used to
-        inflate the covariance matrix of the measurement errors satisfy the
-        following condition:
-
-        .. math::
-            \sum_{l=1}^{N_{a}} \frac{1}{\alpha_{l}} = 1
-
-        In practise, :math:`\alpha_{l} = N_{a}` is a good choice
-        :cite:p:`emerickEnsembleSmootherMultiple2013`.
-        """
-        return self._cov_obs_inflation_factors
-
-    def set_cov_obs_inflation_factors(self, a: Optional[Sequence[float]]) -> None:
-        """Set the inflation factors the covariance matrix of the measurement errors."""
-        if a is None:
-            self._cov_obs_inflation_factors: List[float] = [
-                1 / self.n_assimilations
-            ] * self.n_assimilations
-        elif len(a) != self.n_assimilations:
-            raise ValueError(
-                "The length of cov_obs_inflation_factors should match n_assimilations"
-            )
-        else:
-            self._cov_obs_inflation_factors = list(a)
-
-    @property
-    def cov_mm_inflation_factors(self) -> List[float]:
-        r"""
-        Get the inlfation factors for the adjusted parameters covariance matrix.
-
-        Covariance inflation is a method used to counteract the tendency of ensemble
-        Kalman methods to underestimate the uncertainty because of either undersampling,
-        inbreeding, or spurious correlations
-        :cite:p:`todaroAdvancedTechniquesSolving2021`.
-        The spread of the ensemble is artificially increased before the assimilation
-        of the observations, according to scheme introduced by
-        :cite:`andersonExploringNeedLocalization2007`:
-
-        .. math::
-            m^{l}_{j} \leftarrow r^{l}\left(m^{l}_{j} - \frac{1}{N_{e}}
-            \sum_{j}^{N_{e}}m^{l}_{j}\right) + \frac{1}{N_{e}}\sum_{j}^{N_{e}}m^{l}_{j}
-
-        where :math:`r` is the inflation factor for the assimilation step :math:`l`.
-        """
-        return list(self._cov_mm_inflation_factors)
-
-    @cov_mm_inflation_factors.setter
-    def cov_mm_inflation_factors(self, a: Optional[Sequence[float]]) -> None:
-        """
-        Set the inflation factors the adjusted parameters covariance matrix.
-
-        If no values have been provided by the user, the default is 1.0. at
-        each iteration (no inflation).
-        """
-        if a is None:
-            self._cov_mm_inflation_factors: List[float] = [1.0] * self.n_assimilations
-        elif len(a) != self.n_assimilations:
-            raise ValueError(
-                "The length of cov_mm_inflation_factors should match n_assimilations"
-            )
-        else:
-            self._cov_mm_inflation_factors = list(a)
-
-    @property
     def dd_correlation_matrix(self) -> Optional[csr_matrix]:
         """Get the observations-observations localization matrix."""
         return self._dd_correlation_matrix
 
     @dd_correlation_matrix.setter
     def dd_correlation_matrix(
         self, s: Optional[Union[NDArrayFloat, csr_matrix]]
@@ -475,82 +405,18 @@
         self._md_correlation_matrix: Optional[csr_matrix] = csr_matrix(s)
 
     @property
     def n_batches(self) -> int:
         """Number of batch used in the optimization."""
         return int(self.m_dim / self.batch_size) + 1
 
+    @abstractmethod
     def solve(self) -> None:
         """Solve the optimization problem with ES-MDA algorithm."""
-        if self.n_batches == 1:
-            self._solve()
-        else:
-            # assimilate chunk of parameters rather than everything all at once.
-            self._solve_locally()
-
-    def _solve(self) -> None:
-        """Solve the optimization problem with ES-MDA algorithm."""
-        if self.save_ensembles_history:
-            self.m_history.append(self.m_prior)  # save m_init
-        for self._assimilation_step in range(self.n_assimilations):
-            print(f"Assimilation # {self._assimilation_step + 1}")
-            # inflating the covariance
-            self.m_prior = self._apply_bounds(
-                inflate_ensemble_around_its_mean(
-                    self.m_prior,
-                    self.cov_mm_inflation_factors[self._assimilation_step],
-                )
-            )
-            self._forecast()
-            self._pertrub(self.cov_obs_inflation_factors[self._assimilation_step])
-            self._approximate_covariance_matrices()
-            # Update the prior parameter for next iteration
-            self.m_prior = self._apply_bounds(
-                self._analyse(self.cov_obs_inflation_factors[self._assimilation_step])
-            )
-            # Saving the parameters history
-            if self.save_ensembles_history:
-                self.m_history.append(self.m_prior)
-
-        if self.is_forecast_for_last_assimilation:
-            self._forecast()
-
-    def _solve_locally(self) -> None:
-        """Solve the optimization problem with ES-MDA algorithm."""
-        if self.save_ensembles_history:
-            self.m_history.append(self.m_prior)  # save m_init
-        for self._assimilation_step in range(self.n_assimilations):
-            print(f"Assimilation # {self._assimilation_step + 1}")
-            self._forecast()
-            self._pertrub(self.cov_obs_inflation_factors[self._assimilation_step])
-
-            # covariance approximation dd
-            self.cov_dd = approximate_covariance_matrix_from_ensembles(
-                self.d_pred, self.d_pred
-            )
-            # Spatial and temporal localization: obs - obs
-            if self.dd_correlation_matrix is not None:
-                self.cov_dd = self.dd_correlation_matrix.multiply(self.cov_dd).toarray()
-
-            # Update the prior parameter for next iteration
-            self.m_prior = self._apply_bounds(
-                inflate_ensemble_around_its_mean(
-                    self._local_analyse(
-                        self.cov_obs_inflation_factors[self._assimilation_step]
-                    ),
-                    self.cov_mm_inflation_factors[self._assimilation_step],
-                )
-            )
-
-            # Saving the parameters history
-            if self.save_ensembles_history:
-                self.m_history.append(self.m_prior)
-
-        if self.is_forecast_for_last_assimilation:
-            self._forecast()
+        ...  # pragma: no cover
 
     def _forecast(self) -> None:
         r"""
         Forecast step of ES-MDA.
 
         Run the forward model from time zero until the end of the historical
         period from time zero until the end of the historical period to
```

### Comparing `pyesmda-0.4.2/pyesmda/esmda_rs.py` & `pyesmda-0.4.3/pyesmda/esmda.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,233 +1,260 @@
 """
-Implement the ES-MDA-RS algorithms.
+Implement the ES-MDA algorithms.
 
 @author: acollet
 """
-from typing import Any, Callable, Dict, List, Optional, Sequence
+from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 import numpy as np
-import numpy.typing as npt
+from scipy.sparse import csr_matrix
 
-from pyesmda.esmda import ESMDA
-from pyesmda.utils import compute_ensemble_average_normalized_objective_function
+from pyesmda.base import ESMDABase
+from pyesmda.utils import (
+    NDArrayFloat,
+    approximate_covariance_matrix_from_ensembles,
+    inflate_ensemble_around_its_mean,
+)
 
 # pylint: disable=C0103 # Does not conform to snake_case naming style
 
 
-class ESMDA_RS(ESMDA):
+class ESMDA(ESMDABase):
     r"""
-    Restricted Step Ensemble Smoother with Multiple Data Assimilation.
+    Ensemble Smoother with Multiple Data Assimilation.
 
-    Implement an adaptative version of the original ES-MDA algorithm proposed by
-    Emerick, A. A. and A. C. Reynolds
+    Implement the ES-MDA as proposed by  Emerick, A. A. and A. C. Reynolds
     :cite:p:`emerickEnsembleSmootherMultiple2013,
-    emerickHistoryMatchingProductionSeismic2013`. This adaptative version introduced by
-    :cite:p:`leAdaptiveEnsembleSmoother2016` provides an automatic procedure for
-    choosing the inflation factor for the next data-assimilation step adaptively
-    as the history match proceeds. The procedure also decides when to stop,
-    i.e. the number of assimilation, which is no longer a user input.
+    emerickHistoryMatchingProductionSeismic2013`.
 
     Attributes
     ----------
     d_dim : int
         Number of observation values :math:`N_{obs}`, and consequently of
         predicted values.
-    obs : npt.NDArray[np.float64]
+    obs : NDArrayFloat
         Obsevrations vector with dimensions (:math:`N_{obs}`).
-    cov_obs: npt.NDArray[np.float64]
+    cov_obs: NDArrayFloat
         Covariance matrix of observed data measurement errors with dimensions
         (:math:`N_{obs}`, :math:`N_{obs}`). Also denoted :math:`R`.
-    std_m_prior: npt.NDArray[np.float64]
-        Vector of a priori standard deviation :math:`sigma` of the estimated
-        parameter. The expected dimension is (:math:`N_{m}`).
-        It is the diagonal of :math:`C_{M}`.
-    d_obs_uc: npt.NDArray[np.float64]
+    d_obs_uc: NDArrayFloat
         Vectors of pertubed observations with dimension
         (:math:`N_{e}`, :math:`N_{obs}`).
-    d_pred: npt.NDArray[np.float64]
+    d_pred: NDArrayFloat
         Vectors of predicted values (one for each ensemble member)
         with dimensions (:math:`N_{e}`, :math:`N_{obs}`).
-    d_history: List[npt.NDArray[np.float64]]
+    d_history: List[NDArrayFloat]
         List of vectors of predicted values obtained at each assimilation step.
     m_prior:
         Vectors of parameter values (one vector for each ensemble member) used in the
         last assimilation step. Dimensions are (:math:`N_{e}`, :math:`N_{m}`).
-    m_bounds : npt.NDArray[np.float64]
+    m_bounds : NDArrayFloat
         Lower and upper bounds for the :math:`N_{m}` parameter values.
         Expected dimensions are (:math:`N_{m}`, 2) with lower bounds on the first
         column and upper on the second one.
-    m_history: List[npt.NDArray[np.float64]]
+    m_history: List[NDArrayFloat]
         List of successive `m_prior`.
-    cov_md: npt.NDArray[np.float64]
+    cov_md: NDArrayFloat
         Cross-covariance matrix between the forecast state vector and predicted data.
         Dimensions are (:math:`N_{m}, N_{obs}`).
-    cov_dd: npt.NDArray[np.float64]
+    cov_obs: csr_matrix
         Autocovariance matrix of predicted data.
         Dimensions are (:math:`N_{obs}, N_{obs}`).
-    cov_mm: npt.NDArray[np.float64]
+    cov_mm: NDArrayFloat
         Autocovariance matrix of estimated parameters.
         Dimensions are (:math:`N_{m}, N_{m}`).
     forward_model: callable
         Function calling the non-linear observation model (forward model)
         for all ensemble members and returning the predicted data for
         each ensemble member.
     forward_model_args: Tuple[Any]
         Additional args for the callable forward_model.
     forward_model_kwargs: Dict[str, Any]
         Additional kwargs for the callable forward_model.
     n_assimilations : int
-        Number of data assimilations (:math:`N_{a}`) performed.
-        Automatically determined. Initially at 0.
+        Number of data assimilations (:math:`N_{a}`).
     cov_obs_inflation_factors : List[float]
         List of multiplication factor used to inflate the covariance matrix of the
-        measurement errors. It is determined automatically.
+        measurement errors.
     cov_mm_inflation_factors: List[float]
         List of factors used to inflate the adjusted parameters covariance among
         iterations:
         Each realization of the ensemble at the end of each update step i,
         is linearly inflated around its mean.
         See :cite:p:`andersonExploringNeedLocalization2007`.
-    dd_correlation_matrix : Optional[npt.NDArray[np.float64]]
+    dd_correlation_matrix : Optional[Union[NDArrayFloat, csr_matrix]]
         Correlation matrix based on spatial and temporal distances between
         observations and observations :math:`\rho_{DD}`. It is used to localize the
         autocovariance matrix of predicted data by applying an elementwise
         multiplication by this matrix.
-        Expected dimensions are (:math:`N_{obs}`, :math:`N_{obs}`).
-    md_correlation_matrix : Optional[npt.NDArray[np.float64]]
+        Expected dimensions are (:math:`N_{obs}`, :math:`N_{obs}`). A sparse matrix
+        format can be provided to save some memory.
+    md_correlation_matrix : Optional[Union[NDArrayFloat, csr_matrix]]
         Correlation matrix based on spatial and temporal distances between
         parameters and observations :math:`\rho_{MD}`. It is used to localize the
         cross-covariance matrix between the forecast state vector (parameters)
         and predicted data by applying an elementwise
         multiplication by this matrix.
-        Expected dimensions are (:math:`N_{m}`, :math:`N_{obs}`).
+        Expected dimensions are (:math:`N_{m}`, :math:`N_{obs}`). . A sparse matrix
+        format can be provided to save some memory.
     save_ensembles_history: bool
         Whether to save the history predictions and parameters over the assimilations.
     rng: np.random.Generator
         The random number generator used in the predictions perturbation step.
     is_forecast_for_last_assimilation: bool
         Whether to compute the predictions for the ensemble obtained at the
         last assimilation step.
-    """
+    batch_size: int
+            Number of parameters that are assimilated at once. This option is
+            available to overcome memory limitations when the number of parameters is
+            large. In that case, the size of the covariance matrices tends to explode
+            and the update step must be performed by chunks of parameters.
+    is_parallel_analyse_step: bool, optional
+            Whether to use parallel computing for the analyse step if the number of
+            batch is above one. The default is True.
+    n_batches: int
+            Number of batches required during the update step.
 
+    """
     # pylint: disable=R0902 # Too many instance attributes
-    __slots__: List[str] = ["std_m_prior"]
+    __slots__: List[str] = [
+        "_cov_obs_inflation_factors",
+        "_cov_mm_inflation_factors",
+    ]
 
     def __init__(
         self,
-        obs: npt.NDArray[np.float64],
-        m_init: npt.NDArray[np.float64],
-        cov_obs: npt.NDArray[np.float64],
-        std_m_prior: npt.NDArray[np.float64],
-        forward_model: Callable[..., npt.NDArray[np.float64]],
+        obs: NDArrayFloat,
+        m_init: NDArrayFloat,
+        cov_obs: Union[NDArrayFloat, csr_matrix],
+        forward_model: Callable[..., NDArrayFloat],
         forward_model_args: Sequence[Any] = (),
         forward_model_kwargs: Optional[Dict[str, Any]] = None,
+        n_assimilations: int = 4,
+        cov_obs_inflation_factors: Optional[Sequence[float]] = None,
         cov_mm_inflation_factors: Optional[Sequence[float]] = None,
-        dd_correlation_matrix: Optional[npt.NDArray[np.float64]] = None,
-        md_correlation_matrix: Optional[npt.NDArray[np.float64]] = None,
-        m_bounds: Optional[npt.NDArray[np.float64]] = None,
+        dd_correlation_matrix: Optional[Union[NDArrayFloat, csr_matrix]] = None,
+        md_correlation_matrix: Optional[Union[NDArrayFloat, csr_matrix]] = None,
+        m_bounds: Optional[NDArrayFloat] = None,
         save_ensembles_history: bool = False,
         seed: Optional[int] = None,
         is_forecast_for_last_assimilation: bool = True,
+        random_state: Optional[
+            Union[int, np.random.Generator, np.random.RandomState]
+        ] = 198873,
+        batch_size: int = 5000,
+        is_parallel_analyse_step: bool = True,
     ) -> None:
         # pylint: disable=R0913 # Too many arguments
         # pylint: disable=R0914 # Too many local variables
         r"""Construct the instance.
 
         Parameters
         ----------
-        obs : npt.NDArray[np.float64]
+        obs : NDArrayFloat
             Obsevrations vector with dimension :math:`N_{obs}`.
-        m_init : npt.NDArray[np.float64]
+        m_init : NDArrayFloat
             Initial ensemble of parameters vector with dimensions
             (:math:`N_{e}`, :math:`N_{m}`).
-        cov_obs: npt.NDArray[np.float64]
+        cov_obs: NDArrayFloat
             Covariance matrix of observed data measurement errors with dimensions
             (:math:`N_{obs}`, :math:`N_{obs}`). Also denoted :math:`R`.
-        std_m_prior: npt.NDArray[np.float64]
-            Vector of a priori standard deviation :math:`sigma` of the estimated
-            parameter. The expected dimension is (:math:`N_{m}`).
-            It is the diagonal of :math:`C_{M}`.
+            It can be a numpy array or a sparse matrix (scipy.linalg).
         forward_model: callable
             Function calling the non-linear observation model (forward model)
             for all ensemble members and returning the predicted data for
             each ensemble member.
         forward_model_args: Optional[Tuple[Any]]
             Additional args for the callable forward_model. The default is None.
         forward_model_kwargs: Optional[Dict[str, Any]]
             Additional kwargs for the callable forward_model. The default is None.
+        n_assimilations : int, optional
+            Number of data assimilations (:math:`N_{a}`). The default is 4.
+        cov_obs_inflation_factors : Optional[Sequence[float]]
+            Multiplication factor used to inflate the covariance matrix of the
+            measurement errors.
+            Must match the number of data assimilations (:math:`N_{a}`).
+            The default is None.
         cov_mm_inflation_factors: Optional[Sequence[float]]
             List of factors used to inflate the adjusted parameters covariance
             among iterations:
             Each realization of the ensemble at the end of each update step i,
             is linearly inflated around its mean.
             Must match the number of data assimilations (:math:`N_{a}`).
             See :cite:p:`andersonExploringNeedLocalization2007`.
             If None, the default is 1.0. at each iteration (no inflation).
             The default is None.
-        dd_correlation_matrix : Optional[npt.NDArray[np.float64]]
+        dd_correlation_matrix : Optional[NDArrayFloat]
             Correlation matrix based on spatial and temporal distances between
             observations and observations :math:`\rho_{DD}`. It is used to localize the
             autocovariance matrix of predicted data by applying an elementwise
             multiplication by this matrix.
             Expected dimensions are (:math:`N_{obs}`, :math:`N_{obs}`).
             The default is None.
-        md_correlation_matrix : Optional[npt.NDArray[np.float64]]
+        md_correlation_matrix : Optional[NDArrayFloat]
             Correlation matrix based on spatial and temporal distances between
             parameters and observations :math:`\rho_{MD}`. It is used to localize the
             cross-covariance matrix between the forecast state vector (parameters)
             and predicted data by applying an elementwise
             multiplication by this matrix.
             Expected dimensions are (:math:`N_{m}`, :math:`N_{obs}`).
             The default is None.
-        m_bounds : Optional[npt.NDArray[np.float64]], optional
+        m_bounds : Optional[NDArrayFloat], optional
             Lower and upper bounds for the :math:`N_{m}` parameter values.
             Expected dimensions are (:math:`N_{m}`, 2) with lower bounds on the first
             column and upper on the second one. The default is None.
         save_ensembles_history: bool, optional
             Whether to save the history predictions and parameters over
             the assimilations. The default is False.
         seed: Optional[int]
-            Seed for the white noise generator used in the perturbation step.
-            If None, the default :func:`numpy.random.default_rng()` is used.
-            The default is None.
+            .. deprecated:: 0.4.2
+                Since 0.4.2, you can use the parameter `random_state` instead.
         is_forecast_for_last_assimilation: bool, optional
             Whether to compute the predictions for the ensemble obtained at the
             last assimilation step. The default is True.
+        random_state: Optional[Union[int, np.random.Generator, np.random.RandomState]]
+            Pseudorandom number generator state used to generate resamples.
+            If `random_state` is ``None`` (or `np.random`), the
+            `numpy.random.RandomState` singleton is used.
+            If `random_state` is an int, a new ``RandomState`` instance is used,
+            seeded with `random_state`.
+            If `random_state` is already a ``Generator`` or ``RandomState``
+            instance then that instance is used.
+        batch_size: int
+            Number of parameters that are assimilated at once. This option is
+            available to overcome memory limitations when the number of parameters is
+            large. In that case, the size of the covariance matrices tends to explode
+            and the update step must be performed by chunks of parameters.
+            The default is 5000.
+        is_parallel_analyse_step: bool, optional
+            Whether to use parallel computing for the analyse step if the number of
+            batch is above one. It relies on `concurrent.futures` multiprocessing.
+            The default is True.
 
         """
-        self.obs: npt.NDArray[np.float64] = obs
-        self.m_prior: npt.NDArray[np.float64] = m_init
-        self.save_ensembles_history: bool = save_ensembles_history
-        self.m_history: list[npt.NDArray[np.float64]] = []
-        self.d_history: list[npt.NDArray[np.float64]] = []
-        self.d_pred: npt.NDArray[np.float64] = np.zeros([self.n_ensemble, self.d_dim])
-        self.cov_obs = cov_obs
-        self.std_m_prior: npt.NDArray[np.float64] = std_m_prior
-        self.d_obs_uc: npt.NDArray[np.float64] = np.array([])
-        self.cov_md: npt.NDArray[np.float64] = np.array([])
-        self.cov_dd: npt.NDArray[np.float64] = np.array([])
-        self.forward_model: Callable = forward_model
-        self.forward_model_args: Sequence[Any] = forward_model_args
-        if forward_model_kwargs is None:
-            forward_model_kwargs = {}
-        self.forward_model_kwargs: Dict[str, Any] = forward_model_kwargs
-        self._assimilation_step: int = 0
-        self.cov_obs_inflation_factors = []
+        super().__init__(
+            obs=obs,
+            m_init=m_init,
+            cov_obs=cov_obs,
+            forward_model=forward_model,
+            forward_model_args=forward_model_args,
+            forward_model_kwargs=forward_model_kwargs,
+            n_assimilations=n_assimilations,
+            dd_correlation_matrix=dd_correlation_matrix,
+            md_correlation_matrix=md_correlation_matrix,
+            m_bounds=m_bounds,
+            save_ensembles_history=save_ensembles_history,
+            seed=seed,
+            is_forecast_for_last_assimilation=is_forecast_for_last_assimilation,
+            random_state=random_state,
+            batch_size=batch_size,
+            is_parallel_analyse_step=is_parallel_analyse_step,
+        )
+        self.set_cov_obs_inflation_factors(cov_obs_inflation_factors)
         self.cov_mm_inflation_factors = cov_mm_inflation_factors
-        self.dd_correlation_matrix = dd_correlation_matrix
-        self.md_correlation_matrix = md_correlation_matrix
-        self.m_bounds = m_bounds
-        self.rng: np.random.Generator = np.random.default_rng(seed)
-        self.is_forecast_for_last_assimilation = is_forecast_for_last_assimilation
-
-    @property
-    def n_assimilations(self) -> int:
-        """Get the number of assimilations performed. Read-only."""
-        return self._assimilation_step
 
     @property
     def cov_obs_inflation_factors(self) -> List[float]:
         r"""
         Get the inlfation factors for the covariance matrix of the measurement errors.
 
         Single and multiple data assimilation are equivalent for the
@@ -239,104 +266,105 @@
             \sum_{l=1}^{N_{a}} \frac{1}{\alpha_{l}} = 1
 
         In practise, :math:`\alpha_{l} = N_{a}` is a good choice
         :cite:p:`emerickEnsembleSmootherMultiple2013`.
         """
         return self._cov_obs_inflation_factors
 
-    @cov_obs_inflation_factors.setter
-    def cov_obs_inflation_factors(self, a: List[float]) -> None:
+    def set_cov_obs_inflation_factors(self, a: Optional[Sequence[float]]) -> None:
         """Set the inflation factors the covariance matrix of the measurement errors."""
-        self._cov_obs_inflation_factors = a
+        if a is None:
+            self._cov_obs_inflation_factors: List[float] = [
+                1 / self.n_assimilations
+            ] * self.n_assimilations
+        elif len(a) != self.n_assimilations:
+            raise ValueError(
+                "The length of cov_obs_inflation_factors should match n_assimilations"
+            )
+        else:
+            self._cov_obs_inflation_factors = list(a)
+
+    @property
+    def cov_mm_inflation_factors(self) -> List[float]:
+        r"""
+        Get the inlfation factors for the adjusted parameters covariance matrix.
+
+        Covariance inflation is a method used to counteract the tendency of ensemble
+        Kalman methods to underestimate the uncertainty because of either undersampling,
+        inbreeding, or spurious correlations
+        :cite:p:`todaroAdvancedTechniquesSolving2021`.
+        The spread of the ensemble is artificially increased before the assimilation
+        of the observations, according to scheme introduced by
+        :cite:`andersonExploringNeedLocalization2007`:
+
+        .. math::
+            m^{l}_{j} \leftarrow r^{l}\left(m^{l}_{j} - \frac{1}{N_{e}}
+            \sum_{j}^{N_{e}}m^{l}_{j}\right) + \frac{1}{N_{e}}\sum_{j}^{N_{e}}m^{l}_{j}
+
+        where :math:`r` is the inflation factor for the assimilation step :math:`l`.
+        """
+        return list(self._cov_mm_inflation_factors)
+
+    @cov_mm_inflation_factors.setter
+    def cov_mm_inflation_factors(self, a: Optional[Sequence[float]]) -> None:
+        """
+        Set the inflation factors the adjusted parameters covariance matrix.
+
+        If no values have been provided by the user, the default is 1.0. at
+        each iteration (no inflation).
+        """
+        if a is None:
+            self._cov_mm_inflation_factors: List[float] = [1.0] * self.n_assimilations
+        elif len(a) != self.n_assimilations:
+            raise ValueError(
+                "The length of cov_mm_inflation_factors should match n_assimilations"
+            )
+        else:
+            self._cov_mm_inflation_factors = list(a)
 
     def solve(self) -> None:
-        """Solve the optimization problem with ES-MDA-RS algorithm."""
+        """Solve the optimization problem with ES-MDA algorithm."""
         if self.save_ensembles_history:
             self.m_history.append(self.m_prior)  # save m_init
-
-        current_inflation_factor: float = 10.0  # to initiate the while
-        while not self._is_unity_reached(current_inflation_factor):
-            self._assimilation_step += 1
-            print(f"Assimilation # {self._assimilation_step}")
-            self._forecast()
-            # Divide per 2, because it is multiplied by 2 as the beginning
-            # of the second while loop
-            current_inflation_factor: float = (
-                self._compute_initial_inflation_factor() / 2
+        for self._assimilation_step in range(self.n_assimilations):
+            print(f"Assimilation # {self._assimilation_step + 1}")
+            # inflating the covariance
+            self.m_prior = self._apply_bounds(
+                inflate_ensemble_around_its_mean(
+                    self.m_prior,
+                    self.cov_mm_inflation_factors[self._assimilation_step],
+                )
             )
-            is_valid_parameter_change: bool = False
-            while not is_valid_parameter_change:
-                current_inflation_factor *= 2  # double the inflation (dumping) factor
-                self._pertrub(current_inflation_factor)
+            self._forecast()
+            self._pertrub(self.cov_obs_inflation_factors[self._assimilation_step])
+
+            if self.n_batches == 1:
                 self._approximate_covariance_matrices()
-                m_pred = self._apply_bounds(self._analyse(current_inflation_factor))
-                is_valid_parameter_change: bool = self._is_valid_parameter_change(
-                    m_pred
+                # Update the prior parameter for next iteration
+                self.m_prior = self._apply_bounds(
+                    self._analyse(
+                        self.cov_obs_inflation_factors[self._assimilation_step]
+                    )
                 )
-
-            # If the criteria is reached -> Get exactly one for the sum
-            if self._is_unity_reached(current_inflation_factor):
-                current_inflation_factor = 1 / (
-                    1 - np.sum([1 / a for a in self.cov_obs_inflation_factors])
+            else:
+                # covariance approximation dd
+                self.cov_dd = approximate_covariance_matrix_from_ensembles(
+                    self.d_pred, self.d_pred
                 )
-                self._pertrub(current_inflation_factor)
-                self._approximate_covariance_matrices()
-                m_pred = self._analyse(current_inflation_factor)
-                is_valid_parameter_change: bool = self._is_valid_parameter_change(
-                    m_pred
+                # Spatial and temporal localization: obs - obs
+                if self.dd_correlation_matrix is not None:
+                    self.cov_dd = self.dd_correlation_matrix.multiply(
+                        self.cov_dd
+                    ).toarray()
+
+                # Update the prior parameter for next iteration
+                self.m_prior = self._apply_bounds(
+                    self._local_analyse(
+                        self.cov_obs_inflation_factors[self._assimilation_step]
+                    )
                 )
-
-            self.cov_obs_inflation_factors.append(current_inflation_factor)
-            print(f"- Inflation factor = {current_inflation_factor:.3f}")
-
-            # Update the prior parameter for next iteration
-            self.m_prior = m_pred
             # Saving the parameters history
             if self.save_ensembles_history:
-                self.m_history.append(m_pred)
+                self.m_history.append(self.m_prior)
 
-        # Last assimilation
         if self.is_forecast_for_last_assimilation:
             self._forecast()
-
-    def _compute_initial_inflation_factor(self) -> float:
-        r"""Compute the :math:`\alpha_{l}` inflation (dumping) factor."""
-        return 0.25 * compute_ensemble_average_normalized_objective_function(
-            self.d_pred, self.obs, self.cov_obs
-        )
-
-    def _is_unity_reached(self, current_inflation_factor: float) -> bool:
-        """
-        Whether the sum of the inverse inflation factors is above one.
-
-        It includes all factors up to the current iteration.
-
-        Parameters
-        ----------
-        current_inflation_factor: float
-            Multiplication factor used to inflate the covariance matrix of the
-            measurement errors for the current (last) iteration.
-        """
-        return (
-            np.sum([1 / a for a in self.cov_obs_inflation_factors])
-            + 1 / current_inflation_factor
-            >= 1
-        )
-
-    def _is_valid_parameter_change(self, m_pred: npt.NDArray[np.float64]) -> bool:
-        """Check if all change residuals are below 2 sigma.
-
-        Parameters
-        ----------
-        m_pred : npt.NDArray[np.float64]
-            _description_
-
-        Returns
-        -------
-        bool
-            _description_
-        """
-
-        def is_lower(residuals) -> bool:
-            return np.all(residuals < 2 * self.std_m_prior)
-
-        return np.all(list(map(is_lower, np.abs(m_pred - self.m_prior))))
```

### Comparing `pyesmda-0.4.2/pyesmda/localization.py` & `pyesmda-0.4.3/pyesmda/localization.py`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/pyesmda/utils.py` & `pyesmda-0.4.3/pyesmda/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,19 @@
         return (
             1
             / (2 * obs.size)
             * np.dot(residuals.T, np.linalg.solve(cov_obs, residuals))
         )
     except Exception:
         # case of sparse matrices
-        return 1 / (2 * obs.size) * np.dot(residuals.T, gmres(cov_obs, residuals)[0])
+        return (
+            1
+            / (2 * obs.size)
+            * np.dot(residuals.T, gmres(cov_obs, residuals, atol=1e-15)[0])
+        )
 
 
 def inflate_ensemble_around_its_mean(
     ensemble: NDArrayFloat, inflation_factor: float
 ) -> NDArrayFloat:
     r"""
     Inflate the given parameter ensemble around its mean.
```

### Comparing `pyesmda-0.4.2/pyesmda.egg-info/PKG-INFO` & `pyesmda-0.4.3/pyesmda.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyesmda
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python Ensemble Smoother with Multiple Data Assimilation.
 Home-page: https://gitlab.com/antoinecollet5/pyesmda
 Author: attr: pyesmda.__author__
 Author-email: antoinecollet5@gmail.com
 License: MIT license
 Keywords: esmda,es-mda,inversion,inverse problem,parameter estimation,stochastic-optimization,ensemble smoother
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -91,15 +91,15 @@
 * Documentation: https://pyesmda.readthedocs.io.
 
 How to Cite
 -----------
 
 **Software/Code citation for pyESMDA:**
 
-Antoine Collet. (2023). pyESMDA - Python Ensemble Smoother with Multiple Data Assimilation (v0.4.2). Zenodo. https://doi.org/10.5281/zenodo.7425670
+Antoine Collet. (2023). pyESMDA - Python Ensemble Smoother with Multiple Data Assimilation (v0.4.3). Zenodo. https://doi.org/10.5281/zenodo.7425670
 
 
 References
 ----------
 
 * [1] Emerick, A. A. and A. C. Reynolds, Ensemble smoother with multiple
   data assimilation, Computers & Geosciences, 2012.
@@ -109,14 +109,22 @@
   Engineers - SPE Reservoir Simulation Symposium
   1.    2. 10.2118/163675-MS.
 
 ==============
 Changelog
 ==============
 
+0.4.3 (2023-08-03)
+------------------
+
+* `!PR39 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/39>`_ ENH: introduce abstraction through a base class and remove some code duplication (see solve methods) and remove some conflicts around the inflation parameters.
+  ESMDA-RS now supports local update (**batch_size** and **is_parallel_analyse_step**) and initial inflation of the ensemble (**cov_mm_inflation_factor**). The keyword `seed` has been replaced by a more flexible `random_state`, that accepts
+  **np.random.RandomState** and **Generator** in addition to classic seeds. In ESMDA-RS, the **std_m_prior** is no longer mandatory and can be omitted. In that case,
+  the initial adjusted parameter variance is estimated from the ensemble.
+
 0.4.2 (2023-08-02)
 ------------------
 
 * `!PR36 <https://gitlab.com/antoinecollet5/pyesmda/-/merge_requests/36>`_ ENH: add some correlation functions.
 * Also add new hooks in pre-commit.
 
 0.4.1 (2023-07-31)
```

### Comparing `pyesmda-0.4.2/pyesmda.egg-info/SOURCES.txt` & `pyesmda-0.4.3/pyesmda.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 docs/source/_templates/custom-module-template.rst
 docs/source/_templates/module.rst
 docs/source/_templates/autosummary/base.rst
 docs/source/_templates/autosummary/class.rst
 docs/source/_templates/autosummary/module.rst
 pyesmda/__about__.py
 pyesmda/__init__.py
+pyesmda/base.py
 pyesmda/esmda.py
 pyesmda/esmda_rs.py
 pyesmda/localization.py
 pyesmda/utils.py
 pyesmda.egg-info/PKG-INFO
 pyesmda.egg-info/SOURCES.txt
 pyesmda.egg-info/dependency_links.txt
```

### Comparing `pyesmda-0.4.2/setup.cfg` & `pyesmda-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/tests/test_esmda.py` & `pyesmda-0.4.3/tests/test_esmda.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,15 +345,15 @@
         np.average(solver.m_prior, axis=0), np.array([a, b]), rtol=5e-2
     ).all()
 
     # Get the uncertainty on the parameters
     a_std, b_std = np.sqrt(np.diagonal(solver.cov_mm))
 
     assert np.isclose(
-        np.array([a_std, b_std]), np.array([1.02e-1, 6.74e-5]), rtol=5e-2
+        np.array([a_std, b_std]), np.array([9.51e-2, 5.96e-5]), rtol=5e-2
     ).all()
 
 
 @pytest.mark.parametrize(
     "batch_size, is_parallel_analyse_step",
     [
         (
@@ -451,9 +451,9 @@
         np.average(solver.m_prior, axis=0), np.array([a, b]), rtol=5e-2
     ).all()
 
     # Get the uncertainty on the parameters
     a_std, b_std = np.sqrt(np.diagonal(solver.cov_mm))
 
     assert np.isclose(
-        np.array([a_std, b_std]), np.array([1.5e-1, 9.954e-5]), rtol=5e-2
+        np.array([a_std, b_std]), np.array([1.2e-1, 7.8e-5]), rtol=5e-2
     ).all()
```

### Comparing `pyesmda-0.4.2/tests/test_localization.py` & `pyesmda-0.4.3/tests/test_localization.py`

 * *Files identical despite different names*

### Comparing `pyesmda-0.4.2/tests/test_utils.py` & `pyesmda-0.4.3/tests/test_utils.py`

 * *Files identical despite different names*

