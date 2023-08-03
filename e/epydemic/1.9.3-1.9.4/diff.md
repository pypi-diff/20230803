# Comparing `tmp/epydemic-1.9.3.tar.gz` & `tmp/epydemic-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epydemic-1.9.3.tar", last modified: Sun Mar 27 14:00:50 2022, max compression
+gzip compressed data, was "epydemic-1.9.4.tar", last modified: Sun Mar 27 14:10:38 2022, max compression
```

## Comparing `epydemic-1.9.3.tar` & `epydemic-1.9.4.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr--   0 sd80      (1000) sd80      (1000)        0 2022-03-27 14:00:50.407754 epydemic-1.9.3/
--rw-rw-r--   0 sd80      (1000) sd80      (1000)    35141 2021-03-08 12:11:21.000000 epydemic-1.9.3/LICENSE
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3301 2022-03-27 14:00:50.407754 epydemic-1.9.3/PKG-INFO
--rw-r--r--   0 sd80      (1000) sd80      (1000)     2516 2022-03-19 12:24:11.000000 epydemic-1.9.3/README.rst
-drwxrwxr--   0 sd80      (1000) sd80      (1000)        0 2022-03-27 14:00:50.404421 epydemic-1.9.3/epydemic/
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3881 2022-03-08 11:14:37.000000 epydemic-1.9.3/epydemic/__init__.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     5694 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/adddelete.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)    16334 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/bbt.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3360 2021-04-27 09:29:54.000000 epydemic-1.9.3/epydemic/bitstream.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)    23768 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/compartmentedmodel.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     4654 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/drawset.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     5465 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/generator.py
-drwxrwxr--   0 sd80      (1000) sd80      (1000)        0 2022-03-27 14:00:50.404421 epydemic-1.9.3/epydemic/gf/
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     1167 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/gf/__init__.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3791 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/gf/continuous_gf.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3181 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/gf/discrete_gf.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2958 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/gf/function_gf.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     4167 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/gf/gf.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2077 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/gf/interface.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3024 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/gf/standard_gfs.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3258 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/loci.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     4445 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/monitor.py
--rw-r--r--   0 sd80      (1000) sd80      (1000)    15664 2022-03-26 13:27:09.000000 epydemic-1.9.3/epydemic/networkdynamics.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     6035 2022-03-08 11:14:37.000000 epydemic-1.9.3/epydemic/networkexperiment.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)    17143 2022-03-08 11:14:37.000000 epydemic-1.9.3/epydemic/newmanziff.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     7487 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/opinion_model.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     4322 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/percolate.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     5476 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/plc_generator.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)    14640 2022-03-08 11:14:37.000000 epydemic-1.9.3/epydemic/process.py
--rw-r--r--   0 sd80      (1000) sd80      (1000)     5978 2022-03-22 10:18:58.000000 epydemic-1.9.3/epydemic/processsequence.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)        0 2021-03-08 12:11:21.000000 epydemic-1.9.3/epydemic/py.typed
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     6825 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/seir_model.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     4341 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/shuffle.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3772 2022-03-22 09:34:18.000000 epydemic-1.9.3/epydemic/sir_model.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3648 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/sir_model_fixed_recovery.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2416 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/sirs_model.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     5720 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/sis_model.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3649 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/sis_model_fixed_recovery.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     6965 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/sivr_model.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     6080 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/standard_generators.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3606 2022-03-08 11:14:37.000000 epydemic-1.9.3/epydemic/statistics.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     4434 2022-03-26 12:48:29.000000 epydemic-1.9.3/epydemic/stochasticdynamics.py
--rw-r--r--   0 sd80      (1000) sd80      (1000)     4162 2022-03-26 13:13:03.000000 epydemic-1.9.3/epydemic/synchronousdynamics.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     1110 2021-03-08 12:11:21.000000 epydemic-1.9.3/epydemic/types.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2582 2022-01-26 13:44:59.000000 epydemic-1.9.3/epydemic/vaccinate_model.py
-drwxrwxr--   0 sd80      (1000) sd80      (1000)        0 2022-03-27 14:00:50.404421 epydemic-1.9.3/epydemic.egg-info/
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3301 2022-03-27 14:00:50.000000 epydemic-1.9.3/epydemic.egg-info/PKG-INFO
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     1822 2022-03-27 14:00:50.000000 epydemic-1.9.3/epydemic.egg-info/SOURCES.txt
--rw-rw-r--   0 sd80      (1000) sd80      (1000)        1 2022-03-27 14:00:50.000000 epydemic-1.9.3/epydemic.egg-info/dependency_links.txt
--rw-rw-r--   0 sd80      (1000) sd80      (1000)        1 2022-03-27 12:35:51.000000 epydemic-1.9.3/epydemic.egg-info/not-zip-safe
--rw-rw-r--   0 sd80      (1000) sd80      (1000)       95 2022-03-27 14:00:50.000000 epydemic-1.9.3/epydemic.egg-info/requires.txt
--rw-rw-r--   0 sd80      (1000) sd80      (1000)        9 2022-03-27 14:00:50.000000 epydemic-1.9.3/epydemic.egg-info/top_level.txt
--rw-rw-r--   0 sd80      (1000) sd80      (1000)      211 2022-03-27 14:00:50.407754 epydemic-1.9.3/setup.cfg
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2115 2022-03-27 12:35:50.000000 epydemic-1.9.3/setup.py
-drwxrwxr--   0 sd80      (1000) sd80      (1000)        0 2022-03-27 14:00:50.407754 epydemic-1.9.3/test/
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3158 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_adddelete.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     6304 2022-03-08 11:14:37.000000 epydemic-1.9.3/test/test_adddeletesir.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)    14377 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_bbt.py
--rw-r--r--   0 sd80      (1000) sd80      (1000)     1377 2022-03-22 10:18:58.000000 epydemic-1.9.3/test/test_bitstream.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)    10186 2021-06-07 09:48:01.000000 epydemic-1.9.3/test/test_compartmentedmodel.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     7133 2022-03-08 11:14:37.000000 epydemic-1.9.3/test/test_events.py
--rw-r--r--   0 sd80      (1000) sd80      (1000)     5531 2021-05-13 12:22:20.000000 epydemic-1.9.3/test/test_generators.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     8743 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_gf.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     7450 2022-03-08 12:50:18.000000 epydemic-1.9.3/test/test_gof.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2749 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_hitting.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2422 2021-04-27 09:29:54.000000 epydemic-1.9.3/test/test_loci.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3479 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_monitor.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     5947 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_networkdynamics.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     4048 2022-03-08 11:14:37.000000 epydemic-1.9.3/test/test_newmanziff.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2342 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_opinion.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2001 2021-06-07 14:06:17.000000 epydemic-1.9.3/test/test_percolate.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3771 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_process.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     4429 2022-03-08 11:14:37.000000 epydemic-1.9.3/test/test_processsequence.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2233 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_seir.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2613 2021-06-10 15:10:59.000000 epydemic-1.9.3/test/test_shuffle.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     1984 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_sir.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     1340 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_sir_fixedrecovery.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2087 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_sirs.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     1970 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_sis.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     1380 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_sis_fixedrecovery.py
--rw-r--r--   0 sd80      (1000) sd80      (1000)     2142 2022-03-26 13:36:42.000000 epydemic-1.9.3/test/test_sto_sync.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     3970 2021-03-08 12:11:21.000000 epydemic-1.9.3/test/test_stochasticrates.py
--rw-rw-r--   0 sd80      (1000) sd80      (1000)     2012 2022-01-26 13:44:59.000000 epydemic-1.9.3/test/test_vaccination.py
+drwxrwxr--   0 sd80      (1000) sd80      (1000)        0 2022-03-27 14:10:38.913767 epydemic-1.9.4/
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)    35141 2021-03-08 12:11:21.000000 epydemic-1.9.4/LICENSE
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3301 2022-03-27 14:10:38.913767 epydemic-1.9.4/PKG-INFO
+-rw-r--r--   0 sd80      (1000) sd80      (1000)     2516 2022-03-19 12:24:11.000000 epydemic-1.9.4/README.rst
+drwxrwxr--   0 sd80      (1000) sd80      (1000)        0 2022-03-27 14:10:38.913767 epydemic-1.9.4/epydemic/
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3881 2022-03-08 11:14:37.000000 epydemic-1.9.4/epydemic/__init__.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     5694 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/adddelete.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)    16334 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/bbt.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3360 2021-04-27 09:29:54.000000 epydemic-1.9.4/epydemic/bitstream.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)    23768 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/compartmentedmodel.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     4654 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/drawset.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     5465 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/generator.py
+drwxrwxr--   0 sd80      (1000) sd80      (1000)        0 2022-03-27 14:10:38.913767 epydemic-1.9.4/epydemic/gf/
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     1167 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/gf/__init__.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3791 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/gf/continuous_gf.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3181 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/gf/discrete_gf.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2958 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/gf/function_gf.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     4167 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/gf/gf.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2077 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/gf/interface.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3024 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/gf/standard_gfs.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3258 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/loci.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     4445 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/monitor.py
+-rw-r--r--   0 sd80      (1000) sd80      (1000)    15664 2022-03-27 14:06:38.000000 epydemic-1.9.4/epydemic/networkdynamics.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     6035 2022-03-08 11:14:37.000000 epydemic-1.9.4/epydemic/networkexperiment.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)    17143 2022-03-08 11:14:37.000000 epydemic-1.9.4/epydemic/newmanziff.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     7487 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/opinion_model.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     4322 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/percolate.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     5476 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/plc_generator.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)    14640 2022-03-08 11:14:37.000000 epydemic-1.9.4/epydemic/process.py
+-rw-r--r--   0 sd80      (1000) sd80      (1000)     5978 2022-03-22 10:18:58.000000 epydemic-1.9.4/epydemic/processsequence.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)        0 2021-03-08 12:11:21.000000 epydemic-1.9.4/epydemic/py.typed
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     6825 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/seir_model.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     4341 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/shuffle.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3772 2022-03-22 09:34:18.000000 epydemic-1.9.4/epydemic/sir_model.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3648 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/sir_model_fixed_recovery.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2416 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/sirs_model.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     5720 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/sis_model.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3649 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/sis_model_fixed_recovery.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     6965 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/sivr_model.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     6080 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/standard_generators.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3606 2022-03-08 11:14:37.000000 epydemic-1.9.4/epydemic/statistics.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     4434 2022-03-26 12:48:29.000000 epydemic-1.9.4/epydemic/stochasticdynamics.py
+-rw-r--r--   0 sd80      (1000) sd80      (1000)     4162 2022-03-26 13:13:03.000000 epydemic-1.9.4/epydemic/synchronousdynamics.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     1110 2021-03-08 12:11:21.000000 epydemic-1.9.4/epydemic/types.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2582 2022-01-26 13:44:59.000000 epydemic-1.9.4/epydemic/vaccinate_model.py
+drwxrwxr--   0 sd80      (1000) sd80      (1000)        0 2022-03-27 14:10:38.913767 epydemic-1.9.4/epydemic.egg-info/
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3301 2022-03-27 14:10:38.000000 epydemic-1.9.4/epydemic.egg-info/PKG-INFO
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     1822 2022-03-27 14:10:38.000000 epydemic-1.9.4/epydemic.egg-info/SOURCES.txt
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)        1 2022-03-27 14:10:38.000000 epydemic-1.9.4/epydemic.egg-info/dependency_links.txt
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)        1 2022-03-27 12:35:51.000000 epydemic-1.9.4/epydemic.egg-info/not-zip-safe
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)       95 2022-03-27 14:10:38.000000 epydemic-1.9.4/epydemic.egg-info/requires.txt
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)        9 2022-03-27 14:10:38.000000 epydemic-1.9.4/epydemic.egg-info/top_level.txt
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)      211 2022-03-27 14:10:38.913767 epydemic-1.9.4/setup.cfg
+-rw-r--r--   0 sd80      (1000) sd80      (1000)     2115 2022-03-27 14:10:09.000000 epydemic-1.9.4/setup.py
+drwxrwxr--   0 sd80      (1000) sd80      (1000)        0 2022-03-27 14:10:38.913767 epydemic-1.9.4/test/
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3158 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_adddelete.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     6304 2022-03-08 11:14:37.000000 epydemic-1.9.4/test/test_adddeletesir.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)    14377 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_bbt.py
+-rw-r--r--   0 sd80      (1000) sd80      (1000)     1377 2022-03-22 10:18:58.000000 epydemic-1.9.4/test/test_bitstream.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)    10186 2021-06-07 09:48:01.000000 epydemic-1.9.4/test/test_compartmentedmodel.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     7133 2022-03-08 11:14:37.000000 epydemic-1.9.4/test/test_events.py
+-rw-r--r--   0 sd80      (1000) sd80      (1000)     5531 2021-05-13 12:22:20.000000 epydemic-1.9.4/test/test_generators.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     8743 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_gf.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     7450 2022-03-08 12:50:18.000000 epydemic-1.9.4/test/test_gof.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2749 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_hitting.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2422 2021-04-27 09:29:54.000000 epydemic-1.9.4/test/test_loci.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3479 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_monitor.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     5947 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_networkdynamics.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     4048 2022-03-08 11:14:37.000000 epydemic-1.9.4/test/test_newmanziff.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2342 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_opinion.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2001 2021-06-07 14:06:17.000000 epydemic-1.9.4/test/test_percolate.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3771 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_process.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     4429 2022-03-08 11:14:37.000000 epydemic-1.9.4/test/test_processsequence.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2233 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_seir.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2613 2021-06-10 15:10:59.000000 epydemic-1.9.4/test/test_shuffle.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     1984 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_sir.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     1340 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_sir_fixedrecovery.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2087 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_sirs.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     1970 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_sis.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     1380 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_sis_fixedrecovery.py
+-rw-r--r--   0 sd80      (1000) sd80      (1000)     2142 2022-03-27 14:06:38.000000 epydemic-1.9.4/test/test_sto_sync.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     3970 2021-03-08 12:11:21.000000 epydemic-1.9.4/test/test_stochasticrates.py
+-rw-rw-r--   0 sd80      (1000) sd80      (1000)     2012 2022-01-26 13:44:59.000000 epydemic-1.9.4/test/test_vaccination.py
```

### Comparing `epydemic-1.9.3/LICENSE` & `epydemic-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/PKG-INFO` & `epydemic-1.9.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epydemic
-Version: 1.9.3
+Version: 1.9.4
 Summary: Epidemic network simulations in Python
 Home-page: http://github.com/simoninireland/epydemic
 Author: Simon Dobson
 Author-email: simoninireland@gmail.com
 License: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `epydemic-1.9.3/README.rst` & `epydemic-1.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/__init__.py` & `epydemic-1.9.4/epydemic/__init__.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/adddelete.py` & `epydemic-1.9.4/epydemic/adddelete.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/bbt.py` & `epydemic-1.9.4/epydemic/bbt.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/bitstream.py` & `epydemic-1.9.4/epydemic/bitstream.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/compartmentedmodel.py` & `epydemic-1.9.4/epydemic/compartmentedmodel.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/drawset.py` & `epydemic-1.9.4/epydemic/drawset.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/generator.py` & `epydemic-1.9.4/epydemic/generator.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/gf/__init__.py` & `epydemic-1.9.4/epydemic/gf/__init__.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/gf/continuous_gf.py` & `epydemic-1.9.4/epydemic/gf/continuous_gf.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/gf/discrete_gf.py` & `epydemic-1.9.4/epydemic/gf/discrete_gf.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/gf/function_gf.py` & `epydemic-1.9.4/epydemic/gf/function_gf.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/gf/gf.py` & `epydemic-1.9.4/epydemic/gf/gf.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/gf/interface.py` & `epydemic-1.9.4/epydemic/gf/interface.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/gf/standard_gfs.py` & `epydemic-1.9.4/epydemic/gf/standard_gfs.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/loci.py` & `epydemic-1.9.4/epydemic/loci.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/monitor.py` & `epydemic-1.9.4/epydemic/monitor.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/networkdynamics.py` & `epydemic-1.9.4/epydemic/networkdynamics.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/networkexperiment.py` & `epydemic-1.9.4/epydemic/networkexperiment.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/newmanziff.py` & `epydemic-1.9.4/epydemic/newmanziff.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/opinion_model.py` & `epydemic-1.9.4/epydemic/opinion_model.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/percolate.py` & `epydemic-1.9.4/epydemic/percolate.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/plc_generator.py` & `epydemic-1.9.4/epydemic/plc_generator.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/process.py` & `epydemic-1.9.4/epydemic/process.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/processsequence.py` & `epydemic-1.9.4/epydemic/processsequence.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/seir_model.py` & `epydemic-1.9.4/epydemic/seir_model.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/shuffle.py` & `epydemic-1.9.4/epydemic/shuffle.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/sir_model.py` & `epydemic-1.9.4/epydemic/sir_model.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/sir_model_fixed_recovery.py` & `epydemic-1.9.4/epydemic/sir_model_fixed_recovery.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/sirs_model.py` & `epydemic-1.9.4/epydemic/sirs_model.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/sis_model.py` & `epydemic-1.9.4/epydemic/sis_model.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/sis_model_fixed_recovery.py` & `epydemic-1.9.4/epydemic/sis_model_fixed_recovery.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/sivr_model.py` & `epydemic-1.9.4/epydemic/sivr_model.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/standard_generators.py` & `epydemic-1.9.4/epydemic/standard_generators.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/statistics.py` & `epydemic-1.9.4/epydemic/statistics.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/stochasticdynamics.py` & `epydemic-1.9.4/epydemic/stochasticdynamics.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/synchronousdynamics.py` & `epydemic-1.9.4/epydemic/synchronousdynamics.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/types.py` & `epydemic-1.9.4/epydemic/types.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic/vaccinate_model.py` & `epydemic-1.9.4/epydemic/vaccinate_model.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/epydemic.egg-info/PKG-INFO` & `epydemic-1.9.4/epydemic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epydemic
-Version: 1.9.3
+Version: 1.9.4
 Summary: Epidemic network simulations in Python
 Home-page: http://github.com/simoninireland/epydemic
 Author: Simon Dobson
 Author-email: simoninireland@gmail.com
 License: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `epydemic-1.9.3/epydemic.egg-info/SOURCES.txt` & `epydemic-1.9.4/epydemic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/setup.py` & `epydemic-1.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from setuptools import setup
 
 with open('README.rst') as f:
     longDescription = f.read()
 
 setup(name='epydemic',
-      version='1.9.3',
+      version='1.9.4',
       description='Epidemic network simulations in Python',
       long_description=longDescription,
       url='http://github.com/simoninireland/epydemic',
       author='Simon Dobson',
       author_email='simoninireland@gmail.com',
       license='License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
       classifiers=['Development Status :: 4 - Beta',
```

### Comparing `epydemic-1.9.3/test/test_adddelete.py` & `epydemic-1.9.4/test/test_adddelete.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_adddeletesir.py` & `epydemic-1.9.4/test/test_adddeletesir.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_bbt.py` & `epydemic-1.9.4/test/test_bbt.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_bitstream.py` & `epydemic-1.9.4/test/test_bitstream.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_compartmentedmodel.py` & `epydemic-1.9.4/test/test_compartmentedmodel.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_events.py` & `epydemic-1.9.4/test/test_events.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_generators.py` & `epydemic-1.9.4/test/test_generators.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_gf.py` & `epydemic-1.9.4/test/test_gf.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_gof.py` & `epydemic-1.9.4/test/test_gof.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_hitting.py` & `epydemic-1.9.4/test/test_hitting.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_loci.py` & `epydemic-1.9.4/test/test_loci.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_monitor.py` & `epydemic-1.9.4/test/test_monitor.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_networkdynamics.py` & `epydemic-1.9.4/test/test_networkdynamics.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_newmanziff.py` & `epydemic-1.9.4/test/test_newmanziff.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_opinion.py` & `epydemic-1.9.4/test/test_opinion.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_percolate.py` & `epydemic-1.9.4/test/test_percolate.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_process.py` & `epydemic-1.9.4/test/test_process.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_processsequence.py` & `epydemic-1.9.4/test/test_processsequence.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_seir.py` & `epydemic-1.9.4/test/test_seir.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_shuffle.py` & `epydemic-1.9.4/test/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_sir.py` & `epydemic-1.9.4/test/test_sir.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_sir_fixedrecovery.py` & `epydemic-1.9.4/test/test_sir_fixedrecovery.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_sirs.py` & `epydemic-1.9.4/test/test_sirs.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_sis.py` & `epydemic-1.9.4/test/test_sis.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_sis_fixedrecovery.py` & `epydemic-1.9.4/test/test_sis_fixedrecovery.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_sto_sync.py` & `epydemic-1.9.4/test/test_sto_sync.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_stochasticrates.py` & `epydemic-1.9.4/test/test_stochasticrates.py`

 * *Files identical despite different names*

### Comparing `epydemic-1.9.3/test/test_vaccination.py` & `epydemic-1.9.4/test/test_vaccination.py`

 * *Files identical despite different names*

