# Comparing `tmp/investing_algorithm_framework-1.2.tar.gz` & `tmp/investing_algorithm_framework-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investing_algorithm_framework-1.2.tar", last modified: Wed Aug  2 06:48:44 2023, max compression
+gzip compressed data, was "investing_algorithm_framework-1.3.tar", last modified: Wed Aug  2 21:10:16 2023, max compression
```

## Comparing `investing_algorithm_framework-1.2.tar` & `investing_algorithm_framework-1.3.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.685703 investing_algorithm_framework-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-08-02 06:48:44.685703 investing_algorithm_framework-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.673703 investing_algorithm_framework-1.2/investing_algorithm_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.677703 investing_algorithm_framework-1.2/investing_algorithm_framework/app/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.677703 investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.677703 investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.677703 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.677703 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/controllers/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/controllers/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/controllers/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/run_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.677703 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/schemas/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/schemas/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/schemas/position.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/setup_cors.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/dependency_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.677703 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.681702 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.681702 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/market_data/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/market_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/market_data/asset_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/market_data/ohlcv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/market_data/order_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/market_data/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.681702 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/order_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/order_side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/order_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/order_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.681702 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/portfolio/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.681702 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/position/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/position/position.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/position/position_cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/time_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/time_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/trading_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/trading_time_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/stateless_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.681702 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/utils/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/utils/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/utils/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/domain/utils/synchronized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.681702 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.681702 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/database/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.681702 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/model_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.685703 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/order/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/order/order_fee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.685703 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.685703 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/position/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/position/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/position/position_cost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.685703 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/order_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/position_cost_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/position_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.685703 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/services/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/services/market_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.685703 investing_algorithm_framework-1.2/investing_algorithm_framework/services/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/services/market_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15968 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/services/order_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/services/portfolio_configuration_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/services/portfolio_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/services/position_cost_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/services/position_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/services/repository_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/services/strategy_orchestrator_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/investing_algorithm_framework/setup_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.673703 investing_algorithm_framework-1.2/investing_algorithm_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-08-02 06:48:44.000000 investing_algorithm_framework-1.2/investing_algorithm_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-08-02 06:48:44.000000 investing_algorithm_framework-1.2/investing_algorithm_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 06:48:44.000000 investing_algorithm_framework-1.2/investing_algorithm_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-02 06:48:44.000000 investing_algorithm_framework-1.2/investing_algorithm_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 06:48:44.000000 investing_algorithm_framework-1.2/investing_algorithm_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 06:48:44.685703 investing_algorithm_framework-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 06:48:44.685703 investing_algorithm_framework-1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-02 06:48:03.000000 investing_algorithm_framework-1.2/tests/test_create_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.981214 investing_algorithm_framework-1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-08-02 21:10:16.981214 investing_algorithm_framework-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.957214 investing_algorithm_framework-1.3/investing_algorithm_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.961214 investing_algorithm_framework-1.3/investing_algorithm_framework/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.961214 investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.961214 investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.961214 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.965214 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/controllers/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/controllers/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/controllers/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/run_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.965214 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/schemas/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/schemas/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/schemas/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/setup_cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/dependency_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.965214 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.965214 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.969214 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/market_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/market_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/market_data/asset_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/market_data/ohlcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/market_data/order_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/market_data/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.969214 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/order_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/order_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/order_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/order_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.969214 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/portfolio/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.969214 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/position/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/position/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/position/position_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/time_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/time_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/trading_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/trading_time_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/stateless_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.973214 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/utils/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/utils/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/utils/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/domain/utils/synchronized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.973214 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.973214 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.973214 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/model_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.973214 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/order/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/order/order_fee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.973214 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.973214 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/position/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/position/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/position/position_cost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.977214 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/order_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/position_cost_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/position_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.977214 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/services/market_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.977214 investing_algorithm_framework-1.3/investing_algorithm_framework/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/services/market_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/services/order_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/services/portfolio_configuration_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/services/portfolio_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/services/position_cost_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/services/position_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/services/repository_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/services/strategy_orchestrator_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/investing_algorithm_framework/setup_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.957214 investing_algorithm_framework-1.3/investing_algorithm_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-08-02 21:10:16.000000 investing_algorithm_framework-1.3/investing_algorithm_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-08-02 21:10:16.000000 investing_algorithm_framework-1.3/investing_algorithm_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:10:16.000000 investing_algorithm_framework-1.3/investing_algorithm_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-02 21:10:16.000000 investing_algorithm_framework-1.3/investing_algorithm_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 21:10:16.000000 investing_algorithm_framework-1.3/investing_algorithm_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 21:10:16.981214 investing_algorithm_framework-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:10:16.977214 investing_algorithm_framework-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-02 21:09:26.000000 investing_algorithm_framework-1.3/tests/test_create_app.py
```

### Comparing `investing_algorithm_framework-1.2/LICENSE` & `investing_algorithm_framework-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/PKG-INFO` & `investing_algorithm_framework-1.3/investing_algorithm_framework.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: investing_algorithm_framework
-Version: 1.2
+Name: investing-algorithm-framework
+Version: 1.3
 Summary: A framework for creating an investment algorithm
 Home-page: https://github.com/coding-kitties/investing-algorithm-framework.git
 Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
 Author: coding kitties
 License: Apache License 2.0
 Keywords: TRADING,INVESTING,BOT,ALGORITHM,FRAMEWORK
 Classifier: Intended Audience :: Developers
@@ -29,21 +29,21 @@
 ###### Sponsors
 <p align="left">
 <a href="https://logicfunds.io">
   <img alt="logicfunds" src="https://logicfunds-web-app-images.s3.eu-central-1.amazonaws.com/logicfunds-logo.png" width="200px" />
 </a>
 </p>
 
-# Investing Algorithm Framework
-The Investing Algorithm Framework is a python framework for building
-investment algorithms. It encourages rapid development and clean, pragmatic code design.
-
-The framework provides you with all the components you need to create an 
-investing algorithm (data providing, portfolio management, order execution, etc..). Also,
-it has various deployment options, such as web server, stateless, etc..
+
+# [Investing Algorithm Framework](https://github.com/coding-kitties/investing-algorithm-framework)
+
+The Investing Algorithm Framework is a Python tool that enables swift and 
+elegant development of investment algorithms and trading bots. It comes with all the necessary 
+components for creating algorithms, including data provisioning, portfolio management, and order execution.
+
 
 ## Example
 The following algorithm connects to binance and buys BTC every 5 seconds. 
 It also exposes an REST API that allows you to interact with the algorithm.
 ```python
 import pathlib
 from datetime import datetime, timedelta
```

### Comparing `investing_algorithm_framework-1.2/README.md` & `investing_algorithm_framework-1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,49 @@
+Metadata-Version: 2.1
+Name: investing_algorithm_framework
+Version: 1.3
+Summary: A framework for creating an investment algorithm
+Home-page: https://github.com/coding-kitties/investing-algorithm-framework.git
+Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
+Author: coding kitties
+License: Apache License 2.0
+Keywords: TRADING,INVESTING,BOT,ALGORITHM,FRAMEWORK
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+
 <a href=https://investing-algorithm-framework.com><img src="https://img.shields.io/badge/docs-website-brightgreen"></a>
 [![Build](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml/badge.svg)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml)
 [![Tests](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml)
 [![Downloads](https://pepy.tech/badge/investing-algorithm-framework)](https://pepy.tech/badge/investing-algorithm-framework)
 [![Current Version](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)
 <a href="https://www.reddit.com/r/InvestingBots/"><img src="https://img.shields.io/reddit/subreddit-subscribers/investingbots?style=social"></a>
 ###### Sponsors
 <p align="left">
 <a href="https://logicfunds.io">
   <img alt="logicfunds" src="https://logicfunds-web-app-images.s3.eu-central-1.amazonaws.com/logicfunds-logo.png" width="200px" />
 </a>
 </p>
 
-# Investing Algorithm Framework
-The Investing Algorithm Framework is a python framework for building
-investment algorithms. It encourages rapid development and clean, pragmatic code design.
-
-The framework provides you with all the components you need to create an 
-investing algorithm (data providing, portfolio management, order execution, etc..). Also,
-it has various deployment options, such as web server, stateless, etc..
+
+# [Investing Algorithm Framework](https://github.com/coding-kitties/investing-algorithm-framework)
+
+The Investing Algorithm Framework is a Python tool that enables swift and 
+elegant development of investment algorithms and trading bots. It comes with all the necessary 
+components for creating algorithms, including data provisioning, portfolio management, and order execution.
+
 
 ## Example
 The following algorithm connects to binance and buys BTC every 5 seconds. 
 It also exposes an REST API that allows you to interact with the algorithm.
 ```python
 import pathlib
 from datetime import datetime, timedelta
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/__init__.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/algorithm.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,43 +68,61 @@
             {
                 "target_symbol": target_symbol,
                 "price": price,
                 "amount": amount,
                 "type": type,
                 "side": side,
                 "portfolio_id": portfolio.id,
-                "status": OrderStatus.PENDING.value,
+                "status": OrderStatus.CREATED.value,
                 "trading_symbol": portfolio.trading_symbol,
             },
             execute=execute,
             validate=validate,
             sync=sync
         )
 
     def create_limit_order(
-            self,
-            target_symbol,
-            price,
-            side,
-            amount,
-            market=None,
-            execute=True,
-            validate=True,
-            sync=True
+        self,
+        target_symbol,
+        price,
+        side,
+        amount=None,
+        percentage_of_portfolio=None,
+        percentage_of_position=None,
+        market=None,
+        execute=True,
+        validate=True,
+        sync=True
     ):
         portfolio = self.portfolio_service.find({"market": market})
+
+        if percentage_of_portfolio is not None and OrderSide.BUY.equals(side):
+            size = portfolio.net_size * (percentage_of_portfolio / 100)
+            amount = size / price
+
+        if percentage_of_position is not None and OrderSide.SELL.equals(side):
+            print(target_symbol)
+            print(portfolio.id)
+            position = self.position_service.find(
+                {
+                    "symbol": target_symbol,
+                    "portfolio": portfolio.id
+                }
+            )
+            amount = position.amount * (percentage_of_position / 100)
+
         return self.order_service.create(
             {
                 "target_symbol": target_symbol,
                 "price": price,
                 "amount": amount,
                 "type": OrderType.LIMIT.value,
                 "side": OrderSide.from_value(side).value,
                 "portfolio_id": portfolio.id,
-                "status": OrderStatus.PENDING.value,
+                "status": OrderStatus.CREATED.value,
                 "trading_symbol": portfolio.trading_symbol,
             },
             execute=execute,
             validate=validate,
             sync=sync
         )
 
@@ -122,28 +140,22 @@
         return self.order_service.create(
             {
                 "target_symbol": target_symbol,
                 "amount": amount,
                 "type": OrderType.MARKET.value,
                 "side": OrderSide.from_value(side).value,
                 "portfolio_id": portfolio.id,
-                "status": OrderStatus.PENDING.value,
+                "status": OrderStatus.CREATED.value,
                 "trading_symbol": portfolio.trading_symbol,
             },
             execute=execute,
             validate=validate,
             sync=sync
         )
 
-    def check_order_status(self, market=None, symbol=None, status=None):
-        portfolio = self.portfolio_service.get({"market": market})
-        orders = self.order_service \
-            .get_all({"target_symbol": symbol, "status": status})
-        self.order_service.check_order_status(portfolio, orders)
-
     def get_portfolio(self, market=None) -> Portfolio:
 
         if market is None:
             return self.portfolio_service.find({})
 
         return self.portfolio_service.find({{"market": market}})
 
@@ -152,15 +164,15 @@
         if market:
             portfolio = self.portfolio_service.find({{"market": market}})
         else:
             portfolio = self.portfolio_service.find({})
 
         trading_symbol = portfolio.trading_symbol
         return self.position_service.find(
-            {"portfolio": portfolio.identifier, "symbol": trading_symbol}
+            {"portfolio": portfolio.id, "symbol": trading_symbol}
         ).amount
 
     def reset(self):
         self._workers = []
         self._running_workers = []
 
     def get_order(
@@ -238,15 +250,15 @@
         portfolios = self.portfolio_service.get_all(query_params)
 
         if not portfolios:
             raise ApiException("No portfolio found.")
 
         portfolio = portfolios[0]
         return self.position_service.get_all(
-            {"portfolio": portfolio.identifier}
+            {"portfolio": portfolio.id}
         )
 
     def get_position(self, symbol, market=None, identifier=None) -> Position:
         query_params = {}
 
         if market is not None:
             query_params["market"] = market
@@ -259,15 +271,15 @@
         if not portfolios:
             raise ApiException("No portfolio found.")
 
         portfolio = portfolios[0]
 
         try:
             return self.position_service.find(
-                {"portfolio": portfolio.identifier, "symbol": symbol}
+                {"portfolio": portfolio.id, "symbol": symbol}
             )
         except ApiException:
             return None
 
     def position_exists(self, symbol, market=None, identifier=None) -> bool:
         query_params = {}
 
@@ -294,22 +306,57 @@
         portfolios = self.portfolio_service.get_all(query_params)
 
         if not portfolios:
             raise ApiException("No portfolio found.")
 
         portfolio = portfolios[0]
         position = self.position_service.find(
-            {"portfolio": portfolio.identifier, "symbol": symbol}
+            {"portfolio": portfolio.id, "symbol": symbol}
         )
         ticker = self.market_service.get_ticker(
             f"{symbol.upper()}/{portfolio.trading_symbol.upper()}"
         )
         return (position.amount * ticker["bid"] /
                 self.get_allocated(identifier=portfolio.identifier)) * 100
 
+    def close_position(self, symbol, market=None, identifier=None):
+        query_params = {}
+
+        if market is not None:
+            query_params["market"] = market
+
+        if identifier is not None:
+            query_params["identifier"] = identifier
+
+        position = self.get_position(symbol, market, identifier)
+
+        if position is None:
+            raise ApiException("No position found.")
+
+        if position.amount == 0:
+            return
+
+        for order in self.order_service\
+                .get_all({
+                    "position": position.id, "status": OrderStatus.OPEN.value
+                }):
+            self.order_service.cancel_order(order.id)
+
+        portfolio = self.portfolio_service.find({"position": position.id})
+        self.market_service.market = portfolio.market
+        ticker = self.market_service.get_ticker(
+            symbol=f"{symbol.upper()}/{portfolio.trading_symbol.upper()}"
+        )
+        self.create_limit_order(
+            target_symbol=position.symbol,
+            amount=position.amount,
+            side=OrderSide.SELL.value,
+            price=ticker["bid"],
+        )
+
     def add_strategies(self, strategies):
         self.strategy_orchestrator_service.add_strategies(strategies)
 
     def add_tasks(self, tasks):
         self.strategy_orchestrator_service.add_tasks(tasks)
 
     def get_allocated(self, market=None, identifier=None) -> float:
@@ -342,15 +389,15 @@
             portfolio.configuration = portfolio_configuration
             portfolios.append(portfolio)
 
         allocated = 0
 
         for portfolio in portfolios:
             positions = self.position_service.get_all(
-                {"portfolio": portfolio.identifier}
+                {"portfolio": portfolio.id}
             )
 
             for position in positions:
                 if portfolio.trading_symbol == position.symbol:
                     continue
 
                 symbol = f"{position.symbol.upper()}/" \
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/app.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
                 name='Web App', target=self._flask_app.run
             )
             flask_thread.setDaemon(True)
             flask_thread.start()
 
         order_service = self.container.order_service()
         number_of_iterations_since_last_orders_check = 1
+        order_service.check_pending_orders()
 
         try:
             while self.algorithm.running:
                 if number_of_iterations_since_last_orders_check == 30:
                     order_service.check_pending_orders()
                     number_of_iterations_since_last_orders_check = 1
 
@@ -303,14 +304,15 @@
 
             unallocated = float(
                 balances[portfolio_configuration.trading_symbol.upper()]
                 ["free"]
             )
             portfolio_repository.create(
                 {
+                    "unallocated": unallocated,
                     "identifier": portfolio_configuration.identifier,
                     "trading_symbol": portfolio_configuration.trading_symbol,
                     "market": portfolio_configuration.market,
                 }
             )
             portfolio = portfolio_repository.find(
                 {"identifier": portfolio_configuration.identifier}
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/__init__.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/action_handlers/__init__.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/action_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/stateless/exception_handler.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/stateless/exception_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/strategy.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/task.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/task.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/controllers/__init__.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/controllers/orders.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/controllers/orders.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/controllers/portfolio.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/controllers/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/controllers/positions.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/controllers/positions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/error_handler.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/error_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/responses.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/responses.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/app/web/schemas/portfolio.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/app/web/schemas/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     def get_orders(obj):
         order_service = DependencyContainer.order_service()
         return order_service.count({"portfolio": obj.identifier})
 
     @staticmethod
     def get_positions(obj):
         position_service = DependencyContainer.position_service()
-        return position_service.count({"portfolio": obj.identifier})
+        return position_service.count({"portfolio": obj.id})
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/dependency_container.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/dependency_container.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/__init__.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/config.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/config.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/constants.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/constants.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/exceptions.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/__init__.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/base_model.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/base_model.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/market_data/asset_price.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/market_data/asset_price.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/market_data/ohlcv.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/market_data/ohlcv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/market_data/order_book.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/market_data/order_book.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/market_data/ticker.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/market_data/ticker.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/order.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             "remaining_amount": self.remaining_amount,
             "cost": self.cost,
             "fee": self.fee.to_dict() if self.fee is not None else None,
         }
 
     @staticmethod
     def from_ccxt_order(ccxt_order):
-        status = OrderStatus.from_ccxt_status(ccxt_order["status"])
+        status = OrderStatus.from_value(ccxt_order["status"])
         target_symbol = ccxt_order.get("symbol").split("/")[0]
         trading_symbol = ccxt_order.get("symbol").split("/")[1]
 
         return Order(
             external_id=ccxt_order.get("id", None),
             target_symbol=target_symbol,
             trading_symbol=trading_symbol,
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/order_fee.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/order_side.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/order_side.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/order/order_type.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/order/order_type.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/position/position.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/position/position_cost.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/position/position_cost.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/time_frame.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/time_interval.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/time_interval.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/time_unit.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/time_unit.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/trading_data_types.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/trading_data_types.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/models/trading_time_frame.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/models/trading_time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/strategy.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/utils/csv.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/utils/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/domain/utils/stoppable_thread.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/domain/utils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/__init__.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/database/sql_alchemy.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/database/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/order/order.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/order/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             trade_closed_at=order.get_trade_closed_at(),
             trade_closed_price=order.get_trade_closed_price(),
             net_gain=order.get_net_gain(),
         )
 
     @staticmethod
     def from_ccxt_order(ccxt_order):
-        status = OrderStatus.from_ccxt_status(ccxt_order["status"])
+        status = OrderStatus.from_value(ccxt_order["status"])
         target_symbol = ccxt_order.get("symbol").split("/")[0]
         trading_symbol = ccxt_order.get("symbol").split("/")[1]
 
         return Order(
             external_id=ccxt_order.get("id", None),
             target_symbol=target_symbol,
             trading_symbol=trading_symbol,
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/order/order_fee.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     id = Column(Integer, primary_key=True)
     identifier = Column(String, nullable=False, unique=True)
     trading_symbol = Column(String, nullable=False)
     realized = Column(Float, nullable=False, default=0)
     total_revenue = Column(Float, nullable=False, default=0)
     total_cost = Column(Float, nullable=False, default=0)
     total_net_gain = Column(Float, nullable=False, default=0)
+    net_size = Column(Float, nullable=False, default=0)
     unallocated = Column(Float, nullable=False, default=0)
     market = Column(String, nullable=False)
     positions = relationship(
         "SQLPosition",
         back_populates="portfolio",
         lazy="dynamic",
         cascade="all,delete",
@@ -38,18 +39,22 @@
     def _write_once(self, key, value):
         existing = getattr(self, key)
 
         if existing is not None:
             raise ValueError("{} is write-once".format(key))
         return value
 
-    def __init__(self, trading_symbol, market, identifier=None):
-        super().__init__()
-        self.realized = 0
-        self.total_revenue = 0
-        self.total_cost = 0
-        self.market = market
-        self.identifier = identifier
-        self.trading_symbol = trading_symbol
+    def __init__(self, trading_symbol, market, unallocated, identifier=None):
 
-        if self.identifier is None:
-            self.identifier = self.market
+        if identifier is None:
+            identifier = market
+
+        super().__init__(
+            trading_symbol=trading_symbol,
+            market=market,
+            identifier=identifier,
+            net_size=unallocated,
+            unallocated=unallocated,
+            realized=0,
+            total_revenue=0,
+            total_cost=0,
+        )
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/position/position.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/models/position/position_cost.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/models/position/position_cost.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/order_repository.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/order_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/position_cost_repository.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/position_cost_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/position_repository.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/position_repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,9 @@
         if amount_query_param:
             query = query.filter(SQLPosition.amount == amount_query_param)
 
         if symbol_query_param:
             query = query.filter_by(symbol=symbol_query_param)
 
         if portfolio_query_param:
-            portfolio = db.query(SQLPortfolio).filter_by(
-                identifier=portfolio_query_param
-            ).first()
-
-            if portfolio is None:
-                return query.filter_by(id=-1)
-
-            query = query.filter_by(portfolio_id=portfolio.id)
+            query = query.filter_by(portfolio_id=portfolio_query_param)
         return query
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/repositories/repository.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/infrastructure/services/market_service.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/infrastructure/services/market_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,15 +265,15 @@
             order = self.exchange.createMarketSellOrder(symbol, amount)
             return Order.from_ccxt_order(order)
         except Exception as e:
             logger.exception(e)
             raise OperationalException("Could not create market sell order")
 
     def cancel_order(self, order):
-
+        print("cancel order")
         if not self.exchange.has['cancelOrder']:
             raise OperationalException(
                 f"Market service {self.market} does not support "
                 f"functionality cancel_order"
             )
 
         self.exchange.cancelOrder(
@@ -375,14 +375,17 @@
                 f"Market service {self.market} does not support "
                 f"functionality get_ohclvs"
             )
 
         now = self.exchange.milliseconds()
         ohlcvs = {}
 
+        # Set timeout to 30 seconds
+        self.exchange.timeout = 30000
+
         for symbol in symbols:
 
             try:
                 time_stamp = self.exchange.parse8601(
                     from_timestamp.strftime(":%Y-%m-%d %H:%M:%S")
                 )
                 dfs = []
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/services/__init__.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/services/market_data_service.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/services/market_data_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/services/order_service.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/services/order_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -93,33 +93,32 @@
             if OrderSide.BUY.equals(order.get_side()):
                 self.market_service.create_limit_buy_order(
                     target_symbol=order.get_target_symbol(),
                     trading_symbol=order.get_trading_symbol(),
                     amount=order.get_amount(),
                     price=order.get_price
                 )
-                return order
             else:
                 self.market_service.create_limit_sell_order(
                     target_symbol=order.get_target_symbol(),
                     trading_symbol=order.get_trading_symbol(),
                     amount=order.get_amount(),
                     price=order.get_price()
                 )
-                return order
         else:
             if OrderSide.BUY.equals(order.get_side()):
                 raise OperationalException("Market buy order not supported")
             else:
                 self.market_service.create_market_sell_order(
                     target_symbol=order.get_target_symbol(),
                     trading_symbol=order.get_trading_symbol(),
                     amount=order.get_amount(),
                 )
-            return order
+
+        self.update(order_id, {"status": OrderStatus.OPEN.value})
 
     def validate_order(self, order_data, portfolio):
 
         if OrderSide.BUY.equals(order_data["side"]):
             self.validate_buy_order(order_data, portfolio)
         else:
             self.validate_sell_order(order_data, portfolio)
@@ -129,26 +128,26 @@
         else:
             self.validate_market_order(order_data, portfolio)
 
     def validate_sell_order(self, order_data, portfolio):
         if not self.position_repository.exists(
             {
                 "symbol": order_data["target_symbol"],
-                "portfolio": portfolio.identifier
+                "portfolio": portfolio.id
             }
         ):
             raise OperationalException(
                 "Can't add sell order to non existing position"
             )
 
         position = self.position_repository\
             .find(
                 {
                     "symbol": order_data["target_symbol"],
-                    "portfolio": portfolio.identifier
+                    "portfolio": portfolio.id
                 }
             )
 
         if position.amount < order_data["amount"]:
             raise OperationalException(
                 "Order amount is larger then amount of open position"
             )
@@ -167,30 +166,47 @@
             raise OperationalException(
                 f"Can't add buy order with trading "
                 f"symbol {order_data['trading_symbol']} to "
                 f"portfolio with trading symbol {portfolio.trading_symbol}"
             )
 
     def validate_limit_order(self, order_data, portfolio):
-        total_price = order_data["amount"] * order_data["price"]
-        unallocated_position = self.position_repository\
-            .find(
-                {
-                    "portfolio": portfolio.identifier,
-                    "symbol": portfolio.trading_symbol
-                }
-            )
-        amount = unallocated_position.amount
 
-        if amount < total_price:
-            raise OperationalException(
-                f"Order total: {total_price} {portfolio.trading_symbol}, is "
-                f"larger then unallocated size: {amount} "
-                f"{portfolio.trading_symbol} of the portfolio"
-            )
+        if OrderSide.SELL.equals(order_data["side"]):
+            amount = order_data["amount"]
+            position = self.position_repository\
+                .find(
+                    {
+                        "portfolio": portfolio.id,
+                        "symbol": portfolio.trading_symbol
+                    }
+                )
+            if amount > position.amount:
+                raise OperationalException(
+                    f"Order amount: {amount} {portfolio.trading_symbol}, is "
+                    f"larger then position size: {position.amount} "
+                    f"{portfolio.trading_symbol} of the portfolio"
+                )
+        else:
+            total_price = order_data["amount"] * order_data["price"]
+            unallocated_position = self.position_repository\
+                .find(
+                    {
+                        "portfolio": portfolio.id,
+                        "symbol": portfolio.trading_symbol
+                    }
+                )
+            amount = unallocated_position.amount
+
+            if amount < total_price:
+                raise OperationalException(
+                    f"Order total: {total_price} {portfolio.trading_symbol}, is "
+                    f"larger then unallocated size: {amount} "
+                    f"{portfolio.trading_symbol} of the portfolio"
+                )
 
     def validate_market_order(self, order_data, portfolio):
 
         if OrderSide.BUY.equals(order_data["side"]):
 
             if "amount" not in order_data:
                 raise OperationalException(
@@ -207,30 +223,30 @@
                     f"{portfolio.trading_symbol.upper()}"
                 )
         else:
             position = self.position_repository\
                 .find(
                     {
                         "symbol": order_data["target_symbol"],
-                        "portfolio": portfolio.identifier
+                        "portfolio": portfolio.id
                     }
                 )
 
             if position is None:
                 raise OperationalException(
                     "Can't add market sell order to non existing position"
                 )
 
             if order_data['amount'] > position.amount:
                 raise OperationalException(
                     "Sell order amount larger then position size"
                 )
 
     def check_pending_orders(self):
-        pending_orders = self.get_all({"status": OrderStatus.PENDING.value})
+        pending_orders = self.get_all({"status": OrderStatus.OPEN.value})
 
         for order in pending_orders:
             position = self.position_repository.get(order.position_id)
             portfolio = self.portfolio_repository.get(position.portfolio_id)
             portfolio_configuration = self.portfolio_configuration_service\
                 .get(portfolio.identifier)
             self.market_service.initialize(portfolio_configuration)
@@ -238,15 +254,15 @@
 
             if OrderStatus.from_value(external_order.status)\
                     .equals(order.status):
                 continue
 
             updated_order = self.update(order.id, external_order.to_dict())
 
-            if OrderStatus.SUCCESS.equals(updated_order.status):
+            if OrderStatus.CLOSED.equals(updated_order.status):
 
                 if OrderSide.BUY.equals(updated_order.side):
                     self._sync_portfolio_with_executed_buy_order(updated_order)
                 else:
                     self._sync_portfolio_with_executed_sell_order(updated_order)
             elif OrderStatus.CANCELED.equals(updated_order.status):
 
@@ -254,41 +270,42 @@
                     self._sync_portfolio_with_cancelled_buy_order(
                         updated_order
                     )
                 else:
                     self._sync_portfolio_with_cancelled_sell_order(
                         updated_order
                     )
-            elif OrderStatus.FAILED.equals(updated_order.status):
+            elif OrderStatus.REJECTED.equals(updated_order.status) \
+                    or OrderStatus.EXPIRED.equals(updated_order.status):
 
                 if OrderSide.BUY.equals(updated_order.side):
                     self._sync_portfolio_with_failed_buy_order(updated_order)
                 else:
                     self._sync_portfolio_with_failed_sell_order(updated_order)
 
     def _create_position_if_not_exists(self, symbol, portfolio):
         if not self.position_repository.exists(
-            {"portfolio": portfolio.identifier, "symbol": symbol}
+            {"portfolio": portfolio.id, "symbol": symbol}
         ):
             self.position_repository \
                 .create({"portfolio_id": portfolio.id, "symbol": symbol})
             position = self.position_repository \
-                .find({"portfolio": portfolio.identifier, "symbol": symbol})
+                .find({"portfolio": portfolio.id, "symbol": symbol})
         else:
             position = self.position_repository \
-                .find({"portfolio": portfolio.identifier, "symbol": symbol})
+                .find({"portfolio": portfolio.id, "symbol": symbol})
 
         return position
 
     def _sync_portfolio_with_created_buy_order(self, order):
         position = self.position_repository.get(order.position_id)
         portfolio = self.portfolio_repository.get(position.portfolio_id)
         trading_symbol_position = self.position_repository.find(
             {
-                "portfolio": portfolio.identifier,
+                "portfolio": portfolio.id,
                 "symbol": portfolio.trading_symbol
             }
         )
         self.portfolio_repository.update(
             portfolio.id,
             {"unallocated": portfolio.unallocated - order.amount * order.price}
         )
@@ -306,25 +323,33 @@
             {
                 "amount": position.amount - order.amount
             }
         )
 
     def _sync_portfolio_with_executed_buy_order(self, order):
         position = self.position_repository.get(order.position_id)
-        self.position_cost_repository.create(
+        position_cost = self.position_cost_repository.create(
             {
                 "position_id": position.id,
                 "price": order.price,
                 "amount": order.amount,
                 "created_at": order.created_at,
             }
         )
         self.position_repository.update(
             position.id, {"amount": position.amount + order.amount}
         )
+        cost = position_cost.price * position_cost.amount
+        portfolio = self.portfolio_repository.get(position.portfolio_id)
+        self.portfolio_repository.update(
+            portfolio.id,
+            {
+                "total_cost": portfolio.total_cost + cost,
+            }
+        )
 
     def _sync_portfolio_with_executed_sell_order(self, order):
         position = self.position_repository.get(order.position_id)
         portfolio = self.portfolio_repository.get(position.portfolio_id)
         amount_to_sell = order.amount
         net_gain = 0
         revenue = order.amount * order.price
@@ -372,14 +397,15 @@
 
         # Update the portfolio
         self.portfolio_repository.update(
             portfolio.id,
             {
                 "unallocated": portfolio.unallocated + revenue,
                 "total_net_gain": portfolio.total_net_gain + net_gain,
+                "net_size": portfolio.net_size + revenue,
             }
         )
 
     def _sync_portfolio_with_cancelled_buy_order(self, order):
         position = self.position_repository.find({"id": order.position_id})
         portfolio = self.portfolio_repository.get(position.portfolio_id)
 
@@ -418,7 +444,21 @@
         position = self.position_repository.find({"id": order.position_id})
         self.position_repository.update(
             position.id,
             {
                 "amount": position.amount + order.amount
             }
         )
+
+    def cancel_order(self, order_id):
+        self.check_pending_orders()
+        order = self.order_repository.get(order_id)
+
+        if order is not None:
+
+            if OrderStatus.OPEN.equals(order.status):
+                portfolio = self.portfolio_repository\
+                    .find({"position": order.position_id})
+                portfolio_configuration = self.portfolio_configuration_service\
+                    .get(portfolio.identifier)
+                self.market_service.initialize(portfolio_configuration)
+                self.market_service.cancel_order(order_id)
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/services/portfolio_configuration_service.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/services/portfolio_configuration_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     def get(self, identifier):
         portfolio_configuration = next(
             (portfolio_configuration for portfolio_configuration in
                 self.portfolio_configurations if
                 portfolio_configuration.market == identifier.lower()),
             None
         )
+
         if portfolio_configuration is None:
             raise ApiException('Portfolio configuration not found', 404)
 
         return portfolio_configuration
 
     def find(self, query_params):
         market = query_params.get("market", None)
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/services/portfolio_service.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/services/portfolio_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,21 @@
     ):
         self.market_service = market_service
         self.position_repository = position_repository
         self.portfolio_configuration_service = portfolio_configuration_service
         self.order_service = order_service
         super(PortfolioService, self).__init__(portfolio_repository)
 
+    def find(self, query_params):
+        portfolio = self.repository.find(query_params)
+        portfolio_configuration = self.portfolio_configuration_service\
+            .get(portfolio.identifier)
+        portfolio.configuration = portfolio_configuration
+        return portfolio
+
     def create(self, data):
         unallocated = data.get("unallocated", 0)
         del data["unallocated"]
         portfolio = super(PortfolioService, self).create(data)
         self.position_repository.create(
             {
                 "symbol": portfolio.get_trading_symbol(),
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/services/position_service.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/services/position_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/services/repository_service.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/services/repository_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/services/strategy_orchestrator_service.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/services/strategy_orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework/setup_logging.py` & `investing_algorithm_framework-1.3/investing_algorithm_framework/setup_logging.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework.egg-info/PKG-INFO` & `investing_algorithm_framework-1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,27 @@
-Metadata-Version: 2.1
-Name: investing-algorithm-framework
-Version: 1.2
-Summary: A framework for creating an investment algorithm
-Home-page: https://github.com/coding-kitties/investing-algorithm-framework.git
-Download-URL: https://github.com/coding-kitties/investing-algorithm-framework/archive/v0.1.1.tar.gz
-Author: coding kitties
-License: Apache License 2.0
-Keywords: TRADING,INVESTING,BOT,ALGORITHM,FRAMEWORK
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.md
-
 <a href=https://investing-algorithm-framework.com><img src="https://img.shields.io/badge/docs-website-brightgreen"></a>
 [![Build](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml/badge.svg)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/build.yml)
 [![Tests](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/coding-kitties/investing-algorithm-framework/actions/workflows/test.yml)
 [![Downloads](https://pepy.tech/badge/investing-algorithm-framework)](https://pepy.tech/badge/investing-algorithm-framework)
 [![Current Version](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)](https://img.shields.io/pypi/v/investing_algorithm_framework.svg)
 <a href="https://www.reddit.com/r/InvestingBots/"><img src="https://img.shields.io/reddit/subreddit-subscribers/investingbots?style=social"></a>
 ###### Sponsors
 <p align="left">
 <a href="https://logicfunds.io">
   <img alt="logicfunds" src="https://logicfunds-web-app-images.s3.eu-central-1.amazonaws.com/logicfunds-logo.png" width="200px" />
 </a>
 </p>
 
-# Investing Algorithm Framework
-The Investing Algorithm Framework is a python framework for building
-investment algorithms. It encourages rapid development and clean, pragmatic code design.
 
-The framework provides you with all the components you need to create an 
-investing algorithm (data providing, portfolio management, order execution, etc..). Also,
-it has various deployment options, such as web server, stateless, etc..
+# [Investing Algorithm Framework](https://github.com/coding-kitties/investing-algorithm-framework)
+
+The Investing Algorithm Framework is a Python tool that enables swift and 
+elegant development of investment algorithms and trading bots. It comes with all the necessary 
+components for creating algorithms, including data provisioning, portfolio management, and order execution.
+
 
 ## Example
 The following algorithm connects to binance and buys BTC every 5 seconds. 
 It also exposes an REST API that allows you to interact with the algorithm.
 ```python
 import pathlib
 from datetime import datetime, timedelta
```

### Comparing `investing_algorithm_framework-1.2/investing_algorithm_framework.egg-info/SOURCES.txt` & `investing_algorithm_framework-1.3/investing_algorithm_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/setup.py` & `investing_algorithm_framework-1.3/setup.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-1.2/tests/test_create_app.py` & `investing_algorithm_framework-1.3/tests/test_create_app.py`

 * *Files identical despite different names*

