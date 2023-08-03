# Comparing `tmp/dspeed-1.1.0.tar.gz` & `tmp/dspeed-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspeed-1.1.0.tar", last modified: Wed May 24 15:37:41 2023, max compression
+gzip compressed data, was "dspeed-1.2.0.tar", last modified: Thu Aug  3 14:42:16 2023, max compression
```

## Comparing `dspeed-1.1.0.tar` & `dspeed-1.2.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.246807 dspeed-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 15:37:33.000000 dspeed-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-24 15:37:41.246807 dspeed-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-24 15:37:33.000000 dspeed-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-24 15:37:33.000000 dspeed-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-24 15:37:41.246807 dspeed-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-24 15:37:33.000000 dspeed-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.234807 dspeed-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.238807 dspeed-1.1.0/src/dspeed/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    72618 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processing_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.242807 dspeed-1.1.0/src/dspeed/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/bl_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/dplms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/dwt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/fftw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/gaussian_filter1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/linear_slope_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/log_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/min_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/moving_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/multi_a_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/multi_t_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/param_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/peak_snr_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/pole_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/presum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/pulse_injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/soft_pileup_corr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/time_over_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/time_point_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/trap_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/wiener_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/processors/windower.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.242807 dspeed-1.1.0/src/dspeed/vis/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-05-24 15:37:33.000000 dspeed-1.1.0/src/dspeed/vis/waveform_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.238807 dspeed-1.1.0/src/dspeed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 15:37:41.000000 dspeed-1.1.0/src/dspeed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.242807 dspeed-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.242807 dspeed-1.1.0/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/configs/icpc-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/configs/numpy-parsing.json
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/configs/sipm-dplms-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/configs/sipm-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.246807 dspeed-1.1.0/tests/processors/
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/dplms_noise_mat.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_dplms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_dwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_fftw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/processors/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_list_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_numpy_constants_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_processing_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.246807 dspeed-1.1.0/tests/vis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:37:41.246807 dspeed-1.1.0/tests/vis/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/vis/configs/hpge-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-24 15:37:33.000000 dspeed-1.1.0/tests/vis/test_waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.638967 dspeed-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 14:42:05.000000 dspeed-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-03 14:42:16.638967 dspeed-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-03 14:42:05.000000 dspeed-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-03 14:42:05.000000 dspeed-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-03 14:42:16.638967 dspeed-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-03 14:42:05.000000 dspeed-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.618967 dspeed-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.622967 dspeed-1.2.0/src/dspeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 14:42:16.000000 dspeed-1.2.0/src/dspeed/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72618 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processing_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.630967 dspeed-1.2.0/src/dspeed/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/bl_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/dplms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/fftw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/gaussian_filter1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/linear_slope_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/log_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/moving_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/multi_a_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/multi_t_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/param_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/peak_snr_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/pole_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/presum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/pulse_injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/soft_pileup_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/time_over_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/time_point_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/trap_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/wiener_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/processors/windower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.630967 dspeed-1.2.0/src/dspeed/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-08-03 14:42:05.000000 dspeed-1.2.0/src/dspeed/vis/waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.622967 dspeed-1.2.0/src/dspeed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-03 14:42:16.000000 dspeed-1.2.0/src/dspeed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-08-03 14:42:16.000000 dspeed-1.2.0/src/dspeed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:42:16.000000 dspeed-1.2.0/src/dspeed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 14:42:16.000000 dspeed-1.2.0/src/dspeed.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:42:16.000000 dspeed-1.2.0/src/dspeed.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-03 14:42:16.000000 dspeed-1.2.0/src/dspeed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 14:42:16.000000 dspeed-1.2.0/src/dspeed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.634967 dspeed-1.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.634967 dspeed-1.2.0/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/configs/icpc-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/configs/numpy-parsing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/configs/sipm-dplms-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/configs/sipm-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.638967 dspeed-1.2.0/tests/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/processors/dplms_noise_mat.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/processors/test_dplms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/processors/test_dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/processors/test_fftw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/processors/test_fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/processors/test_get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/processors/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/test_build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/test_list_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/test_numpy_constants_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/test_processing_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.638967 dspeed-1.2.0/tests/vis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:42:16.638967 dspeed-1.2.0/tests/vis/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/vis/configs/hpge-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-03 14:42:05.000000 dspeed-1.2.0/tests/vis/test_waveform_browser.py
```

### Comparing `dspeed-1.1.0/LICENSE` & `dspeed-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/PKG-INFO` & `dspeed-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspeed
-Version: 1.1.0
+Version: 1.2.0
 Summary: Fast Digital Signal Processing for particle detectors in Python
 Home-page: https://github.com/legend-exp/dspeed
 Author: Ian Guinn
 Author-email: iguinn@email.unc.edu
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dspeed-1.1.0/README.md` & `dspeed-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/setup.cfg` & `dspeed-1.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/legend-exp/dspeed
 author = Ian Guinn
 author_email = iguinn@email.unc.edu
 maintainer = The LEGEND Collaboration
 license = GPL-3.0
-license_file = LICENSE
 license_files = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dspeed-1.1.0/src/dspeed/build_dsp.py` & `dspeed-1.2.0/src/dspeed/build_dsp.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/cli.py` & `dspeed-1.2.0/src/dspeed/cli.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/errors.py` & `dspeed-1.2.0/src/dspeed/errors.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/logging.py` & `dspeed-1.2.0/src/dspeed/logging.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processing_chain.py` & `dspeed-1.2.0/src/dspeed/processing_chain.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/__init__.py` & `dspeed-1.2.0/src/dspeed/processors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
    add up very quickly: ``e = a*b + c*d``, for example, would allocate 3
    different arrays: one for ``a*b``, one for ``c*d``, and one for the sum of
    those two. As we write :class:`~numpy.ufunc`\ s, it is important that we try
    to use functions that operate in place as much as possible!
 """
 
 from .bl_subtract import bl_subtract
-from .convolutions import cusp_filter, t0_filter, zac_filter
+from .convolutions import cusp_filter, moving_slope, t0_filter, zac_filter
 from .dplms import dplms
 from .dwt import discrete_wavelet_transform
 from .fftw import dft, inv_dft, psd
 from .fixed_time_pickoff import fixed_time_pickoff
 from .gaussian_filter1d import gaussian_filter1d
 from .get_multi_local_extrema import get_multi_local_extrema
 from .histogram import histogram, histogram_stats
@@ -139,8 +139,9 @@
     "trap_pickoff",
     "upsampler",
     "interpolating_upsampler",
     "wiener_filter",
     "windower",
     "time_over_threshold",
     "dplms",
+    "moving_slope",
 ]
```

### Comparing `dspeed-1.1.0/src/dspeed/processors/bl_subtract.py` & `dspeed-1.2.0/src/dspeed/processors/bl_subtract.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/convolutions.py` & `dspeed-1.2.0/src/dspeed/processors/convolutions.py`

 * *Files 9% similar despite different names*

```diff
@@ -282,7 +282,70 @@
 
         if len(t0_kern) > len(w_in):
             raise DSPFatal("The filter is longer than the input waveform")
 
         w_out[:] = np.convolve(w_in, t0_kern)[: len(w_in)]
 
     return t0_filter_out
+
+
+def moving_slope(length):
+    """Calculates the linear slope of a waveform in sections of length
+
+    Note
+    ----
+    This processor is composed of a factory function that is called using the
+    `init_args` argument. The input and output waveforms are passed using
+    `args`.
+
+    Parameters
+    ----------
+    length
+        the length of the section to calculate slope
+
+    JSON Configuration Example
+    --------------------------
+
+    .. code-block :: json
+
+        "wf_slopes": {
+            "function": "moving_slope",
+            "module": "pygama.dsp.processors",
+            "args": ["wf_pz", "wf_slopes(len(wf_pz)-11,f)"],
+            "unit": "ADC",
+            "init_args": ["12"]
+        }
+    """
+
+    if length <= 0:
+        raise DSPFatal("The length of the filter must be positive")
+
+    if np.floor(length) != length:
+        raise DSPFatal("The length of the filter must be an integer")
+
+    sum_x = length * (length + 1) / 2
+    sum_x2 = length * (length + 1) * (2 * length + 1) / 6
+
+    kernel = (np.arange(1, length + 1, 1) * length) - (np.ones(length) * sum_x)
+    kernel /= length * sum_x2 - sum_x * sum_x
+    kernel = kernel[::-1]
+
+    @guvectorize(
+        ["void(float32[:], float32[:])", "void(float64[:], float64[:])"],
+        "(n),(m)",
+        **nb_kwargs(
+            cache=False,
+            forceobj=True,
+        ),
+    )
+    def moving_slope_out(w_in, w_out):
+        w_out[:] = np.nan
+
+        if np.isnan(w_in).any():
+            return
+
+        if len(kernel) > len(w_in):
+            raise DSPFatal("The filter is longer than the input waveform")
+
+        w_out[:] = np.convolve(w_in, kernel, "valid")
+
+    return moving_slope_out
```

### Comparing `dspeed-1.1.0/src/dspeed/processors/dplms.py` & `dspeed-1.2.0/src/dspeed/processors/dplms.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/dwt.py` & `dspeed-1.2.0/src/dspeed/processors/dwt.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/fftw.py` & `dspeed-1.2.0/src/dspeed/processors/fftw.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/fixed_time_pickoff.py` & `dspeed-1.2.0/src/dspeed/processors/fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/gaussian_filter1d.py` & `dspeed-1.2.0/src/dspeed/processors/gaussian_filter1d.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/get_multi_local_extrema.py` & `dspeed-1.2.0/src/dspeed/processors/get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/histogram.py` & `dspeed-1.2.0/src/dspeed/processors/histogram.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/linear_slope_fit.py` & `dspeed-1.2.0/src/dspeed/processors/linear_slope_fit.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/log_check.py` & `dspeed-1.2.0/src/dspeed/processors/log_check.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/min_max.py` & `dspeed-1.2.0/src/dspeed/processors/min_max.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/moving_windows.py` & `dspeed-1.2.0/src/dspeed/processors/moving_windows.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/multi_a_filter.py` & `dspeed-1.2.0/src/dspeed/processors/multi_a_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/multi_t_filter.py` & `dspeed-1.2.0/src/dspeed/processors/multi_t_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/optimize.py` & `dspeed-1.2.0/src/dspeed/processors/optimize.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/param_lookup.py` & `dspeed-1.2.0/src/dspeed/processors/param_lookup.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/peak_snr_threshold.py` & `dspeed-1.2.0/src/dspeed/processors/peak_snr_threshold.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/pole_zero.py` & `dspeed-1.2.0/src/dspeed/processors/pole_zero.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/presum.py` & `dspeed-1.2.0/src/dspeed/processors/presum.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/pulse_injector.py` & `dspeed-1.2.0/src/dspeed/processors/pulse_injector.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/saturation.py` & `dspeed-1.2.0/src/dspeed/processors/saturation.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/soft_pileup_corr.py` & `dspeed-1.2.0/src/dspeed/processors/soft_pileup_corr.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/time_over_threshold.py` & `dspeed-1.2.0/src/dspeed/processors/time_over_threshold.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/time_point_thresh.py` & `dspeed-1.2.0/src/dspeed/processors/time_point_thresh.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/trap_filters.py` & `dspeed-1.2.0/src/dspeed/processors/trap_filters.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/upsampler.py` & `dspeed-1.2.0/src/dspeed/processors/upsampler.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/wiener_filter.py` & `dspeed-1.2.0/src/dspeed/processors/wiener_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/processors/windower.py` & `dspeed-1.2.0/src/dspeed/processors/windower.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/utils.py` & `dspeed-1.2.0/src/dspeed/utils.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed/vis/waveform_browser.py` & `dspeed-1.2.0/src/dspeed/vis/waveform_browser.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/src/dspeed.egg-info/PKG-INFO` & `dspeed-1.2.0/src/dspeed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspeed
-Version: 1.1.0
+Version: 1.2.0
 Summary: Fast Digital Signal Processing for particle detectors in Python
 Home-page: https://github.com/legend-exp/dspeed
 Author: Ian Guinn
 Author-email: iguinn@email.unc.edu
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dspeed-1.1.0/src/dspeed.egg-info/SOURCES.txt` & `dspeed-1.2.0/src/dspeed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/configs/icpc-dsp-config.json` & `dspeed-1.2.0/tests/configs/icpc-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/configs/numpy-parsing.json` & `dspeed-1.2.0/tests/configs/numpy-parsing.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/configs/sipm-dplms-config.json` & `dspeed-1.2.0/tests/configs/sipm-dplms-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/configs/sipm-dsp-config.json` & `dspeed-1.2.0/tests/configs/sipm-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/conftest.py` & `dspeed-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/processors/dplms_noise_mat.dat` & `dspeed-1.2.0/tests/processors/dplms_noise_mat.dat`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/processors/test_dplms.py` & `dspeed-1.2.0/tests/processors/test_dplms.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/processors/test_dwt.py` & `dspeed-1.2.0/tests/processors/test_dwt.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/processors/test_fftw.py` & `dspeed-1.2.0/tests/processors/test_fftw.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/processors/test_fixed_time_pickoff.py` & `dspeed-1.2.0/tests/processors/test_fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/processors/test_get_multi_local_extrema.py` & `dspeed-1.2.0/tests/processors/test_get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/processors/test_histogram.py` & `dspeed-1.2.0/tests/processors/test_histogram.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/test_build_dsp.py` & `dspeed-1.2.0/tests/test_build_dsp.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/test_cli.py` & `dspeed-1.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/test_list_parsing.py` & `dspeed-1.2.0/tests/test_list_parsing.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/test_numpy_constants_parsing.py` & `dspeed-1.2.0/tests/test_numpy_constants_parsing.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/test_processing_chain.py` & `dspeed-1.2.0/tests/test_processing_chain.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/vis/configs/hpge-dsp-config.json` & `dspeed-1.2.0/tests/vis/configs/hpge-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.1.0/tests/vis/test_waveform_browser.py` & `dspeed-1.2.0/tests/vis/test_waveform_browser.py`

 * *Files identical despite different names*

