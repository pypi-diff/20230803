# Comparing `tmp/siman-1.3.9.tar.gz` & `tmp/siman-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.3.9.tar", last modified: Wed Jul 26 16:54:36 2023, max compression
+gzip compressed data, was "dist/siman-1.4.0.tar", last modified: Thu Aug  3 08:59:39 2023, max compression
```

## Comparing `siman-1.3.9.tar` & `siman-1.4.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.633509 siman-1.3.9/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.9/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.9/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-26 16:54:36.633509 siman-1.3.9/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.9/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-26 16:54:36.633509 siman-1.3.9/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-26 16:54:24.000000 siman-1.3.9/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.630509 siman-1.3.9/siman/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.3.9/siman/3d_plot.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2023-07-14 10:44:19.000000 siman-1.3.9/siman/SSHTools.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.3.9/siman/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50708 2023-07-16 18:04:57.000000 siman-1.3.9/siman/analysis.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.3.9/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.631509 siman-1.3.9/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.9/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.9/siman/analyze/segregation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.3.9/siman/approximation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.3.9/siman/bands.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120786 2023-07-16 18:04:57.000000 siman-1.3.9/siman/calc_manage.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.3.9/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.631509 siman-1.3.9/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.9/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.9/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.9/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.9/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56599 2023-07-16 18:04:57.000000 siman-1.3.9/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.9/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.632509 siman-1.3.9/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.9/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.9/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.9/siman/chg/vasputil_chgarith_module.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.3.9/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.632509 siman-1.3.9/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.9/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53318 2023-07-16 18:04:57.000000 siman-1.3.9/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.9/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2023-07-14 09:47:42.000000 siman-1.3.9/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3783 2023-07-26 16:52:32.000000 siman-1.3.9/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.3.9/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   119405 2023-07-16 18:04:57.000000 siman-1.3.9/siman/core/structure.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.3.9/siman/database.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.3.9/siman/default_project_conf.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.3.9/siman/dev_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33287 2023-07-14 10:44:19.000000 siman-1.3.9/siman/dos_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.3.9/siman/fit_hex.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-14 10:44:19.000000 siman-1.3.9/siman/functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   113839 2023-07-14 10:44:19.000000 siman-1.3.9/siman/geo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16531 2023-07-26 16:52:32.000000 siman-1.3.9/siman/header.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.3.9/siman/helper_for_writing_beatiful_code.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.3.9/siman/impurity.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    88140 2023-07-26 16:53:10.000000 siman-1.3.9/siman/inout.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.3.9/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.633509 siman-1.3.9/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.9/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.9/siman/mat_prop/mat_prop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.3.9/siman/matproj_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.3.9/siman/monte.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.3.9/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31637 2023-07-14 10:44:19.000000 siman-1.3.9/siman/neb.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.3.9/siman/pairs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50595 2023-07-18 15:59:51.000000 siman-1.3.9/siman/picture_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.3.9/siman/plot_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.3.9/siman/polaron.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.3.9/siman/polaron_hop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.3.9/siman/polaron_mod.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194610 2023-07-14 10:44:19.000000 siman-1.3.9/siman/project_funcs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.3.9/siman/properties_2d.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.3.9/siman/properties_energy.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.3.9/siman/properties_lattice.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    30687 2023-07-14 10:44:19.000000 siman-1.3.9/siman/set_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.3.9/siman/simanrc.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.3.9/siman/small_classes.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6663 2023-07-14 10:44:19.000000 siman-1.3.9/siman/small_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.3.9/siman/structure_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.3.9/siman/table_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.3.9/siman/thermo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.3.9/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-26 16:54:36.631509 siman-1.3.9/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-26 16:54:36.000000 siman-1.3.9/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-07-26 16:54:36.000000 siman-1.3.9/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-26 16:54:36.000000 siman-1.3.9/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-26 16:54:36.000000 siman-1.3.9/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-26 16:54:36.000000 siman-1.3.9/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.780261 siman-1.4.0/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.4.0/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.4.0/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-08-03 08:59:39.780261 siman-1.4.0/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.4.0/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-08-03 08:59:39.780261 siman-1.4.0/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-08-03 08:59:36.000000 siman-1.4.0/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.777261 siman-1.4.0/siman/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.4.0/siman/3d_plot.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2023-07-14 10:44:19.000000 siman-1.4.0/siman/SSHTools.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.4.0/siman/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50708 2023-07-16 18:04:57.000000 siman-1.4.0/siman/analysis.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.4.0/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.777261 siman-1.4.0/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.0/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.4.0/siman/analyze/segregation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.4.0/siman/approximation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.4.0/siman/bands.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120904 2023-07-26 17:08:05.000000 siman-1.4.0/siman/calc_manage.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.4.0/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.778261 siman-1.4.0/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.0/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.4.0/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.4.0/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.4.0/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56599 2023-07-16 18:04:57.000000 siman-1.4.0/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.4.0/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.778261 siman-1.4.0/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.4.0/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.4.0/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.4.0/siman/chg/vasputil_chgarith_module.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.4.0/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.779261 siman-1.4.0/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.0/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53318 2023-07-16 18:04:57.000000 siman-1.4.0/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.4.0/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2023-07-14 09:47:42.000000 siman-1.4.0/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3783 2023-07-26 16:52:32.000000 siman-1.4.0/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.4.0/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   119405 2023-07-16 18:04:57.000000 siman-1.4.0/siman/core/structure.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.4.0/siman/database.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.4.0/siman/default_project_conf.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.4.0/siman/dev_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33287 2023-07-14 10:44:19.000000 siman-1.4.0/siman/dos_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.4.0/siman/fit_hex.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-14 10:44:19.000000 siman-1.4.0/siman/functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   113839 2023-07-14 10:44:19.000000 siman-1.4.0/siman/geo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16531 2023-07-26 16:52:32.000000 siman-1.4.0/siman/header.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.4.0/siman/helper_for_writing_beatiful_code.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.4.0/siman/impurity.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    88257 2023-08-03 08:41:20.000000 siman-1.4.0/siman/inout.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.4.0/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.779261 siman-1.4.0/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.4.0/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.4.0/siman/mat_prop/mat_prop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.4.0/siman/matproj_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.4.0/siman/monte.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.4.0/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31637 2023-07-14 10:44:19.000000 siman-1.4.0/siman/neb.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.4.0/siman/pairs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50595 2023-07-29 18:04:07.000000 siman-1.4.0/siman/picture_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.4.0/siman/plot_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.4.0/siman/polaron.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.4.0/siman/polaron_hop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.4.0/siman/polaron_mod.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194660 2023-07-26 17:00:29.000000 siman-1.4.0/siman/project_funcs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.4.0/siman/properties_2d.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.4.0/siman/properties_energy.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.4.0/siman/properties_lattice.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    30687 2023-07-14 10:44:19.000000 siman-1.4.0/siman/set_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.4.0/siman/simanrc.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.4.0/siman/small_classes.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6663 2023-07-14 10:44:19.000000 siman-1.4.0/siman/small_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.4.0/siman/structure_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.4.0/siman/table_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.4.0/siman/thermo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.4.0/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-08-03 08:59:39.777261 siman-1.4.0/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-08-03 08:59:39.000000 siman-1.4.0/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-08-03 08:59:39.000000 siman-1.4.0/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-08-03 08:59:39.000000 siman-1.4.0/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-08-03 08:59:39.000000 siman-1.4.0/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-08-03 08:59:39.000000 siman-1.4.0/siman.egg-info/top_level.txt
```

### Comparing `siman-1.3.9/LICENSE` & `siman-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/PKG-INFO` & `siman-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.9
+Version: 1.4.0
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.9/setup.py` & `siman-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.3.9",
+    version="1.4.0",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.3.9/siman/3d_plot.py` & `siman-1.4.0/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/SSHTools.py` & `siman-1.4.0/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/analysis.py` & `siman-1.4.0/siman/analysis.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/analysis_functions.py` & `siman-1.4.0/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/analyze/segregation.py` & `siman-1.4.0/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/approximation.py` & `siman-1.4.0/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/bands.py` & `siman-1.4.0/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/calc_manage.py` & `siman-1.4.0/siman/calc_manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -961,19 +961,22 @@
                     sts = scale_cell_by_matrix(st, scale_region = scale_region, n_scale_images = n_scale_images, parent_calc_name = pname, mul_matrix = mul_matrix)
 
                 if ise_new:
                     inputset = ise_new
                     id_s = (it,inputset,v)
 
                 #cl_temp = db[id_s].copy()
-                #sys.exit()
                 try:
                     cl_temp = db[id_s].copy()
                 except:
                     cl_temp = CalculationVasp(varset[inputset], id_s)
+                # print('here', cl_temp.id, )
+                # print(cl_temp.calculator)
+
+                # sys.exit()
 
 
 
 
 
 
                 for i, s in enumerate(sts):
@@ -2955,15 +2958,15 @@
             
 
             printlog('read_results() output', outst)
 
 
 
 
-
+            # print(cl.id)
             if cl.calculator == 'vasp':
                 e   = cl.energy_sigma0
             else:
                 e = 0
 
             try:
                 v = cl.end.vol
```

### Comparing `siman-1.3.9/siman/calcul.py` & `siman-1.4.0/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/calculators/aims.py` & `siman-1.4.0/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/calculators/gaussian.py` & `siman-1.4.0/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/calculators/qe.py` & `siman-1.4.0/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/calculators/vasp.py` & `siman-1.4.0/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/calculators/vasp_old.py` & `siman-1.4.0/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/chg/chg_func.py` & `siman-1.4.0/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/chg/vasputil_chgarith_module.py` & `siman-1.4.0/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/classes.py` & `siman-1.4.0/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/core/calculation.py` & `siman-1.4.0/siman/core/calculation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/core/calculation_old.py` & `siman-1.4.0/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/core/cluster_batch_script.py` & `siman-1.4.0/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/core/cluster_run_script.py` & `siman-1.4.0/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/core/molecule.py` & `siman-1.4.0/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/core/structure.py` & `siman-1.4.0/siman/core/structure.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/database.py` & `siman-1.4.0/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/default_project_conf.py` & `siman-1.4.0/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/dev_functions.py` & `siman-1.4.0/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/dos_functions.py` & `siman-1.4.0/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/fit_hex.py` & `siman-1.4.0/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/functions.py` & `siman-1.4.0/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/geo.py` & `siman-1.4.0/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/header.py` & `siman-1.4.0/siman/header.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/impurity.py` & `siman-1.4.0/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/inout.py` & `siman-1.4.0/siman/inout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1859,15 +1859,18 @@
 
                     i = 0
                     while 'ELASTIC MODULI CONTR FROM IONIC RELAXATION' not in line:
                         i+=1
                         line = outcarlines[i_line+i]
                         if 'f  =' in line:
                             freq.append(float(line.split()[3]) ) #THz
+                        elif 'f/i=' in line:
+                            freq.append(-float(line.split()[2]) ) #THz
                             # print(line)
+
                     self.freq = freq
 
 
             if 'TOTAL ELASTIC MODULI' in line:
                 eltensor = []
                 for i in range(9):
                     line = outcarlines[i_line+i]
```

### Comparing `siman-1.3.9/siman/kpoints_functions.py` & `siman-1.4.0/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/mat_prop/mat_prop.py` & `siman-1.4.0/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/matproj_functions.py` & `siman-1.4.0/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/monte.py` & `siman-1.4.0/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/monte_functions.py` & `siman-1.4.0/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/neb.py` & `siman-1.4.0/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/pairs.py` & `siman-1.4.0/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/picture_functions.py` & `siman-1.4.0/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/plot_functions.py` & `siman-1.4.0/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/polaron.py` & `siman-1.4.0/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/polaron_hop.py` & `siman-1.4.0/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/polaron_mod.py` & `siman-1.4.0/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/project_funcs.py` & `siman-1.4.0/siman/project_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4197,14 +4197,16 @@
     if add: 
         printlog('Calc_method', calc_method, imp = 'y')
         add_loop(it_new, ise, 1, up = 'up2', calc_method = calc_method, inherit_option = 'inherit_xred', input_st = st, it_folder = it_folder, **add_loop_dic)
 
     else:
         idd = (it_new+suf, ise, 100)
         if fit:
+            # print(idd)
+            # sys.exit()
             res_loop(*idd[0:2], list(range(1,8))+[100], analys_type = 'fit_a', show = 'fitfomag', up = up_res)
 
         else:
             res_loop(*idd, show = 'fo', up = up_res)#list(range(1,8))+[100], analys_type = 'fit_a', show = 'fitfo', up = '1')
         # st = calc[idd].end
         # print(st.get_space_group_info())
         # alpha, beta, gamma = st.get_angles()
```

### Comparing `siman-1.3.9/siman/properties_2d.py` & `siman-1.4.0/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/properties_energy.py` & `siman-1.4.0/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/properties_lattice.py` & `siman-1.4.0/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/set_functions.py` & `siman-1.4.0/siman/set_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/simanrc.py` & `siman-1.4.0/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/small_functions.py` & `siman-1.4.0/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/structure_functions.py` & `siman-1.4.0/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/table_functions.py` & `siman-1.4.0/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/thermo.py` & `siman-1.4.0/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman/workflow_utilities.py` & `siman-1.4.0/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.9/siman.egg-info/PKG-INFO` & `siman-1.4.0/siman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.9
+Version: 1.4.0
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.9/siman.egg-info/SOURCES.txt` & `siman-1.4.0/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

