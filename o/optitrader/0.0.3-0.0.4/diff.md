# Comparing `tmp/optitrader-0.0.3.tar.gz` & `tmp/optitrader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optitrader-0.0.3.tar", max compression
+gzip compressed data, was "optitrader-0.0.4.tar", max compression
```

## Comparing `optitrader-0.0.3.tar` & `optitrader-0.0.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1073 2023-08-02 15:23:56.882993 optitrader-0.0.3/LICENSE
--rw-r--r--   0        0        0     8749 2023-08-02 15:23:56.882993 optitrader-0.0.3/README.md
--rw-r--r--   0        0        0     6611 2023-08-02 15:23:56.906993 optitrader-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      218 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/__init__.py
--rw-r--r--   0        0        0     2239 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/api.py
--rw-r--r--   0        0        0       87 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/1_🏠_Home.py
--rw-r--r--   0        0        0      177 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/__init__.py
--rw-r--r--   0        0        0      389 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/about.py
--rw-r--r--   0        0        0      518 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/account.py
--rw-r--r--   0        0        0     1187 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/backtester.py
--rw-r--r--   0        0        0     3575 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/explore.py
--rw-r--r--   0        0        0     1305 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/home.py
--rw-r--r--   0        0        0     1129 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/page.py
--rw-r--r--   0        0        0      105 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/pages/2_📈_Backtester.py
--rw-r--r--   0        0        0       96 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/pages/3_🗺️_Explore.py
--rw-r--r--   0        0        0       96 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/pages/4_💼_Account.py
--rw-r--r--   0        0        0       90 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/pages/5_👨🏻‍💻_About.py
--rw-r--r--   0        0        0       12 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/pages/__init__.py
--rw-r--r--   0        0        0    24191 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/session_manager.py
--rw-r--r--   0        0        0    24190 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp
--rw-r--r--   0        0        0     2621 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/backtester.py
--rw-r--r--   0        0        0      469 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/cli.py
--rw-r--r--   0        0        0     1556 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/config.py
--rw-r--r--   0        0        0      422 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/enums/__init__.py
--rw-r--r--   0        0        0      228 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/enums/backtester.py
--rw-r--r--   0        0        0      736 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/enums/iterable.py
--rw-r--r--   0        0        0     1712 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/enums/market.py
--rw-r--r--   0        0        0      860 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/enums/optimization.py
--rw-r--r--   0        0        0     7356 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/main.py
--rw-r--r--   0        0        0      231 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/__init__.py
--rw-r--r--   0        0        0     8461 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/alpaca_market_data.py
--rw-r--r--   0        0        0     8460 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp
--rw-r--r--   0        0        0      768 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/base_data_provider.py
--rw-r--r--   0        0        0       12 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/__init__.py
--rw-r--r--   0        0        0     5339 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/database.py
--rw-r--r--   0        0        0     5338 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp
--rw-r--r--   0        0        0     1935 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/models.py
--rw-r--r--   0        0        0       12 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/scripts/__init__.py
--rw-r--r--   0        0        0      743 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/scripts/add_asset.py
--rw-r--r--   0        0        0     1311 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/scripts/create_assets_table.py
--rw-r--r--   0        0        0      733 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/db/scripts/update_number_of_shares.py
--rw-r--r--   0        0        0     2830 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/finnhub_market_data.py
--rw-r--r--   0        0        0     3473 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/investment_universe.py
--rw-r--r--   0        0        0    14305 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/market_data.py
--rw-r--r--   0        0        0    14239 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp
--rw-r--r--   0        0        0     3330 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/news.py
--rw-r--r--   0        0        0     4446 2023-08-02 15:23:56.906993 optitrader-0.0.3/src/optitrader/market/trading.py
--rw-r--r--   0        0        0     6381 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/market/yahoo_market_data.py
--rw-r--r--   0        0        0      270 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/models/__init__.py
--rw-r--r--   0        0        0     2112 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/models/asset.py
--rw-r--r--   0        0        0      243 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/models/base.py
--rw-r--r--   0        0        0     1962 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/models/optimization.py
--rw-r--r--   0        0        0     1962 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp
--rw-r--r--   0        0        0       12 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/optimization/__init__.py
--rw-r--r--   0        0        0     7861 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/optimization/constraints.py
--rw-r--r--   0        0        0    12717 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/optimization/objectives.py
--rw-r--r--   0        0        0     6440 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/optimization/solver.py
--rw-r--r--   0        0        0     6510 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/portfolio.py
--rw-r--r--   0        0        0        0 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/py.typed
--rw-r--r--   0        0        0      203 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/utils/__init__.py
--rw-r--r--   0        0        0      953 2023-08-02 15:23:56.910993 optitrader-0.0.3/src/optitrader/utils/utils.py
--rw-r--r--   0        0        0    10040 1970-01-01 00:00:00.000000 optitrader-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-03 14:38:50.967027 optitrader-0.0.4/LICENSE
+-rw-r--r--   0        0        0     8749 2023-08-03 14:38:50.967027 optitrader-0.0.4/README.md
+-rw-r--r--   0        0        0     6611 2023-08-03 14:38:50.991027 optitrader-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/__init__.py
+-rw-r--r--   0        0        0     2239 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/api.py
+-rw-r--r--   0        0        0       87 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/1_🏠_Home.py
+-rw-r--r--   0        0        0      177 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/__init__.py
+-rw-r--r--   0        0        0      389 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/about.py
+-rw-r--r--   0        0        0      518 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/account.py
+-rw-r--r--   0        0        0     1187 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/backtester.py
+-rw-r--r--   0        0        0     3575 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/explore.py
+-rw-r--r--   0        0        0     1305 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/home.py
+-rw-r--r--   0        0        0     1129 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/page.py
+-rw-r--r--   0        0        0      105 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/pages/2_📈_Backtester.py
+-rw-r--r--   0        0        0       96 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/pages/3_🗺️_Explore.py
+-rw-r--r--   0        0        0       96 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/pages/4_💼_Account.py
+-rw-r--r--   0        0        0       90 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/pages/5_👨🏻‍💻_About.py
+-rw-r--r--   0        0        0       12 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/pages/__init__.py
+-rw-r--r--   0        0        0    24191 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/session_manager.py
+-rw-r--r--   0        0        0    24190 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp
+-rw-r--r--   0        0        0     2621 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/backtester.py
+-rw-r--r--   0        0        0      469 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/cli.py
+-rw-r--r--   0        0        0     1556 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/config.py
+-rw-r--r--   0        0        0      422 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/enums/__init__.py
+-rw-r--r--   0        0        0      228 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/enums/backtester.py
+-rw-r--r--   0        0        0      736 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/enums/iterable.py
+-rw-r--r--   0        0        0     1712 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/enums/market.py
+-rw-r--r--   0        0        0      860 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/enums/optimization.py
+-rw-r--r--   0        0        0     7356 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/main.py
+-rw-r--r--   0        0        0      231 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/__init__.py
+-rw-r--r--   0        0        0     8484 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/alpaca_market_data.py
+-rw-r--r--   0        0        0     8460 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp
+-rw-r--r--   0        0        0      768 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/base_data_provider.py
+-rw-r--r--   0        0        0       12 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/db/__init__.py
+-rw-r--r--   0        0        0     5339 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/db/database.py
+-rw-r--r--   0        0        0     5338 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp
+-rw-r--r--   0        0        0     1935 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/db/models.py
+-rw-r--r--   0        0        0       12 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/db/scripts/__init__.py
+-rw-r--r--   0        0        0      743 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/db/scripts/add_asset.py
+-rw-r--r--   0        0        0     1311 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/db/scripts/create_assets_table.py
+-rw-r--r--   0        0        0      733 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/db/scripts/update_number_of_shares.py
+-rw-r--r--   0        0        0     2830 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/finnhub_market_data.py
+-rw-r--r--   0        0        0     3473 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/investment_universe.py
+-rw-r--r--   0        0        0    14305 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/market_data.py
+-rw-r--r--   0        0        0    14239 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp
+-rw-r--r--   0        0        0     3330 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/news.py
+-rw-r--r--   0        0        0     4446 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/trading.py
+-rw-r--r--   0        0        0     6381 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/market/yahoo_market_data.py
+-rw-r--r--   0        0        0      270 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/models/__init__.py
+-rw-r--r--   0        0        0     2112 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/models/asset.py
+-rw-r--r--   0        0        0      243 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/models/base.py
+-rw-r--r--   0        0        0     1962 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/models/optimization.py
+-rw-r--r--   0        0        0     1962 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp
+-rw-r--r--   0        0        0       12 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/optimization/__init__.py
+-rw-r--r--   0        0        0     7861 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/optimization/constraints.py
+-rw-r--r--   0        0        0    12717 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/optimization/objectives.py
+-rw-r--r--   0        0        0     6440 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/optimization/solver.py
+-rw-r--r--   0        0        0     6510 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/portfolio.py
+-rw-r--r--   0        0        0        0 2023-08-03 14:38:50.991027 optitrader-0.0.4/src/optitrader/py.typed
+-rw-r--r--   0        0        0      203 2023-08-03 14:38:50.995027 optitrader-0.0.4/src/optitrader/utils/__init__.py
+-rw-r--r--   0        0        0      953 2023-08-03 14:38:50.995027 optitrader-0.0.4/src/optitrader/utils/utils.py
+-rw-r--r--   0        0        0    10040 1970-01-01 00:00:00.000000 optitrader-0.0.4/PKG-INFO
```

### Comparing `optitrader-0.0.3/LICENSE` & `optitrader-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/README.md` & `optitrader-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/pyproject.toml` & `optitrader-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "optitrader"
-version = "0.0.3"
+version = "0.0.4"
 description = "Optitrader is an opne-source Python package for portfolio optimization. "
 authors = ["Alessio Castrica <castricaalessio@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Ale-Cas/optitrader"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
```

### Comparing `optitrader-0.0.3/src/optitrader/api.py` & `optitrader-0.0.4/src/optitrader/api.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/app/account.py` & `optitrader-0.0.4/src/optitrader/app/account.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/app/backtester.py` & `optitrader-0.0.4/src/optitrader/app/backtester.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/app/explore.py` & `optitrader-0.0.4/src/optitrader/app/explore.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/app/home.py` & `optitrader-0.0.4/src/optitrader/app/home.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/app/page.py` & `optitrader-0.0.4/src/optitrader/app/page.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/app/session_manager.py` & `optitrader-0.0.4/src/optitrader/app/session_manager.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp` & `optitrader-0.0.4/src/optitrader/app/session_manager.py.aeacae1dba05799ae3b187801467b414.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/backtester.py` & `optitrader-0.0.4/src/optitrader/backtester.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/config.py` & `optitrader-0.0.4/src/optitrader/config.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/enums/iterable.py` & `optitrader-0.0.4/src/optitrader/enums/iterable.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/enums/market.py` & `optitrader-0.0.4/src/optitrader/enums/market.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/enums/optimization.py` & `optitrader-0.0.4/src/optitrader/enums/optimization.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/main.py` & `optitrader-0.0.4/src/optitrader/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -61,26 +61,26 @@
             The tickers investment universe to consider. Mutually exclusive with universe_name.
         `constraints`: list[PortfolioConstraint] | None = None
             The constraints of the optimal portfolio.
         `market_data`: MarketData | None = None
             The market data instance to get the data from,
             you can pass your own with your API keys and preferred data provider.
         """
-        self.investment_universe = InvestmentUniverse(tickers=tickers, name=universe_name)
-        self.objectives = objectives
-        self.constraints = constraints or [SumToOneConstraint(), NoShortSellConstraint()]
         assert (
             market_data or (trading_key and trading_secret) or (broker_key and broker_secret)
         ), "You must pass either a MarketData instance, the Trading API keys or Broker API keys."
         self.market_data = market_data or MarketData(
             trading_key=trading_key,
             trading_secret=trading_secret,
             broker_key=broker_key,
             broker_secret=broker_secret,
         )
+        self.investment_universe = InvestmentUniverse(tickers=tickers, name=universe_name)
+        self.objectives = objectives
+        self.constraints = constraints or [SumToOneConstraint(), NoShortSellConstraint()]
 
     def add_constraint(self, constraint: PortfolioConstraint) -> None:
         """Add a constraint."""
         self.constraints.append(constraint)
 
     def add_objective(self, objective: PortfolioObjective) -> None:
         """Add an objective."""
```

### Comparing `optitrader-0.0.3/src/optitrader/market/alpaca_market_data.py` & `optitrader-0.0.4/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from functools import lru_cache
 
 import pandas as pd
 from alpaca.broker import BrokerClient
 from alpaca.data import Adjustment, BarSet, StockBarsRequest, StockHistoricalDataClient, TimeFrame
 from alpaca.trading import Asset, AssetClass, AssetStatus, GetAssetsRequest, TradingClient
-
 from optitrader.config import SETTINGS
 from optitrader.enums import BarsField
 from optitrader.market.base_data_provider import BaseDataProvider
 from optitrader.market.news import AlpacaNewsAPI, NewsArticle
 
 
 class AlpacaMarketData(BaseDataProvider):
```

### Comparing `optitrader-0.0.3/src/optitrader/market/alpaca_market_data.py.9fafeb33ede105e202d2a274793d58ee.tmp` & `optitrader-0.0.4/src/optitrader/market/alpaca_market_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from functools import lru_cache
 
 import pandas as pd
 from alpaca.broker import BrokerClient
 from alpaca.data import Adjustment, BarSet, StockBarsRequest, StockHistoricalDataClient, TimeFrame
 from alpaca.trading import Asset, AssetClass, AssetStatus, GetAssetsRequest, TradingClient
+
 from optitrader.config import SETTINGS
 from optitrader.enums import BarsField
 from optitrader.market.base_data_provider import BaseDataProvider
 from optitrader.market.news import AlpacaNewsAPI, NewsArticle
 
 
 class AlpacaMarketData(BaseDataProvider):
@@ -19,16 +20,16 @@
         self,
         trading_key: str | None = SETTINGS.ALPACA_TRADING_API_KEY,
         trading_secret: str | None = SETTINGS.ALPACA_TRADING_API_SECRET,
         broker_key: str | None = SETTINGS.ALPACA_BROKER_API_KEY,
         broker_secret: str | None = SETTINGS.ALPACA_BROKER_API_SECRET,
     ) -> None:
         super().__init__()
-        assert (
-            SETTINGS.is_trading or SETTINGS.is_broker
+        assert (trading_key and trading_secret) or (
+            broker_key and broker_secret
         ), "Either Trading API or Broker API keys must be provided to use this service."
         self.__data_client = (
             StockHistoricalDataClient(
                 api_key=trading_key,
                 secret_key=trading_secret,
             )
             if SETTINGS.is_trading
```

### Comparing `optitrader-0.0.3/src/optitrader/market/base_data_provider.py` & `optitrader-0.0.4/src/optitrader/market/base_data_provider.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/db/database.py` & `optitrader-0.0.4/src/optitrader/market/db/database.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp` & `optitrader-0.0.4/src/optitrader/market/db/database.py.7b38a0f9e78f0ef64524afe7b2c0c608.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/db/models.py` & `optitrader-0.0.4/src/optitrader/market/db/models.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/db/scripts/add_asset.py` & `optitrader-0.0.4/src/optitrader/market/db/scripts/add_asset.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/db/scripts/create_assets_table.py` & `optitrader-0.0.4/src/optitrader/market/db/scripts/create_assets_table.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/db/scripts/update_number_of_shares.py` & `optitrader-0.0.4/src/optitrader/market/db/scripts/update_number_of_shares.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/finnhub_market_data.py` & `optitrader-0.0.4/src/optitrader/market/finnhub_market_data.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/investment_universe.py` & `optitrader-0.0.4/src/optitrader/market/investment_universe.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/market_data.py` & `optitrader-0.0.4/src/optitrader/market/market_data.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp` & `optitrader-0.0.4/src/optitrader/market/market_data.py.185a99388c8a3ef51cc2541e94dbdc63.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/news.py` & `optitrader-0.0.4/src/optitrader/market/news.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/trading.py` & `optitrader-0.0.4/src/optitrader/market/trading.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/market/yahoo_market_data.py` & `optitrader-0.0.4/src/optitrader/market/yahoo_market_data.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/models/asset.py` & `optitrader-0.0.4/src/optitrader/models/asset.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/models/optimization.py` & `optitrader-0.0.4/src/optitrader/models/optimization.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp` & `optitrader-0.0.4/src/optitrader/models/optimization.py.0f97aab178a762049bd1442f7826f63f.tmp`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/optimization/constraints.py` & `optitrader-0.0.4/src/optitrader/optimization/constraints.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/optimization/objectives.py` & `optitrader-0.0.4/src/optitrader/optimization/objectives.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/optimization/solver.py` & `optitrader-0.0.4/src/optitrader/optimization/solver.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/portfolio.py` & `optitrader-0.0.4/src/optitrader/portfolio.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/src/optitrader/utils/utils.py` & `optitrader-0.0.4/src/optitrader/utils/utils.py`

 * *Files identical despite different names*

### Comparing `optitrader-0.0.3/PKG-INFO` & `optitrader-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optitrader
-Version: 0.0.3
+Version: 0.0.4
 Summary: Optitrader is an opne-source Python package for portfolio optimization. 
 Home-page: https://github.com/Ale-Cas/optitrader
 Author: Alessio Castrica
 Author-email: castricaalessio@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

