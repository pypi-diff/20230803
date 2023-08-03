# Comparing `tmp/oilanalytics-0.3.2.tar.gz` & `tmp/oilanalytics-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oilanalytics-0.3.2.tar", last modified: Fri Jul  7 14:37:59 2023, max compression
+gzip compressed data, was "oilanalytics-0.3.3.tar", last modified: Thu Aug  3 08:26:58 2023, max compression
```

## Comparing `oilanalytics-0.3.2.tar` & `oilanalytics-0.3.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.861636 oilanalytics-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-07 14:37:59.857636 oilanalytics-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.849636 oilanalytics-0.3.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/notebooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.849636 oilanalytics-0.3.2/oilanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.853636 oilanalytics-0.3.2/oilanalytics/balances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/balances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/balances/balance_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/balances/balance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/balances/global_oil_balances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/balances/key_agency_comparisons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.853636 oilanalytics-0.3.2/oilanalytics/eia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/eia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/eia/eia.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/eia/monthly_drilling_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/eia/steo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/eia/weeklypetreport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.853636 oilanalytics-0.3.2/oilanalytics/energyaspects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/energyaspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/energyaspects/china_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/energyaspects/europe_diesel_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/energyaspects/fsu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/energyaspects/tars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.853636 oilanalytics-0.3.2/oilanalytics/euroilstock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/euroilstock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/euroilstock/euroilstock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.853636 oilanalytics-0.3.2/oilanalytics/geo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.853636 oilanalytics-0.3.2/oilanalytics/highfreq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/highfreq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/highfreq/ara.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/highfreq/singapore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.853636 oilanalytics-0.3.2/oilanalytics/iea/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/iea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/iea/omr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.853636 oilanalytics-0.3.2/oilanalytics/jodi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/jodi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/jodi/jodiapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.853636 oilanalytics-0.3.2/oilanalytics/opec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/opec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/opec/momr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.853636 oilanalytics-0.3.2/oilanalytics/prices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/prices/futures_prices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.857636 oilanalytics-0.3.2/oilanalytics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/utils/chartutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/utils/eikonutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/oilanalytics/utils/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.849636 oilanalytics-0.3.2/oilanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-07 14:37:59.000000 oilanalytics-0.3.2/oilanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-07 14:37:59.000000 oilanalytics-0.3.2/oilanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:37:59.000000 oilanalytics-0.3.2/oilanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 14:37:59.000000 oilanalytics-0.3.2/oilanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 14:37:59.000000 oilanalytics-0.3.2/oilanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:37:59.861636 oilanalytics-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:59.857636 oilanalytics-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/test/test_ea_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/test/test_eia.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/test/test_eia_weekly_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/test/test_futures_prices.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/test/test_highfreq.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/test/test_iea.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/test/test_key_agency_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-07 14:37:45.000000 oilanalytics-0.3.2/test/test_opec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.840361 oilanalytics-0.3.3/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/notebooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.840361 oilanalytics-0.3.3/oilanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.840361 oilanalytics-0.3.3/oilanalytics/balances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/balances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/balances/balance_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/balances/balance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/balances/global_oil_balances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/balances/key_agency_comparisons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.840361 oilanalytics-0.3.3/oilanalytics/eia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/eia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/eia/eia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/eia/monthly_drilling_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/eia/steo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/eia/weeklypetreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.840361 oilanalytics-0.3.3/oilanalytics/energyaspects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/energyaspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/energyaspects/china_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/energyaspects/europe_diesel_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/energyaspects/fsu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/energyaspects/tars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.840361 oilanalytics-0.3.3/oilanalytics/euroilstock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/euroilstock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/euroilstock/euroilstock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/oilanalytics/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/oilanalytics/highfreq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/highfreq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/highfreq/ara.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/highfreq/singapore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/oilanalytics/iea/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/iea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/iea/omr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/oilanalytics/jodi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/jodi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/jodi/jodiapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/oilanalytics/opec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/opec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/opec/momr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/oilanalytics/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/prices/futures_prices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/oilanalytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/utils/chartutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/utils/eikonutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/oilanalytics/utils/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.840361 oilanalytics-0.3.3/oilanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-03 08:26:58.000000 oilanalytics-0.3.3/oilanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-03 08:26:58.000000 oilanalytics-0.3.3/oilanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 08:26:58.000000 oilanalytics-0.3.3/oilanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-03 08:26:58.000000 oilanalytics-0.3.3/oilanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 08:26:58.000000 oilanalytics-0.3.3/oilanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:58.844361 oilanalytics-0.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/test/test_ea_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/test/test_eia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/test/test_eia_weekly_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/test/test_futures_prices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/test/test_highfreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/test/test_iea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/test/test_key_agency_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-03 08:26:46.000000 oilanalytics-0.3.3/test/test_opec.py
```

### Comparing `oilanalytics-0.3.2/oilanalytics/balances/balance_utils.py` & `oilanalytics-0.3.3/oilanalytics/balances/balance_utils.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/balances/global_oil_balances.py` & `oilanalytics-0.3.3/oilanalytics/balances/global_oil_balances.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/balances/key_agency_comparisons.py` & `oilanalytics-0.3.3/oilanalytics/balances/key_agency_comparisons.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/eia/eia.py` & `oilanalytics-0.3.3/oilanalytics/eia/eia.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import typing as t
 from deprecated import deprecated
 from functools import reduce
 
 
-
 import pandas as pd
 from dotenv import load_dotenv
 from eiapy import Category, MultiSeries
 
 # Load environmental variables from '.env' file.
 load_dotenv()
 
+
 @deprecated(reason="EIAPY doesn't support V2 API.")
 def extract_dataframe(data: list, series_id: str, freq: str = "M") -> pd.DataFrame:
     df = pd.DataFrame(data, columns=["date", series_id]).set_index("date")
     f = None
     if freq == "M":
         f = "%Y%m"
     df.index = pd.to_datetime(df.index, format=f)
```

### Comparing `oilanalytics-0.3.2/oilanalytics/eia/monthly_drilling_report.py` & `oilanalytics-0.3.3/oilanalytics/eia/monthly_drilling_report.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,119 +25,143 @@
     "Bakken Region",
     "Eagle Ford Region",
     "Haynesville Region",
     "Niobrara Region",
     "Permian Region",
 ]
 
-def read_release_date():
 
+def read_release_date():
     r = urllib2.urlopen(eia_webpage).read()
     x = []
-    soup = BeautifulSoup(r, 'html.parser')
-    result = soup.find_all('span', {'class': 'date'})[0].text.strip()
+    soup = BeautifulSoup(r, "html.parser")
+    result = soup.find_all("span", {"class": "date"})[0].text.strip()
     if result:
         release_date = datetime.strptime(result, "%B %d, %Y")
     return release_date
 
 
-
 def create_dualaxis_graph(df, title=None):
     # ensure that the DF is of format index / secondary axis col / primary axis col
     tf_list = [True, False]
     fig = make_subplots(specs=[[{"secondary_y": True}]])
     for col, tf in zip(df.columns, tf_list):
         if tf is False:
             fig.add_trace(go.Bar(x=df.index, y=df[col], name=col), secondary_y=tf)
         else:
             fig.add_trace(go.Scatter(x=df.index, y=df[col], name=col), secondary_y=tf)
         fig.update_yaxes(title_text=col, secondary_y=tf, showgrid=not tf)
     fig.update_layout(title=title)
     return fig
 
 
-
 def read_rig_report(name):
     filename = fileloc % name
     ex = excel_scraper.read_excel_file(filename)
     tot_prod_list = []
     graphs = []
     for tab in sheets_to_graph:
         d = ex.parse(tab, index_col=0).iloc[:, :4]
         # reorganise the DF (as parameters don't work in parse)
         new_header = d.iloc[0]
         d = d.iloc[1:]
         d.columns = new_header
         title = d.index.name
         d.index.name = None
         tot_prod_list.append(d["Total production"].rename(title))
-        fig = create_dualaxis_graph(d[['Production per rig', 'Rig count']], title=f"{title} Rig Count")
+        fig = create_dualaxis_graph(
+            d[["Production per rig", "Rig count"]], title=f"{title} Rig Count"
+        )
         graphs.append(fig)
-        d['MoM'] = d['Total production'] - d['Total production'].shift(1)
-        fig_mom = create_dualaxis_graph(d[['Total production', 'MoM']], title=f"{title} Production")
+        d["MoM"] = d["Total production"] - d["Total production"].shift(1)
+        fig_mom = create_dualaxis_graph(
+            d[["Total production", "MoM"]], title=f"{title} Production"
+        )
         graphs.append(fig_mom)
     total_prod = pd.concat(tot_prod_list, axis=1)
-    fig = cpl.seas_line_plot(total_prod.sum(axis=1).astype(float),
-                             title="Total Shale Production - 3 Main Plays",
-                             precision_format='{0:,.0f}')
+    fig = cpl.seas_line_plot(
+        total_prod.sum(axis=1).astype(float),
+        title="Total Shale Production - 3 Main Plays",
+        precision_format="{0:,.0f}",
+    )
     graphs.append(fig)
-    total_prod["YoY Changes"] = total_prod.sum(axis=1) - total_prod.sum(axis=1).shift(12)
-    total_prod["YoY Average Changes"] = total_prod["YoY Changes"].rolling(window=12).mean()
-    fig = cpl.bar_line_plot(total_prod[["YoY Changes", "YoY Average Changes"]],
-                            linecol="YoY Average Changes",
-                            title="US Shale Production")
+    total_prod["YoY Changes"] = total_prod.sum(axis=1) - total_prod.sum(axis=1).shift(
+        12
+    )
+    total_prod["YoY Average Changes"] = (
+        total_prod["YoY Changes"].rolling(window=12).mean()
+    )
+    fig = cpl.bar_line_plot(
+        total_prod[["YoY Changes", "YoY Average Changes"]],
+        linecol="YoY Average Changes",
+        title="US Shale Production",
+    )
     graphs.append(fig)
     return graphs
 
 
 def read_duc_report(name):
     filename = fileloc % name
     ex = excel_scraper.read_excel_file(filename)
-    d = ex.parse('Data', index_col=0)
-    header = pd.MultiIndex.from_product([[x.strip() for x in list(d.iloc[1]) if str(x) != 'nan'],
-                                         list(dict.fromkeys([x.strip() for x in list(d.iloc[2]) if str(x) != 'nan']))],
-                                        names=['loc', 'drill_type'])
-    d.dropna(axis=1, how='all', inplace=True)
+    d = ex.parse("Data", index_col=0)
+    header = pd.MultiIndex.from_product(
+        [
+            [x.strip() for x in list(d.iloc[1]) if str(x) != "nan"],
+            list(
+                dict.fromkeys([x.strip() for x in list(d.iloc[2]) if str(x) != "nan"])
+            ),
+        ],
+        names=["loc", "drill_type"],
+    )
+    d.dropna(axis=1, how="all", inplace=True)
     d.columns = header
     d = d.iloc[3:]
     locs = [x.replace(" Region", "") for x in sheets_to_graph]
     graphs = []
     for loc in locs:
-        df = d.xs(loc, level='loc', axis=1)
-        fig = cpl.seas_line_plot(df['DUC'].astype(float), shaded_range=[2017, 2020], title=f"{loc} DUCs")
+        df = d.xs(loc, level="loc", axis=1)
+        fig = cpl.seas_line_plot(
+            df["DUC"].astype(float), shaded_range=[2017, 2020], title=f"{loc} DUCs"
+        )
         graphs.append(fig)
     return graphs
 
 
 def get_jinja_dict():
-    data = {'title': 'EIA Productivity Report', 'name': 'EIA Productivity Report'}
-    data['release_date'] = read_release_date()
-    data['rig_charts'] = read_rig_report(filenames[0])
-    data['duc_charts'] = read_duc_report(filenames[1])
+    data = {"title": "EIA Productivity Report", "name": "EIA Productivity Report"}
+    data["release_date"] = read_release_date()
+    data["rig_charts"] = read_rig_report(filenames[0])
+    data["duc_charts"] = read_duc_report(filenames[1])
 
     return data
 
 
 def generate_page(filename=None):
-    return ju.render_html(data=get_jinja_dict(),
-                          template='monthly_drilling_report.html',
-                          filename=filename,
-                          package_loader_name='oilanalytics.eia',
-                          template_globals={'cu': cu})
+    return ju.render_html(
+        data=get_jinja_dict(),
+        template="monthly_drilling_report.html",
+        filename=filename,
+        package_loader_name="oilanalytics.eia",
+        template_globals={"cu": cu},
+    )
 
 
 def generate_email():
-    compose_and_send_jinja_report('EIA Productivity Report',
-                                  data=get_jinja_dict(),
-                                  template='monthly_drilling_report_email.html',
-                                  package_loader_name='oilanalytics.eia',
-                                  template_globals={'cu': cu})
+    compose_and_send_jinja_report(
+        "EIA Productivity Report",
+        data=get_jinja_dict(),
+        template="monthly_drilling_report_email.html",
+        package_loader_name="oilanalytics.eia",
+        template_globals={"cu": cu},
+    )
 
-if __name__ == "__main__":
 
-    proxy_support = urllib2.ProxyHandler({"http": "http://proxy-rwest-uk.energy.local:8080"})
+if __name__ == "__main__":
+    proxy_support = urllib2.ProxyHandler(
+        {"http": "http://proxy-rwest-uk.energy.local:8080"}
+    )
     opener = urllib2.build_opener(proxy_support)
     urllib2.install_opener(opener)
     # graphs = read_rig_report(filenames[0])
-    generate_page('test.html')
+    generate_page("test.html")
     # date = read_release_date()
-    # generate_email()
+    # generate_email()
```

### Comparing `oilanalytics-0.3.2/oilanalytics/eia/steo.py` & `oilanalytics-0.3.3/oilanalytics/eia/steo.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/eia/weeklypetreport.py` & `oilanalytics-0.3.3/oilanalytics/eia/weeklypetreport.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 import urllib3
 from commodplot import jinjautils as ju
 from commodplot.messaging import compose_and_send_jinja_report
 from excel_scraper import excel_scraper
 
 from oilanalytics.utils import chartutils as cu
 
-fileloc = "https://ir.eia.gov/wpsr/psw09.xls"
+fileloc_09 = "https://ir.eia.gov/wpsr/psw09.xls"
+
+fileloc_01 = "https://ir.eia.gov/wpsr/psw01.xls"
 
 canada_importa_file_loc = (
     "https://www.eia.gov/dnav/pet/hist_xls/W_EPC0_IM0_NUS-NCA_MBBLDw.xls"
 )
 
 eia_url = "https://www.eia.gov/opendata/qb.php?sdid=PET.%s.W"
 
-sheets_to_parse = [
+file_09_sheets_to_parse = [
     "Contents",
-    "Data 1",
+    # "Data 1", read from p01
     "Data 2",
     "Data 3",
     "Data 4",
     "Data 5",
     "Data 6",
     "Data 7",
     "Data 8",
@@ -31,96 +33,112 @@
     "Data 10",
     "Data 11",
     "Data 14",
     "Data 16",
 ]
 
 
-def report_symbols() -> dict:
-    """
-    Get a list of all the symbols in the Weekly Report
-    :return:
-    """
-    ex = excel_scraper.read_excel_file(fileloc)
-    symbols = {}
-    for tab in sheets_to_parse:
-        if "Data" in tab:
-            d = ex.parse(tab, skiprows=[0]).head(1).iloc[0].to_dict()
-            symbols = {**symbols, **d}
-    return symbols
-
-
 def read_canada_imports():
     df = excel_scraper.read_table(
         canada_importa_file_loc, sheet_name="Data 1", skiprows=(0, 2), index_col=0
     )
     return df
 
 
-def read_report() -> pd.DataFrame:
+def modify_level(level0, level1):
+    return [
+        item + "_4wa" if "4-Week Avg" in level1[i] else item
+        for i, item in enumerate(level0)
+    ]
+
+
+def read_release_date(fileloc):
+    ex = excel_scraper.read_excel_file(fileloc)
+    d = ex.parse("Contents")
+    ind_row = 27
+    ind_col = 2
+    # Check that the values we have match the location of 'Release Date:' in the file
+    rl_date_ind = int(d[d.eq("Release Date:").any(1)].index.values)
+    if rl_date_ind == ind_row:
+        release_date = pd.to_datetime(d.iloc[ind_row][ind_col], dayfirst=False)
+        return release_date
+    else:
+        raise ValueError("Row indexes do not match")
+
+
+def read_tab(d):
+    d = d["2000":]
+    d = d / 1000
+    # rename and columns with 4wa
+    levels = list(d.columns.levels)
+    levels[0] = modify_level(levels[0], levels[1])
+    d.columns.set_levels(levels, inplace=True)
+    d.columns = d.columns.droplevel(1)
+    return d
+
+
+def read_report_09() -> pd.DataFrame:
     """
     Read all the timeseries in the report
     :return:
     """
-    ex = excel_scraper.read_excel_file(fileloc)
+    ex = excel_scraper.read_excel_file(fileloc_09)
     dfs = []
-    for tab in sheets_to_parse:
+    for tab in file_09_sheets_to_parse:
         if "Data" in tab:
-            d = ex.parse(tab, skiprows=[0, 2], index_col=0)
-            d = d["2000":]
-            # if tab in ['Data 1', 'Data 2', 'Data 6']:
-            d = d / 1000
-            if tab == "Data 14":
-                # d.rename(columns={'WDIRPUS2':'WDIRPUS2_4wk', 'WKJRPUS2':'WKJRPUS2_4wk'}, inplace=True)
-
-                d.rename(columns={"WDIRPUS2": "WDIRPUS2_4wk"}, inplace=True)
-                d = d["WDIRPUS2_4wk"]
-            if tab == "Data 16":
-                d.rename(
-                    columns={"W_EPOOXE_YOP_NUS_MBBLD": "W_EPOOXE_YOP_NUS_MBBLD_4wk"},
-                    inplace=True,
-                )
-                d = d["W_EPOOXE_YOP_NUS_MBBLD_4wk"]
-
-            dfs.append(d)
-        else:
-            d = ex.parse(tab)
-            ind_row = 27
-            ind_col = 2
-            # Check that the values we have match the location of 'Release Date:' in the file
-            rl_date_ind = int(d[d.eq("Release Date:").any(1)].index.values)
-            if rl_date_ind == ind_row:
-                release_date = pd.to_datetime(d.iloc[ind_row][ind_col], dayfirst=False)
-            else:
-                raise ValueError("Row indexes do not match")
+            d = ex.parse(tab, skiprows=[0], header=[0, 1], index_col=0)
+            dx = read_tab(d)
+            dfs.append(dx)
+
     res = pd.concat(dfs, axis=1)
 
     res["Gas Yield"] = (res["W_EPM0F_YPR_NUS_MBBLD"] / res["WCRRIUS2"]) * 100
     res["Non Oxy Yield"] = (
         (res["W_EPM0F_YPR_NUS_MBBLD"] - res["W_EPOOXE_YOP_NUS_MBBLD"]) / res["WCRRIUS2"]
     ) * 100
     res["Dist Yield"] = (res["WDIRPUS2"] / res["WCRRIUS2"]) * 100
 
     res["mogas_dc"] = (res["WGTSTUS1"] / res["WGFUPUS2"]).rolling(window=4).mean()
     res["distillate_dc"] = (res["WDISTUS1"] / res["WDIRPUS2"]).rolling(window=4).mean()
     res["jet_dc"] = (res["WKJSTUS1"] / res["WKJUPUS2"]).rolling(window=4).mean()
 
     res = pdu.mergets(res, read_canada_imports())
 
-    return res, release_date
+    return res
+
+
+def read_report_01() -> pd.DataFrame:
+    ex = excel_scraper.read_excel_file(fileloc_01)
+    dfs = []
+    for tab in ["Data 2"]:
+        if "Data" in tab:
+            d = ex.parse(tab, skiprows=[0], header=[0, 1], index_col=0)
+            dx = read_tab(d)
+            dfs.append(dx)
+    res = pd.concat(dfs, axis=1)
+    return res
+
+
+def read_report():
+    r09 = read_report_09()
+    r01 = read_report_01()
+    report = pd.concat([r09, r01], axis=1)
+    return report
 
 
 def gen_page(
     title: str, template: str, filename: str = None, report_data: pd.DataFrame = None
 ):
     data = {"name": title, "title": title, "eia_url": eia_url}
 
     if report_data is None:
-        report_data = read_report()
-    data["report"], data["release_date"] = report_data
+        report = read_report()
+        report = report.loc[:, ~report.columns.duplicated()]
+        data["report"] = report
+    data["release_date"] = read_release_date(fileloc_09)
 
     return ju.render_html(
         data,
         template=template,
         filename=filename,
         package_loader_name="oilanalytics.eia",
         template_globals={"cu": cu},
@@ -131,15 +149,15 @@
     data = {
         "name": "DOE Weekly Quick Report",
         "title": "DOE Weekly Quick",
         "eia_url": eia_url,
     }
 
     if report_data is None:
-        report_data = read_report()
+        report_data = read_report_09()
     data["report"] = report_data
 
     return ju.render_html(
         data,
         "doe_weekly_em.html",
         filename=filename,
         package_loader_name="oilanalytics.eia",
@@ -155,15 +173,15 @@
 ):
     data = {
         "name": "DOE Weekly Petroleum Report",
         "title": "DOE Weekly",
         "eia_url": eia_url,
     }
     if report_data is None:
-        report_data = read_report()[0]
+        report_data = read_report_09()[0]
 
     summary_table_items = {
         "WCESTUS1": "Crude Stocks",
         "W_EPC0_SAX_YCUOK_MBBL": "Cushing Stocks",
         "WGTSTUS1": "Mogas Stocks",
         "WDISTUS1": "Distillate Stocks",
         "WGFUPUS2": "Mogas Demand",
@@ -247,12 +265,12 @@
         filename=r"ethanol.html",
     )
     gen_page(
         title="DOE Weekly Report - Crude",
         template="doe_weekly_crude.html",
         filename=r"crude.html",
     )
-    gen_page(
-        title="DOE Weekly Report - Gasoline",
-        template="doe_weekly_gasoline.html",
-        filename=r"gasoline.html",
-    )
+    # gen_page(
+    #     title="DOE Weekly Report - Gasoline",
+    #     template="doe_weekly_gasoline.html",
+    #     filename=r"gasoline.html",
+    # )
```

### Comparing `oilanalytics-0.3.2/oilanalytics/energyaspects/china_stats.py` & `oilanalytics-0.3.3/oilanalytics/energyaspects/china_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     3332,
     1446,
     1481,
     1479,
     1480,
     3324,
     15160,
-
 ]
 
 
 def generate_page(
     file_path: str = None,
     title_url: str = None,
 ):
```

### Comparing `oilanalytics-0.3.2/oilanalytics/energyaspects/europe_diesel_balance.py` & `oilanalytics-0.3.3/oilanalytics/energyaspects/europe_diesel_balance.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/energyaspects/fsu_stats.py` & `oilanalytics-0.3.3/oilanalytics/energyaspects/fsu_stats.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/energyaspects/tars.py` & `oilanalytics-0.3.3/oilanalytics/energyaspects/tars.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/euroilstock/euroilstock.py` & `oilanalytics-0.3.3/oilanalytics/euroilstock/euroilstock.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/highfreq/ara.py` & `oilanalytics-0.3.3/oilanalytics/highfreq/ara.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/highfreq/singapore.py` & `oilanalytics-0.3.3/oilanalytics/highfreq/singapore.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/iea/omr.py` & `oilanalytics-0.3.3/oilanalytics/iea/omr.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/opec/momr.py` & `oilanalytics-0.3.3/oilanalytics/opec/momr.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics/prices/futures_prices.py` & `oilanalytics-0.3.3/oilanalytics/prices/futures_prices.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,14 @@
         "novdec",
         "decjan",
     ]:
         d = forwards.spread_combination(contracts=contracts, combination_type=spread)
         data[spread] = cpl.reindex_year_line_plot(d, title=spread)
 
     if cust_charts:
-
         index = 1
         for cust_chart in cust_charts:
             d = forwards.spread_combination(contracts, cust_chart)
             f = cpl.reindex_year_line_plot(d, title=cust_charts[cust_chart])
             data["cust_ch%s" % index] = f
             index += 1
```

### Comparing `oilanalytics-0.3.2/oilanalytics/utils/chartutils.py` & `oilanalytics-0.3.3/oilanalytics/utils/chartutils.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/oilanalytics.egg-info/SOURCES.txt` & `oilanalytics-0.3.3/oilanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/setup.py` & `oilanalytics-0.3.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="oilanalytics",
-    version="0.3.2",
+    version="0.3.3",
     author="aeorxc",
     description="Utilities for oil analytics",
     url="https://github.com/aeorxc/oilanalytics",
     project_urls={
         "Source": "https://github.com/aeorxc/oilanalytics",
     },
     packages=setuptools.find_packages(),
```

### Comparing `oilanalytics-0.3.2/test/test_eia.py` & `oilanalytics-0.3.3/test/test_eia.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.2/test/test_highfreq.py` & `oilanalytics-0.3.3/test/test_highfreq.py`

 * *Files identical despite different names*

