# Comparing `tmp/clover-energy-5.1.1.tar.gz` & `tmp/clover-energy-5.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/bewinche/modelling/CLOVER/dist/.tmp-uu0k8rq_/clover-energy-5.1.1.tar", last modified: Tue Jul 25 13:19:21 2023, max compression
+gzip compressed data, was "/home/bewinche/modelling/CLOVER/dist/.tmp-b80rycjl/clover-energy-5.1.2b1.tar", last modified: Thu Aug  3 15:09:15 2023, max compression
```

## Comparing `clover-energy-5.1.1.tar` & `clover-energy-5.1.2b1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1080 2023-06-30 07:49:00.000000 clover-energy-5.1.1/LICENSE
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)       47 2023-06-30 07:49:00.000000 clover-energy-5.1.1/MANIFEST.in
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16573 2023-07-25 13:19:21.000000 clover-energy-5.1.1/PKG-INFO
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    15933 2023-07-17 10:28:59.000000 clover-energy-5.1.1/README.md
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      103 2023-06-30 07:49:00.000000 clover-energy-5.1.1/pyproject.toml
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1296 2023-07-25 13:19:21.000000 clover-energy-5.1.1/setup.cfg
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2049 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    51535 2023-07-25 12:11:04.000000 clover-energy-5.1.1/src/clover/__main__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    97316 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    36718 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/analysis.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8512 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/argparser.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/conversion/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      710 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/conversion/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    26993 2023-07-17 10:28:59.000000 clover-energy-5.1.1/src/clover/conversion/conversion.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/conversion/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/conversion/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/conversion/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/conversion/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)   107239 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/fileparser.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/generation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/generation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    20730 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/generation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    27727 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/generation/solar.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/generation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/generation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/generation/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/generation/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/generation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/generation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4554 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/generation/weather.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3563 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/generation/wind.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/impact/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1141 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/impact/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4199 2023-07-17 10:28:59.000000 clover-energy-5.1.1/src/clover/impact/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    44572 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/impact/finance.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    31219 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/impact/ghgs.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/impact/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/impact/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/impact/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/impact/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/impact/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/impact/tests/unit/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/load/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      931 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/load/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    39767 2023-07-17 10:28:59.000000 clover-energy-5.1.1/src/clover/load/load.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/load/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/load/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/load/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/load/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/mains_supply/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      774 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/mains_supply/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4473 2023-07-11 16:32:53.000000 clover-energy-5.1.1/src/clover/mains_supply/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4578 2023-07-11 16:32:53.000000 clover-energy-5.1.1/src/clover/mains_supply/grid.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/mains_supply/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11741 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/mains_supply/water_source.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/optimisation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1069 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/optimisation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43348 2023-07-18 10:01:36.000000 clover-energy-5.1.1/src/clover/optimisation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    29385 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/optimisation/appraisal.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    64706 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/optimisation/optimisation.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43556 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/optimisation/single_line_simulation.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/optimisation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/optimisation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/optimisation/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/optimisation/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/optimisation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/optimisation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8754 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/printer.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/scripts/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1309 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1202 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/clover_hpc_clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1298 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/clover_hpc_outbox_assembly.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1138 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/clover_new_location.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1360 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/clover_update_api_token.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     6682 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/scripts/hpc.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    10191 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/hpc_clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4894 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/hpc_outbox_assembly.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    22944 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/scripts/hpc_utils.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11904 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/new_location.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/scripts/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/scripts/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3638 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/scripts/update_api_token.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/simulation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1199 2023-07-17 10:09:36.000000 clover-energy-5.1.1/src/clover/simulation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    21928 2023-07-18 09:54:23.000000 clover-energy-5.1.1/src/clover/simulation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    12992 2023-07-17 10:28:59.000000 clover-energy-5.1.1/src/clover/simulation/diesel.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    88978 2023-07-25 10:34:01.000000 clover-energy-5.1.1/src/clover/simulation/energy_system.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2450 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/simulation/exchanger.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    24234 2023-07-17 10:28:59.000000 clover-energy-5.1.1/src/clover/simulation/solar.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    31896 2023-07-25 12:19:28.000000 clover-energy-5.1.1/src/clover/simulation/storage.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19002 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/simulation/storage_utils.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/simulation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/simulation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/simulation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/simulation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     5411 2023-07-11 16:48:20.000000 clover-energy-5.1.1/src/clover/simulation/transmission.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/src/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/src/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    56900 2023-07-25 10:16:42.000000 clover-energy-5.1.1/src/clover/src/new_location.yaml
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/tests/integration/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.1/src/clover/tests/integration/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:49:00.000000 clover-energy-5.1.1/src/clover/tests/unit/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-25 13:19:21.000000 clover-energy-5.1.1/src/clover_energy.egg-info/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16573 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/PKG-INFO
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3003 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/SOURCES.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)        1 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/dependency_links.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      299 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/entry_points.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      119 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/requires.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)        7 2023-07-25 13:19:20.000000 clover-energy-5.1.1/src/clover_energy.egg-info/top_level.txt
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1080 2023-06-30 07:49:00.000000 clover-energy-5.1.2b1/LICENSE
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)       47 2023-06-30 07:49:00.000000 clover-energy-5.1.2b1/MANIFEST.in
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16575 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/PKG-INFO
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    15933 2023-07-17 10:28:59.000000 clover-energy-5.1.2b1/README.md
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      103 2023-06-30 07:49:00.000000 clover-energy-5.1.2b1/pyproject.toml
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1298 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/setup.cfg
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2063 2023-08-03 09:11:13.000000 clover-energy-5.1.2b1/src/clover/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    51720 2023-08-03 09:29:41.000000 clover-energy-5.1.2b1/src/clover/__main__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    97953 2023-08-03 09:13:06.000000 clover-energy-5.1.2b1/src/clover/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    36718 2023-07-18 09:54:23.000000 clover-energy-5.1.2b1/src/clover/analysis.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8512 2023-07-18 09:54:23.000000 clover-energy-5.1.2b1/src/clover/argparser.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/conversion/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      710 2023-07-17 10:09:36.000000 clover-energy-5.1.2b1/src/clover/conversion/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    26993 2023-07-17 10:28:59.000000 clover-energy-5.1.2b1/src/clover/conversion/conversion.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/conversion/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/conversion/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/conversion/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/conversion/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)   109376 2023-08-03 10:16:33.000000 clover-energy-5.1.2b1/src/clover/fileparser.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/generation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/generation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    20862 2023-07-27 17:44:33.000000 clover-energy-5.1.2b1/src/clover/generation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    29087 2023-08-03 09:24:45.000000 clover-energy-5.1.2b1/src/clover/generation/solar.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/generation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/generation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/generation/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/generation/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/generation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/generation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4638 2023-07-27 17:44:33.000000 clover-energy-5.1.2b1/src/clover/generation/weather.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3647 2023-07-27 17:44:33.000000 clover-energy-5.1.2b1/src/clover/generation/wind.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/impact/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1141 2023-07-17 10:09:36.000000 clover-energy-5.1.2b1/src/clover/impact/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4199 2023-07-17 10:28:59.000000 clover-energy-5.1.2b1/src/clover/impact/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    44607 2023-08-03 09:10:24.000000 clover-energy-5.1.2b1/src/clover/impact/finance.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    31276 2023-08-03 09:24:55.000000 clover-energy-5.1.2b1/src/clover/impact/ghgs.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/impact/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/impact/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/impact/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/impact/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/impact/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/impact/tests/unit/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/load/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      931 2023-07-17 10:09:36.000000 clover-energy-5.1.2b1/src/clover/load/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    39767 2023-07-17 10:28:59.000000 clover-energy-5.1.2b1/src/clover/load/load.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/load/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/load/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/load/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/load/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/mains_supply/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      774 2023-07-17 10:09:36.000000 clover-energy-5.1.2b1/src/clover/mains_supply/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4473 2023-07-11 16:32:53.000000 clover-energy-5.1.2b1/src/clover/mains_supply/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4578 2023-07-11 16:32:53.000000 clover-energy-5.1.2b1/src/clover/mains_supply/grid.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/mains_supply/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/mains_supply/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/mains_supply/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/mains_supply/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover/mains_supply/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/mains_supply/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11741 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/mains_supply/water_source.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/optimisation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1069 2023-07-17 10:09:36.000000 clover-energy-5.1.2b1/src/clover/optimisation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43379 2023-08-03 10:16:55.000000 clover-energy-5.1.2b1/src/clover/optimisation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    29817 2023-08-03 09:10:43.000000 clover-energy-5.1.2b1/src/clover/optimisation/appraisal.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    64764 2023-08-03 08:55:50.000000 clover-energy-5.1.2b1/src/clover/optimisation/optimisation.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43591 2023-08-03 08:56:02.000000 clover-energy-5.1.2b1/src/clover/optimisation/single_line_simulation.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/optimisation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/optimisation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/optimisation/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/optimisation/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/optimisation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/optimisation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8754 2023-07-18 09:54:23.000000 clover-energy-5.1.2b1/src/clover/printer.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/scripts/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1309 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1202 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/clover_hpc_clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1298 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/clover_hpc_outbox_assembly.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1138 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/clover_new_location.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1360 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/clover_update_api_token.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     6682 2023-07-17 10:09:36.000000 clover-energy-5.1.2b1/src/clover/scripts/hpc.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    10191 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/hpc_clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4894 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/hpc_outbox_assembly.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    22944 2023-07-17 10:09:36.000000 clover-energy-5.1.2b1/src/clover/scripts/hpc_utils.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11904 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/new_location.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/scripts/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/scripts/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/scripts/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3490 2023-07-27 17:44:33.000000 clover-energy-5.1.2b1/src/clover/scripts/update_api_token.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/simulation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1199 2023-08-03 09:11:23.000000 clover-energy-5.1.2b1/src/clover/simulation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    23270 2023-08-03 10:16:00.000000 clover-energy-5.1.2b1/src/clover/simulation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    12992 2023-07-17 10:28:59.000000 clover-energy-5.1.2b1/src/clover/simulation/diesel.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    88978 2023-08-03 08:50:10.000000 clover-energy-5.1.2b1/src/clover/simulation/energy_system.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2450 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/simulation/exchanger.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    24234 2023-07-17 10:28:59.000000 clover-energy-5.1.2b1/src/clover/simulation/solar.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    31896 2023-07-26 10:55:23.000000 clover-energy-5.1.2b1/src/clover/simulation/storage.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19828 2023-07-26 16:11:27.000000 clover-energy-5.1.2b1/src/clover/simulation/storage_utils.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/simulation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/simulation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/simulation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/simulation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     5411 2023-07-11 16:48:20.000000 clover-energy-5.1.2b1/src/clover/simulation/transmission.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/src/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/src/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    56528 2023-08-03 09:00:05.000000 clover-energy-5.1.2b1/src/clover/src/new_location.yaml
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/tests/integration/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.1.2b1/src/clover/tests/integration/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:49:00.000000 clover-energy-5.1.2b1/src/clover/tests/unit/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-08-03 15:09:15.000000 clover-energy-5.1.2b1/src/clover_energy.egg-info/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16575 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover_energy.egg-info/PKG-INFO
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3003 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover_energy.egg-info/SOURCES.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)        1 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover_energy.egg-info/dependency_links.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      299 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover_energy.egg-info/entry_points.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      119 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover_energy.egg-info/requires.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)        7 2023-08-03 15:09:14.000000 clover-energy-5.1.2b1/src/clover_energy.egg-info/top_level.txt
```

### Comparing `clover-energy-5.1.1/LICENSE` & `clover-energy-5.1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/PKG-INFO` & `clover-energy-5.1.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clover-energy
-Version: 5.1.1
+Version: 5.1.2b1
 Summary: Continuous Lifetime Optimisation of Variable Electricity Resources
 Home-page: https://github.com/CLOVER-energy/CLOVER
 Author: Phil Sandwell, Ben Winchester and Hamish Beath
 Author-email: philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 Project-URL: Bug Tracker, https://github.com/CLOVER-energy/CLOVER/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clover-energy-5.1.1/README.md` & `clover-energy-5.1.2b1/README.md`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/setup.cfg` & `clover-energy-5.1.2b1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = clover-energy
-version = 5.1.1
+version = 5.1.2b1
 author = Phil Sandwell, Ben Winchester and Hamish Beath
 author_email = philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 description = Continuous Lifetime Optimisation of Variable Electricity Resources
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CLOVER-energy/CLOVER
 project_urls =
```

### Comparing `clover-energy-5.1.1/src/clover/__init__.py` & `clover-energy-5.1.2b1/src/clover/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     get_logger,
     HEAT_CAPACITY_OF_WATER,
     HotWaterScenario,
     hourly_profile_to_daily_sum,
     HTFMode,
     InputFileError,
     InternalError,
+    Inverter,
     KEROSENE_DEVICE_NAME,
     KeyResults,
     Location,
     LOCATIONS_FOLDER_NAME,
     LOGGER_DIRECTORY,
     monthly_profile_to_daily_profile,
     monthly_times_to_daily_times,
```

### Comparing `clover-energy-5.1.1/src/clover/__main__.py` & `clover-energy-5.1.2b1/src/clover/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 CLOVER (Continuous Lifetime Optimisation of Variable Electricity Resources) can evaluate
 and optimise minigrid systems, determining whether a demand is met whilst minimising
 environmental and economic impacts. The main flow of CLOVER can be executed by running
 the clover module from the command-line interface.
 
 """
 
-__version__ = "5.1.1"
+__version__ = "5.1.2b1"
 
 import collections
 import datetime
 import logging
 import math
 import os
 import re
@@ -572,14 +572,15 @@
         (
             converters,
             device_utilisations,
             minigrid,
             finance_inputs,
             generation_inputs,
             ghg_inputs,
+            global_settings_inputs,
             grid_times,
             location,
             optimisation_inputs,
             optimisations,
             scenarios,
             simulations,
             electric_load_profile,
@@ -699,14 +700,15 @@
 
     # Generate and save the wind data for each year as a background task.
     if any(scenario.pv_t for scenario in scenarios):
         logger.info("Beginning wind-data fetching.")
         wind_data_thread: Optional[wind.WindDataThread] = wind.WindDataThread(
             os.path.join(auto_generated_files_directory, "wind"),
             generation_inputs,
+            global_settings_inputs,
             location,
             f"{parsed_args.location}_{wind.WIND_LOGGER_NAME}",
             ninja_pause_index,
             parsed_args.refetch,
             num_ninjas,
             parsed_args.verbose,
         )
@@ -726,14 +728,15 @@
         # Set up the system to call renewables.ninja at a slower rate.
         logger.info("Begining weather-data fetching.")
         weather_data_thread: Optional[
             weather.WeatherDataThread
         ] = weather.WeatherDataThread(
             os.path.join(auto_generated_files_directory, "weather"),
             generation_inputs,
+            global_settings_inputs,
             location,
             f"{parsed_args.location}_{weather.WEATHER_LOGGER_NAME}",
             ninja_pause_index,
             parsed_args.refetch,
             num_ninjas,
             parsed_args.verbose,
         )
@@ -753,14 +756,15 @@
     # Generate and save the solar data for each year as a background task.
     logger.info("Beginning solar-data fetching.")
     solar_data_threads: Dict[solar.PVPanel, solar.SolarDataThread] = {}
     for pv_panel in panels_to_fetch:
         solar_data_threads[pv_panel] = solar.SolarDataThread(
             os.path.join(auto_generated_files_directory, "solar"),
             generation_inputs,
+            global_settings_inputs,
             location,
             f"{parsed_args.location}_{solar.SOLAR_LOGGER_NAME}_"
             f"{solar.get_profile_prefix(pv_panel)}_{run_number_string}",
             ninja_pause_index,
             parsed_args.refetch,
             pv_panel,
             num_ninjas,
@@ -1189,14 +1193,15 @@
                         "system despite these being needed to appraise the system."
                     )
                 system_appraisal: Optional[SystemAppraisal] = appraise_system(
                     electric_yearly_load_statistics,
                     simulation.end_year,
                     finance_inputs,
                     ghg_inputs,
+                    minigrid.inverter,
                     location,
                     logger,
                     None,
                     scenario,
                     system_performance_outputs,
                     simulation.start_year,
                     system_details,
```

### Comparing `clover-energy-5.1.1/src/clover/__utils__.py` & `clover-energy-5.1.2b1/src/clover/__utils__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import pandas as pd  # pylint: disable=import-error
 import scipy  # pylint: disable=import-error
 import yaml  # pylint: disable=import-error
 
 from tqdm import tqdm  # pylint: disable=import-error
 
 __all__ = (
+    "API_TOKEN_PLACEHOLDER_TEXT",
     "BColours",
     "CleanWaterMode",
     "Criterion",
     "CUT_OFF_TIME",
     "daily_sum_to_monthly_sum",
     "DEFAULT_SCENARIO",
     "DemandType",
@@ -52,14 +53,15 @@
     "get_logger",
     "HEAT_CAPACITY_OF_WATER",
     "HotWaterScenario",
     "hourly_profile_to_daily_sum",
     "HTFMode",
     "InputFileError",
     "InternalError",
+    "Inverter",
     "KEROSENE_DEVICE_NAME",
     "KeyResults",
     "Location",
     "LOCATIONS_FOLDER_NAME",
     "LOGGER_DIRECTORY",
     "monthly_profile_to_daily_profile",
     "monthly_times_to_daily_times",
@@ -78,14 +80,18 @@
     "Simulation",
     "SystemAppraisal",
     "SystemDetails",
     "ZERO_CELCIUS_OFFSET",
 )
 
 
+# API token placeholder text:
+#   Placeholder text to use when the renewables.ninja API token has not been specified.
+API_TOKEN_PLACEHOLDER_TEXT: str = "YOUR API TOKEN HERE"
+
 # Cold water:
 #   Used for parsing cold-water related information.
 COLD_WATER: str = "cold_water"
 
 # Conventional sources:
 #   Keyword used for parsing conventional-source information.
 CONVENTIONAL_SOURCES: str = "conventional_sources"
@@ -213,14 +219,18 @@
 #   optimisations.
 STEP: str = "step"
 
 # Supply temperature:
 #   Used to parse supply-temperature information.
 SUPPLY_TEMPERATURE: str = "supply_temperature"
 
+# Token:
+#   Keyword used when parsing the generation token.
+TOKEN: str = "renewables_ninja_token"
+
 # Zero celcius offset:
 #   Used for offsetting zero degrees celcius in Kelvin.
 ZERO_CELCIUS_OFFSET: float = 273.15
 
 
 class AuxiliaryHeaterType(enum.Enum):
     """
@@ -878,14 +888,31 @@
 
         """
 
         super().__init__(f"An error occured internally within CLOVER: {msg}")
 
 
 @dataclasses.dataclass
+class Inverter:
+    """
+    Represents an inverter within the system.
+
+    .. attribute:: lifetime
+        The lifetime, in years, of the inverter.
+
+    .. attribute:: size_increment
+        The size increment of the inverter in kW.
+
+    """
+
+    lifetime: int
+    size_increment: float
+
+
+@dataclasses.dataclass
 class KeyResults:
     """
     Contains the key results from a simulation.
 
     .. attribute:: average_pv_generation
         The average energy generated by the PV set up per day, measured in kWh/day, for
         each of the PV panel types installed.
```

### Comparing `clover-energy-5.1.1/src/clover/analysis.py` & `clover-energy-5.1.2b1/src/clover/analysis.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/argparser.py` & `clover-energy-5.1.2b1/src/clover/argparser.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/conversion/__init__.py` & `clover-energy-5.1.2b1/src/clover/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/conversion/conversion.py` & `clover-energy-5.1.2b1/src/clover/conversion/conversion.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/fileparser.py` & `clover-energy-5.1.2b1/src/clover/fileparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 
 from collections import defaultdict
 from logging import Logger
 from typing import Any, DefaultDict, Dict, List, Optional, Set, Tuple, Union
 
 import json
 import pandas as pd  # pylint: disable=import-error
+import yaml
 
 # from sklearn.linear_model._coordinate_descent import Lasso
 
 from . import load
 from .generation import solar
 from .impact.finance import COSTS, FINANCE_IMPACT, ImpactingComponent
 from .impact.ghgs import EMISSIONS, GHG_IMPACT
 from .simulation.diesel import DIESEL_CONSUMPTION, MINIMUM_LOAD, DieselWaterHeater
 
 from .__utils__ import (
+    API_TOKEN_PLACEHOLDER_TEXT,
     AuxiliaryHeaterType,
     BColours,
     DesalinationScenario,
     DieselMode,
     EXCHANGER,
     HotWaterScenario,
     HTFMode,
@@ -47,28 +49,30 @@
     LOCATIONS_FOLDER_NAME,
     NAME,
     PACKAGE_NAME,
     RAW_CLOVER_PATH,
     read_yaml,
     Scenario,
     Simulation,
+    TOKEN,
 )
 from .conversion.conversion import (
     Converter,
     MultiInputConverter,
     ThermalDesalinationPlant,
     WaterSource,
 )
 from .optimisation.__utils__ import Optimisation, OptimisationParameters
 from .simulation.diesel import DieselGenerator
 from .simulation.energy_system import Minigrid
 from .simulation.transmission import Transmitter
 
 __all__ = (
     "GENERATION_INPUTS_FILE",
+    "GLOBAL_SETTINGS_FILE",
     "INPUTS_DIRECTORY",
     "KEROSENE_TIMES_FILE",
     "KEROSENE_USAGE_FILE",
     "LOCATIONS_FOLDER_NAME",
     "parse_input_files",
     "parse_scenario_inputs",
 )
@@ -173,14 +177,18 @@
 #   The relative path to the generation-inputs file.
 GENERATION_INPUTS_FILE: str = os.path.join("generation", "generation_inputs.yaml")
 
 # GHG inputs file:
 #   The relative path to the GHG inputs file.
 GHG_INPUTS_FILE: str = os.path.join("impact", "ghg_inputs.yaml")
 
+# Global settings file:
+#   The relative path to the global-settings file.
+GLOBAL_SETTINGS_FILE: str = "global_settings.yaml"
+
 # Grid inputs file:
 #   The relative path to the grid-inputs file.
 GRID_TIMES_FILE: str = os.path.join("generation", "grid_times.csv")
 
 # Hot-water scenarios:
 #   Keyword used for parsing hot-water scenarios.
 HOT_WATER_SCENARIOS: str = "hot_water_scenarios"
@@ -940,14 +948,52 @@
         exchanger_costs,
         exchanger_emissions,
         exchanger_inputs[EXCHANGERS],
         exchanger_inputs_filepath,
     )
 
 
+def _parse_global_settings(logger: Logger) -> Dict[str, Any]:
+    """Parses the global-settings file."""
+
+    def _create_global_setings_file() -> None:
+        """Create a default global-settings file if missing."""
+
+        with open(GLOBAL_SETTINGS_FILE, "w", encoding="UTF-8") as global_settings_file:
+            yaml.dump({TOKEN: API_TOKEN_PLACEHOLDER_TEXT}, global_settings_file)
+
+    # Parse global settings.
+    if not os.path.isfile(GLOBAL_SETTINGS_FILE):
+        _create_global_setings_file()
+
+    try:
+        global_settings_inputs: Optional[
+            Union[Dict[str, Any], List[Dict[str, Any]]]
+        ] = read_yaml(GLOBAL_SETTINGS_FILE, logger)
+    except FileNotFoundError:
+        logger.error(
+            "No global-settings file found, check that this file was correctly created "
+            "and exists in your current CLOVER directory."
+        )
+        raise InternalError("Error parsing global-settings file.") from None
+    logger.info("Global settings inputs successfully read.")
+
+    # Ensure that the global-settings inputs are the correct format.
+    if not isinstance(global_settings_inputs, dict):
+        if global_settings_inputs is None:
+            global_settings_inputs = {}
+        else:
+            logger.error("Global settings inputs are not of type `dict`.")
+            raise InputFileError(
+                "global_settings.yaml", "Global-settings must be of type `dict`."
+            )
+
+    return global_settings_inputs
+
+
 def _parse_pvt_reduced_models(  # pylint: disable=too-many-statements
     debug: bool, logger: Logger, scenarios: List[Scenario]
 ) -> Tuple[Any, Any]:
     """
     Parses the PV-T models from the installed package or raw files.
 
     Inputs:
@@ -1749,14 +1795,15 @@
         tank_inputs_filepath,
     )
 
 
 def _parse_minigrid_inputs(  # pylint: disable=too-many-locals, too-many-statements
     converters: Dict[str, Converter],
     debug: bool,
+    finance_inputs: DefaultDict[str, DefaultDict[str, float]],
     inputs_directory_relative_path: str,
     logger: Logger,
     scenarios: List[Scenario],
 ) -> Tuple[
     Optional[Dict[str, float]],
     Optional[Dict[str, float]],
     str,
@@ -1792,14 +1839,16 @@
 
     Inputs:
         - converters:
             The `list` of :class:`Converter` instances available to the system.
         - debug:
             Whether to use the PV-T reduced models (False) or invented data for
             debugging purposes (True).
+        - finance_inputs:
+            The financial input information.
         - inputs_directory_relative_path:
             The relative path to the inputs folder directory.
         - logger:
             The :class:`logging.Logger` to use for the run.
         - scenarios:
             The `list` of :class:`Scenario` instances being used for the run.
 
@@ -2019,14 +2068,16 @@
     else:
         electric_water_heater = None
 
     minigrid: Minigrid = Minigrid.from_dict(
         diesel_generator,
         diesel_water_heater,
         electric_water_heater,
+        finance_inputs,
+        logger,
         energy_system_inputs,
         pv_panels,
         pvt_panels,
         battery_inputs,
         exchanger_inputs,
         tank_inputs,
         water_pump,
@@ -2229,14 +2280,15 @@
 ) -> Tuple[
     Dict[str, Converter],
     Dict[load.load.Device, pd.DataFrame],
     Minigrid,
     DefaultDict[str, DefaultDict[str, float]],
     Dict[str, Union[int, str]],
     DefaultDict[str, DefaultDict[str, float]],
+    Dict[str, str],
     pd.DataFrame,
     Location,
     Optional[OptimisationParameters],
     List[Optimisation],
     List[Scenario],
     List[Simulation],
     Optional[pd.DataFrame],
@@ -2265,28 +2317,33 @@
         - A tuple containing:
             - converters,
             - device_utilisations, optional if carrying out load-profile generation,
             - diesel_inputs,
             - minigrid,
             - finance_inputs,
             - ghg_inputs,
+            - global_settings_inputs,
             - grid_times,
             - optimisation_inputs,
             - optimisations, the `set` of optimisations to run,
             - scenarios,
             - simulations, the `list` of simulations to run,
             - a `list` of :class:`solar.SolarPanel` instances and their children which
               contain information about the PV panels being considered,
             - total_load_profile, optional if specified to be overriden,
             - a `dict` mapping the :class:`WaterSource`s available to provide
               conventional water to the system and the seasonal availabilities,
             - a `dict` containing information about the input files used.
 
     """
 
+    # Parse global-settings files
+    global_settings_inputs = _parse_global_settings(logger)
+
+    # Parse location-specific files.
     inputs_directory_relative_path = os.path.join(
         LOCATIONS_FOLDER_NAME,
         location_name,
         INPUTS_DIRECTORY,
     )
 
     # Parse the conversion inputs file.
@@ -2421,14 +2478,44 @@
         raise InputFileError(
             "simulation inputs", "Simulation inputs must be of type `list`."
         )
     simulations: List[Simulation] = [
         Simulation.from_dict(entry) for entry in simulations_file_contents
     ]
 
+    # Parse and collate the impact information.
+    finance_inputs_filepath = os.path.join(
+        inputs_directory_relative_path, FINANCE_INPUTS_FILE
+    )
+    # Finance input type: Dict[str, Union[float, Dict[str, float]]]
+    finance_data = read_yaml(finance_inputs_filepath, logger)
+    if not isinstance(finance_data, dict):
+        raise InputFileError(
+            "finance inputs", "Finance inputs must be of type `dict` not `list`."
+        )
+    finance_inputs: DefaultDict[str, DefaultDict[str, float]] = defaultdict(
+        lambda: defaultdict(float)
+    )
+    finance_inputs.update(finance_data)
+    logger.info("Finance inputs successfully parsed.")
+
+    ghg_inputs_filepath = os.path.join(inputs_directory_relative_path, GHG_INPUTS_FILE)
+    # Ghg data type: Dict[str, Union[float, Dict[str, float]]]
+    ghg_data = read_yaml(ghg_inputs_filepath, logger)
+    if not isinstance(finance_data, dict):
+        raise InputFileError(
+            "ghg inputs", "GHG inputs must be of type `dict` not `list`."
+        )
+    # Generate a default dict to take care of missing data.
+    ghg_inputs: DefaultDict[str, DefaultDict[str, float]] = defaultdict(
+        lambda: defaultdict(float)
+    )
+    ghg_inputs.update(ghg_data)  # type: ignore
+    logger.info("GHG inputs successfully parsed.")
+
     # Parse the energy-system input information.
     (
         battery_costs,
         battery_emissions,
         battery_inputs_filepath,
         buffer_tank_costs,
         buffer_tank_emissions,
@@ -2453,15 +2540,20 @@
         solar_generation_inputs_filepath,
         tank_inputs_filepath,
         transmission_costs,
         transmission_emissions,
         transmission_inputs_filepath,
         transmitters,
     ) = _parse_minigrid_inputs(
-        converters, debug, inputs_directory_relative_path, logger, scenarios
+        converters,
+        debug,
+        finance_inputs,
+        inputs_directory_relative_path,
+        logger,
+        scenarios,
     )
     logger.info("Energy-system inputs successfully parsed.")
 
     generation_inputs_filepath = os.path.join(
         inputs_directory_relative_path, GENERATION_INPUTS_FILE
     )
     generation_inputs = read_yaml(generation_inputs_filepath, logger)
@@ -2564,44 +2656,14 @@
     location: Location = Location.from_dict(location_inputs)
     if not isinstance(location, Location):
         raise InternalError(
             "Location was not returned when calling `Location.from_dict`."
         )
     logger.info("Location inputs successfully parsed.")
 
-    # Parse and collate the impact information.
-    finance_inputs_filepath = os.path.join(
-        inputs_directory_relative_path, FINANCE_INPUTS_FILE
-    )
-    # Finance input type: Dict[str, Union[float, Dict[str, float]]]
-    finance_data = read_yaml(finance_inputs_filepath, logger)
-    if not isinstance(finance_data, dict):
-        raise InputFileError(
-            "finance inputs", "Finance inputs must be of type `dict` not `list`."
-        )
-    finance_inputs: DefaultDict[str, DefaultDict[str, float]] = defaultdict(
-        lambda: defaultdict(float)
-    )
-    finance_inputs.update(finance_data)
-    logger.info("Finance inputs successfully parsed.")
-
-    ghg_inputs_filepath = os.path.join(inputs_directory_relative_path, GHG_INPUTS_FILE)
-    # Ghg data type: Dict[str, Union[float, Dict[str, float]]]
-    ghg_data = read_yaml(ghg_inputs_filepath, logger)
-    if not isinstance(finance_data, dict):
-        raise InputFileError(
-            "ghg inputs", "GHG inputs must be of type `dict` not `list`."
-        )
-    # Generate a default dict to take care of missing data.
-    ghg_inputs: DefaultDict[str, DefaultDict[str, float]] = defaultdict(
-        lambda: defaultdict(float)
-    )
-    ghg_inputs.update(ghg_data)  # type: ignore
-    logger.info("GHG inputs successfully parsed.")
-
     # Update the finance and GHG inputs accordingly with the PV data.
     logger.info("Updating with PV impact data.")
     finance_inputs[ImpactingComponent.PV.value] = defaultdict(
         lambda: defaultdict(float), pv_panel_costs  # type: ignore [arg-type, return-value]
     )
     ghg_inputs[ImpactingComponent.PV.value] = defaultdict(
         lambda: defaultdict(float), pv_panel_emissions  # type: ignore [arg-type, return-value]
@@ -2844,15 +2906,15 @@
         "finance_inputs": finance_inputs_filepath,
         "generation_inputs": generation_inputs_filepath,
         "ghg_inputs": ghg_inputs_filepath,
         "grid_times": grid_times_filepath,
         "location_inputs": location_inputs_filepath,
         "optimisation_inputs": optimisation_inputs_filepath,
         "scenarios": scenario_inputs_filepath,
-        "simularion": simulations_inputs_filepath,
+        "simulation": simulations_inputs_filepath,
         "solar_inputs": solar_generation_inputs_filepath,
         "transmission_inputs": transmission_inputs_filepath,
     }
 
     if any(scenario.desalination_scenario is not None for scenario in scenarios):
         if conventional_water_source_inputs_filepath is not None:
             input_file_info[
@@ -2903,14 +2965,15 @@
     return (
         converters,
         device_utilisations,
         minigrid,
         finance_inputs,
         generation_inputs,
         ghg_inputs,
+        global_settings_inputs,
         grid_times,
         location,
         optimisation_parameters,
         optimisations,
         scenarios,
         simulations,
         total_load_profile,
```

### Comparing `clover-energy-5.1.1/src/clover/generation/__utils__.py` & `clover-energy-5.1.2b1/src/clover/generation/__utils__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,19 +41,19 @@
 
 from ..__utils__ import (
     BColours,
     InternalError,
     get_logger,
     Location,
     RenewablesNinjaError,
+    TOKEN,
 )
 
 __all__ = (
     "BaseRenewablesNinjaThread",
-    "TOKEN",
     "total_profile_output",
 )
 
 
 # Api base:
 #   The base API name of renewables.ninja.
 API_BASE = "https://www.renewables.ninja/api/"
@@ -63,18 +63,14 @@
 FEB_29: int = (31 + 28) * 24
 
 # Renewables.ninja sleep time:
 #   To avoid being locked out of the renewables.ninja API, it is necessary for CLOVER to
 #   sleep between requests. The time taken for this, in seconds, is set below.
 RENEWABLES_NINJA_SLEEP_TIME = 12
 
-# Token:
-#   Keyword used when parsing the generation token.
-TOKEN = "token"
-
 
 class SolarDataType(enum.Enum):
     """
     Denotes the types of solar data being stored.
 
     - DIFFUSE_IRRADIANCE:
         Denotes the diffuse irradiance striking a panel.
@@ -356,14 +352,15 @@
     profile_name: str
     profile_key: str
 
     def __init__(
         self,
         auto_generated_files_directory: str,
         generation_inputs: Dict[str, Any],
+        global_settings_inputs: Dict[str, str],
         location: Location,
         logger_name: str,
         pause_time: int,
         regenerate: bool,
         sleep_multiplier: int,
         verbose: bool,
         *,
@@ -374,14 +371,16 @@
         Instantiate a renewables-ninja-base-data thread.
 
         Inputs:
             - auto_generated_files_directory:
                 The directory in which CLOVER-generated files should be saved.
             - generation_inputs:
                 The generation inputs.
+            - global_settings_inputs:
+                The global-settings inputs.
             - location:
                 The location currently being considerted.
             - logger_name:
                 The name to use for the logger.
             - pause_time:
                 A time for which to pause before initialising data fetching to avoid
                 short-burst errors from renewables.ninja.
@@ -399,14 +398,15 @@
 
         """
 
         self.auto_generated_files_directory: str = auto_generated_files_directory
         self.generation_inputs: Dict[
             str, Union[bool, int, str, float]
         ] = generation_inputs
+        self.global_settings_inputs: Dict[str, str] = global_settings_inputs
         self.location: Location = location
         self.logger: Logger = get_logger(logger_name, verbose)
         self.logger_name: str = logger_name
         self.pause_time: int = pause_time
         self.profile_prefix: str = profile_prefix
         self.regenerate: bool = regenerate
         self.renewables_ninja_params: Dict[str, Any] = renewables_ninja_params
@@ -483,15 +483,15 @@
                 self.logger.info(
                     "Fetching %s data for year %s.",
                     self.profile_name,
                     year,
                 )
                 try:
                     data = _get_profile_output(
-                        str(self.generation_inputs[TOKEN]),
+                        str(self.global_settings_inputs[TOKEN]),
                         self.location,
                         self.logger,
                         self.profile_key,
                         self.renewables_ninja_params,
                         year,
                     )
                 except KeyError as e:  # pylint: disable=invalid-name
```

### Comparing `clover-energy-5.1.1/src/clover/generation/solar.py` & `clover-energy-5.1.2b1/src/clover/generation/solar.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 from ..__utils__ import (
     BColours,
     InputFileError,
     Location,
     NAME,
     ProgrammerJudgementFault,
+    RenewablesNinjaError,
 )
 from .__utils__ import BaseRenewablesNinjaThread, SolarDataType, total_profile_output
 
 __all__ = (
     "get_profile_prefix",
     "HybridPVTPanel",
     "PVPanel",
@@ -131,14 +132,30 @@
                 text,
                 ", ".join([f"'{key}'" for key in _TRACKING_MAP]),
             )
             raise InputFileError(
                 "solar_generation_inputs", f"Tracking mode '{text}' is not valid."
             ) from err
 
+    @property
+    def as_string(self) -> str:
+        """
+        Return a string representing the class.
+
+        :return:
+            A `str` containing the tracking information.
+
+        """
+
+        if self.value == 0:
+            return "fixed"
+        if self.value == 1:
+            return "single_axis"
+        return "dual_axis"
+
 
 class SolarPanel:  # pylint: disable=too-few-public-methods
     """
     Represents a solar panel being considered.
 
     .. attribute:: azimuthal_orientation
         The azimuthal orientation of the panel, defined in degrees from North.
@@ -345,14 +362,38 @@
 
         return (  # type: ignore[no-any-return]
             self.tracking == other.tracking
             and self.azimuthal_orientation == other.azimuthal_orientation
             and self.tilt == other.tilt
         )
 
+    @property
+    def as_dict(self) -> Dict[str, Any]:
+        """
+        Return a dictionary based on the panel information.
+
+        Outputs:
+            - A mapping containing the input information based on the panel.
+
+        """
+
+        return {
+            "azimuthal_orientation": self.azimuthal_orientation,
+            "lifetime": self.lifetime,
+            "name": self.name,
+            "pv_unit": self.pv_unit,
+            "pv_unit_overrided": self.pv_unit_overrided,
+            "reference_efficiency": self.reference_efficiency,
+            "reference_temperature": self.reference_temperature,
+            "thermal_coefficient": self.thermal_coefficient,
+            "tilt": self.tilt,
+            "tracking": self.tracking.as_string,
+            "type": self.panel_type.value,
+        }
+
     @classmethod
     def from_dict(cls, logger: Logger, solar_inputs: Dict[str, Any]) -> Any:
         """
         Instantiate a :class:`PVPanel` instance based on the input data.
 
         Inputs:
             - logger:
@@ -758,14 +799,15 @@
 
     """
 
     def __init__(
         self,
         auto_generated_files_directory: str,
         generation_inputs: Dict[str, Any],
+        global_settings_inputs: Dict[str, str],
         location: Location,
         logger_name: str,
         pause_time: int,
         regenerate: bool,
         pv_panel: PVPanel,
         sleep_multiplier: int = 1,
         verbose: bool = False,
@@ -798,14 +840,15 @@
 
         # Determine the prefix to use for the solar profiles dependent on tracking.
         profile_prefix = get_profile_prefix(pv_panel)
 
         super().__init__(
             auto_generated_files_directory,
             generation_inputs,
+            global_settings_inputs,
             location,
             logger_name,
             pause_time,
             regenerate,
             sleep_multiplier,
             verbose,
             renewables_ninja_params=renewables_ninja_params,
@@ -817,12 +860,15 @@
     *args, pv_panel: Union[PVPanel, HybridPVTPanel]
 ) -> pd.DataFrame:  # type: ignore
     """
     Wrapper function to wrap the total solar output.
 
     """
 
-    return total_profile_output(
-        *args,
-        profile_name="solar",
-        profile_prefix=get_profile_prefix(pv_panel),
-    )
+    try:
+        return total_profile_output(
+            *args,
+            profile_name="solar",
+            profile_prefix=get_profile_prefix(pv_panel),
+        )
+    except FileNotFoundError:
+        raise RenewablesNinjaError() from None
```

### Comparing `clover-energy-5.1.1/src/clover/generation/weather.py` & `clover-energy-5.1.2b1/src/clover/generation/weather.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 
     """
 
     def __init__(
         self,
         auto_generated_files_directory: str,
         generation_inputs: Dict[str, Any],
+        global_settings_inputs: Dict[str, str],
         location: Location,
         logger_name: str,
         pause_time: int,
         regenerate: bool,
         sleep_multiplier: int = 1,
         verbose: bool = False,
     ):
@@ -119,14 +120,15 @@
             "var_prectotland": "true",
             "var_swgdn": "true",
             "var_cldtot": "true",
         }
         super().__init__(
             auto_generated_files_directory,
             generation_inputs,
+            global_settings_inputs,
             location,
             logger_name,
             pause_time,
             regenerate,
             sleep_multiplier,
             verbose,
             renewables_ninja_params=renewables_ninja_params,
```

### Comparing `clover-energy-5.1.1/src/clover/generation/wind.py` & `clover-energy-5.1.2b1/src/clover/generation/wind.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
     """
 
     def __init__(
         self,
         auto_generated_files_directory: str,
         generation_inputs: Dict[str, Any],
+        global_settings_inputs: Dict[str, str],
         location: Location,
         logger_name: str,
         pause_time: int,
         regenerate: bool,
         sleep_multiplier: int = 1,
         verbose: bool = False,
     ):
@@ -76,14 +77,15 @@
             "height": 10,
             "turbine": "Vestas V80 2000",
             "raw": "true",
         }
         super().__init__(
             auto_generated_files_directory,
             generation_inputs,
+            global_settings_inputs,
             location,
             logger_name,
             pause_time,
             regenerate,
             sleep_multiplier,
             verbose,
             renewables_ninja_params=renewables_ninja_params,
```

### Comparing `clover-energy-5.1.1/src/clover/impact/__init__.py` & `clover-energy-5.1.2b1/src/clover/impact/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/impact/__utils__.py` & `clover-energy-5.1.2b1/src/clover/impact/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/impact/finance.py` & `clover-energy-5.1.2b1/src/clover/impact/finance.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 
 from logging import Logger
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np  # pylint: disable=import-error
 import pandas as pd  # pylint: disable=import-error
 
-from .__utils__ import ImpactingComponent, LIFETIME, SIZE_INCREMENT
+from .__utils__ import ImpactingComponent
 from ..__utils__ import (
     BColours,
     ColumnHeader,
     hourly_profile_to_daily_sum,
     InputFileError,
     InternalError,
+    Inverter,
     Location,
     Scenario,
 )
 
 __all_ = (
     "connections_expenditure",
     "COSTS",
@@ -251,28 +252,31 @@
     ]
 
     return pd.DataFrame(discounted_fraction_array)
 
 
 def _inverter_expenditure(  # pylint: disable=too-many-locals
     finance_inputs: Dict[str, Any],
+    inverter: Inverter,
     location: Location,
     logger: Logger,
     scenario: Scenario,
     yearly_load_statistics: pd.DataFrame,
     *,
     start_year: int,
     end_year: int,
 ) -> float:
     """
     Calculates cost of inverters based on load calculations
 
     Inputs:
         - finance_inputs:
             The finance-input information for the system.
+        - inverter:
+            The inverter being modelled.
         - location:
             The location being considered.
         - logger:
             The :class:`logging.Logger` to use for the run.
         - yearly_load_statistics:
             The yearly-load statistics for the system.
         - scenario:
@@ -284,44 +288,43 @@
 
     Outputs:
         Discounted cost
 
     """
 
     # Initialise inverter replacement periods
-    replacement_period = finance_inputs[ImpactingComponent.INVERTER.value][LIFETIME]
     replacement_intervals = pd.DataFrame(
-        np.arange(0, location.max_years, replacement_period)
+        np.arange(0, location.max_years, inverter.lifetime)
     )
     replacement_intervals.columns = pd.Index([ColumnHeader.INSTALLATION_YEAR.value])
 
     # Check if inverter should be replaced in the specified time interval
     if not any(
         replacement_intervals[ColumnHeader.INSTALLATION_YEAR.value].isin(
             list(np.array(range(start_year, end_year)))
         )
     ):
         inverter_discounted_cost = float(0.0)
         return inverter_discounted_cost
 
     # Initialise inverter sizing calculation
     max_power = []
-    inverter_step = finance_inputs[ImpactingComponent.INVERTER.value][SIZE_INCREMENT]
     inverter_size: List[float] = []
     for i in range(len(replacement_intervals)):
         # Calculate maximum power in interval years
         start = replacement_intervals[ColumnHeader.INSTALLATION_YEAR.value].iloc[i]
-        end = start + replacement_period
+        end = start + inverter.lifetime
         max_power_interval = (
             yearly_load_statistics[ColumnHeader.MAXIMUM.value].iloc[start:end].max()
         )
         max_power.append(max_power_interval)
         # Calculate resulting inverter size
         inverter_size_interval: float = (
-            np.ceil(0.001 * max_power_interval / inverter_step) * inverter_step
+            np.ceil(0.001 * max_power_interval / inverter.size_increment)
+            * inverter.size_increment
         )
         inverter_size.append(inverter_size_interval)
     inverter_size_data_frame: pd.DataFrame = pd.DataFrame(inverter_size)
     inverter_size_data_frame.columns = pd.Index([ColumnHeader.INVERTER_SIZE.value])
     inverter_info = pd.concat([replacement_intervals, inverter_size_data_frame], axis=1)
     # Calculate
     inverter_info[ColumnHeader.DISCOUNT_RATE.value] = [
@@ -1034,28 +1037,31 @@
         end_year=end_year,
     )
     return total_discounted_cost
 
 
 def independent_expenditure(
     finance_inputs: Dict[str, Any],
+    inverter: Inverter,
     location: Location,
     logger: Logger,
     scenario: Scenario,
     yearly_load_statistics: pd.DataFrame,
     *,
     start_year: int,
     end_year: int,
 ) -> float:
     """
     Calculates cost of equipment which is independent of simulation periods
 
     Inputs:
         - finance_inputs:
             The financial input information.
+        - inverter:
+            The inverter being modelled.
         - location:
             The location currently being considered.
         - logger:
             The :class:`logging.Logger` to use for the run.
         - yearly_load_statistics:
             The yearly load statistics information.
         - scenario:
@@ -1068,14 +1074,15 @@
     Outputs:
         Discounted cost
 
     """
 
     inverter_expenditure = _inverter_expenditure(
         finance_inputs,
+        inverter,
         location,
         logger,
         scenario,
         yearly_load_statistics,
         start_year=start_year,
         end_year=end_year,
     )
```

### Comparing `clover-energy-5.1.1/src/clover/impact/ghgs.py` & `clover-energy-5.1.2b1/src/clover/impact/ghgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,24 @@
 
 from logging import Logger
 from typing import Any, Dict, List, Optional
 
 import numpy as np  # pylint: disable=import-error
 import pandas as pd  # pylint: disable=import-error
 
+from .__utils__ import ImpactingComponent
 from ..__utils__ import (
     BColours,
     ColumnHeader,
     hourly_profile_to_daily_sum,
     InputFileError,
+    Inverter,
     Location,
     Scenario,
 )
-from .__utils__ import ImpactingComponent, LIFETIME, SIZE_INCREMENT
 
 __all__ = (
     "calculate_connections_ghgs",
     "calculate_diesel_fuel_ghgs",
     "calculate_grid_ghgs",
     "calculate_independent_ghgs",
     "calculate_kerosene_ghgs",
@@ -491,14 +492,15 @@
     ) + float(ghg_inputs[ImpactingComponent.GRID.value][INFRASTRUCTURE_GHGS])
 
 
 def _calculate_inverter_ghgs(  # pylint: disable=too-many-locals
     electric_yearly_load_statistics: pd.DataFrame,
     end_year: int,
     ghg_inputs: Dict[str, Any],
+    inverter: Inverter,
     location: Location,
     logger: Logger,
     scenario: Scenario,
     start_year: int,
 ) -> float:
     """
     Calculates ghgs of inverters based on load calculations
@@ -506,14 +508,16 @@
     Inputs:
         - electric_yearly_load_statistics:
             The yearly load statistics for the electric load.
         - end_year:
             End year of simulation period
         - ghg_inputs:
             GHG input information.
+        - inverter:
+            The :class:`Inverter` to use for the run.
         - location:
             The location being considered.
         - logger:
             The :class:`logging.Logger` to use for the run.
         - scenario:
             The :class:`Scenario` currently being considered.
         - start_year:
@@ -521,46 +525,45 @@
 
     Outputs:
         GHGs
 
     """
 
     # Calcualte inverter replacement periods
-    replacement_period = int(ghg_inputs[ImpactingComponent.INVERTER.value][LIFETIME])
     replacement_intervals = pd.DataFrame(
-        np.arange(0, location.max_years, replacement_period)
+        np.arange(0, location.max_years, inverter.lifetime)
     )
     replacement_intervals.columns = pd.Index([ColumnHeader.INSTALLATION_YEAR.value])
 
     # Check if inverter should be replaced in the specified time interval
     if not any(
         replacement_intervals[ColumnHeader.INSTALLATION_YEAR.value].isin(
             list(np.array(range(start_year, end_year)))
         )
     ):
         return float(0.0)
 
     # Initialise inverter sizing calculation
     max_power = []
-    inverter_step = float(ghg_inputs[ImpactingComponent.INVERTER.value][SIZE_INCREMENT])
     inverter_size: List[float] = []
     for i in range(len(replacement_intervals)):
         # Calculate maximum power in interval years
         start = replacement_intervals[ColumnHeader.INSTALLATION_YEAR.value].iloc[i]
-        end = start + replacement_period
+        end = start + inverter.lifetime
         max_power_interval = (
             electric_yearly_load_statistics[ColumnHeader.MAXIMUM.value]
             .iloc[start:end]
             .max()
         )
         max_power.append(max_power_interval)
 
         # Calculate resulting inverter size
         inverter_size_interval: float = (
-            np.ceil(0.001 * max_power_interval / inverter_step) * inverter_step
+            np.ceil(0.001 * max_power_interval / inverter.size_increment)
+            * inverter.size_increment
         )
         inverter_size.append(inverter_size_interval)
 
     inverter_size_data_frame: pd.DataFrame = pd.DataFrame(inverter_size)
     inverter_size_data_frame.columns = pd.Index([ColumnHeader.INVERTER_SIZE.value])
     inverter_info = pd.concat([replacement_intervals, inverter_size_data_frame], axis=1)
 
@@ -614,14 +617,15 @@
     return inverter_ghgs
 
 
 def calculate_independent_ghgs(
     electric_yearly_load_statistics: pd.DataFrame,
     end_year: int,
     ghg_inputs: Dict[str, Any],
+    inverter: Inverter,
     location: Location,
     logger: Logger,
     scenario: Scenario,
     start_year: int,
 ) -> float:
     """
     Calculates ghgs of equipment which is independent of simulation periods
@@ -629,14 +633,16 @@
     Inputs:
         - electric_yearly_load_statistics:
             The electric yearly load statistics for the simulation period.
         - end_year:
             End year of simulation period
         - ghg_inputs:
             The GHG input informaiton.
+        - inverter:
+            The :class:`Inverter` to use for the run.
         - location:
             The location being considered.
         - logger:
             The :class:`logging.Logger` to use for the run.
         - scenario:
             The :class:`Scenario` currently being considered.
         - start_year:
@@ -647,14 +653,15 @@
 
     """
 
     inverter_ghgs = _calculate_inverter_ghgs(
         electric_yearly_load_statistics,
         end_year,
         ghg_inputs,
+        inverter,
         location,
         logger,
         scenario,
         start_year,
     )
     total_ghgs = inverter_ghgs  # ... + other components as required
```

### Comparing `clover-energy-5.1.1/src/clover/load/__init__.py` & `clover-energy-5.1.2b1/src/clover/load/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/load/load.py` & `clover-energy-5.1.2b1/src/clover/load/load.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/mains_supply/__init__.py` & `clover-energy-5.1.2b1/src/clover/mains_supply/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/mains_supply/__utils__.py` & `clover-energy-5.1.2b1/src/clover/mains_supply/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/mains_supply/grid.py` & `clover-energy-5.1.2b1/src/clover/mains_supply/grid.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/mains_supply/water_source.py` & `clover-energy-5.1.2b1/src/clover/mains_supply/water_source.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/optimisation/__init__.py` & `clover-energy-5.1.2b1/src/clover/optimisation/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/optimisation/__utils__.py` & `clover-energy-5.1.2b1/src/clover/optimisation/__utils__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1066,14 +1066,15 @@
         )
 
         new_appraisal = appraise_system(
             yearly_electric_load_statistics,
             end_year,
             finance_inputs,
             ghg_inputs,
+            minigrid.inverter,
             location,
             logger,
             previous_system,
             optimisation.scenario,
             simulation_results,
             start_year,
             system_details,
```

### Comparing `clover-energy-5.1.1/src/clover/optimisation/appraisal.py` & `clover-energy-5.1.2b1/src/clover/optimisation/appraisal.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     BColours,
     ColumnHeader,
     Criterion,
     CumulativeResults,
     EnvironmentalAppraisal,
     FinancialAppraisal,
     InternalError,
+    Inverter,
     hourly_profile_to_daily_sum,
     Location,
     Scenario,
     SystemAppraisal,
     SystemDetails,
     TechnicalAppraisal,
 )
@@ -53,14 +54,15 @@
     converter_addition: Dict[str, int],
     diesel_addition: float,
     electric_yearly_load_statistics: pd.DataFrame,
     end_year: int,
     ghg_inputs: Dict[str, Any],
     heat_exchanger_addition: int,
     hot_water_tank_addition: int,
+    inverter: Inverter,
     location: Location,
     logger: Logger,
     pv_addition: Dict[str, float],
     pvt_addition: float,
     scenario: Scenario,
     simulation_results: pd.DataFrame,
     start_year: int,
@@ -86,14 +88,16 @@
             The end year of the simulation period.
         - ghg_inputs:
             The GHG input information.
         - heat_exchanger_addition:
             The additional number of heat exchangers added this iteration.
         - hot_water_tank_addition:
             The additional number of hot-water tanks added this iteration.
+        - inverter:
+            The :class:`Inverter` being used for the run.
         - location:
             The location being considered.
         - logger:
             The logger to use for the run.
         - pv_addition:
             The additional number of PV panels added this iteration.
         - pvt_addition:
@@ -129,14 +133,15 @@
             pv_addition,
             pvt_addition,
             storage_addition,
         ) + ghgs.calculate_independent_ghgs(
             electric_yearly_load_statistics,
             end_year,
             ghg_inputs,
+            inverter,
             location,
             logger,
             scenario,
             start_year,
         )
     except KeyError as e:
         logger.error("Missing system equipment GHG input information: %s", str(e))
@@ -251,14 +256,15 @@
     buffer_tank_addition: int,
     clean_water_tank_addition: int,
     converter_addition: Dict[str, int],
     diesel_addition: float,
     finance_inputs: Dict[str, Any],
     heat_exchanger_addition: int,
     hot_water_tank_addition: int,
+    inverter: Inverter,
     location: Location,
     logger: Logger,
     pv_addition: Dict[str, float],
     pvt_addition: float,
     scenario: Scenario,
     simulation_results: pd.DataFrame,
     storage_addition: float,
@@ -280,14 +286,16 @@
             The additional diesel capacity added this iteration.
         - finance_inputs:
             The finance input information.
         - heat_exchanger_addition:
             The additional number of heat exchangers added this iteration.
         - hot_water_tank_addition:
             The additional number of hot-water tanks added this iteration.
+        - inverter:
+            The inverter being modelled.
         - location:
             The :class:`Location` being considered.
         - logger:
             The logger to use for the run.
         - pv_addition:
             The additional number of PV panels added this iteration.
         - pvt_addition:
@@ -321,14 +329,15 @@
         logger,
         pv_addition,
         pvt_addition,
         storage_addition,
         system_details.start_year,
     ) + finance.independent_expenditure(
         finance_inputs,
+        inverter,
         location,
         logger,
         scenario,
         yearly_load_statistics,
         start_year=system_details.start_year,
         end_year=system_details.end_year,
     )
@@ -571,14 +580,15 @@
 
 
 def appraise_system(  # pylint: disable=too-many-locals
     electric_yearly_load_statistics: pd.DataFrame,
     end_year: int,
     finance_inputs: Dict[str, Any],
     ghg_inputs: Dict[str, Any],
+    inverter: Inverter,
     location: Location,
     logger: Logger,
     previous_system: Optional[SystemAppraisal],
     scenario: Scenario,
     simulation_results: pd.DataFrame,
     start_year: int,
     system_details: SystemDetails,
@@ -589,14 +599,18 @@
     Inputs:
         - electric_yearly_load_statistics:
             The yearly electric load statistics.
         - end_year:
             The end year for the simulation that was just run.
         - finance_inputs:
             The finance input information.
+        - ghg_inputs:
+            The GHG input information.
+        - inverter:
+            The :class:`Inverter` being modelled.
         - location:
             The location currently being considered.
         - logger:
             The logger to use for the run.
         - previous_system:
             Report from previously installed system (not required if no system was
             previously deployed)
@@ -699,14 +713,15 @@
         buffer_tank_addition,
         clean_water_tank_addition,
         converter_addition,
         diesel_addition,
         finance_inputs,
         heat_exchanger_addition,
         hot_water_tank_addition,
+        inverter,
         location,
         logger,
         pv_addition,
         pvt_addition,
         scenario,
         simulation_results,
         storage_addition,
@@ -719,14 +734,15 @@
         converter_addition,
         diesel_addition,
         electric_yearly_load_statistics,
         end_year,
         ghg_inputs,
         heat_exchanger_addition,
         hot_water_tank_addition,
+        inverter,
         location,
         logger,
         pv_addition,
         pvt_addition,
         scenario,
         simulation_results,
         start_year,
```

### Comparing `clover-energy-5.1.1/src/clover/optimisation/optimisation.py` & `clover-energy-5.1.2b1/src/clover/optimisation/optimisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,14 +504,15 @@
     )
 
     largest_system_appraisal: SystemAppraisal = appraise_system(
         yearly_electric_load_statistics,
         end_year,
         finance_inputs,
         ghg_inputs,
+        minigrid.inverter,
         location,
         logger,
         previous_system,
         optimisation.scenario,
         simulation_results,
         start_year,
         system_details,
@@ -610,14 +611,15 @@
         )
 
         largest_system_appraisal = appraise_system(
             yearly_electric_load_statistics,
             end_year,
             finance_inputs,
             ghg_inputs,
+            minigrid.inverter,
             location,
             logger,
             previous_system,
             optimisation.scenario,
             simulation_results,
             start_year,
             system_details,
```

### Comparing `clover-energy-5.1.1/src/clover/optimisation/single_line_simulation.py` & `clover-energy-5.1.2b1/src/clover/optimisation/single_line_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,14 +377,15 @@
 
             # Appraise the system.
             new_appraisal = appraise_system(
                 yearly_electric_load_statistics,
                 end_year,
                 finance_inputs,
                 ghg_inputs,
+                minigrid.inverter,
                 location,
                 logger,
                 previous_system,
                 optimisation.scenario,
                 simulation_results,
                 start_year,
                 system_details,
```

### Comparing `clover-energy-5.1.1/src/clover/printer.py` & `clover-energy-5.1.2b1/src/clover/printer.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/clover.py` & `clover-energy-5.1.2b1/src/clover/scripts/clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/clover_hpc_clover.py` & `clover-energy-5.1.2b1/src/clover/scripts/clover_hpc_clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/clover_hpc_outbox_assembly.py` & `clover-energy-5.1.2b1/src/clover/scripts/clover_hpc_outbox_assembly.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/clover_new_location.py` & `clover-energy-5.1.2b1/src/clover/scripts/clover_new_location.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/clover_update_api_token.py` & `clover-energy-5.1.2b1/src/clover/scripts/clover_update_api_token.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/hpc.py` & `clover-energy-5.1.2b1/src/clover/scripts/hpc.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/hpc_clover.py` & `clover-energy-5.1.2b1/src/clover/scripts/hpc_clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/hpc_outbox_assembly.py` & `clover-energy-5.1.2b1/src/clover/scripts/hpc_outbox_assembly.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/hpc_utils.py` & `clover-energy-5.1.2b1/src/clover/scripts/hpc_utils.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/new_location.py` & `clover-energy-5.1.2b1/src/clover/scripts/new_location.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/scripts/update_api_token.py` & `clover-energy-5.1.2b1/src/clover/scripts/update_api_token.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 import os
 import sys
 
 from typing import Any, Dict, List
 
 import yaml  # pylint: disable=import-error
 
-from ..__utils__ import get_logger, read_yaml
-from ..fileparser import GENERATION_INPUTS_FILE, INPUTS_DIRECTORY, LOCATIONS_FOLDER_NAME
-from ..generation.__utils__ import TOKEN
+from ..__utils__ import get_logger, read_yaml, TOKEN
+from ..fileparser import GLOBAL_SETTINGS_FILE
 
 __all__ = ("main",)
 
 # Logger name:
 #   The name to use for the logger.
 LOGGER_NAME: str = "update_api_token"
 
@@ -75,38 +74,35 @@
     # Error if not all arguments passed in.
     if parsed_args.location is None:
         raise Exception("A location to update must be specified.")
     if parsed_args.token is None:
         raise Exception("The renewables.ninja API token must be specifeid.")
 
     # Check whether the generation file exists.
-    generation_file_path = os.path.join(
-        LOCATIONS_FOLDER_NAME,
-        parsed_args.location,
-        INPUTS_DIRECTORY,
-        GENERATION_INPUTS_FILE,
-    )
+    global_settings_file_path = GLOBAL_SETTINGS_FILE
 
-    if not os.path.isfile(generation_file_path):
+    if not os.path.isfile(global_settings_file_path):
         raise FileNotFoundError(
             "The generation inputs file could not be found within the location "
             f"{parsed_args.location}.",
         )
 
     # Attempt to update the token.
     filedata: Dict[str, Any]
     try:
-        filedata = read_yaml(generation_file_path, logger)  # type: ignore
+        filedata = read_yaml(global_settings_file_path, logger)  # type: ignore
     except Exception:
-        logger.error("Error reading generation inputs file '%s'.", generation_file_path)
+        logger.error(
+            "Error reading generation inputs file '%s'.", global_settings_file_path
+        )
         raise
 
     filedata[TOKEN] = parsed_args.token
 
     logger.info("Attempting to save updated token to the generation inputs file.")
-    with open(generation_file_path, "w") as f:
+    with open(global_settings_file_path, "w") as f:
         yaml.dump(filedata, f)
     logger.info("Updated API token successfully saved.")
 
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `clover-energy-5.1.1/src/clover/simulation/__init__.py` & `clover-energy-5.1.2b1/src/clover/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/simulation/__utils__.py` & `clover-energy-5.1.2b1/src/clover/simulation/__utils__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,32 +22,34 @@
 
 """
 
 from argparse import Namespace
 import dataclasses
 from logging import Logger
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, DefaultDict, Dict, List, Optional, Union
 
 from ..__utils__ import (
     AuxiliaryHeaterType,
     BColours,
     CleanWaterMode,
     EXCHANGER,
     InputFileError,
+    Inverter,
     NAME,
     RESOURCE_NAME_TO_RESOURCE_TYPE_MAPPING,
     OperatingMode,
     ProgrammerJudgementFault,
     ResourceType,
     Scenario,
 )
 
 from ..conversion.conversion import Converter
 from ..generation.solar import HybridPVTPanel, PVPanel
+from ..impact.__utils__ import ImpactingComponent, LIFETIME, SIZE_INCREMENT
 from .diesel import DieselGenerator, DieselWaterHeater
 from .exchanger import Exchanger
 from .storage_utils import Battery, CleanWaterTank, HotWaterTank
 from .transmission import Transmitter
 
 __all__ = (
     "check_scenario",
@@ -125,14 +127,17 @@
 
     .. attribute:: heat_exchanger
         The heat exchanger associated with the minigrid system.
 
     .. attribute:: hot_water_tank
         The hot-water tank being modelled, if applicable.
 
+    .. attribute:: inverter
+        The inverter being modelled.
+
     .. attribute:: pv_panels
         The PV panel(s) being considered.
 
     .. attribute:: pvt_panels
         The PV-T panel(s) being considered, if applicable.
 
     .. attribute:: water_pump
@@ -151,24 +156,27 @@
     dc_to_dc_conversion_efficiency: Optional[float]
     dc_transmission_efficiency: Optional[float]
     diesel_generator: Optional[DieselGenerator]
     diesel_water_heater: Optional[DieselWaterHeater]
     electric_water_heater: Optional[Converter]
     heat_exchanger: Optional[Exchanger]
     hot_water_tank: Optional[HotWaterTank]
+    inverter: Inverter
     pv_panels: List[PVPanel]
     pvt_panels: List[HybridPVTPanel]
     water_pump: Optional[Transmitter]
 
     @classmethod
     def from_dict(  # pylint: disable=too-many-locals
         cls,
         diesel_generator: DieselGenerator,
         diesel_water_heater: Optional[DieselWaterHeater],
         electric_water_heater: Optional[Converter],
+        finance_inputs: DefaultDict[str, DefaultDict[str, float]],
+        logger: Logger,
         minigrid_inputs: Dict[str, Any],
         pv_panels: List[PVPanel],
         pvt_panels: List[HybridPVTPanel],
         battery_inputs: Optional[List[Dict[str, Any]]] = None,
         exchanger_inputs: Optional[List[Dict[str, Any]]] = None,
         tank_inputs: Optional[List[Dict[str, Any]]] = None,
         water_pump: Optional[Transmitter] = None,
@@ -181,14 +189,16 @@
                 The diesel backup generator to use for the run.
             - diesel_water_heater:
                 The diesel water heater associated with the minigrid system, if
                 appropriate.
             - electric_water_heater:
                 The electric water heater associated with the minigrid system, if
                 appropriate.
+            - finance_inputs:
+                The financial input information.
             - minigrid_inputs:
                 The inputs for the minigrid/energy system, extracted from the input
                 file.
             - pv_panels:
                 The `list` of :class:`PVPanel` instances to use for the run.
             - pvt_panels:
                 The `list` of :class:`HybridPVTPanel` instances to use for the run,
@@ -292,14 +302,36 @@
                 raise InputFileError(
                     "energy system inputs",
                     "The hot-water tank selected must be a hot-water tank.",
                 )
         else:
             hot_water_tank = None
 
+        # Attempt to fetch inverter information from the energy-system inputs.
+        try:
+            inverter = Inverter(
+                minigrid_inputs[ImpactingComponent.INVERTER.value][LIFETIME],
+                minigrid_inputs[ImpactingComponent.INVERTER.value][SIZE_INCREMENT],
+            )
+        except KeyError:
+            try:
+                inverter = Inverter(
+                    int(finance_inputs[ImpactingComponent.INVERTER.value][LIFETIME]),
+                    finance_inputs[ImpactingComponent.INVERTER.value][SIZE_INCREMENT],
+                )
+            except KeyError:
+                raise InputFileError(
+                    "energy system inputs",
+                    "Inverter information should be in energy system inputs.",
+                )
+            logger.warning(
+                "Specifying inverter information in the finance inputs is deprecated. "
+                "Use the energy-system inputs."
+            )
+
         # Return the minigrid instance.
         return cls(
             minigrid_inputs[CONVERSION][AC_TO_AC]
             if AC_TO_AC in minigrid_inputs[CONVERSION]
             else None,
             minigrid_inputs[CONVERSION][AC_TO_DC]
             if AC_TO_DC in minigrid_inputs[CONVERSION]
@@ -324,14 +356,15 @@
             diesel_generator,
             diesel_water_heater,
             electric_water_heater,
             exchangers[minigrid_inputs[EXCHANGER]]
             if EXCHANGER in minigrid_inputs
             else None,
             hot_water_tank,
+            inverter,
             pv_panels,
             pvt_panels,
             water_pump,
         )
 
     @property
     def pv_panel(self) -> PVPanel:
```

### Comparing `clover-energy-5.1.1/src/clover/simulation/diesel.py` & `clover-energy-5.1.2b1/src/clover/simulation/diesel.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/simulation/energy_system.py` & `clover-energy-5.1.2b1/src/clover/simulation/energy_system.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/simulation/exchanger.py` & `clover-energy-5.1.2b1/src/clover/simulation/exchanger.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/simulation/solar.py` & `clover-energy-5.1.2b1/src/clover/simulation/solar.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/simulation/storage.py` & `clover-energy-5.1.2b1/src/clover/simulation/storage.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/simulation/storage_utils.py` & `clover-energy-5.1.2b1/src/clover/simulation/storage_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -302,14 +302,39 @@
         return (
             "Battery("
             + f"{self.label} storing {self.resource_type.value} loads, "
             + f"name={self.name}, capacity={self.capacity}"
             + ")"
         )
 
+    @property
+    def as_dict(self) -> Dict[str, Any]:
+        """
+        Return a dictionary based on the battery information.
+
+        Outputs:
+            - A mapping containing the input information based on the battery.
+
+        """
+
+        return {
+            "capacity": self.capacity,
+            "cycle_lifetime": self.cycle_lifetime,
+            "leakage": self.leakage,
+            "maximum_charge": self.maximum_charge,
+            "minimum_charge": self.minimum_charge,
+            NAME: self.name,
+            "c_rate_charging": self.charge_rate,
+            "c_rate_discharging": self.discharge_rate,
+            "conversion_in": self.conversion_in,
+            "conversion_out": self.conversion_out,
+            "lifetime_loss": self.lifetime_loss,
+            "storage_unit": self.storage_unit,
+        }
+
     @classmethod
     def from_dict(cls, storage_data: Dict[str, Any]) -> Any:
         """
         Create a :class:`Battery` instance based on the file data passed in.
 
         Inputs:
             - storage_data:
```

### Comparing `clover-energy-5.1.1/src/clover/simulation/transmission.py` & `clover-energy-5.1.2b1/src/clover/simulation/transmission.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.1.1/src/clover/src/new_location.yaml` & `clover-energy-5.1.2b1/src/clover/src/new_location.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -160,22 +160,16 @@
                 #                                                                              #
                 # Author: Phil Sandwell, Ben Winchester                                        #
                 # Copyright: Phil Sandwell & Ben Winchester, 2021                              #
                 # Date created: 14/07/2021                                                     #
                 # License: Open source                                                         #
                 ################################################################################
 
-                # NOTE: The renewables.ninja API token must be entered under the `token` field.
-                # For more information, consult the User Guide, available within the repository
-                # and online.
-                #
-
                 end_year: 2016 # The absolute end year for gathering solar data.
                 start_year: 2007 # The absolute start year for gathering solar data.
-                token: "YOUR API TOKEN HERE" # renewables.ninja API token
             - file: "grid_times.csv"
               contents: |-
                 Name,none,all,example,eight_hours,default
                 0,0,1,0,0.33,0.57
                 1,0,1,0,0.33,0.61
                 2,0,1,0,0.33,0.54
                 3,0,1,0,0.33,0.5
@@ -289,16 +283,14 @@
                   extension cost: 5000 # [$/km]
                   infrastructure_cost: 2000 # [$]
                 households:
                   connection_cost: 100 # [$/household]
                 inverter:
                   cost: 200 # [$/kW]
                   cost_decrease: 2 # [% p.a.]
-                  lifetime: 4 # [years]
-                  size_increment: 1 # [kW]
                 kerosene:
                   cost: 0.008 # [$/hour]
             - file: ghg_inputs.yaml
               contents: |+
                 ---
                 ################################################################################
                 # ghg_inputs.yaml - GHG input information.                                     #
@@ -328,16 +320,14 @@
                   initial_ghgs: 0.8 # [kgCO2/kWh]
                   final_ghgs: 0.4 # [kgCO2/kWh]
                 households:
                   connection_ghgs: 10 # [kgCO2/household]
                 inverter:
                   ghgs: 75 # [kgCO2/kW]
                   ghg_decrease: 2 # [2,% p.a.]
-                  lifetime: 4 # [years]
-                  size_increment: 1 # [kW]
                 kerosene:
                   ghgs: 0.055 # [kgCO2/hour]
         - directory: load
           contents:
             - file: devices.yaml
               contents: |+
                 ---
@@ -879,14 +869,17 @@
                 battery: default_battery
                 conversion:
                   dc_to_ac: 0.95 # Conversion efficiency (0.0-1.0)
                   dc_to_dc: 0.95 # Conversion efficiency (0.0-1.0)
                   ac_to_dc: 0.8 # Conversion efficiency (0.0-1.0)
                   ac_to_ac: 0.98 # Conversion efficiency (0.0-1.0)
                 diesel_generator: default_diesel
+                inverter:
+                  lifetime: 4 # [years]
+                  size_increment: 1 # [kW]
                 pv_panel: default_pv
             # - file: "energy_system.yaml"
             #   contents: |+
             #     ---
             #     ################################################################################
             #     # energy_system.yaml - Parameters for specifying a CLOVER energy system.       #
             #     #                                                                              #
```

### Comparing `clover-energy-5.1.1/src/clover_energy.egg-info/PKG-INFO` & `clover-energy-5.1.2b1/src/clover_energy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clover-energy
-Version: 5.1.1
+Version: 5.1.2b1
 Summary: Continuous Lifetime Optimisation of Variable Electricity Resources
 Home-page: https://github.com/CLOVER-energy/CLOVER
 Author: Phil Sandwell, Ben Winchester and Hamish Beath
 Author-email: philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 Project-URL: Bug Tracker, https://github.com/CLOVER-energy/CLOVER/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `clover-energy-5.1.1/src/clover_energy.egg-info/SOURCES.txt` & `clover-energy-5.1.2b1/src/clover_energy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

