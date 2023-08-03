# Comparing `tmp/fooof-1.1.0rc1.tar.gz` & `tmp/fooof-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tom/Code/ModCode/fooof/dist/.tmp-cwsuvxtn/fooof-1.1.0rc1.tar", last modified: Fri Jul 21 19:21:34 2023, max compression
+gzip compressed data, was "/Users/tom/Code/ModCode/fooof/dist/.tmp-xvkfehuz/fooof-1.1.0rc2.tar", last modified: Thu Aug  3 15:21:06 2023, max compression
```

## Comparing `fooof-1.1.0rc1.tar` & `fooof-1.1.0rc2.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.771598 fooof-1.1.0rc1/
--rw-r--r--   0 tom        (501) staff       (20)    11340 2019-01-23 01:14:03.000000 fooof-1.1.0rc1/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       33 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)    13337 2023-07-21 19:21:34.771198 fooof-1.1.0rc1/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    11796 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/README.rst
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.723908 fooof-1.1.0rc1/fooof/
--rw-r--r--   0 tom        (501) staff       (20)      825 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.727379 fooof-1.1.0rc1/fooof/analysis/
--rw-r--r--   0 tom        (501) staff       (20)      169 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/analysis/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3837 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/analysis/error.py
--rw-r--r--   0 tom        (501) staff       (20)     9350 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/analysis/periodic.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.729415 fooof-1.1.0rc1/fooof/bands/
--rw-r--r--   0 tom        (501) staff       (20)       60 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/bands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4091 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/bands/bands.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.733976 fooof-1.1.0rc1/fooof/core/
--rw-r--r--   0 tom        (501) staff       (20)       47 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      616 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/errors.py
--rw-r--r--   0 tom        (501) staff       (20)     5271 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/funcs.py
--rw-r--r--   0 tom        (501) staff       (20)     3860 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/info.py
--rw-r--r--   0 tom        (501) staff       (20)     8226 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/core/io.py
--rw-r--r--   0 tom        (501) staff       (20)      411 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/items.py
--rw-r--r--   0 tom        (501) staff       (20)     9298 2023-07-21 19:20:06.000000 fooof-1.1.0rc1/fooof/core/modutils.py
--rw-r--r--   0 tom        (501) staff       (20)     4843 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/core/reports.py
--rw-r--r--   0 tom        (501) staff       (20)    14814 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/core/strings.py
--rw-r--r--   0 tom        (501) staff       (20)     6880 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/core/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.735170 fooof-1.1.0rc1/fooof/data/
--rw-r--r--   0 tom        (501) staff       (20)      106 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/data/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3894 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/data/conversions.py
--rw-r--r--   0 tom        (501) staff       (20)     3784 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/data/data.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.737380 fooof-1.1.0rc1/fooof/objs/
--rw-r--r--   0 tom        (501) staff       (20)      217 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/objs/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    54716 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/objs/fit.py
--rw-r--r--   0 tom        (501) staff       (20)    24050 2023-07-21 19:17:17.000000 fooof-1.1.0rc1/fooof/objs/group.py
--rw-r--r--   0 tom        (501) staff       (20)     9236 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/objs/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.742296 fooof-1.1.0rc1/fooof/plts/
--rw-r--r--   0 tom        (501) staff       (20)       84 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    10159 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/plts/annotate.py
--rw-r--r--   0 tom        (501) staff       (20)     4754 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/plts/aperiodic.py
--rw-r--r--   0 tom        (501) staff       (20)     1912 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/plts/error.py
--rw-r--r--   0 tom        (501) staff       (20)     4115 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/fg.py
--rw-r--r--   0 tom        (501) staff       (20)    12213 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/fm.py
--rw-r--r--   0 tom        (501) staff       (20)     5105 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/plts/periodic.py
--rw-r--r--   0 tom        (501) staff       (20)     2028 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/settings.py
--rw-r--r--   0 tom        (501) staff       (20)     8110 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/spectra.py
--rw-r--r--   0 tom        (501) staff       (20)     9326 2023-07-21 19:18:09.000000 fooof-1.1.0rc1/fooof/plts/style.py
--rw-r--r--   0 tom        (501) staff       (20)     3930 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/templates.py
--rw-r--r--   0 tom        (501) staff       (20)     6682 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/plts/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.745448 fooof-1.1.0rc1/fooof/sim/
--rw-r--r--   0 tom        (501) staff       (20)      220 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/sim/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    17522 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/sim/gen.py
--rw-r--r--   0 tom        (501) staff       (20)     9749 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/sim/params.py
--rw-r--r--   0 tom        (501) staff       (20)     9002 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/sim/transform.py
--rw-r--r--   0 tom        (501) staff       (20)      468 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/sim/utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.747771 fooof-1.1.0rc1/fooof/tests/
--rw-r--r--   0 tom        (501) staff       (20)       23 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.749202 fooof-1.1.0rc1/fooof/tests/analysis/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/analysis/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1065 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/analysis/test_error.py
--rw-r--r--   0 tom        (501) staff       (20)     2771 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/analysis/test_periodic.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.749792 fooof-1.1.0rc1/fooof/tests/bands/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/bands/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1176 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/bands/test_bands.py
--rw-r--r--   0 tom        (501) staff       (20)     1844 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/conftest.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.753671 fooof-1.1.0rc1/fooof/tests/core/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     2960 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/test_funcs.py
--rw-r--r--   0 tom        (501) staff       (20)     1485 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/test_info.py
--rw-r--r--   0 tom        (501) staff       (20)     5966 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/core/test_io.py
--rw-r--r--   0 tom        (501) staff       (20)     3389 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/core/test_modutils.py
--rw-r--r--   0 tom        (501) staff       (20)      766 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/test_reports.py
--rw-r--r--   0 tom        (501) staff       (20)     1355 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/test_strings.py
--rw-r--r--   0 tom        (501) staff       (20)     4127 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/core/test_utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.754665 fooof-1.1.0rc1/fooof/tests/data/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/data/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1997 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/data/test_conversions.py
--rw-r--r--   0 tom        (501) staff       (20)     1284 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/data/test_data.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.756084 fooof-1.1.0rc1/fooof/tests/objs/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/objs/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    14153 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/objs/test_fit.py
--rw-r--r--   0 tom        (501) staff       (20)    11469 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/objs/test_group.py
--rw-r--r--   0 tom        (501) staff       (20)     4482 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/objs/test_utils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.760636 fooof-1.1.0rc1/fooof/tests/plts/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      895 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_annotate.py
--rw-r--r--   0 tom        (501) staff       (20)     1461 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_aperiodic.py
--rw-r--r--   0 tom        (501) staff       (20)      637 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_error.py
--rw-r--r--   0 tom        (501) staff       (20)     1248 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_fg.py
--rw-r--r--   0 tom        (501) staff       (20)     1549 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/plts/test_fm.py
--rw-r--r--   0 tom        (501) staff       (20)     1104 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_periodic.py
--rw-r--r--   0 tom        (501) staff       (20)     4095 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_spectra.py
--rw-r--r--   0 tom        (501) staff       (20)     2625 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_styles.py
--rw-r--r--   0 tom        (501) staff       (20)      809 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_templates.py
--rw-r--r--   0 tom        (501) staff       (20)     3396 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/plts/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)      544 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/settings.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.763173 fooof-1.1.0rc1/fooof/tests/sim/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/sim/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4266 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/sim/test_gen.py
--rw-r--r--   0 tom        (501) staff       (20)     4050 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/sim/test_params.py
--rw-r--r--   0 tom        (501) staff       (20)     2503 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/sim/test_transform.py
--rw-r--r--   0 tom        (501) staff       (20)      328 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/sim/test_utils.py
--rw-r--r--   0 tom        (501) staff       (20)     2860 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/tutils.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.766448 fooof-1.1.0rc1/fooof/tests/utils/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3384 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/tests/utils/test_data.py
--rw-r--r--   0 tom        (501) staff       (20)      315 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/test_debug.py
--rw-r--r--   0 tom        (501) staff       (20)     1268 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/test_download.py
--rw-r--r--   0 tom        (501) staff       (20)     1430 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/test_io.py
--rw-r--r--   0 tom        (501) staff       (20)      575 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/test_params.py
--rw-r--r--   0 tom        (501) staff       (20)      573 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/tests/utils/test_reports.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.770344 fooof-1.1.0rc1/fooof/utils/
--rw-r--r--   0 tom        (501) staff       (20)      112 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/utils/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     8781 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/utils/data.py
--rw-r--r--   0 tom        (501) staff       (20)      924 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/utils/debug.py
--rw-r--r--   0 tom        (501) staff       (20)     2549 2023-07-21 19:15:35.000000 fooof-1.1.0rc1/fooof/utils/download.py
--rw-r--r--   0 tom        (501) staff       (20)     1634 2023-07-21 19:12:54.000000 fooof-1.1.0rc1/fooof/utils/io.py
--rw-r--r--   0 tom        (501) staff       (20)     1637 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/utils/params.py
--rw-r--r--   0 tom        (501) staff       (20)     1675 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/fooof/utils/reports.py
--rw-r--r--   0 tom        (501) staff       (20)       24 2023-07-21 19:13:09.000000 fooof-1.1.0rc1/fooof/version.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-21 19:21:34.725460 fooof-1.1.0rc1/fooof.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)    13337 2023-07-21 19:21:34.000000 fooof-1.1.0rc1/fooof.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     2675 2023-07-21 19:21:34.000000 fooof-1.1.0rc1/fooof.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-07-21 19:21:34.000000 fooof-1.1.0rc1/fooof.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      105 2023-07-21 19:21:34.000000 fooof-1.1.0rc1/fooof.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-07-21 19:21:34.000000 fooof-1.1.0rc1/fooof.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       17 2020-05-18 17:32:04.000000 fooof-1.1.0rc1/requirements.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-07-21 19:21:34.771690 fooof-1.1.0rc1/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     2466 2023-07-21 13:55:16.000000 fooof-1.1.0rc1/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.425408 fooof-1.1.0rc2/
+-rw-r--r--   0 tom        (501) staff       (20)    11340 2019-01-23 01:14:03.000000 fooof-1.1.0rc2/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       33 2023-07-22 19:10:52.000000 fooof-1.1.0rc2/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)    13337 2023-08-03 15:21:06.425126 fooof-1.1.0rc2/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    11796 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/README.rst
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.377382 fooof-1.1.0rc2/fooof/
+-rw-r--r--   0 tom        (501) staff       (20)      825 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.380663 fooof-1.1.0rc2/fooof/analysis/
+-rw-r--r--   0 tom        (501) staff       (20)      169 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/analysis/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3837 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/analysis/error.py
+-rw-r--r--   0 tom        (501) staff       (20)     9350 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/analysis/periodic.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.381761 fooof-1.1.0rc2/fooof/bands/
+-rw-r--r--   0 tom        (501) staff       (20)       60 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/bands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4091 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/bands/bands.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.388344 fooof-1.1.0rc2/fooof/core/
+-rw-r--r--   0 tom        (501) staff       (20)       47 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      616 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/core/errors.py
+-rw-r--r--   0 tom        (501) staff       (20)     5271 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/core/funcs.py
+-rw-r--r--   0 tom        (501) staff       (20)     3986 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/core/info.py
+-rw-r--r--   0 tom        (501) staff       (20)     8226 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/core/io.py
+-rw-r--r--   0 tom        (501) staff       (20)      411 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/core/items.py
+-rw-r--r--   0 tom        (501) staff       (20)     9298 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/core/modutils.py
+-rw-r--r--   0 tom        (501) staff       (20)     4843 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/core/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)    14814 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/core/strings.py
+-rw-r--r--   0 tom        (501) staff       (20)     7164 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/core/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.390734 fooof-1.1.0rc2/fooof/data/
+-rw-r--r--   0 tom        (501) staff       (20)      121 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/data/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3894 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/data/conversions.py
+-rw-r--r--   0 tom        (501) staff       (20)     4287 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/data/data.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.395546 fooof-1.1.0rc2/fooof/objs/
+-rw-r--r--   0 tom        (501) staff       (20)      242 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/objs/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    60107 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/objs/fit.py
+-rw-r--r--   0 tom        (501) staff       (20)    24105 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/objs/group.py
+-rw-r--r--   0 tom        (501) staff       (20)     9236 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/objs/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.402100 fooof-1.1.0rc2/fooof/plts/
+-rw-r--r--   0 tom        (501) staff       (20)       84 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    10159 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/annotate.py
+-rw-r--r--   0 tom        (501) staff       (20)     4754 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/aperiodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     1912 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/error.py
+-rw-r--r--   0 tom        (501) staff       (20)     4115 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/fg.py
+-rw-r--r--   0 tom        (501) staff       (20)    12213 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/fm.py
+-rw-r--r--   0 tom        (501) staff       (20)     5105 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/periodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     2028 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/settings.py
+-rw-r--r--   0 tom        (501) staff       (20)     8110 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/spectra.py
+-rw-r--r--   0 tom        (501) staff       (20)     9326 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/style.py
+-rw-r--r--   0 tom        (501) staff       (20)     3930 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/templates.py
+-rw-r--r--   0 tom        (501) staff       (20)     6682 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/plts/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.404551 fooof-1.1.0rc2/fooof/sim/
+-rw-r--r--   0 tom        (501) staff       (20)      220 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/sim/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    17522 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/sim/gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     9885 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/sim/params.py
+-rw-r--r--   0 tom        (501) staff       (20)     9002 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/sim/transform.py
+-rw-r--r--   0 tom        (501) staff       (20)      468 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/sim/utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.406283 fooof-1.1.0rc2/fooof/tests/
+-rw-r--r--   0 tom        (501) staff       (20)       23 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.407292 fooof-1.1.0rc2/fooof/tests/analysis/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/analysis/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1065 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/analysis/test_error.py
+-rw-r--r--   0 tom        (501) staff       (20)     2771 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/analysis/test_periodic.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.407913 fooof-1.1.0rc2/fooof/tests/bands/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/bands/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1176 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/bands/test_bands.py
+-rw-r--r--   0 tom        (501) staff       (20)     1844 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/conftest.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.410712 fooof-1.1.0rc2/fooof/tests/core/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/core/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     2960 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/core/test_funcs.py
+-rw-r--r--   0 tom        (501) staff       (20)     1483 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/core/test_info.py
+-rw-r--r--   0 tom        (501) staff       (20)     5966 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/core/test_io.py
+-rw-r--r--   0 tom        (501) staff       (20)     3389 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/core/test_modutils.py
+-rw-r--r--   0 tom        (501) staff       (20)      766 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/core/test_reports.py
+-rw-r--r--   0 tom        (501) staff       (20)     1355 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/core/test_strings.py
+-rw-r--r--   0 tom        (501) staff       (20)     4280 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/core/test_utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.411598 fooof-1.1.0rc2/fooof/tests/data/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/data/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1997 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/data/test_conversions.py
+-rw-r--r--   0 tom        (501) staff       (20)     1476 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/data/test_data.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.412914 fooof-1.1.0rc2/fooof/tests/objs/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/objs/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    15103 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/objs/test_fit.py
+-rw-r--r--   0 tom        (501) staff       (20)    11469 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/objs/test_group.py
+-rw-r--r--   0 tom        (501) staff       (20)     4482 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/objs/test_utils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.416948 fooof-1.1.0rc2/fooof/tests/plts/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      895 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/test_annotate.py
+-rw-r--r--   0 tom        (501) staff       (20)     1461 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/test_aperiodic.py
+-rw-r--r--   0 tom        (501) staff       (20)      637 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/test_error.py
+-rw-r--r--   0 tom        (501) staff       (20)     1248 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/test_fg.py
+-rw-r--r--   0 tom        (501) staff       (20)     1549 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/test_fm.py
+-rw-r--r--   0 tom        (501) staff       (20)     1104 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/test_periodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     4095 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/test_spectra.py
+-rw-r--r--   0 tom        (501) staff       (20)     2625 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/test_styles.py
+-rw-r--r--   0 tom        (501) staff       (20)      809 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/test_templates.py
+-rw-r--r--   0 tom        (501) staff       (20)     3396 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/plts/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      544 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/settings.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.418761 fooof-1.1.0rc2/fooof/tests/sim/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/sim/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4266 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/sim/test_gen.py
+-rw-r--r--   0 tom        (501) staff       (20)     4050 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/sim/test_params.py
+-rw-r--r--   0 tom        (501) staff       (20)     2503 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/sim/test_transform.py
+-rw-r--r--   0 tom        (501) staff       (20)      328 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/sim/test_utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     2860 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/tutils.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.421209 fooof-1.1.0rc2/fooof/tests/utils/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/utils/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3384 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/utils/test_data.py
+-rw-r--r--   0 tom        (501) staff       (20)      315 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/utils/test_debug.py
+-rw-r--r--   0 tom        (501) staff       (20)     1268 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/utils/test_download.py
+-rw-r--r--   0 tom        (501) staff       (20)     1430 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/utils/test_io.py
+-rw-r--r--   0 tom        (501) staff       (20)      575 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/utils/test_params.py
+-rw-r--r--   0 tom        (501) staff       (20)      573 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/tests/utils/test_reports.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.424608 fooof-1.1.0rc2/fooof/utils/
+-rw-r--r--   0 tom        (501) staff       (20)      133 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/utils/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     8781 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/utils/data.py
+-rw-r--r--   0 tom        (501) staff       (20)      924 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/utils/debug.py
+-rw-r--r--   0 tom        (501) staff       (20)     2549 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/utils/download.py
+-rw-r--r--   0 tom        (501) staff       (20)     1634 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/utils/io.py
+-rw-r--r--   0 tom        (501) staff       (20)     1637 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/utils/params.py
+-rw-r--r--   0 tom        (501) staff       (20)     1675 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/fooof/utils/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)       24 2023-08-03 15:20:13.000000 fooof-1.1.0rc2/fooof/version.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-08-03 15:21:06.379101 fooof-1.1.0rc2/fooof.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)    13337 2023-08-03 15:21:06.000000 fooof-1.1.0rc2/fooof.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     2675 2023-08-03 15:21:06.000000 fooof-1.1.0rc2/fooof.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-08-03 15:21:06.000000 fooof-1.1.0rc2/fooof.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      105 2023-08-03 15:21:06.000000 fooof-1.1.0rc2/fooof.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-08-03 15:21:06.000000 fooof-1.1.0rc2/fooof.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       17 2020-05-18 17:32:04.000000 fooof-1.1.0rc2/requirements.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-08-03 15:21:06.425479 fooof-1.1.0rc2/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     2466 2023-08-03 15:19:52.000000 fooof-1.1.0rc2/setup.py
```

### Comparing `fooof-1.1.0rc1/LICENSE` & `fooof-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/PKG-INFO` & `fooof-1.1.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fooof
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: fitting oscillations & one-over f
 Home-page: https://github.com/fooof-tools/fooof
 Download-URL: https://github.com/fooof-tools/fooof/releases
 Author: The Voytek Lab
 Author-email: voyteklab@gmail.com
 Maintainer: Thomas Donoghue
 Maintainer-email: tdonoghue.research@gmail.com
```

### Comparing `fooof-1.1.0rc1/README.rst` & `fooof-1.1.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/__init__.py` & `fooof-1.1.0rc2/fooof/__init__.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/analysis/error.py` & `fooof-1.1.0rc2/fooof/analysis/error.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/analysis/periodic.py` & `fooof-1.1.0rc2/fooof/analysis/periodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/bands/bands.py` & `fooof-1.1.0rc2/fooof/bands/bands.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/core/errors.py` & `fooof-1.1.0rc2/fooof/core/errors.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/core/funcs.py` & `fooof-1.1.0rc2/fooof/core/funcs.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/core/info.py` & `fooof-1.1.0rc2/fooof/core/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 
     Notes
     -----
     This function organizes public FOOOF object attributes into:
 
     - results : parameters for and measures of the model
     - settings : model settings
+    - run_modes: checks performed and errors raised
     - data : input data
     - meta_data : meta data of the inputs
     - arrays : data stored in arrays
     - model_components : component pieces of the model
     - descriptors : descriptors of the object status and model results
     """
 
     attributes = {'results' : ['aperiodic_params_', 'gaussian_params_', 'peak_params_',
                                'r_squared_', 'error_'],
                   'settings' : ['peak_width_limits', 'max_n_peaks',
                                 'min_peak_height', 'peak_threshold',
                                 'aperiodic_mode'],
+                  'run_modes': ['_debug', '_check_freqs', '_check_data'],
                   'data' : ['power_spectrum', 'freq_range', 'freq_res'],
                   'meta_data' : ['freq_range', 'freq_res'],
                   'arrays' : ['freqs', 'power_spectrum', 'aperiodic_params_',
                               'peak_params_', 'gaussian_params_'],
                   'model_components' : ['fooofed_spectrum_', '_spectrum_flat',
                                         '_spectrum_peak_rm', '_ap_fit', '_peak_fit'],
                   'descriptors' : ['has_data', 'has_model', 'n_peaks_']
```

### Comparing `fooof-1.1.0rc1/fooof/core/io.py` & `fooof-1.1.0rc2/fooof/core/io.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/core/modutils.py` & `fooof-1.1.0rc2/fooof/core/modutils.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/core/reports.py` & `fooof-1.1.0rc2/fooof/core/reports.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/core/strings.py` & `fooof-1.1.0rc2/fooof/core/strings.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/core/utils.py` & `fooof-1.1.0rc2/fooof/core/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,33 @@
 from itertools import chain, repeat
 
 import numpy as np
 
 ###################################################################################################
 ###################################################################################################
 
+def unlog(arr, base=10):
+    """Helper function to unlog an array.
+
+    Parameters
+    ----------
+    arr : ndarray
+        Array.
+    base : float
+        Base of the log to undo.
+
+    Returns
+    -------
+    ndarray
+        Unlogged array.
+    """
+
+    return np.power(base, arr)
+
+
 def group_three(vec):
     """Group an array of values into threes.
 
     Parameters
     ----------
     vec : list or 1d array
         List or array of items to group by 3. Length of array must be divisible by three.
```

### Comparing `fooof-1.1.0rc1/fooof/data/conversions.py` & `fooof-1.1.0rc2/fooof/data/conversions.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/data/data.py` & `fooof-1.1.0rc2/fooof/data/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,14 +34,33 @@
     Notes
     -----
     This object is a data object, based on a NamedTuple, with immutable data attributes.
     """
     __slots__ = ()
 
 
+class FOOOFRunModes(namedtuple('FOOOFRunModes', ['debug', 'check_freqs', 'check_data'])):
+    """Checks performed and errors raised by the model.
+
+    Parameters
+    ----------
+    debug :  bool
+       Whether to run in debug mode.
+    check_freqs : bool
+        Whether to run in check freqs mode.
+    check_data : bool
+        Whether to run in check data mode.
+
+    Notes
+    -----
+    This object is a data object, based on a NamedTuple, with immutable data attributes.
+    """
+    __slots__ = ()
+
+
 class FOOOFMetaData(namedtuple('FOOOFMetaData', ['freq_range', 'freq_res'])):
     """Metadata information about a power spectrum.
 
     Parameters
     ----------
     freq_range : list of [float, float]
         Frequency range of the power spectrum, as [lowest_freq, highest_freq].
```

### Comparing `fooof-1.1.0rc1/fooof/objs/fit.py` & `fooof-1.1.0rc2/fooof/objs/fit.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,30 +41,33 @@
     The error metric to use for post-hoc measures of model fit error.
 
 Run Modes
 ---------
 _debug : bool
     Whether the object is set in debug mode.
     This should be controlled by using the `set_debug_mode` method.
-_check_data : bool
-    Whether to check added data for NaN or Inf values, and fail out if present.
-    This should be controlled by using the `set_check_data_mode` method.
+_check_data, _check_freqs : bool
+    Whether to check added inputs for incorrect inputs, failing if present.
+    Frequency data is checked for linear spacing.
+    Power values are checked for data for NaN or Inf values.
+    These modes default to True, and can be controlled with the `set_check_modes` method.
 
 Code Notes
 ----------
 Methods without defined docstrings import docs at runtime, from aliased external functions.
 """
 
 import warnings
 from copy import deepcopy
 
 import numpy as np
 from numpy.linalg import LinAlgError
 from scipy.optimize import curve_fit
 
+from fooof.core.utils import unlog
 from fooof.core.items import OBJ_DESC
 from fooof.core.info import get_indices
 from fooof.core.io import save_fm, load_json
 from fooof.core.reports import save_report_fm
 from fooof.core.modutils import copy_doc_func_to_method
 from fooof.core.utils import group_three, check_array_dim
 from fooof.core.funcs import gaussian_function, get_ap_func, infer_ap_func
@@ -72,15 +75,15 @@
                                NoDataError, InconsistentDataError)
 from fooof.core.strings import (gen_settings_str, gen_results_fm_str,
                                 gen_issue_str, gen_width_warning_str)
 
 from fooof.plts.fm import plot_fm
 from fooof.utils.data import trim_spectrum
 from fooof.utils.params import compute_gauss_std
-from fooof.data import FOOOFResults, FOOOFSettings, FOOOFMetaData
+from fooof.data import FOOOFSettings, FOOOFRunModes, FOOOFMetaData, FOOOFResults
 from fooof.data.conversions import model_to_dataframe
 from fooof.sim.gen import gen_freqs, gen_aperiodic, gen_periodic, gen_model
 
 ###################################################################################################
 ###################################################################################################
 
 class FOOOF():
@@ -195,15 +198,15 @@
         #   Note: this is for checking error post fitting, not an objective function for fitting
         self._error_metric = 'MAE'
 
         ## RUN MODES
         # Set default debug mode - controls if an error is raised if model fitting is unsuccessful
         self._debug = False
         # Set default data checking modes - controls which checks get run on input data
-        #   check_freqs: check the frequency values, and raises an error for uneven spacing
+        #   check_freqs: checks the frequency values, and raises an error for uneven spacing
         self._check_freqs = True
         #   check_data: checks the power values and raises an error for any NaN / Inf values
         self._check_data = True
 
         # Set internal settings, based on inputs, and initialize data & results attributes
         self._reset_internal_settings()
         self._reset_data_results(True, True, True)
@@ -564,27 +567,133 @@
             Object containing the settings from the current object.
         """
 
         return FOOOFSettings(**{key : getattr(self, key) \
                              for key in OBJ_DESC['settings']})
 
 
+    def get_run_modes(self):
+        """Return run modes of the current object.
+
+        Returns
+        -------
+        FOOOFRunModes
+            Object containing the run modes from the current object.
+        """
+
+        return FOOOFRunModes(**{key.strip('_') : getattr(self, key) \
+                             for key in OBJ_DESC['run_modes']})
+
+
     def get_meta_data(self):
         """Return data information from the current object.
 
         Returns
         -------
         FOOOFMetaData
             Object containing meta data from the current object.
         """
 
         return FOOOFMetaData(**{key : getattr(self, key) \
                              for key in OBJ_DESC['meta_data']})
 
 
+    def get_data(self, component='full', space='log'):
+        """Get a data component.
+
+        Parameters
+        ----------
+        component : {'full', 'aperiodic', 'peak'}
+            Which data component to return.
+                'full' - full power spectrum
+                'aperiodic' - isolated aperiodic data component
+                'peak' - isolated peak data component
+        space : {'log', 'linear'}
+            Which space to return the data component in.
+                'log' - returns in log10 space.
+                'linear' - returns in linear space.
+
+        Returns
+        -------
+        output : 1d array
+            Specified data component, in specified spacing.
+
+        Notes
+        -----
+        The 'space' parameter doesn't just define the spacing of the data component
+        values, but rather defines the space of the additive data definition such that
+        `power_spectrum = aperiodic_component + peak_component`.
+        With space set as 'log', this combination holds in log space.
+        With space set as 'linear', this combination holds in linear space.
+        """
+
+        if not self.has_data:
+            raise NoDataError("No data available to fit, can not proceed.")
+        assert space in ['linear', 'log'], "Input for 'space' invalid."
+
+        if component == 'full':
+            output = self.power_spectrum if space == 'log' else unlog(self.power_spectrum)
+        elif component == 'aperiodic':
+            output = self._spectrum_peak_rm if space == 'log' else \
+                unlog(self.power_spectrum) / unlog(self._peak_fit)
+        elif component == 'peak':
+            output = self._spectrum_flat if space == 'log' else \
+                unlog(self.power_spectrum) - unlog(self._ap_fit)
+        else:
+            raise ValueError('Input for component invalid.')
+
+        return output
+
+
+    def get_model(self, component='full', space='log'):
+        """Get a model component.
+
+        Parameters
+        ----------
+        component : {'full', 'aperiodic', 'peak'}
+            Which model component to return.
+                'full' - full model
+                'aperiodic' - isolated aperiodic model component
+                'peak' - isolated peak model component
+        space : {'log', 'linear'}
+            Which space to return the model component in.
+                'log' - returns in log10 space.
+                'linear' - returns in linear space.
+
+        Returns
+        -------
+        output : 1d array
+            Specified model component, in specified spacing.
+
+        Notes
+        -----
+        The 'space' parameter doesn't just define the spacing of the model component
+        values, but rather defines the space of the additive model such that
+        `model = aperiodic_component + peak_component`.
+        With space set as 'log', this combination holds in log space.
+        With space set as 'linear', this combination holds in linear space.
+        """
+
+        if not self.has_model:
+            raise NoModelError("No model fit results are available, can not proceed.")
+        assert space in ['linear', 'log'], "Input for 'space' invalid."
+
+        if component == 'full':
+            output = self.fooofed_spectrum_ if space == 'log' else unlog(self.fooofed_spectrum_)
+        elif component == 'aperiodic':
+            output = self._ap_fit if space == 'log' else unlog(self._ap_fit)
+        elif component == 'peak':
+            output = self._peak_fit if space == 'log' else \
+                unlog(self.fooofed_spectrum_) - unlog(self._ap_fit)
+        else:
+            raise ValueError('Input for component invalid.')
+
+        return output
+
+
     def get_params(self, name, col=None):
         """Return model fit parameters for specified feature(s).
 
         Parameters
         ----------
         name : {'aperiodic_params', 'peak_params', 'gaussian_params', 'error', 'r_squared'}
             Name of the data field to extract.
@@ -719,24 +828,59 @@
         debug : bool
             Whether to run in debug mode.
         """
 
         self._debug = debug
 
 
+    def set_check_modes(self, check_freqs=None, check_data=None):
+        """Set check modes, which controls if an error is raised based on check on the inputs.
+
+        Parameters
+        ----------
+        check_freqs : bool, optional
+            Whether to run in check freqs mode, which checks the frequency data.
+        check_data : bool, optional
+            Whether to run in check data mode, which checks the power spectrum values data.
+        """
+
+        if check_freqs is not None:
+            self._check_freqs = check_freqs
+        if check_data is not None:
+            self._check_data = check_data
+
+
+    # This kept for backwards compatibility, but to be removed in 2.0 in favor of `set_check_modes`
     def set_check_data_mode(self, check_data):
         """Set check data mode, which controls if an error is raised if NaN or Inf data are added.
 
         Parameters
         ----------
         check_data : bool
             Whether to run in check data mode.
         """
 
-        self._check_data = check_data
+        self.set_check_modes(check_data=check_data)
+
+
+    def set_run_modes(self, debug, check_freqs, check_data):
+        """Simultaneously set all run modes.
+
+        Parameters
+        ----------
+        debug : bool
+            Whether to run in debug mode.
+        check_freqs : bool
+            Whether to run in check freqs mode.
+        check_data : bool
+            Whether to run in check data mode.
+        """
+
+        self.set_debug_mode(debug)
+        self.set_check_modes(check_freqs, check_data)
 
 
     def to_df(self, peak_org):
         """Convert and extract the model results as a pandas object.
 
         Parameters
         ----------
```

### Comparing `fooof-1.1.0rc1/fooof/objs/group.py` & `fooof-1.1.0rc2/fooof/objs/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,17 +452,17 @@
 
         Returns
         -------
         fm : FOOOF
             The FOOOFResults data loaded into a FOOOF object.
         """
 
-        # Initialize a FOOOF object, with same settings & check data mode as current FOOOFGroup
+        # Initialize a FOOOF object, with same settings & run modes as current FOOOFGroup
         fm = FOOOF(*self.get_settings(), verbose=self.verbose)
-        fm.set_check_data_mode(self._check_data)
+        fm.set_run_modes(*self.get_run_modes())
 
         # Add data for specified single power spectrum, if available
         #   The power spectrum is inverted back to linear, as it is re-logged when added to FOOOF
         if self.has_data:
             fm.add_data(self.freqs, np.power(10, self.power_spectra[ind]))
         # If no power spectrum data available, copy over data information & regenerate freqs
         else:
@@ -490,16 +490,17 @@
         fg : FOOOFGroup
             The requested selection of results data loaded into a new FOOOFGroup object.
         """
 
         # Check and convert indices encoding to list of int
         inds = check_inds(inds)
 
-        # Initialize a new FOOOFGroup object, with same settings as current FOOOFGroup
+        # Initialize a new FOOOFGroup object, with same settings and run modes as current FOOOFGroup
         fg = FOOOFGroup(*self.get_settings(), verbose=self.verbose)
+        fg.set_run_modes(*self.get_run_modes())
 
         # Add data for specified power spectra, if available
         #   The power spectra are inverted back to linear, as they are re-logged when added to FOOOF
         if self.has_data:
             fg.add_data(self.freqs, np.power(10, self.power_spectra[inds, :]))
         # If no power spectrum data available, copy over data information & regenerate freqs
         else:
```

### Comparing `fooof-1.1.0rc1/fooof/objs/utils.py` & `fooof-1.1.0rc2/fooof/objs/utils.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/annotate.py` & `fooof-1.1.0rc2/fooof/plts/annotate.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/aperiodic.py` & `fooof-1.1.0rc2/fooof/plts/aperiodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/error.py` & `fooof-1.1.0rc2/fooof/plts/error.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/fg.py` & `fooof-1.1.0rc2/fooof/plts/fg.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/fm.py` & `fooof-1.1.0rc2/fooof/plts/fm.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/periodic.py` & `fooof-1.1.0rc2/fooof/plts/periodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/settings.py` & `fooof-1.1.0rc2/fooof/plts/settings.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/spectra.py` & `fooof-1.1.0rc2/fooof/plts/spectra.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/style.py` & `fooof-1.1.0rc2/fooof/plts/style.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/templates.py` & `fooof-1.1.0rc2/fooof/plts/templates.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/plts/utils.py` & `fooof-1.1.0rc2/fooof/plts/utils.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/sim/gen.py` & `fooof-1.1.0rc2/fooof/sim/gen.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/sim/params.py` & `fooof-1.1.0rc2/fooof/sim/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,21 +142,24 @@
 
         Raises
         ------
         ValueError
             If the given values for defining the iteration range are inconsistent.
         """
 
-        if any(ii < 0 for ii in [start, stop, step]):
-            raise ValueError("Inputs 'start', 'stop', and 'step' should all be positive values.")
+        if any(ii < 0 for ii in [start, stop]):
+            raise ValueError("Inputs 'start' and 'stop' should be positive values.")
 
-        if not start < stop:
-            raise ValueError("Input 'start' should be less than 'stop'.")
+        if (stop - start) * step < 0:
+            raise ValueError("The sign of input 'step' does not align with 'start' / 'stop' values.")
 
-        if not step < (stop - start):
+        if start == stop:
+            raise ValueError("Input 'start' and 'stop' must be different values.")
+
+        if not abs(step) < abs(stop - start):
             raise ValueError("Input 'step' is too large given values for 'start' and 'stop'.")
 
 
 def param_iter(params):
     """Create a generator to iterate across parameter ranges.
 
     Parameters
```

### Comparing `fooof-1.1.0rc1/fooof/sim/transform.py` & `fooof-1.1.0rc2/fooof/sim/transform.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/analysis/test_error.py` & `fooof-1.1.0rc2/fooof/tests/analysis/test_error.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/analysis/test_periodic.py` & `fooof-1.1.0rc2/fooof/tests/analysis/test_periodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/bands/test_bands.py` & `fooof-1.1.0rc2/fooof/tests/bands/test_bands.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/conftest.py` & `fooof-1.1.0rc2/fooof/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/core/test_funcs.py` & `fooof-1.1.0rc2/fooof/tests/core/test_funcs.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/core/test_info.py` & `fooof-1.1.0rc2/fooof/tests/core/test_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     objs = dir(tfm)
 
     # Test that everything in dict is a valid component of the fooof object
     for ke, va in desc.items():
         for it in va:
             assert it in objs
 
-
 def test_get_peak_indices():
 
     indices = get_peak_indices()
 
     # Check it returns a valid object & that values are correct
     assert indices
     for ind, val in enumerate(['CF', 'PW', 'BW']):
@@ -29,15 +28,14 @@
 
     indices_fixed = get_indices('fixed')
 
     assert indices_fixed
     for ind, val in enumerate(['offset', 'exponent']):
         assert indices_fixed[val] == ind
 
-
     indices_knee = get_indices('knee')
 
     assert indices_knee
     for ind, val in enumerate(['offset', 'knee', 'exponent']):
         assert indices_knee[val] == ind
 
 def test_get_indices():
```

### Comparing `fooof-1.1.0rc1/fooof/tests/core/test_io.py` & `fooof-1.1.0rc2/fooof/tests/core/test_io.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/core/test_modutils.py` & `fooof-1.1.0rc2/fooof/tests/core/test_modutils.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/core/test_reports.py` & `fooof-1.1.0rc2/fooof/tests/core/test_reports.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/core/test_strings.py` & `fooof-1.1.0rc2/fooof/tests/core/test_strings.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/core/test_utils.py` & `fooof-1.1.0rc2/fooof/tests/core/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 from pytest import raises
 
 from fooof.core.utils import *
 
 ###################################################################################################
 ###################################################################################################
 
+def test_unlog():
+
+    orig = np.array([1, 2, 3, 4])
+    logged = np.log10(orig)
+    unlogged = unlog(logged)
+    assert np.array_equal(orig, unlogged)
+
 def test_group_three():
 
     dat = [0, 1, 2, 3, 4, 5]
     assert group_three(dat) == [[0, 1, 2], [3, 4, 5]]
 
     with raises(ValueError):
         group_three([0, 1, 2, 3])
```

### Comparing `fooof-1.1.0rc1/fooof/tests/data/test_conversions.py` & `fooof-1.1.0rc2/fooof/tests/data/test_conversions.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/data/test_data.py` & `fooof-1.1.0rc2/fooof/tests/data/test_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 
     settings = FOOOFSettings([1, 8], 8, 0.25, 2, 'fixed')
     assert settings
 
     for field in OBJ_DESC['settings']:
         assert getattr(settings, field)
 
+def test_fooof_run_modes():
+
+    run_modes = FOOOFRunModes(True, True, True)
+    assert run_modes
+
+    for field in OBJ_DESC['run_modes']:
+        assert getattr(run_modes, field.strip('_'))
+
 def test_fooof_meta_data():
 
     meta_data = FOOOFMetaData([1, 50], 0.5)
     assert meta_data
 
     for field in OBJ_DESC['meta_data']:
         assert getattr(meta_data, field)
```

### Comparing `fooof-1.1.0rc1/fooof/tests/objs/test_fit.py` & `fooof-1.1.0rc2/fooof/tests/objs/test_fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -307,14 +307,25 @@
     settings = tfm.get_settings()
     assert isinstance(settings, FOOOFSettings)
     meta_data = tfm.get_meta_data()
     assert isinstance(meta_data, FOOOFMetaData)
     results = tfm.get_results()
     assert isinstance(results, FOOOFResults)
 
+def test_get_components(tfm):
+
+    # Make sure test object has been fit
+    tfm.fit()
+
+    # Test get data & model components
+    for comp in ['full', 'aperiodic', 'peak']:
+        for space in ['log', 'linear']:
+            assert isinstance(tfm.get_data(comp, space), np.ndarray)
+            assert isinstance(tfm.get_model(comp, space), np.ndarray)
+
 def test_get_params(tfm):
     """Test the get_params method."""
 
     for dname in ['aperiodic_params', 'aperiodic', 'peak_params', 'peak',
                   'error', 'r_squared', 'gaussian_params', 'gaussian']:
         assert np.any(tfm.get_params(dname))
 
@@ -410,32 +421,51 @@
 
     tfm.set_debug_mode(True)
     assert tfm._debug is True
 
     with raises(FitError):
         tfm.fit(*gen_power_spectrum([3, 50], [50, 2], [10, 0.5, 2, 20, 0.3, 4]))
 
-def test_fooof_check_data():
-    """Test FOOOF in with check data mode turned off, including with NaN data."""
+def test_fooof_set_check_modes(tfm):
+    """Test changing check_modes using set_check_modes, and that checks get turned off.
+    Note that testing for checks raising errors happens in test_fooof_checks.`"""
 
     tfm = FOOOF(verbose=False)
 
-    tfm.set_check_data_mode(False)
+    tfm.set_check_modes(False, False)
+    assert tfm._check_freqs is False
     assert tfm._check_data is False
 
-    # Add data, with check data turned off
-    #   In check data mode, adding data with NaN should run
-    freqs = gen_freqs([3, 50], 0.5)
+    # Add bad frequency data, with check freqs turned off
+    freqs = np.array([1, 2, 4])
+    powers = np.array([1, 2, 3])
+    tfm.add_data(freqs, powers)
+    assert tfm.has_data
+
+    # Add bad power values data, with check data turned off
+    freqs = gen_freqs([3, 30], 1)
     powers = np.ones_like(freqs) * np.nan
     tfm.add_data(freqs, powers)
     assert tfm.has_data
 
     # Model fitting should execute, but return a null model fit, given the NaNs, without failing
     tfm.fit()
     assert not tfm.has_model
 
+    # Reset check modes to true
+    tfm.set_check_modes(True, True)
+    assert tfm._check_freqs is True
+    assert tfm._check_data is True
+
+def test_set_run_modes():
+
+    tfm = FOOOF(verbose=False)
+    tfm.set_run_modes(False, False, False)
+    for field in OBJ_DESC['run_modes']:
+        assert getattr(tfm, field) is False
+
 def test_fooof_to_df(tfm, tbands, skip_if_no_pandas):
 
     df1 = tfm.to_df(2)
     assert isinstance(df1, pd.Series)
     df2 = tfm.to_df(tbands)
     assert isinstance(df2, pd.Series)
```

### Comparing `fooof-1.1.0rc1/fooof/tests/objs/test_group.py` & `fooof-1.1.0rc2/fooof/tests/objs/test_group.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/objs/test_utils.py` & `fooof-1.1.0rc2/fooof/tests/objs/test_utils.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/plts/test_annotate.py` & `fooof-1.1.0rc2/fooof/tests/plts/test_annotate.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/plts/test_aperiodic.py` & `fooof-1.1.0rc2/fooof/tests/plts/test_aperiodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/plts/test_error.py` & `fooof-1.1.0rc2/fooof/tests/plts/test_error.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/plts/test_fg.py` & `fooof-1.1.0rc2/fooof/tests/plts/test_fg.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/plts/test_fm.py` & `fooof-1.1.0rc2/fooof/tests/plts/test_fm.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/plts/test_periodic.py` & `fooof-1.1.0rc2/fooof/tests/plts/test_periodic.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/plts/test_spectra.py` & `fooof-1.1.0rc2/fooof/tests/plts/test_spectra.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/plts/test_styles.py` & `fooof-1.1.0rc2/fooof/tests/plts/test_styles.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/plts/test_templates.py` & `fooof-1.1.0rc2/fooof/tests/plts/test_templates.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/plts/test_utils.py` & `fooof-1.1.0rc2/fooof/tests/plts/test_utils.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/settings.py` & `fooof-1.1.0rc2/fooof/tests/settings.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/sim/test_gen.py` & `fooof-1.1.0rc2/fooof/tests/sim/test_gen.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/sim/test_params.py` & `fooof-1.1.0rc2/fooof/tests/sim/test_params.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/sim/test_transform.py` & `fooof-1.1.0rc2/fooof/tests/sim/test_transform.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/tutils.py` & `fooof-1.1.0rc2/fooof/tests/tutils.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/utils/test_data.py` & `fooof-1.1.0rc2/fooof/tests/utils/test_data.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/utils/test_download.py` & `fooof-1.1.0rc2/fooof/tests/utils/test_download.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/utils/test_io.py` & `fooof-1.1.0rc2/fooof/tests/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/utils/test_params.py` & `fooof-1.1.0rc2/fooof/tests/utils/test_params.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/tests/utils/test_reports.py` & `fooof-1.1.0rc2/fooof/tests/utils/test_reports.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/utils/data.py` & `fooof-1.1.0rc2/fooof/utils/data.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/utils/debug.py` & `fooof-1.1.0rc2/fooof/utils/debug.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/utils/download.py` & `fooof-1.1.0rc2/fooof/utils/download.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/utils/io.py` & `fooof-1.1.0rc2/fooof/utils/io.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/utils/params.py` & `fooof-1.1.0rc2/fooof/utils/params.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof/utils/reports.py` & `fooof-1.1.0rc2/fooof/utils/reports.py`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/fooof.egg-info/PKG-INFO` & `fooof-1.1.0rc2/fooof.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fooof
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: fitting oscillations & one-over f
 Home-page: https://github.com/fooof-tools/fooof
 Download-URL: https://github.com/fooof-tools/fooof/releases
 Author: The Voytek Lab
 Author-email: voyteklab@gmail.com
 Maintainer: Thomas Donoghue
 Maintainer-email: tdonoghue.research@gmail.com
```

### Comparing `fooof-1.1.0rc1/fooof.egg-info/SOURCES.txt` & `fooof-1.1.0rc2/fooof.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fooof-1.1.0rc1/setup.py` & `fooof-1.1.0rc2/setup.py`

 * *Files identical despite different names*

