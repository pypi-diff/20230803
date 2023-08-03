# Comparing `tmp/frequenz-sdk-0.22.1.tar.gz` & `tmp/frequenz-sdk-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-sdk-0.22.1.tar", last modified: Tue Jul 11 15:43:51 2023, max compression
+gzip compressed data, was "frequenz-sdk-0.23.0.tar", last modified: Thu Aug  3 08:13:11 2023, max compression
```

## Comparing `frequenz-sdk-0.22.1.tar` & `frequenz-sdk-0.23.0.tar`

### file list

```diff
@@ -1,128 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/docs/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/css/style.css
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/mkdocstrings_autoapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3897 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/
--rw-r--r--   0 runner    (1001) docker     (122)     6208 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.275658 frequenz-sdk-0.22.1/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/frequenz/sdk/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/frequenz/sdk/_api_client/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_api_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      845 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_math.py
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_singleton_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_channel_registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_config_managing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.279658 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
--rw-r--r--   0 runner    (1001) docker     (122)    15805 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
--rw-r--r--   0 runner    (1001) docker     (122)     7120 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6947 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_resampling.py
--rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_run_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7745 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    17218 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/_battery_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    28316 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/power_distributing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/request.py
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/config/
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/config/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12014 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/_data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23526 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/
--rw-r--r--   0 runner    (1001) docker     (122)      721 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component.py
--rw-r--r--   0 runner    (1001) docker     (122)    10579 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component_states.py
--rw-r--r--   0 runner    (1001) docker     (122)     5480 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/connection_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.283658 frequenz-sdk-0.22.1/src/frequenz/sdk/power/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18962 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/power/_distribution_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.287659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4269 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_base_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.287659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    32060 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     5949 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.287659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3885 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     5242 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3683 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_producer_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     9501 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)    13082 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_moving_window.py
--rw-r--r--   0 runner    (1001) docker     (122)    16175 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)    21539 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_quantities.py
--rw-r--r--   0 runner    (1001) docker     (122)    28782 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_resampling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.287659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18830 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8411 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     9179 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)    16979 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    18773 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13600 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
--rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/logical_meter/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/logical_meter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15511 2023-07-11 15:43:36.000000 frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:43:51.291659 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-07-11 15:43:51.000000 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4904 2023-07-11 15:43:51.000000 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 15:43:51.000000 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-07-11 15:43:51.000000 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-11 15:43:51.000000 frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.937173 frequenz-sdk-0.23.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     5144 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/.cookiecutter-replay.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4314 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-08-03 08:13:11.937173 frequenz-sdk-0.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.925173 frequenz-sdk-0.23.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.925173 frequenz-sdk-0.23.0/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1790 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.925173 frequenz-sdk-0.23.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4333 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 08:13:11.937173 frequenz-sdk-0.23.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.925173 frequenz-sdk-0.23.0/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     6369 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.921173 frequenz-sdk-0.23.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.925173 frequenz-sdk-0.23.0/src/frequenz/sdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.925173 frequenz-sdk-0.23.0/src/frequenz/sdk/_api_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/_api_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.925173 frequenz-sdk-0.23.0/src/frequenz/sdk/_internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/_internal/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/_internal/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      845 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/_internal/_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/_internal/_singleton_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.925173 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_channel_registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2844 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_config_managing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.929173 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_data_sourcing/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_data_sourcing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15869 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7005 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6947 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_run_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.929173 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7745 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19121 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/_battery_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28316 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/power_distributing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.929173 frequenz-sdk-0.23.0/src/frequenz/sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/config/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.929173 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12014 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/_data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.929173 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/client/
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23526 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/client/_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/client/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/client/_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.929173 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/component/
+-rw-r--r--   0 runner    (1001) docker     (122)      721 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4695 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/component/_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10566 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/component/_component_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/component/_component_states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5480 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/connection_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.929173 frequenz-sdk-0.23.0/src/frequenz/sdk/power/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18962 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/power/_distribution_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.933173 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4269 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_base_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.933173 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30597 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5949 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5013 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.933173 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3276 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3885 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5242 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3683 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_producer_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9509 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4590 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13233 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_moving_window.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16218 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31960 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28782 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.933173 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_ringbuffer/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18830 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.937173 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8411 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9179 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19946 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20091 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.937173 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/ev_charger_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13600 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4719 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4107 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.937173 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/logical_meter/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/logical_meter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15511 2023-08-03 08:12:55.000000 frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 08:13:11.937173 frequenz-sdk-0.23.0/src/frequenz_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-08-03 08:13:11.000000 frequenz-sdk-0.23.0/src/frequenz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-08-03 08:13:11.000000 frequenz-sdk-0.23.0/src/frequenz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 08:13:11.000000 frequenz-sdk-0.23.0/src/frequenz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-08-03 08:13:11.000000 frequenz-sdk-0.23.0/src/frequenz_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-08-03 08:13:11.000000 frequenz-sdk-0.23.0/src/frequenz_sdk.egg-info/top_level.txt
```

### Comparing `frequenz-sdk-0.22.1/CONTRIBUTING.md` & `frequenz-sdk-0.23.0/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Contributing to `frequenz-sdk`
+# Contributing to Frequenz Python SDK
 
 ## Build
 
 You can use `build` to simply build the source and binary distribution:
 
 ```sh
 python -m pip install build
@@ -24,53 +24,53 @@
 python -m pip install -e .[dev]
 ```
 
 If you don't want to install all the dependencies, you can also use `nox` to
 run the tests and other checks creating its own virtual environments:
 
 ```sh
-python -m pip install nox toml
+python -m pip install .[dev-noxfile]
 nox
 ```
 
 You can also use `nox -R` to reuse the current testing environment to speed up
 test at the expense of a higher chance to end up with a dirty test environment.
 
 ### Running tests / checks individually
 
 For a better development test cycle you can install the runtime and test
 dependencies and run `pytest` manually.
 
 ```sh
-python -m pip install .[pytest]  # included in .[dev] too
+python -m pip install .[dev-pytest]  # included in .[dev] too
 
 # And for example
-pytest tests/test_sdk.py
+pytest tests/test_*.py
 ```
 
 Or you can use `nox`:
 
 ```sh
-nox -R -s pytest -- test/test_sdk.py
+nox -R -s pytest -- test/test_*.py
 ```
 
 The same appliest to `pylint` or `mypy` for example:
 
 ```sh
-nox -R -s pylint -- test/test_sdk.py
-nox -R -s mypy -- test/test_sdk.py
+nox -R -s pylint -- test/test_*.py
+nox -R -s mypy -- test/test_*.py
 ```
 
 ### Building the documentation
 
 To build the documentation, first install the dependencies (if you didn't
 install all `dev` dependencies):
 
 ```sh
-python -m pip install -e .[docs-gen]
+python -m pip install -e .[dev-mkdocs]
 ```
 
 Then you can build the documentation (it will be written in the `site/`
 directory):
 
 ```sh
 mkdocs build
@@ -118,36 +118,35 @@
 ## Releasing
 
 These are the steps to create a new release:
 
 1. Get the latest head you want to create a release from.
 
 2. Update the `RELEASE_NOTES.md` file if it is not complete, up to date, and
-   clean from template comments (`<!-- ... ->`) and empty sections. Submit
-   a pull request if an update is needed, wait until it is merged, and update
-   the latest head you want to create a release from to get the new merged pull
+   remove template comments (`<!-- ... ->`) and empty sections. Submit a pull
+   request if an update is needed, wait until it is merged, and update the
+   latest head you want to create a release from to get the new merged pull
    request.
 
 3. Create a new signed tag using the release notes and
    a [semver](https://semver.org/) compatible version number with a `v` prefix,
    for example:
 
    ```sh
-   git tag -s -F RELEASE_NOTES.md v0.0.1
+   git tag -s --cleanup=whitespace -F RELEASE_NOTES.md v0.0.1
    ```
 
 4. Push the new tag.
 
 5. A GitHub action will test the tag and if all goes well it will create
    a [GitHub
    Release](https://github.com/frequenz-floss/frequenz-sdk-python/releases),
-   create a new
-   [announcement](https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/announcements)
-   about the release, and upload a new package to
-   [PyPI](https://pypi.org/project/frequenz-sdk/) automatically.
+   and upload a new package to
+   [PyPI](https://pypi.org/project/frequenz-sdk/)
+   automatically.
 
 6. Once this is done, reset the `RELEASE_NOTES.md` with the template:
 
    ```sh
    cp .github/RELEASE_NOTES.template.md RELEASE_NOTES.md
    ```
```

### Comparing `frequenz-sdk-0.22.1/LICENSE` & `frequenz-sdk-0.23.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Frequenz Energy-as-a-Service GmbH
+Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `frequenz-sdk-0.22.1/PKG-INFO` & `frequenz-sdk-0.23.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,69 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 0.22.1
-Summary: Frequenz Python SDK
+Version: 0.23.0
+Summary: A development kit to interact with the Frequenz development platform
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
-Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
+Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/support
-Keywords: frequenz,sdk,microgrid,actor
+Keywords: frequenz,python,lib,library,sdk,microgrid
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: docs-gen
-Provides-Extra: docs-lint
-Provides-Extra: format
-Provides-Extra: nox
-Provides-Extra: examples
-Provides-Extra: pytest
-Provides-Extra: mypy
-Provides-Extra: pylint
+Provides-Extra: dev-docstrings
+Provides-Extra: dev-examples
+Provides-Extra: dev-formatting
+Provides-Extra: dev-mkdocs
+Provides-Extra: dev-mypy
+Provides-Extra: dev-noxfile
+Provides-Extra: dev-pylint
+Provides-Extra: dev-pytest
 Provides-Extra: dev
 License-File: LICENSE
 
 # Frequenz Python SDK
 
 [![Build Status](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml)
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-sdk)](https://pypi.org/project/frequenz-sdk/)
 [![Docs](https://img.shields.io/badge/docs-latest-informational)](https://frequenz-floss.github.io/frequenz-sdk-python/)
 
+## Introduction
+
 A development kit to interact with the Frequenz development platform.
 
-## Supported Python versions
+## Quick Start
+
+We assume you are on a system with Python available. If that is not the case,
+please [download and install Python](https://www.python.org/downloads/) first.
+
+To install the SDK, you probably want to create a new virtual environment first.
+For example, if you use a `sh` compatible shell, you can do this:
+
+```sh
+python3 -m venv .venv
+. .venv/bin/activate
+```
+
+Then, just install using `pip`:
+
+```sh
+python3 -m pip install frequenz-sdk
+```
+
+## Documentation
 
-* Only Python 3.11 is fully supported (tested).
+For more information, please visit the [documentation
+website](https://frequenz-floss.github.io/frequenz-sdk-python/).
 
 ## Contributing
 
 If you want to know how to build this project and contribute to it, please
 check out the [Contributing Guide](CONTRIBUTING.md).
```

### Comparing `frequenz-sdk-0.22.1/docs/css/mkdocstrings.css` & `frequenz-sdk-0.23.0/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/docs/css/style.css` & `frequenz-sdk-0.23.0/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/docs/logo.png` & `frequenz-sdk-0.23.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/mkdocs.yml` & `frequenz-sdk-0.23.0/mkdocs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # MkDocs configuration
 # For details see: https://www.mkdocs.org/user-guide/configuration/
 
 # Project information
-site_name: Frequenz Python SDK
-site_description: Frequenz Python SDK.
-site_author: Frequenz Energy-as-a-Service GmbH
-copyright: Frequenz Energy-as-a-Service GmbH
+site_name: "Frequenz Python SDK"
+site_description: "A development kit to interact with the Frequenz development platform"
+site_author: "Frequenz Energy-as-a-Service GmbH"
+copyright: "Copyright © 2022 Frequenz Energy-as-a-Service GmbH"
 repo_name: "frequenz-sdk-python"
 repo_url: "https://github.com/frequenz-floss/frequenz-sdk-python"
 edit_uri: "edit/v0.x.x/docs/"
+strict: true  # Treat warnings as errors
 
 # Build directories
 theme:
   name: "material"
   logo: logo.png
   favicon: logo.png
   language: en
   icon:
     edit: material/file-edit-outline
     repo: fontawesome/brands/github
   custom_dir: docs/overrides
   features:
+    - content.code.annotate
+    - content.code.copy
     - navigation.instant
     - navigation.tabs
     - navigation.top
     - navigation.tracking
     - toc.follow
   palette:
   - media: "(prefers-color-scheme: light)"
@@ -57,24 +60,28 @@
   - css/mkdocstrings.css
 
 # Formatting options
 markdown_extensions:
   - admonition
   - attr_list
   - pymdownx.details
-  - pymdownx.superfences
-  - pymdownx.tasklist
-  - pymdownx.tabbed
+  - pymdownx.highlight:
+      anchor_linenums: true
+      line_spans: __span
+      pygments_lang_class: true
+  - pymdownx.keys
   - pymdownx.snippets:
       check_paths: true
   - pymdownx.superfences:
       custom_fences:
         - name: mermaid
           class: mermaid
           format: "!!python/name:pymdownx.superfences.fence_code_format"
+  - pymdownx.tabbed
+  - pymdownx.tasklist
   - toc:
       permalink: "¤"
 
 plugins:
   - gen-files:
       scripts:
         - docs/mkdocstrings_autoapi.py
@@ -84,24 +91,32 @@
       canonical_version: latest
   - mkdocstrings:
       custom_templates: templates
       default_handler: python
       handlers:
         python:
           options:
-            paths: [src]
+            paths: ["src"]
             docstring_section_style: spacy
             merge_init_into_class: false
             show_category_heading: true
             show_root_heading: true
             show_root_members_full_path: true
             show_source: true
           import:
+            # See https://mkdocstrings.github.io/python/usage/#import for details
             - https://docs.python.org/3/objects.inv
+            - https://frequenz-floss.github.io/frequenz-channels-python/v0.14/objects.inv
+            - https://grpc.github.io/grpc/python/objects.inv
+            - https://networkx.org/documentation/stable/objects.inv
+            - https://numpy.org/doc/stable/objects.inv
+            - https://protobuf.readthedocs.io/en/latest/objects.inv
+            - https://typing-extensions.readthedocs.io/en/stable/objects.inv
+            - https://watchfiles.helpmanual.io/objects.inv
   - search
   - section-index
 
 # Preview controls
 watch:
-  - src
+  - "src"
   - README.md
   - CONTRIBUTING.md
```

### Comparing `frequenz-sdk-0.22.1/pyproject.toml` & `frequenz-sdk-0.23.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,110 +1,118 @@
+# License: MIT
+# Copyright © 2022 Frequenz Energy-as-a-Service GmbH
+
 [build-system]
 requires = [
-  "setuptools >= 65.3.0, < 66",
-  "setuptools_scm[toml] >= 7.0.5, < 8",
-  "wheel",
+  "setuptools == 67.7.2",
+  "setuptools_scm[toml] == 7.1.0",
+  "frequenz-repo-config[lib] == 0.4.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-sdk"
-description = "Frequenz Python SDK"
+description = "A development kit to interact with the Frequenz development platform"
 readme = "README.md"
 license = { text = "MIT" }
-keywords = ["frequenz", "sdk", "microgrid", "actor"]
+keywords = ["frequenz", "python", "lib", "library", "sdk", "microgrid"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries",
+  "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
 dependencies = [
   "frequenz-api-microgrid >= 0.11.0, < 0.12.0",
-  "frequenz-channels >= 0.14.0, < 0.15.0",
+  # Make sure to update the mkdocs.yml file when
+  # changing the version
+  # (plugins.mkdocstrings.handlers.python.import)
+  "frequenz-channels >= 0.16.0, < 0.17.0",
   "google-api-python-client >= 2.71, < 3",
   "grpcio >= 1.54.2, < 2",
   "grpcio-tools >= 1.54.2, < 2",
   "networkx >= 2.8, < 4",
   "numpy >= 1.24.2, < 2",
   "protobuf >= 4.21.6, < 5",
   "pydantic >= 1.9, < 2",
-  "toml >= 0.10",
   "tqdm >= 4.38.0, < 5",
   "typing_extensions >= 4.4.0, < 5",
   "watchfiles >= 0.15.0",
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
-docs-gen = [
+dev-docstrings = [
+  "pydocstyle == 6.3.0",
+  "darglint == 1.8.1",
+  "tomli == 2.0.1",      # Needed by pydocstyle to read pyproject.toml
+]
+dev-examples = ["polars == 0.18.11"]
+dev-formatting = ["black == 23.7.0", "isort == 5.12.0"]
+dev-mkdocs = [
   "mike == 1.1.2",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.0",
-  "mkdocs-material == 9.1.18",
+  "mkdocs-material == 9.1.21",
   "mkdocs-section-index == 0.3.5",
   "mkdocstrings[python] == 0.22.0",
+  "frequenz-repo-config[lib] == 0.4.0",
 ]
-docs-lint = [
-  "pydocstyle == 6.3.0",
-  "darglint == 1.8.1",
-  "tomli == 2.0.1",      # Needed by pydocstyle to read pyproject.toml
+dev-mypy = [
+  "mypy == 1.4.1",
+  "grpc-stubs == 1.24.12",      # This dependency introduces breaking changes in patch releases
+  "types-protobuf == 4.23.0.2",
+  # For checking the noxfile, docs/ script, and tests
+  "frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]",
+]
+dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[lib] == 0.4.0"]
+dev-pylint = [
+  "pylint == 2.17.5",
+  # For checking the noxfile, docs/ script, and tests
+  "frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
-format = ["black == 23.3.0", "isort == 5.12.0"]
-nox = ["nox == 2023.4.22", "toml == 0.10.2"]
-examples = [ "polars == 0.18.4" ]
-pytest = [
+dev-pytest = [
   "pytest == 7.4.0",
-  "pytest-cov == 4.1.0",
   "pytest-mock == 3.11.1",
-  "pytest-asyncio == 0.21.0",
-  "time-machine == 2.10.0",
+  "pytest-asyncio == 0.21.1",
+  "time-machine == 2.11.0",
   "async-solipsism == 0.5",
   # For checking docstring code examples
-  "sybil == 5.0.2",
-  "pylint == 2.17.4",
-  "frequenz-sdk[examples]",
-]
-mypy = [
-  "mypy == 1.4.1",
-  "grpc-stubs == 1.24.12", # This dependency introduces breaking changes in patch releases
-  # For checking the noxfile, docs/ script, and tests
-  "frequenz-sdk[docs-gen,nox,pytest]",
+  "sybil == 5.0.3",
+  "pylint == 2.17.5",
+  "frequenz-sdk[dev-examples]",
 ]
-pylint = [
-  "pylint == 2.17.4",
-  # For checking the noxfile, docs/ script, and tests
-  "frequenz-sdk[docs-gen,nox,pytest]",
+dev = [
+  "frequenz-sdk[dev-mkdocs,dev-docstrings,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
-dev = ["frequenz-sdk[docs-gen,docs-lint,format,nox,pytest,mypy,pylint]"]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-sdk-python/releases"
-Repository = "https://github.com/frequenz-floss/frequenz-sdk-python"
 Issues = "https://github.com/frequenz-floss/frequenz-sdk-python/issues"
+Repository = "https://github.com/frequenz-floss/frequenz-sdk-python"
 Support = "https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/support"
 
-[tool.setuptools]
-include-package-data = true
-
-[tool.setuptools_scm]
-version_scheme = "post-release"
-
 [tool.black]
 line-length = 88
-target-version = ['py38']
+target-version = ['py311']
 include = '\.pyi?$'
 
+[tool.isort]
+profile = "black"
+line_length = 88
+src_paths = ["benchmarks", "examples", "src", "tests"]
+
 [tool.pylint.similarities]
 ignore-comments = ['yes']
 ignore-docstrings = ['yes']
 ignore-imports = ['no']
 min-similarity-lines = 40
 
 [tool.pylint.messages_control]
@@ -117,29 +125,28 @@
   # it is a type-check, for which we already have mypy.
   "unsubscriptable-object",
 ]
 
 [tool.pylint.design]
 max-attributes = 12
 
-[tool.isort]
-profile = "black"
-line_length = 88
-src_paths = ["src", "examples", "tests"]
-
 [tool.pytest.ini_options]
+testpaths = ["tests", "src"]
 asyncio_mode = "auto"
 required_plugins = ["pytest-asyncio", "pytest-mock"]
 
 [[tool.mypy.overrides]]
 module = [
+  "async_solipsism",
+  "async_solipsism.*",
   "grpc.aio",
   "grpc.aio.*",
   # There is a stubs package available, but it's not working:
   # https://github.com/eggplants/networkx-stubs/issues/1
   "networkx",
+  "sybil",
+  "sybil.*",
 ]
 ignore_missing_imports = true
 
-[[tool.mypy.overrides]]
-module = ["async_solipsism", "async_solipsism.*"]
-ignore_missing_imports = true
+[tool.setuptools_scm]
+version_scheme = "post-release"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `frequenz-sdk-0.22.1/src/conftest.py` & `frequenz-sdk-0.23.0/src/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,19 +38,20 @@
     Args:
         code: The code to extract import statements from.
 
     Returns:
         A list of import statements.
     """
     tree = ast.parse(code)
-    import_statements = []
+    import_statements: list[str] = []
 
     for node in ast.walk(tree):
         if isinstance(node, (ast.Import, ast.ImportFrom)):
             import_statement = ast.get_source_segment(code, node)
+            assert import_statement is not None
             import_statements.append(import_statement)
 
     return import_statements
 
 
 def path_to_import_statement(path: Path) -> str:
     """Convert a path to a Python file to an import statement.
@@ -81,15 +82,17 @@
     module_path = ".".join(parts)[:-3]
 
     # Create the import statement
     import_statement = f"from {module_path} import *"
     return import_statement
 
 
-class CustomPythonCodeBlockParser(CodeBlockParser):
+# We need to add the type ignore comment here because the Sybil library does not
+# have type annotations.
+class CustomPythonCodeBlockParser(CodeBlockParser):  # type: ignore[misc]
     """Code block parser that validates extracted code examples using pylint.
 
     This parser is a modified version of the default Python code block parser
     from the Sybil library.
     It uses pylint to validate the extracted code examples.
 
     All code examples are preceded by the original file's import statements as
@@ -99,15 +102,15 @@
 
     Additionally, the code example is padded with empty lines to make sure the
     line numbers are correct.
 
     Pylint warnings which are unimportant for code examples are disabled.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize the parser."""
         super().__init__("python")
 
     def evaluate(self, example: Example) -> None | str:
         """Validate the extracted code example using pylint.
 
         Args:
@@ -118,16 +121,14 @@
         """
         # Get the import statements for the original file
         import_header = get_import_statements(example.document.text)
         # Add a wildcard import of the original file
         import_header.append(
             path_to_import_statement(Path(os.path.relpath(example.path)))
         )
-        # Add microgrid as default import
-        import_header.append("from frequenz.sdk import microgrid")
         imports_code = "\n".join(import_header)
 
         # Dedent the code example
         # There is also example.parsed that is already prepared, but it has
         # empty lines stripped and thus fucks up the line numbers.
         example_code = textwrap.dedent(
             example.document.text[example.start : example.end]
@@ -160,15 +161,15 @@
         ]
 
         response = validate_with_pylint(source, example.path, pylint_disable_params)
 
         if len(response) > 0:
             return (
                 f"Pylint validation failed for code example:\n"
-                f"{example_with_imports}\nOutput: {response}"
+                f"{example_with_imports}\nOutput: " + "\n".join(response)
             )
 
         return None
 
 
 def validate_with_pylint(
     code_example: str, path: str, disable_params: list[str]
@@ -196,15 +197,17 @@
             pylint_command,
             input=code_example,
             text=True,
             capture_output=True,
             check=True,
         )
     except subprocess.CalledProcessError as exception:
-        return exception.output.splitlines()
+        output = exception.output
+        assert isinstance(output, str)
+        return output.splitlines()
 
     return []
 
 
 pytest_collect_file = Sybil(
     parsers=[CustomPythonCodeBlockParser()],
     patterns=["*.py"],
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/_api_client/api_client.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_asyncio.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/_internal/_asyncio.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_constants.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/_internal/_constants.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_math.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/_internal/_math.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/_internal/_singleton_meta.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/_internal/_singleton_meta.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/__init__.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_channel_registry.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_channel_registry.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_config_managing.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_config_managing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Read and update config variables."""
 
 import logging
 import os
-from typing import Any, Dict, Optional, Set
+import tomllib
+from collections import abc
+from typing import Any, Dict
 
-import toml
 from frequenz.channels import Sender
 from frequenz.channels.util import FileWatcher
 
 from ..actor._decorator import actor
 from ..config import Config
 
 _logger = logging.getLogger(__name__)
@@ -27,15 +28,15 @@
     If new file is read, then previous configs will be forgotten.
     """
 
     def __init__(
         self,
         conf_file: str,
         output: Sender[Config],
-        event_types: Optional[Set[FileWatcher.EventType]] = None,
+        event_types: abc.Set[FileWatcher.EventType] = frozenset(FileWatcher.EventType),
     ) -> None:
         """Read config variables from the file.
 
         Args:
             conf_file: Path to file with config variables.
             output: Channel to publish updates to.
             event_types: Which types of events should update the config and
@@ -54,15 +55,16 @@
         Raises:
             ValueError: if config file cannot be read.
 
         Returns:
             A dictionary containing configuration variables.
         """
         try:
-            return toml.load(self._conf_file)
+            with open(self._conf_file, "rb") as toml_file:
+                return tomllib.load(toml_file)
         except ValueError as err:
             logging.error("Can't read config file, err: %s", err)
             raise
 
     async def send_config(self) -> None:
         """Send config file using a broadcast channel."""
         conf_vars = self._read_config()
@@ -74,16 +76,17 @@
 
         At startup, the Config Manager sends the current config so that it
         can be cache in the Broadcast channel and served to receivers even if
         there hasn't been any change to the config file itself.
         """
         await self.send_config()
 
-        async for path in self._file_watcher:
-            if str(path) == self._conf_file:
-                _logger.info(
-                    "Update configs, because file %s was modified.",
-                    self._conf_file,
-                )
-                await self.send_config()
+        async for event in self._file_watcher:
+            if event.type != FileWatcher.EventType.DELETE:
+                if str(event.path) == self._conf_file:
+                    _logger.info(
+                        "Update configs, because file %s was modified.",
+                        self._conf_file,
+                    )
+                    await self.send_config()
 
         _logger.debug("ConfigManager stopped.")
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 _BatteryDataMethods: Dict[ComponentMetricId, Callable[[BatteryData], float]] = {
     ComponentMetricId.SOC: lambda msg: msg.soc,
     ComponentMetricId.SOC_LOWER_BOUND: lambda msg: msg.soc_lower_bound,
     ComponentMetricId.SOC_UPPER_BOUND: lambda msg: msg.soc_upper_bound,
     ComponentMetricId.CAPACITY: lambda msg: msg.capacity,
     ComponentMetricId.POWER_LOWER_BOUND: lambda msg: msg.power_lower_bound,
     ComponentMetricId.POWER_UPPER_BOUND: lambda msg: msg.power_upper_bound,
+    ComponentMetricId.TEMPERATURE: lambda msg: msg.temperature,
 }
 
 _InverterDataMethods: Dict[ComponentMetricId, Callable[[InverterData], float]] = {
     ComponentMetricId.ACTIVE_POWER: lambda msg: msg.active_power,
     ComponentMetricId.ACTIVE_POWER_LOWER_BOUND: lambda msg: msg.active_power_lower_bound,
     ComponentMetricId.ACTIVE_POWER_UPPER_BOUND: lambda msg: msg.active_power_upper_bound,
 }
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_decorator.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     Raises:
         TypeError: when the class doesn't have a `run` method as per spec.
 
     Example (one actor receiving from two receivers):
     ```python
     from frequenz.channels import Broadcast, Receiver, Sender
-    from frequenz.channels.util import Select
+    from frequenz.channels.util import select, selected_from
     @actor
     class EchoActor:
         def __init__(
             self,
             name: str,
             recv1: Receiver[bool],
             recv2: Receiver[bool],
@@ -95,21 +95,17 @@
             self.name = name
 
             self._recv1 = recv1
             self._recv2 = recv2
             self._output = output
 
         async def run(self) -> None:
-            select = Select(channel_1=self._recv1, channel_2=self._recv2)
-            while await select.ready():
-                if msg := select.channel_1:
-                    await self._output.send(msg.inner)
-                elif msg := select.channel_2:
-                    await self._output.send(msg.inner)
-
+            async for selected in select(self._recv1, self._recv2):
+                if selected_from(selected, self._recv1):
+                    await self._output.send(selected.value)
 
     input_chan_1: Broadcast[bool] = Broadcast("input_chan_1")
     input_chan_2: Broadcast[bool] = Broadcast("input_chan_2")
 
     echo_chan: Broadcast[bool] = Broadcast("EchoChannel")
 
     echo_actor = EchoActor(
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_resampling.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_resampling.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/_run_utils.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/_run_utils.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/__init__.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/_battery_status.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/_battery_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from typing import Iterable, Optional, Set, TypeVar, Union
 
 from frequenz.api.microgrid.battery_pb2 import ComponentState as BatteryComponentState
 from frequenz.api.microgrid.battery_pb2 import RelayState as BatteryRelayState
 from frequenz.api.microgrid.common_pb2 import ErrorLevel
 from frequenz.api.microgrid.inverter_pb2 import ComponentState as InverterComponentState
 from frequenz.channels import Receiver, Sender
-from frequenz.channels.util import Select, Timer
+from frequenz.channels.util import Timer, select, selected_from
 
 from frequenz.sdk._internal._asyncio import cancel_and_await
 from frequenz.sdk.microgrid import connection_manager
 from frequenz.sdk.microgrid.component import (
     BatteryData,
     ComponentCategory,
     ComponentData,
@@ -77,14 +77,18 @@
 
 @dataclass
 class _BlockingStatus:
     min_duration_sec: float
     max_duration_sec: float
 
     def __post_init__(self) -> None:
+        assert self.min_duration_sec <= self.max_duration_sec, (
+            f"Minimum blocking duration ({self.min_duration_sec}) cannot be greater "
+            f"than maximum blocking duration ({self.max_duration_sec})"
+        )
         self.last_blocking_duration_sec: float = self.min_duration_sec
         self.blocked_until: Optional[datetime] = None
 
     def block(self) -> float:
         """Block battery.
 
         Battery can be unblocked using `self.unblock()` method.
@@ -193,22 +197,23 @@
         )
 
         inverter_id = self._find_adjacent_inverter_id(battery_id)
         if inverter_id is None:
             raise RuntimeError(f"Can't find inverter adjacent to battery: {battery_id}")
 
         self._battery: _ComponentStreamStatus = _ComponentStreamStatus(
-            battery_id, data_recv_timer=Timer(max_data_age_sec)
+            battery_id,
+            data_recv_timer=Timer.timeout(timedelta(seconds=max_data_age_sec)),
         )
         self._inverter: _ComponentStreamStatus = _ComponentStreamStatus(
-            inverter_id, data_recv_timer=Timer(max_data_age_sec)
+            inverter_id,
+            data_recv_timer=Timer.timeout(timedelta(seconds=max_data_age_sec)),
         )
 
         # Select needs receivers that can be get in async way only.
-        self._select: Select | None = None
 
         self._task: asyncio.Task[None] = asyncio.create_task(
             self._run(status_sender, set_power_result_receiver)
         )
 
     @property
     def battery_id(self) -> int:
@@ -219,16 +224,78 @@
         """
         return self._battery.component_id
 
     async def stop(self) -> None:
         """Stop tracking battery status."""
         await cancel_and_await(self._task)
 
-        if self._select is not None:
-            await self._select.stop()
+    def _handle_status_battery(self, bat_data: BatteryData) -> None:
+        self._battery.last_msg_correct = (
+            self._is_message_reliable(bat_data)
+            and self._is_battery_state_correct(bat_data)
+            and self._no_critical_error(bat_data)
+            and self._is_capacity_present(bat_data)
+        )
+        self._battery.last_msg_timestamp = bat_data.timestamp
+        self._battery.data_recv_timer.reset()
+
+    def _handle_status_inverter(self, inv_data: InverterData) -> None:
+        self._inverter.last_msg_correct = (
+            self._is_message_reliable(inv_data)
+            and self._is_inverter_state_correct(inv_data)
+            and self._no_critical_error(inv_data)
+        )
+        self._inverter.last_msg_timestamp = inv_data.timestamp
+        self._inverter.data_recv_timer.reset()
+
+    def _handle_status_set_power_result(self, result: SetPowerResult) -> None:
+        if self.battery_id in result.succeed:
+            self._blocking_status.unblock()
+
+        elif (
+            self.battery_id in result.failed and self._last_status != Status.NOT_WORKING
+        ):
+            duration = self._blocking_status.block()
+
+            if duration > 0:
+                _logger.warning(
+                    "battery %d failed last response. block it for %f sec",
+                    self.battery_id,
+                    duration,
+                )
+
+    def _handle_status_battery_timer(self) -> None:
+        if self._battery.last_msg_correct:
+            self._battery.last_msg_correct = False
+            _logger.warning(
+                "Battery %d stopped sending data, last timestamp: %s",
+                self._battery.component_id,
+                self._battery.last_msg_timestamp,
+            )
+
+    def _handle_status_inverter_timer(self) -> None:
+        if self._inverter.last_msg_correct:
+            self._inverter.last_msg_correct = False
+            _logger.warning(
+                "Inverter %d stopped sending data, last timestamp: %s",
+                self._inverter.component_id,
+                self._inverter.last_msg_timestamp,
+            )
+
+    def _get_new_status_if_changed(self) -> Optional[Status]:
+        current_status = self._get_current_status()
+        if self._last_status != current_status:
+            self._last_status = current_status
+            _logger.info(
+                "battery %d changed status %s",
+                self.battery_id,
+                str(self._last_status),
+            )
+            return current_status
+        return None
 
     async def _run(
         self,
         status_sender: Sender[Status],
         set_power_result_receiver: Receiver[SetPowerResult],
     ) -> None:
         """Process data from the components and set_power_result_receiver.
@@ -241,102 +308,73 @@
                 components.
         """
         api_client = connection_manager.get().api_client
 
         battery_receiver = await api_client.battery_data(self._battery.component_id)
         inverter_receiver = await api_client.inverter_data(self._inverter.component_id)
 
-        self._select = Select(
-            battery=battery_receiver,
-            battery_timer=self._battery.data_recv_timer,
-            inverter_timer=self._inverter.data_recv_timer,
-            inverter=inverter_receiver,
-            set_power_result=set_power_result_receiver,
-        )
+        battery = battery_receiver
+        battery_timer = self._battery.data_recv_timer
+        inverter_timer = self._inverter.data_recv_timer
+        inverter = inverter_receiver
+        set_power_result = set_power_result_receiver
 
         while True:
             try:
-                while await self._select.ready():
-                    new_status = self._update_status(self._select)
+                async for selected in select(
+                    battery,
+                    battery_timer,
+                    inverter_timer,
+                    inverter,
+                    set_power_result,
+                ):
+                    new_status = None
+
+                    if selected_from(selected, battery):
+                        self._handle_status_battery(selected.value)
+
+                    elif selected_from(selected, inverter):
+                        self._handle_status_inverter(selected.value)
+
+                    elif selected_from(selected, set_power_result):
+                        self._handle_status_set_power_result(selected.value)
+
+                    elif selected_from(selected, battery_timer):
+                        if (
+                            datetime.now(tz=timezone.utc)
+                            - self._battery.last_msg_timestamp
+                        ) < timedelta(seconds=self._max_data_age):
+                            # This means that we have received data from the battery
+                            # since the timer triggered, but the timer event arrived
+                            # late, so we can ignore it.
+                            continue
+                        self._handle_status_battery_timer()
+
+                    elif selected_from(selected, inverter_timer):
+                        if (
+                            datetime.now(tz=timezone.utc)
+                            - self._inverter.last_msg_timestamp
+                        ) < timedelta(seconds=self._max_data_age):
+                            # This means that we have received data from the inverter
+                            # since the timer triggered, but the timer event arrived
+                            # late, so we can ignore it.
+                            continue
+                        self._handle_status_inverter_timer()
+
+                    else:
+                        _logger.error("Unknown message returned from select")
+
+                    new_status = self._get_new_status_if_changed()
 
                     if new_status is not None:
                         await status_sender.send(new_status)
 
             except Exception as err:  # pylint: disable=broad-except
                 _logger.exception("BatteryStatusTracker crashed with error: %s", err)
 
-    def _update_status(self, select: Select) -> Optional[Status]:
-        if msg := select.battery:
-            self._battery.last_msg_correct = (
-                self._is_message_reliable(msg.inner)
-                and self._is_battery_state_correct(msg.inner)
-                and self._no_critical_error(msg.inner)
-                and self._is_capacity_present(msg.inner)
-            )
-            self._battery.last_msg_timestamp = msg.inner.timestamp
-            self._battery.data_recv_timer.reset()
-
-        elif msg := select.inverter:
-            self._inverter.last_msg_correct = (
-                self._is_message_reliable(msg.inner)
-                and self._is_inverter_state_correct(msg.inner)
-                and self._no_critical_error(msg.inner)
-            )
-            self._inverter.last_msg_timestamp = msg.inner.timestamp
-            self._inverter.data_recv_timer.reset()
-
-        elif msg := select.set_power_result:
-            result: SetPowerResult = msg.inner
-            if self.battery_id in result.succeed:
-                self._blocking_status.unblock()
-
-            elif (
-                self.battery_id in result.failed
-                and self._last_status != Status.NOT_WORKING
-            ):
-                duration = self._blocking_status.block()
-
-                if duration > 0:
-                    _logger.warning(
-                        "battery %d failed last response. block it for %f sec",
-                        self.battery_id,
-                        duration,
-                    )
-        elif msg := select.battery_timer:
-            if self._battery.last_msg_correct:
-                self._battery.last_msg_correct = False
-                _logger.warning(
-                    "Battery %d stopped sending data, last timestamp: %s",
-                    self._battery.component_id,
-                    self._battery.last_msg_timestamp,
-                )
-        elif msg := select.inverter_timer:
-            if self._inverter.last_msg_correct:
-                self._inverter.last_msg_correct = False
-                _logger.warning(
-                    "Inverter %d stopped sending data, last timestamp: %s",
-                    self._inverter.component_id,
-                    self._inverter.last_msg_timestamp,
-                )
-
-        else:
-            _logger.error("Unknown message returned from select")
-
-        current_status = self._get_current_status()
-        if self._last_status != current_status:
-            self._last_status = current_status
-            _logger.info(
-                "battery %d changed status %s",
-                self.battery_id,
-                str(self._last_status),
-            )
-            return current_status
-
-        return None
-
     def _get_current_status(self) -> Status:
         """Get current battery status.
 
         Returns:
             Battery status.
         """
         is_msg_correct = (
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/power_distributing.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/power_distributing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/request.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/request.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/actor/power_distributing/result.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/actor/power_distributing/result.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/config/_config.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/config/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Read and update config variables."""
 
 import logging
 from typing import Any, Dict, Optional, TypeVar
 
-from pydantic import ValidationError, parse_raw_as
+# pylint not finding parse_raw_as is a false positive
+from pydantic import ValidationError, parse_raw_as  # pylint: disable=no-name-in-module
 
 _logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 class Config:
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/__init__.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/_data_pipeline.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/_data_pipeline.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/_graph.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/_graph.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_client.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/client/_client.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_connection.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/client/_connection.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/client/_retry.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/client/_retry.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/__init__.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/component/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/component/_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,7 +135,9 @@
     CAPACITY = "capacity"
 
     POWER_LOWER_BOUND = "power_lower_bound"
     POWER_UPPER_BOUND = "power_upper_bound"
 
     ACTIVE_POWER_LOWER_BOUND = "active_power_lower_bound"
     ACTIVE_POWER_UPPER_BOUND = "active_power_upper_bound"
+
+    TEMPERATURE = "temperature"
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component_data.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/component/_component_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,16 @@
     """
 
     power_upper_bound: float
     """The maximum charge power, in Watts, represented in the passive sign convention.
         This will be a positive number, or zero if no charging is possible.
     """
 
-    temperature_max: float
-    """The maximum temperature of all the blocks in a battery, in Celcius (°C)."""
+    temperature: float
+    """The (average) temperature reported by the battery, in Celcius (°C)."""
 
     _relay_state: battery_pb.RelayState.ValueType
     """State of the battery relay."""
 
     _component_state: battery_pb.ComponentState.ValueType
     """State of the battery."""
 
@@ -168,15 +168,15 @@
             timestamp=raw.ts.ToDatetime(tzinfo=timezone.utc),
             soc=raw.battery.data.soc.avg,
             soc_lower_bound=raw.battery.data.soc.system_bounds.lower,
             soc_upper_bound=raw.battery.data.soc.system_bounds.upper,
             capacity=raw.battery.properties.capacity,
             power_lower_bound=raw.battery.data.dc.power.system_bounds.lower,
             power_upper_bound=raw.battery.data.dc.power.system_bounds.upper,
-            temperature_max=raw.battery.data.temperature.max,
+            temperature=raw.battery.data.temperature.avg,
             _relay_state=raw.battery.state.relay_state,
             _component_state=raw.battery.state.component_state,
             _errors=list(raw.battery.errors),
         )
         battery_data._set_raw(raw=raw)
         return battery_data
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/component/_component_states.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/component/_component_states.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/microgrid/connection_manager.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/microgrid/connection_manager.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/power/_distribution_algorithm.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/power/_distribution_algorithm.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/__init__.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,15 +34,24 @@
                                    now = 1970-01-01 00:00:32
     ```
 """
 
 from ._base_types import UNIX_EPOCH, Sample, Sample3Phase
 from ._moving_window import MovingWindow
 from ._periodic_feature_extractor import PeriodicFeatureExtractor
-from ._quantities import Current, Energy, Percentage, Power, Quantity, Voltage
+from ._quantities import (
+    Current,
+    Energy,
+    Frequency,
+    Percentage,
+    Power,
+    Quantity,
+    Temperature,
+    Voltage,
+)
 from ._resampling import ResamplerConfig
 
 __all__ = [
     "MovingWindow",
     "PeriodicFeatureExtractor",
     "ResamplerConfig",
     "Sample",
@@ -51,10 +60,12 @@
     #
     # Quantities
     #
     "Quantity",
     "Current",
     "Energy",
     "Power",
+    "Temperature",
     "Voltage",
+    "Frequency",
     "Percentage",
 ]
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_base_types.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_base_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,33 @@
 
 from __future__ import annotations
 
 import asyncio
 import logging
 from abc import ABC
 from collections import deque
-from datetime import datetime
-from math import isinf, isnan
 from typing import (
     Callable,
     Dict,
     Generic,
     List,
     Optional,
-    Set,
     Tuple,
     Type,
     TypeVar,
     Union,
     overload,
 )
 
 from frequenz.channels import Broadcast, Receiver
 
 from ..._internal._asyncio import cancel_and_await
 from .. import Sample, Sample3Phase
-from .._quantities import QuantityT
+from .._quantities import Quantity, QuantityT
+from ._formula_evaluator import FormulaEvaluator
 from ._formula_steps import (
     Adder,
     Averager,
     Clipper,
     ConstantValue,
     Divider,
     FormulaStep,
@@ -52,134 +50,14 @@
     "*": 2,
     "-": 3,
     "+": 4,
     ")": 5,
 }
 
 
-class FormulaEvaluator(Generic[QuantityT]):
-    """A post-fix formula evaluator that operates on `Sample` receivers."""
-
-    def __init__(
-        self,
-        name: str,
-        steps: List[FormulaStep],
-        metric_fetchers: Dict[str, MetricFetcher[QuantityT]],
-        create_method: Callable[[float], QuantityT],
-    ) -> None:
-        """Create a `FormulaEngine` instance.
-
-        Args:
-            name: A name for the formula.
-            steps: Steps for the engine to execute, in post-fix order.
-            metric_fetchers: Fetchers for each metric stream the formula depends on.
-            create_method: A method to generate the output `Sample` value with.  If the
-                formula is for generating power values, this would be
-                `Power.from_watts`, for example.
-        """
-        self._name = name
-        self._steps = steps
-        self._metric_fetchers: Dict[str, MetricFetcher[QuantityT]] = metric_fetchers
-        self._first_run = True
-        self._create_method: Callable[[float], QuantityT] = create_method
-
-    async def _synchronize_metric_timestamps(
-        self, metrics: Set[asyncio.Task[Optional[Sample[QuantityT]]]]
-    ) -> datetime:
-        """Synchronize the metric streams.
-
-        For synchronised streams like data from the `ComponentMetricsResamplingActor`,
-        this a call to this function is required only once, before the first set of
-        inputs are fetched.
-
-        Args:
-            metrics: The finished tasks from the first `fetch_next` calls to all the
-                `MetricFetcher`s.
-
-        Returns:
-            The timestamp of the latest metric value.
-
-        Raises:
-            RuntimeError: when some streams have no value, or when the synchronization
-                of timestamps fails.
-        """
-        metrics_by_ts: Dict[datetime, list[str]] = {}
-        for metric in metrics:
-            result = metric.result()
-            name = metric.get_name()
-            if result is None:
-                raise RuntimeError(f"Stream closed for component: {name}")
-            metrics_by_ts.setdefault(result.timestamp, []).append(name)
-        latest_ts = max(metrics_by_ts)
-
-        # fetch the metrics with non-latest timestamps again until we have the values
-        # for the same ts for all metrics.
-        for metric_ts, names in metrics_by_ts.items():
-            if metric_ts == latest_ts:
-                continue
-            while metric_ts < latest_ts:
-                for name in names:
-                    fetcher = self._metric_fetchers[name]
-                    next_val = await fetcher.fetch_next()
-                    assert next_val is not None
-                    metric_ts = next_val.timestamp
-            if metric_ts > latest_ts:
-                raise RuntimeError(
-                    "Unable to synchronize resampled metric timestamps, "
-                    f"for formula: {self._name}"
-                )
-        self._first_run = False
-        return latest_ts
-
-    async def apply(self) -> Sample[QuantityT]:
-        """Fetch the latest metrics, apply the formula once and return the result.
-
-        Returns:
-            The result of the formula.
-
-        Raises:
-            RuntimeError: if some samples didn't arrive, or if formula application
-                failed.
-        """
-        eval_stack: List[float] = []
-        ready_metrics, pending = await asyncio.wait(
-            [
-                asyncio.create_task(fetcher.fetch_next(), name=name)
-                for name, fetcher in self._metric_fetchers.items()
-            ],
-            return_when=asyncio.ALL_COMPLETED,
-        )
-
-        if pending or any(res.result() is None for res in iter(ready_metrics)):
-            raise RuntimeError(
-                f"Some resampled metrics didn't arrive, for formula: {self._name}"
-            )
-
-        if self._first_run:
-            metric_ts = await self._synchronize_metric_timestamps(ready_metrics)
-        else:
-            sample = next(iter(ready_metrics)).result()
-            assert sample is not None
-            metric_ts = sample.timestamp
-
-        for step in self._steps:
-            step.apply(eval_stack)
-
-        # if all steps were applied and the formula was correct, there should only be a
-        # single value in the evaluation stack, and that would be the formula result.
-        if len(eval_stack) != 1:
-            raise RuntimeError(f"Formula application failed: {self._name}")
-
-        res = eval_stack.pop()
-        if isnan(res) or isinf(res):
-            return Sample(metric_ts, None)
-
-        return Sample(metric_ts, self._create_method(res))
-
-
 _CompositionType = Union[
     "FormulaEngine",
     "HigherOrderFormulaBuilder",
     "FormulaEngine3Phase",
     "HigherOrderFormulaBuilder3Phase",
 ]
 
@@ -227,60 +105,60 @@
         """Stop a running formula engine."""
         if self._task is None:
             return
         await cancel_and_await(self._task)
 
     def __add__(
         self,
-        other: _GenericEngine | _GenericHigherOrderBuilder,
+        other: _GenericEngine | _GenericHigherOrderBuilder | QuantityT,
     ) -> _GenericHigherOrderBuilder:
         """Return a formula builder that adds (data in) `other` to `self`.
 
         Args:
             other: A formula receiver, or a formula builder instance corresponding to a
                 sub-expression.
 
         Returns:
             A formula builder that can take further expressions, or can be built
                 into a formula engine.
         """
         return self._higher_order_builder(self, self._create_method) + other  # type: ignore
 
     def __sub__(
-        self, other: _GenericEngine | _GenericHigherOrderBuilder
+        self, other: _GenericEngine | _GenericHigherOrderBuilder | QuantityT
     ) -> _GenericHigherOrderBuilder:
         """Return a formula builder that subtracts (data in) `other` from `self`.
 
         Args:
             other: A formula receiver, or a formula builder instance corresponding to a
                 sub-expression.
 
         Returns:
             A formula builder that can take further expressions, or can be built
                 into a formula engine.
         """
         return self._higher_order_builder(self, self._create_method) - other  # type: ignore
 
     def __mul__(
-        self, other: _GenericEngine | _GenericHigherOrderBuilder
+        self, other: _GenericEngine | _GenericHigherOrderBuilder | float
     ) -> _GenericHigherOrderBuilder:
         """Return a formula builder that multiplies (data in) `self` with `other`.
 
         Args:
             other: A formula receiver, or a formula builder instance corresponding to a
                 sub-expression.
 
         Returns:
             A formula builder that can take further expressions, or can be built
                 into a formula engine.
         """
         return self._higher_order_builder(self, self._create_method) * other  # type: ignore
 
     def __truediv__(
-        self, other: _GenericEngine | _GenericHigherOrderBuilder
+        self, other: _GenericEngine | _GenericHigherOrderBuilder | float
     ) -> _GenericHigherOrderBuilder:
         """Return a formula builder that divides (data in) `self` by `other`.
 
         Args:
             other: A formula receiver, or a formula builder instance corresponding to a
                 sub-expression.
 
@@ -321,14 +199,70 @@
         """
         self._higher_order_builder = HigherOrderFormulaBuilder
         self._name: str = builder.name
         self._builder: FormulaBuilder[QuantityT] = builder
         self._create_method = create_method
         self._channel: Broadcast[Sample[QuantityT]] = Broadcast(self._name)
 
+    @classmethod
+    def from_receiver(
+        cls,
+        name: str,
+        receiver: Receiver[Sample[QuantityT]],
+        create_method: Callable[[float], QuantityT],
+        nones_are_zeros: bool = False,
+    ) -> FormulaEngine[QuantityT]:
+        """
+        Create a formula engine from a receiver.
+
+        Can be used to compose a formula engine with a receiver. When composing
+        the new engine with other engines, make sure that receiver gets data
+        from the same resampler and that the `create_method`s match.
+
+        Example:
+            ```python
+            from frequenz.sdk import microgrid
+            from frequenz.sdk.timeseries import Power
+
+            async def run() -> None:
+                producer_power_engine = microgrid.logical_meter().producer_power
+                consumer_power_recv = (
+                    microgrid.logical_meter().consumer_power.new_receiver()
+                )
+
+                excess_power_recv = (
+                    (
+                        producer_power_engine
+                        + FormulaEngine.from_receiver(
+                            "consumer power",
+                            consumer_power_recv,
+                            Power.from_watts,
+                        )
+                    )
+                    .build("excess power")
+                    .new_receiver()
+                )
+
+            asyncio.run(run())
+            ```
+
+        Args:
+            receiver: A receiver that streams `Sample`s.
+            name: A name for the formula engine.
+            create_method: A method to generate the output `Sample` value with,
+                e.g. `Power.from_watts`.
+            nones_are_zeros: If `True`, `None` values in the receiver are treated as 0.
+
+        Returns:
+            A formula engine that streams the `Sample`s from the receiver.
+        """
+        builder = FormulaBuilder(name, create_method)
+        builder.push_metric(name, receiver, nones_are_zeros=nones_are_zeros)
+        return cls(builder, create_method)
+
     async def _run(self) -> None:
         await self._builder.subscribe()
         steps, metric_fetchers = self._builder.finalize()
         evaluator = FormulaEvaluator[QuantityT](
             self._name, steps, metric_fetchers, self._create_method
         )
         sender = self._channel.new_sender()
@@ -680,45 +614,62 @@
             create_method: A method to generate the output `Sample` value with.  If the
                 formula is for generating power values, this would be
                 `Power.from_watts`, for example.
         """
         self._steps: deque[
             tuple[
                 TokenType,
-                FormulaEngine[QuantityT] | FormulaEngine3Phase[QuantityT] | str,
+                FormulaEngine[QuantityT]
+                | FormulaEngine3Phase[QuantityT]
+                | QuantityT
+                | float
+                | str,
             ]
         ] = deque()
         self._steps.append((TokenType.COMPONENT_METRIC, engine))
         self._create_method: Callable[[float], QuantityT] = create_method
 
     @overload
     def _push(
         self, oper: str, other: _CompositionType1Phase
     ) -> HigherOrderFormulaBuilder[QuantityT]:
         ...
 
     @overload
     def _push(
-        self, oper: str, other: _CompositionType3Phase
+        self, oper: str, other: _CompositionType3Phase | QuantityT | float
     ) -> HigherOrderFormulaBuilder3Phase[QuantityT]:
         ...
 
     def _push(
-        self, oper: str, other: _CompositionType
+        self, oper: str, other: _CompositionType | QuantityT | float
     ) -> (
         HigherOrderFormulaBuilder[QuantityT]
         | HigherOrderFormulaBuilder3Phase[QuantityT]
     ):
         self._steps.appendleft((TokenType.OPER, "("))
         self._steps.append((TokenType.OPER, ")"))
         self._steps.append((TokenType.OPER, oper))
 
         # pylint: disable=protected-access
         if isinstance(other, (FormulaEngine, FormulaEngine3Phase)):
             self._steps.append((TokenType.COMPONENT_METRIC, other))
+        elif isinstance(other, (Quantity, float)):
+            match oper:
+                case "+" | "-":
+                    if not isinstance(other, Quantity):
+                        raise RuntimeError(
+                            f"A Quantity must be provided for addition or subtraction to {other}"
+                        )
+                case "*" | "/":
+                    if not isinstance(other, (float, int)):
+                        raise RuntimeError(
+                            f"A float must be provided for scalar multiplication to {other}"
+                        )
+            self._steps.append((TokenType.CONSTANT, other))
         elif isinstance(other, _BaseHOFormulaBuilder):
             self._steps.append((TokenType.OPER, "("))
             self._steps.extend(other._steps)
             self._steps.append((TokenType.OPER, ")"))
         # pylint: enable=protected-access
         else:
             raise RuntimeError(f"Can't build a formula from: {other}")
@@ -731,20 +682,20 @@
     def __add__(
         self, other: _CompositionType1Phase
     ) -> HigherOrderFormulaBuilder[QuantityT]:
         ...
 
     @overload
     def __add__(
-        self, other: _CompositionType3Phase
+        self, other: _CompositionType3Phase | QuantityT
     ) -> HigherOrderFormulaBuilder3Phase[QuantityT]:
         ...
 
     def __add__(
-        self, other: _CompositionType
+        self, other: _CompositionType | QuantityT
     ) -> (
         HigherOrderFormulaBuilder[QuantityT]
         | HigherOrderFormulaBuilder3Phase[QuantityT]
     ):
         """Return a formula builder that adds (data in) `other` to `self`.
 
         Args:
@@ -761,21 +712,21 @@
     def __sub__(
         self, other: _CompositionType1Phase
     ) -> HigherOrderFormulaBuilder[QuantityT]:
         ...
 
     @overload
     def __sub__(
-        self, other: _CompositionType3Phase
+        self, other: _CompositionType3Phase | QuantityT
     ) -> HigherOrderFormulaBuilder3Phase[QuantityT]:
         ...
 
     def __sub__(
         self,
-        other: _CompositionType,
+        other: _CompositionType | QuantityT,
     ) -> (
         HigherOrderFormulaBuilder[QuantityT]
         | HigherOrderFormulaBuilder3Phase[QuantityT]
     ):
         """Return a formula builder that subtracts (data in) `other` from `self`.
 
         Args:
@@ -792,21 +743,21 @@
     def __mul__(
         self, other: _CompositionType1Phase
     ) -> HigherOrderFormulaBuilder[QuantityT]:
         ...
 
     @overload
     def __mul__(
-        self, other: _CompositionType3Phase
+        self, other: _CompositionType3Phase | float
     ) -> HigherOrderFormulaBuilder3Phase[QuantityT]:
         ...
 
     def __mul__(
         self,
-        other: _CompositionType,
+        other: _CompositionType | float,
     ) -> (
         HigherOrderFormulaBuilder[QuantityT]
         | HigherOrderFormulaBuilder3Phase[QuantityT]
     ):
         """Return a formula builder that multiplies (data in) `self` with `other`.
 
         Args:
@@ -823,21 +774,21 @@
     def __truediv__(
         self, other: _CompositionType1Phase
     ) -> HigherOrderFormulaBuilder[QuantityT]:
         ...
 
     @overload
     def __truediv__(
-        self, other: _CompositionType3Phase
+        self, other: _CompositionType3Phase | float
     ) -> HigherOrderFormulaBuilder3Phase[QuantityT]:
         ...
 
     def __truediv__(
         self,
-        other: _CompositionType,
+        other: _CompositionType | float,
     ) -> (
         HigherOrderFormulaBuilder[QuantityT]
         | HigherOrderFormulaBuilder3Phase[QuantityT]
     ):
         """Return a formula builder that divides (data in) `self` by `other`.
 
         Args:
@@ -875,14 +826,19 @@
                     value._name,  # pylint: disable=protected-access
                     value.new_receiver(),
                     nones_are_zeros,
                 )
             elif typ == TokenType.OPER:
                 assert isinstance(value, str)
                 builder.push_oper(value)
+            elif typ == TokenType.CONSTANT:
+                assert isinstance(value, (Quantity, float))
+                builder.push_constant(
+                    value.base_value if isinstance(value, Quantity) else value
+                )
         return builder.build()
 
 
 class HigherOrderFormulaBuilder3Phase(
     Generic[QuantityT], _BaseHOFormulaBuilder[QuantityT]
 ):
     """A specialization of the _BaseHOFormulaBuilder for `FormulaReceiver3Phase`."""
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_producer_power_formula.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_producer_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Steps for building formula engines with."""
 
 from __future__ import annotations
 
+import math
 from abc import ABC, abstractmethod
 from typing import Generic, List, Optional
 
 from frequenz.channels import Receiver
 
 from .. import Sample
 from .._quantities import QuantityT
@@ -322,10 +323,10 @@
             raise RuntimeError("No next value available to append.")
 
         next_value = self._next_value.value
         if next_value is None or next_value.isnan() or next_value.isinf():
             if self._nones_are_zeros:
                 eval_stack.append(0.0)
             else:
-                eval_stack.append(float("NaN"))
+                eval_stack.append(math.nan)
         else:
             eval_stack.append(next_value.base_value)
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,16 @@
         return None
 
 
 class TokenType(Enum):
     """Represents the types of tokens the Tokenizer can return."""
 
     COMPONENT_METRIC = 0
-    OPER = 1
+    CONSTANT = 1
+    OPER = 2
 
 
 @dataclass
 class Token:
     """Represents a Token returned by the Tokenizer."""
 
     type: TokenType
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_moving_window.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_moving_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,14 +301,16 @@
             IndexError: when requesting an out of range timestamp or index
             TypeError: when the key is not a datetime or slice object.
 
         Returns:
             A float if the key is a number or a timestamp.
             an numpy array if the key is a slice.
         """
+        if len(self._buffer) == 0:
+            raise IndexError("The buffer is empty.")
         if isinstance(key, slice):
             if isinstance(key.start, int) or isinstance(key.stop, int):
                 if key.start is None or key.stop is None:
                     key = slice(slice(key.start, key.stop).indices(self.__len__()))
             elif isinstance(key.start, datetime) or isinstance(key.stop, datetime):
                 if key.start is None:
                     key = slice(self._buffer.time_bound_oldest, key.stop)
@@ -323,14 +325,15 @@
                 return self._buffer.window(key.start, key.stop)
             if isinstance(key.start, int) and isinstance(key.stop, int):
                 return self._buffer[key]
         elif isinstance(key, datetime):
             _logger.debug("Returning value at time %s ", key)
             return self._buffer[self._buffer.datetime_to_index(key)]
         elif isinstance(key, SupportsIndex):
+            _logger.debug("Returning value at index %s ", key)
             return self._buffer[key]
 
         raise TypeError(
             "Key has to be either a timestamp or an integer "
             "or a slice of timestamps or integers"
         )
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 
     Note:
         When constructing a `PeriodicFeatureExtractor` object the
         `MovingWindow` size has to be a integer multiple of the period.
 
     Example:
         ```python
+        from frequenz.sdk import microgrid
         from datetime import datetime, timedelta, timezone
 
         moving_window = MovingWindow(
             size=timedelta(days=35),
             resampled_data_recv=microgrid.logical_meter().grid_power.new_receiver(),
             input_sampling_period=timedelta(seconds=1),
         )
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_quantities.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_quantities.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Types for holding quantities with units."""
 
+# pylint: disable=too-many-lines
+
 from __future__ import annotations
 
 import math
 from datetime import timedelta
 from typing import Any, NoReturn, Self, TypeVar, overload
 
 QuantityT = TypeVar(
-    "QuantityT", "Quantity", "Power", "Current", "Voltage", "Energy", "Percentage"
+    "QuantityT",
+    "Quantity",
+    "Power",
+    "Current",
+    "Voltage",
+    "Energy",
+    "Frequency",
+    "Percentage",
+    "Temperature",
 )
 
 
 class Quantity:
-    """A quantity with a unit."""
+    """A quantity with a unit.
+
+    Quantities try to behave like float and are also immutable.
+    """
 
     _base_value: float
     """The value of this quantity in the base unit."""
 
     _exponent_unit_map: dict[int, str] | None = None
     """A mapping from the exponent of the base unit to the unit symbol.
 
@@ -49,14 +62,38 @@
                 (exponent 0).
         """
         if not 0 in exponent_unit_map:
             raise ValueError("Expected a base unit for the type (for exponent 0)")
         cls._exponent_unit_map = exponent_unit_map
         super().__init_subclass__()
 
+    _zero_cache: dict[type, Quantity] = {}
+    """Cache for zero singletons.
+
+    This is a workaround for mypy getting confused when using @functools.cache and
+    @classmethod combined with returning Self. It believes the resulting type of this
+    method is Self and complains that members of the actual class don't exist in Self,
+    so we need to implement the cache ourselves.
+    """
+
+    @classmethod
+    def zero(cls) -> Self:
+        """Return a quantity with value 0.
+
+        Returns:
+            A quantity with value 0.
+        """
+        _zero = cls._zero_cache.get(cls, None)
+        if _zero is None:
+            _zero = cls.__new__(cls)
+            _zero._base_value = 0
+            cls._zero_cache[cls] = _zero
+        assert isinstance(_zero, cls)
+        return _zero
+
     @property
     def base_value(self) -> float:
         """Return the value of this quantity in the base unit.
 
         Returns:
             The value of this quantity in the base unit.
         """
@@ -87,21 +124,31 @@
         """Return whether this quantity is infinite.
 
         Returns:
             Whether this quantity is infinite.
         """
         return math.isinf(self._base_value)
 
-    def __hash__(self) -> int:
-        """Return a hash of this object.
+    def isclose(self, other: Self, rel_tol: float = 1e-9, abs_tol: float = 0.0) -> bool:
+        """Return whether this quantity is close to another.
+
+        Args:
+            other: The quantity to compare to.
+            rel_tol: The relative tolerance.
+            abs_tol: The absolute tolerance.
 
         Returns:
-            A hash of this object.
+            Whether this quantity is close to another.
         """
-        return hash((type(self), self._base_value))
+        return math.isclose(
+            self._base_value,
+            other._base_value,  # pylint: disable=protected-access
+            rel_tol=rel_tol,
+            abs_tol=abs_tol,
+        )
 
     def __repr__(self) -> str:
         """Return a representation of this quantity.
 
         Returns:
             A representation of this quantity.
         """
@@ -159,14 +206,17 @@
                 keep_trailing_zeros = True
             precision = int(fspec_parts[1])
         else:
             precision = 3
         if not self._exponent_unit_map:
             return f"{self._base_value:.{precision}f}"
 
+        if math.isinf(self._base_value) or math.isnan(self._base_value):
+            return f"{self._base_value} {self._exponent_unit_map[0]}"
+
         abs_value = abs(self._base_value)
         exponent = math.floor(math.log10(abs_value)) if abs_value else 0
         unit_place = exponent - exponent % 3
         if unit_place < min(self._exponent_unit_map):
             unit = self._exponent_unit_map[min(self._exponent_unit_map.keys())]
             unit_place = min(self._exponent_unit_map)
         elif unit_place > max(self._exponent_unit_map):
@@ -207,14 +257,30 @@
         """
         if not type(other) is type(self):
             return NotImplemented
         difference = type(self).__new__(type(self))
         difference._base_value = self._base_value - other._base_value
         return difference
 
+    def __mul__(self, percent: Percentage) -> Self:
+        """Return the product of this quantity and a percentage.
+
+        Args:
+            percent: The percentage.
+
+        Returns:
+            The product of this quantity and a percentage.
+        """
+        if not isinstance(percent, Percentage):
+            return NotImplemented
+
+        product = type(self).__new__(type(self))
+        product._base_value = self._base_value * percent.as_fraction()
+        return product
+
     def __gt__(self, other: Self) -> bool:
         """Return whether this quantity is greater than another.
 
         Args:
             other: The other quantity.
 
         Returns:
@@ -276,14 +342,34 @@
             return NotImplemented
         # The above check ensures that both quantities are the exact same type, because
         # `isinstance` returns true for subclasses and superclasses.  But the above check
         # doesn't help mypy identify the type of other,  so the below line is necessary.
         assert isinstance(other, self.__class__)
         return self._base_value == other._base_value
 
+    def __neg__(self) -> Self:
+        """Return the negation of this quantity.
+
+        Returns:
+            The negation of this quantity.
+        """
+        negation = type(self).__new__(type(self))
+        negation._base_value = -self._base_value
+        return negation
+
+    def __abs__(self) -> Self:
+        """Return the absolute value of this quantity.
+
+        Returns:
+            The absolute value of this quantity.
+        """
+        absolute = type(self).__new__(type(self))
+        absolute._base_value = abs(self._base_value)
+        return absolute
+
 
 class _NoDefaultConstructible(type):
     """A metaclass that disables the default constructor."""
 
     def __call__(cls, *_args: Any, **_kwargs: Any) -> NoReturn:
         """Raise a TypeError when the default constructor is called.
 
@@ -297,25 +383,66 @@
         raise TypeError(
             "Use of default constructor NOT allowed for "
             f"{cls.__module__}.{cls.__qualname__}, "
             f"use one of the `{cls.__name__}.from_*()` methods instead."
         )
 
 
+class Temperature(
+    Quantity,
+    metaclass=_NoDefaultConstructible,
+    exponent_unit_map={
+        0: "°C",
+    },
+):
+    """A temperature quantity (in degrees Celsius)."""
+
+    @classmethod
+    def from_celsius(cls, value: float) -> Self:
+        """Initialize a new temperature quantity.
+
+        Args:
+            value: The temperature in degrees Celsius.
+
+        Returns:
+            A new temperature quantity.
+        """
+        power = cls.__new__(cls)
+        power._base_value = value
+        return power
+
+    def as_celsius(self) -> float:
+        """Return the temperature in degrees Celsius.
+
+        Returns:
+            The temperature in degrees Celsius.
+        """
+        return self._base_value
+
+
 class Power(
     Quantity,
     metaclass=_NoDefaultConstructible,
     exponent_unit_map={
         -3: "mW",
         0: "W",
         3: "kW",
         6: "MW",
     },
 ):
-    """A power quantity."""
+    """A power quantity.
+
+    Objects of this type are wrappers around `float` values and are immutable.
+
+    The constructors accept a single `float` value, the `as_*()` methods return a
+    `float` value, and each of the arithmetic operators supported by this type are
+    actually implemented using floating-point arithmetic.
+
+    So all considerations about floating-point arithmetic apply to this type as well.
+    """
 
     @classmethod
     def from_watts(cls, watts: float) -> Self:
         """Initialize a new power quantity.
 
         Args:
             watts: The power in watts.
@@ -389,26 +516,50 @@
         """Return the power in megawatts.
 
         Returns:
             The power in megawatts.
         """
         return self._base_value / 1e6
 
-    def __mul__(self, duration: timedelta) -> Energy:
+    @overload  # type: ignore
+    def __mul__(self, other: Percentage) -> Self:
+        """Return a power from multiplying this power by the given percentage.
+
+        Args:
+            other: The percentage to multiply by.
+        """
+
+    @overload
+    def __mul__(self, other: timedelta) -> Energy:
         """Return an energy from multiplying this power by the given duration.
 
         Args:
-            duration: The duration to multiply by.
+            other: The duration to multiply by.
+        """
+
+    def __mul__(self, other: Percentage | timedelta) -> Self | Energy:
+        """Return a power or energy from multiplying this power by the given value.
+
+        Args:
+            other: The percentage or duration to multiply by.
 
         Returns:
-            An energy from multiplying this power by the given duration.
+            A power or energy.
+
+        Raises:
+            TypeError: If the given value is not a percentage or duration.
         """
-        return Energy.from_watt_hours(
-            self._base_value * duration.total_seconds() / 3600.0
-        )
+        if isinstance(other, Percentage):
+            return super().__mul__(other)
+        if isinstance(other, timedelta):
+            return Energy.from_watt_hours(
+                self._base_value * other.total_seconds() / 3600.0
+            )
+
+        return NotImplemented
 
     @overload
     def __truediv__(self, other: Current) -> Voltage:
         """Return a voltage from dividing this power by the given current.
 
         Args:
             other: The current to divide by.
@@ -447,15 +598,24 @@
     Quantity,
     metaclass=_NoDefaultConstructible,
     exponent_unit_map={
         -3: "mA",
         0: "A",
     },
 ):
-    """A current quantity."""
+    """A current quantity.
+
+    Objects of this type are wrappers around `float` values and are immutable.
+
+    The constructors accept a single `float` value, the `as_*()` methods return a
+    `float` value, and each of the arithmetic operators supported by this type are
+    actually implemented using floating-point arithmetic.
+
+    So all considerations about floating-point arithmetic apply to this type as well.
+    """
 
     @classmethod
     def from_amperes(cls, amperes: float) -> Self:
         """Initialize a new current quantity.
 
         Args:
             amperes: The current in amperes.
@@ -493,32 +653,65 @@
         """Return the current in milliamperes.
 
         Returns:
             The current in milliamperes.
         """
         return self._base_value * 1e3
 
-    def __mul__(self, voltage: Voltage) -> Power:
+    @overload  # type: ignore
+    def __mul__(self, other: Percentage) -> Self:
+        """Return a power from multiplying this power by the given percentage.
+
+        Args:
+            other: The percentage to multiply by.
+        """
+
+    @overload
+    def __mul__(self, other: Voltage) -> Power:
         """Multiply the current by a voltage to get a power.
 
         Args:
-            voltage: The voltage.
+            other: The voltage.
+        """
+
+    def __mul__(self, other: Percentage | Voltage) -> Self | Power:
+        """Return a current or power from multiplying this current by the given value.
+
+        Args:
+            other: The percentage or voltage to multiply by.
 
         Returns:
-            The power.
+            A current or power.
+
+        Raises:
+            TypeError: If the given value is not a percentage or voltage.
         """
-        return Power.from_watts(self._base_value * voltage._base_value)
+        if isinstance(other, Percentage):
+            return super().__mul__(other)
+        if isinstance(other, Voltage):
+            return Power.from_watts(self._base_value * other._base_value)
+
+        return NotImplemented
 
 
 class Voltage(
     Quantity,
     metaclass=_NoDefaultConstructible,
     exponent_unit_map={0: "V", -3: "mV", 3: "kV"},
 ):
-    """A voltage quantity."""
+    """A voltage quantity.
+
+    Objects of this type are wrappers around `float` values and are immutable.
+
+    The constructors accept a single `float` value, the `as_*()` methods return a
+    `float` value, and each of the arithmetic operators supported by this type are
+    actually implemented using floating-point arithmetic.
+
+    So all considerations about floating-point arithmetic apply to this type as well.
+    """
 
     @classmethod
     def from_volts(cls, volts: float) -> Self:
         """Initialize a new voltage quantity.
 
         Args:
             volts: The voltage in volts.
@@ -578,36 +771,69 @@
         """Return the voltage in kilovolts.
 
         Returns:
             The voltage in kilovolts.
         """
         return self._base_value / 1e3
 
-    def __mul__(self, current: Current) -> Power:
+    @overload  # type: ignore
+    def __mul__(self, other: Percentage) -> Self:
+        """Return a power from multiplying this power by the given percentage.
+
+        Args:
+            other: The percentage to multiply by.
+        """
+
+    @overload
+    def __mul__(self, other: Current) -> Power:
         """Multiply the voltage by the current to get the power.
 
         Args:
-            current: The current to multiply the voltage with.
+            other: The current to multiply the voltage with.
+        """
+
+    def __mul__(self, other: Percentage | Current) -> Self | Power:
+        """Return a voltage or power from multiplying this voltage by the given value.
+
+        Args:
+            other: The percentage or current to multiply by.
 
         Returns:
-            The calculated power.
+            The calculated voltage or power.
+
+        Raises:
+            TypeError: If the given value is not a percentage or current.
         """
-        return Power.from_watts(self._base_value * current._base_value)
+        if isinstance(other, Percentage):
+            return super().__mul__(other)
+        if isinstance(other, Current):
+            return Power.from_watts(self._base_value * other._base_value)
+
+        return NotImplemented
 
 
 class Energy(
     Quantity,
     metaclass=_NoDefaultConstructible,
     exponent_unit_map={
         0: "Wh",
         3: "kWh",
         6: "MWh",
     },
 ):
-    """An energy quantity."""
+    """An energy quantity.
+
+    Objects of this type are wrappers around `float` values and are immutable.
+
+    The constructors accept a single `float` value, the `as_*()` methods return a
+    `float` value, and each of the arithmetic operators supported by this type are
+    actually implemented using floating-point arithmetic.
+
+    So all considerations about floating-point arithmetic apply to this type as well.
+    """
 
     @classmethod
     def from_watt_hours(cls, watt_hours: float) -> Self:
         """Initialize a new energy quantity.
 
         Args:
             watt_hours: The energy in watt hours.
@@ -704,20 +930,142 @@
         if isinstance(other, Power):
             return timedelta(seconds=(self._base_value / other._base_value) * 3600.0)
         raise TypeError(
             f"unsupported operand type(s) for /: '{type(self)}' and '{type(other)}'"
         )
 
 
+class Frequency(
+    Quantity,
+    metaclass=_NoDefaultConstructible,
+    exponent_unit_map={0: "Hz", 3: "kHz", 6: "MHz", 9: "GHz"},
+):
+    """A frequency quantity.
+
+    Objects of this type are wrappers around `float` values and are immutable.
+
+    The constructors accept a single `float` value, the `as_*()` methods return a
+    `float` value, and each of the arithmetic operators supported by this type are
+    actually implemented using floating-point arithmetic.
+
+    So all considerations about floating-point arithmetic apply to this type as well.
+    """
+
+    @classmethod
+    def from_hertz(cls, hertz: float) -> Self:
+        """Initialize a new frequency quantity.
+
+        Args:
+            hertz: The frequency in hertz.
+
+        Returns:
+            A new frequency quantity.
+        """
+        frequency = cls.__new__(cls)
+        frequency._base_value = hertz
+        return frequency
+
+    @classmethod
+    def from_kilohertz(cls, kilohertz: float) -> Self:
+        """Initialize a new frequency quantity.
+
+        Args:
+            kilohertz: The frequency in kilohertz.
+
+        Returns:
+            A new frequency quantity.
+        """
+        frequency = cls.__new__(cls)
+        frequency._base_value = kilohertz * 10**3
+        return frequency
+
+    @classmethod
+    def from_megahertz(cls, megahertz: float) -> Self:
+        """Initialize a new frequency quantity.
+
+        Args:
+            megahertz: The frequency in megahertz.
+
+        Returns:
+            A new frequency quantity.
+        """
+        frequency = cls.__new__(cls)
+        frequency._base_value = megahertz * 10**6
+        return frequency
+
+    @classmethod
+    def from_gigahertz(cls, gigahertz: float) -> Self:
+        """Initialize a new frequency quantity.
+
+        Args:
+            gigahertz: The frequency in gigahertz.
+
+        Returns:
+            A new frequency quantity.
+        """
+        frequency = cls.__new__(cls)
+        frequency._base_value = gigahertz * 10**9
+        return frequency
+
+    def as_hertz(self) -> float:
+        """Return the frequency in hertz.
+
+        Returns:
+            The frequency in hertz.
+        """
+        return self._base_value
+
+    def as_kilohertz(self) -> float:
+        """Return the frequency in kilohertz.
+
+        Returns:
+            The frequency in kilohertz.
+        """
+        return self._base_value / 1e3
+
+    def as_megahertz(self) -> float:
+        """Return the frequency in megahertz.
+
+        Returns:
+            The frequency in megahertz.
+        """
+        return self._base_value / 1e6
+
+    def as_gigahertz(self) -> float:
+        """Return the frequency in gigahertz.
+
+        Returns:
+            The frequency in gigahertz.
+        """
+        return self._base_value / 1e9
+
+    def period(self) -> timedelta:
+        """Return the period of the frequency.
+
+        Returns:
+            The period of the frequency.
+        """
+        return timedelta(seconds=1.0 / self._base_value)
+
+
 class Percentage(
     Quantity,
     metaclass=_NoDefaultConstructible,
     exponent_unit_map={0: "%"},
 ):
-    """A percentage quantity."""
+    """A percentage quantity.
+
+    Objects of this type are wrappers around `float` values and are immutable.
+
+    The constructors accept a single `float` value, the `as_*()` methods return a
+    `float` value, and each of the arithmetic operators supported by this type are
+    actually implemented using floating-point arithmetic.
+
+    So all considerations about floating-point arithmetic apply to this type as well.
+    """
 
     @classmethod
     def from_percent(cls, percent: float) -> Self:
         """Initialize a new percentage quantity from a percent value.
 
         Args:
             percent: The percent value, normally in the 0.0-100.0 range.
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_resampling.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_resampling.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_methods.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/_methods.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Set
 from datetime import datetime, timezone
 from typing import Generic, Iterable, TypeVar
 
 from ...microgrid import connection_manager
 from ...microgrid.component import ComponentCategory, ComponentMetricId, InverterType
-from ...timeseries import Energy, Percentage, Sample
+from ...timeseries import Energy, Percentage, Sample, Temperature
 from ._component_metrics import ComponentMetricsData
 from ._result_types import Bound, PowerMetrics
 
 _logger = logging.getLogger(__name__)
 _MIN_TIMESTAMP = datetime.min.replace(tzinfo=timezone.utc)
 
 
@@ -55,15 +55,15 @@
         else:
             bat_inv_map[battery_id] = inverter_id
     return bat_inv_map
 
 
 # Formula output types class have no common interface
 # Print all possible types here.
-T = TypeVar("T", Sample[Percentage], Sample[Energy], PowerMetrics)
+T = TypeVar("T", Sample[Percentage], Sample[Energy], PowerMetrics, Sample[Temperature])
 
 
 class MetricCalculator(ABC, Generic[T]):
     """Define how to calculate high level metrics from many components data.
 
     It specifies:
         * what components and metrics its needs to calculate the results,
@@ -230,14 +230,101 @@
         return (
             None
             if timestamp == _MIN_TIMESTAMP
             else Sample[Energy](timestamp, Energy.from_watt_hours(total_capacity))
         )
 
 
+class TemperatureCalculator(MetricCalculator[Sample[Temperature]]):
+    """Define how to calculate temperature metrics."""
+
+    def __init__(self, batteries: Set[int]) -> None:
+        """Create class instance.
+
+        Args:
+            batteries: What batteries should be used for calculation.
+        """
+        super().__init__(batteries)
+
+        self._metrics = [
+            ComponentMetricId.TEMPERATURE,
+        ]
+
+    @classmethod
+    def name(cls) -> str:
+        """Return name of the calculator.
+
+        Returns:
+            Name of the calculator
+        """
+        return "temperature"
+
+    @property
+    def battery_metrics(self) -> Mapping[int, list[ComponentMetricId]]:
+        """Return what metrics are needed for each battery.
+
+        Returns:
+            Map between battery id and set of required metrics id.
+        """
+        return {bid: self._metrics for bid in self._batteries}
+
+    @property
+    def inverter_metrics(self) -> Mapping[int, list[ComponentMetricId]]:
+        """Return what metrics are needed for each inverter.
+
+        Returns:
+            Map between inverter id and set of required metrics id.
+        """
+        return {}
+
+    def calculate(
+        self,
+        metrics_data: dict[int, ComponentMetricsData],
+        working_batteries: set[int],
+    ) -> Sample[Temperature] | None:
+        """Aggregate the metrics_data and calculate high level metric for temperature.
+
+        Missing components will be ignored. Formula will be calculated for all
+        working batteries that are in metrics_data.
+
+        Args:
+            metrics_data: Components metrics data, that should be used to calculate the
+                result.
+            working_batteries: working batteries. These batteries will be used
+                to calculate the result. It should be subset of the batteries given in a
+                constructor.
+
+        Returns:
+            High level metric calculated from the given metrics.
+            Return None if there are no component metrics.
+        """
+        timestamp = _MIN_TIMESTAMP
+        temperature_sum: float = 0.0
+        temperature_count: int = 0
+        for battery_id in working_batteries:
+            if battery_id not in metrics_data:
+                continue
+            metrics = metrics_data[battery_id]
+            temperature = metrics.get(ComponentMetricId.TEMPERATURE)
+            if temperature is None:
+                continue
+            timestamp = max(timestamp, metrics.timestamp)
+            temperature_sum += temperature
+            temperature_count += 1
+        if timestamp == _MIN_TIMESTAMP:
+            return None
+
+        temperature_avg = temperature_sum / temperature_count
+
+        return Sample[Temperature](
+            timestamp=timestamp,
+            value=Temperature.from_celsius(value=temperature_avg),
+        )
+
+
 class SoCCalculator(MetricCalculator[Sample[Percentage]]):
     """Define how to calculate SoC metrics."""
 
     def __init__(self, batteries: Set[int]) -> None:
         """Create class instance.
 
         Args:
@@ -333,15 +420,16 @@
             # gets cancelled out later.
             #
             # Therefore, the variables are named with a `_x100` suffix.
             usable_capacity_x100 = capacity * (soc_upper_bound - soc_lower_bound)
             soc_scaled = (
                 (soc - soc_lower_bound) / (soc_upper_bound - soc_lower_bound) * 100
             )
-            soc_scaled = max(soc_scaled, 0)
+            # we are clamping here because the SoC might be out of bounds
+            soc_scaled = min(max(soc_scaled, 0), 100)
             timestamp = max(timestamp, metrics.timestamp)
             used_capacity_x100 += usable_capacity_x100 * soc_scaled
             total_capacity_x100 += usable_capacity_x100
 
         if timestamp == _MIN_TIMESTAMP:
             return None
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/_result_types.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/_result_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,22 @@
 from ...timeseries import Sample
 from .._formula_engine import FormulaEngine, FormulaEnginePool
 from .._formula_engine._formula_generators import (
     BatteryPowerFormula,
     FormulaGeneratorConfig,
     FormulaType,
 )
-from .._quantities import Energy, Percentage, Power
+from .._quantities import Energy, Percentage, Power, Temperature
 from ._methods import MetricAggregator, SendOnUpdate
-from ._metric_calculator import CapacityCalculator, PowerBoundsCalculator, SoCCalculator
+from ._metric_calculator import (
+    CapacityCalculator,
+    PowerBoundsCalculator,
+    SoCCalculator,
+    TemperatureCalculator,
+)
 from ._result_types import PowerMetrics
 
 
 class BatteryPool:
     """Calculate high level metrics for a pool of the batteries.
 
     BatterPool accepts subset of the battery ids and provides methods methods for
@@ -116,14 +121,17 @@
 
         Power values need to follow the Passive Sign Convention (PSC). That is, positive
         values indicate charge power and negative values indicate discharge power.
 
         When not using the Passive Sign Convention, the `charge` and `discharge` methods
         might be more convenient.
 
+        The result of the request can be accessed using the receiver returned from
+        the `power_distribution_results` method.
+
         Args:
             power: The power to set for the batteries in the pool.
             adjust_power: If True, the power will be adjusted to fit the power bounds,
                 if necessary. If False, then power requests outside the bounds will be
                 rejected.
             request_timeout: The timeout for the request.
             include_broken_batteries: if True, the power will be set for all batteries
@@ -154,14 +162,17 @@
         """Set the given charge power for the batteries in the pool.
 
         Power values need to be positive values, indicating charge power.
 
         When using the Passive Sign Convention, the `set_power` method might be more
         convenient.
 
+        The result of the request can be accessed using the receiver returned from
+        the `power_distribution_results` method.
+
         Args:
             power: Unsigned charge power to set for the batteries in the pool.
             adjust_power: If True, the power will be adjusted to fit the power bounds,
                 if necessary. If False, then power requests outside the bounds will be
                 rejected.
             request_timeout: The timeout for the request.
             include_broken_batteries: if True, the power will be set for all batteries
@@ -198,14 +209,17 @@
         """Set the given discharge power for the batteries in the pool.
 
         Power values need to be positive values, indicating discharge power.
 
         When using the Passive Sign Convention, the `set_power` method might be more
         convenient.
 
+        The result of the request can be accessed using the receiver returned from
+        the `power_distribution_results` method.
+
         Args:
             power: Unsigned discharge power to set for the batteries in the pool.
             adjust_power: If True, the power will be adjusted to fit the power bounds,
                 if necessary. If False, then power requests outside the bounds will be
                 rejected.
             request_timeout: The timeout for the request.
             include_broken_batteries: if True, the power will be set for all batteries
@@ -329,24 +343,25 @@
         assert isinstance(engine, FormulaEngine)
         return engine
 
     @property
     def soc(self) -> MetricAggregator[Sample[Percentage]]:
         """Fetch the normalized average weighted-by-capacity SoC values for the pool.
 
-        The values are normalized to the 0-100% range.
+        The values are normalized to the 0-100% range and clamped if the SoC is out of
+        bounds.
 
         Average soc is calculated with the formula:
         ```
         working_batteries: Set[BatteryData] # working batteries from the battery pool
 
-        soc_scaled = max(
+        soc_scaled = min(max(
             0,
             (soc - soc_lower_bound) / (soc_upper_bound - soc_lower_bound) * 100,
-        )
+        ), 100)
         used_capacity = sum(
             battery.usable_capacity * battery.soc_scaled
             for battery in working_batteries
         )
         total_capacity = sum(battery.usable_capacity for battery in working_batteries)
         average_soc = used_capacity/total_capacity
         ```
@@ -370,14 +385,32 @@
                 working_batteries=self._working_batteries,
                 min_update_interval=self._min_update_interval,
             )
 
         return self._active_methods[method_name]
 
     @property
+    def temperature(self) -> MetricAggregator[Sample[Temperature]]:
+        """Fetch the average temperature of the batteries in the pool.
+
+        Returns:
+            A MetricAggregator that will calculate and stream the average temperature
+                of all batteries in the pool.
+        """
+        method_name = SendOnUpdate.name() + "_" + TemperatureCalculator.name()
+        if method_name not in self._active_methods:
+            calculator = TemperatureCalculator(self._batteries)
+            self._active_methods[method_name] = SendOnUpdate(
+                metric_calculator=calculator,
+                working_batteries=self._working_batteries,
+                min_update_interval=self._min_update_interval,
+            )
+        return self._active_methods[method_name]
+
+    @property
     def capacity(self) -> MetricAggregator[Sample[Energy]]:
         """Get receiver to receive new capacity metrics when they change.
 
         Calculated with the formula:
         ```
         working_batteries: Set[BatteryData] # working batteries from the battery pool
         total_capacity = sum(
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import asyncio
 import logging
 from dataclasses import dataclass
 from datetime import timedelta
 from typing import Dict
 
 from frequenz.channels import Broadcast, Sender
-from frequenz.channels.util import Select, Timer
+from frequenz.channels.util import Timer, select, selected_from
 
 from ..._internal._asyncio import cancel_and_await
 from ...microgrid import connection_manager
 from ...microgrid.component import ComponentCategory
 
 _logger = logging.getLogger(__name__)
 
@@ -91,39 +91,38 @@
             raise RuntimeError(err)
 
         meter_data = (
             await api_client.meter_data(next(iter(meters)).component_id)
         ).into_peekable()
         latest_bound: Dict[int, ComponentCurrentLimit] = {}
 
-        select = Select(
-            bound_chan=self._bounds_rx,
-            timer=Timer(self._repeat_interval.total_seconds()),
-        )
-        while await select.ready():
+        bound_chan = self._bounds_rx
+        timer = Timer.timeout(timedelta(self._repeat_interval.total_seconds()))
+
+        async for selected in select(bound_chan, timer):
             meter = meter_data.peek()
             if meter is None:
                 raise ValueError("Meter channel closed.")
 
-            if msg := select.bound_chan:
-                bound: ComponentCurrentLimit = msg.inner
+            if selected_from(selected, bound_chan):
+                bound: ComponentCurrentLimit = selected.value
                 if (
                     bound.component_id in latest_bound
                     and latest_bound[bound.component_id] == bound
                 ):
                     continue
                 latest_bound[bound.component_id] = bound
                 min_voltage = min(meter.voltage_per_phase)
                 logging.info("sending new bounds: %s", bound)
                 await api_client.set_bounds(
                     bound.component_id,
                     0,
                     bound.max_amps * min_voltage * self._NUM_PHASES,
                 )
-            elif msg := select.timer:
+            elif selected_from(selected, timer):
                 for bound in latest_bound.values():
                     min_voltage = min(meter.voltage_per_phase)
                     logging.debug("resending bounds: %s", bound)
                     await api_client.set_bounds(
                         bound.component_id,
                         0,
                         bound.max_amps * min_voltage * self._NUM_PHASES,
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py` & `frequenz-sdk-0.23.0/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/PKG-INFO` & `frequenz-sdk-0.23.0/src/frequenz_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,69 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 0.22.1
-Summary: Frequenz Python SDK
+Version: 0.23.0
+Summary: A development kit to interact with the Frequenz development platform
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
-Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
+Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/support
-Keywords: frequenz,sdk,microgrid,actor
+Keywords: frequenz,python,lib,library,sdk,microgrid
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: docs-gen
-Provides-Extra: docs-lint
-Provides-Extra: format
-Provides-Extra: nox
-Provides-Extra: examples
-Provides-Extra: pytest
-Provides-Extra: mypy
-Provides-Extra: pylint
+Provides-Extra: dev-docstrings
+Provides-Extra: dev-examples
+Provides-Extra: dev-formatting
+Provides-Extra: dev-mkdocs
+Provides-Extra: dev-mypy
+Provides-Extra: dev-noxfile
+Provides-Extra: dev-pylint
+Provides-Extra: dev-pytest
 Provides-Extra: dev
 License-File: LICENSE
 
 # Frequenz Python SDK
 
 [![Build Status](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml)
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-sdk)](https://pypi.org/project/frequenz-sdk/)
 [![Docs](https://img.shields.io/badge/docs-latest-informational)](https://frequenz-floss.github.io/frequenz-sdk-python/)
 
+## Introduction
+
 A development kit to interact with the Frequenz development platform.
 
-## Supported Python versions
+## Quick Start
+
+We assume you are on a system with Python available. If that is not the case,
+please [download and install Python](https://www.python.org/downloads/) first.
+
+To install the SDK, you probably want to create a new virtual environment first.
+For example, if you use a `sh` compatible shell, you can do this:
+
+```sh
+python3 -m venv .venv
+. .venv/bin/activate
+```
+
+Then, just install using `pip`:
+
+```sh
+python3 -m pip install frequenz-sdk
+```
+
+## Documentation
 
-* Only Python 3.11 is fully supported (tested).
+For more information, please visit the [documentation
+website](https://frequenz-floss.github.io/frequenz-sdk-python/).
 
 ## Contributing
 
 If you want to know how to build this project and contribute to it, please
 check out the [Contributing Guide](CONTRIBUTING.md).
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/SOURCES.txt` & `frequenz-sdk-0.23.0/src/frequenz_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.cookiecutter-replay.json
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 RELEASE_NOTES.md
 mkdocs.yml
 pyproject.toml
@@ -60,14 +61,15 @@
 src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
 src/frequenz/sdk/timeseries/_quantities.py
 src/frequenz/sdk/timeseries/_resampling.py
 src/frequenz/sdk/timeseries/_formula_engine/__init__.py
 src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
+src/frequenz/sdk/timeseries/_formula_engine/_formula_evaluator.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
 src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
 src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_chp_power_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_consumer_power_formula.py
```

### Comparing `frequenz-sdk-0.22.1/src/frequenz_sdk.egg-info/requires.txt` & `frequenz-sdk-0.23.0/src/frequenz_sdk.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 frequenz-api-microgrid<0.12.0,>=0.11.0
-frequenz-channels<0.15.0,>=0.14.0
+frequenz-channels<0.17.0,>=0.16.0
 google-api-python-client<3,>=2.71
 grpcio<2,>=1.54.2
 grpcio-tools<2,>=1.54.2
 networkx<4,>=2.8
 numpy<2,>=1.24.2
 protobuf<5,>=4.21.6
 pydantic<2,>=1.9
-toml>=0.10
 tqdm<5,>=4.38.0
 typing_extensions<5,>=4.4.0
 watchfiles>=0.15.0
 
 [dev]
-frequenz-sdk[docs-gen,docs-lint,format,mypy,nox,pylint,pytest]
+frequenz-sdk[dev-docstrings,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
-[docs-gen]
-mike==1.1.2
-mkdocs-gen-files==0.5.0
-mkdocs-literate-nav==0.6.0
-mkdocs-material==9.1.18
-mkdocs-section-index==0.3.5
-mkdocstrings[python]==0.22.0
-
-[docs-lint]
+[dev-docstrings]
 pydocstyle==6.3.0
 darglint==1.8.1
 tomli==2.0.1
 
-[examples]
-polars==0.18.4
+[dev-examples]
+polars==0.18.11
 
-[format]
-black==23.3.0
+[dev-formatting]
+black==23.7.0
 isort==5.12.0
 
-[mypy]
+[dev-mkdocs]
+mike==1.1.2
+mkdocs-gen-files==0.5.0
+mkdocs-literate-nav==0.6.0
+mkdocs-material==9.1.21
+mkdocs-section-index==0.3.5
+mkdocstrings[python]==0.22.0
+frequenz-repo-config[lib]==0.4.0
+
+[dev-mypy]
 mypy==1.4.1
 grpc-stubs==1.24.12
-frequenz-sdk[docs-gen,nox,pytest]
+types-protobuf==4.23.0.2
+frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]
 
-[nox]
+[dev-noxfile]
 nox==2023.4.22
-toml==0.10.2
+frequenz-repo-config[lib]==0.4.0
 
-[pylint]
-pylint==2.17.4
-frequenz-sdk[docs-gen,nox,pytest]
+[dev-pylint]
+pylint==2.17.5
+frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]
 
-[pytest]
+[dev-pytest]
 pytest==7.4.0
-pytest-cov==4.1.0
 pytest-mock==3.11.1
-pytest-asyncio==0.21.0
-time-machine==2.10.0
+pytest-asyncio==0.21.1
+time-machine==2.11.0
 async-solipsism==0.5
-sybil==5.0.2
-pylint==2.17.4
-frequenz-sdk[examples]
+sybil==5.0.3
+pylint==2.17.5
+frequenz-sdk[dev-examples]
```

