# Comparing `tmp/fintekkers-ledger-models-0.1.50.tar.gz` & `tmp/fintekkers-ledger-models-0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fintekkers-ledger-models-0.1.50.tar", last modified: Mon Jun 12 14:48:12 2023, max compression
+gzip compressed data, was "fintekkers-ledger-models-0.1.51.tar", last modified: Thu Aug  3 15:22:53 2023, max compression
```

## Comparing `fintekkers-ledger-models-0.1.50.tar` & `fintekkers-ledger-models-0.1.51.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.476071 fintekkers-ledger-models-0.1.50/fintekkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.476071 fintekkers-ledger-models-0.1.50/fintekkers/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.476071 fintekkers-ledger-models-0.1.50/fintekkers/models/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/portfolio/portfolio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/portfolio/portfolio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/portfolio/portfolio_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.480071 fintekkers-ledger-models-0.1.50/fintekkers/models/position/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/field_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/field_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/field_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/measure_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/measure_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/measure_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_filter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_filter_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_filter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_util_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_util_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_util_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.480071 fintekkers-ledger-models-0.1.50/fintekkers/models/price/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/price/price_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/price/price_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/price/price_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.484071 fintekkers-ledger-models-0.1.50/fintekkers/models/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/coupon_frequency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/coupon_frequency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/coupon_frequency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/coupon_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/coupon_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/coupon_type_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.484071 fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/identifier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/identifier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/identifier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/identifier_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/identifier_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/identifier_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_quantity_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_quantity_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_quantity_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/tenor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/tenor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/tenor_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/tenor_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/tenor_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/security/tenor_type_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.488071 fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/strategy_allocation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/strategy_allocation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/strategy_allocation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/strategy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/strategy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/strategy_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.488071 fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/transaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/transaction_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/transaction_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/transaction_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/transaction_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/transaction_type_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.492071 fintekkers-ledger-models-0.1.50/fintekkers/models/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/decimal_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/decimal_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/decimal_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/endpoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/endpoint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/endpoint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/local_date_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/local_date_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/local_date_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/local_timestamp_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/local_timestamp_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/local_timestamp_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.492071 fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/node_partition_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/node_partition_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/node_partition_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/node_state_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/node_state_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/node_state_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/uuid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/uuid_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/models/util/uuid_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.496071 fintekkers-ledger-models-0.1.50/fintekkers/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.496071 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/create_portfolio_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/create_portfolio_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/create_portfolio_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/create_portfolio_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/create_portfolio_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/create_portfolio_response_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/query_portfolio_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/query_portfolio_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/query_portfolio_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/query_portfolio_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/query_portfolio_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/query_portfolio_response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.496071 fintekkers-ledger-models-0.1.50/fintekkers/requests/position/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/position/query_position_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/position/query_position_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/position/query_position_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/position/query_position_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/position/query_position_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/position/query_position_response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.500071 fintekkers-ledger-models-0.1.50/fintekkers/requests/price/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/price/create_price_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/price/create_price_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/price/query_price_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/price/query_price_response_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.500071 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/create_security_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/create_security_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/create_security_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/create_security_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/create_security_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/create_security_response_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/query_security_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/query_security_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/query_security_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/query_security_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/query_security_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/security/query_security_response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.500071 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/create_transaction_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/create_transaction_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/create_transaction_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/create_transaction_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/create_transaction_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/create_transaction_response_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/query_transaction_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/query_transaction_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/query_transaction_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/query_transaction_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/query_transaction_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/query_transaction_response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.500071 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.500071 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/error_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/error_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/message_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/summary_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/summary_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.500071 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/lock_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/lock_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/lock_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/lock_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/lock_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/lock_response_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/operation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/util/operation_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/valuation_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/valuation_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/valuation_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/valuation_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/valuation_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/valuation_response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/services/lock_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/lock_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/lock_service/lock_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/lock_service/lock_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/lock_service/lock_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/services/portfolio_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/portfolio_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/portfolio_service/portfolio_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/portfolio_service/portfolio_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/portfolio_service/portfolio_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/services/position_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/position_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/position_service/position_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/position_service/position_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/position_service/position_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/services/price_service/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/price_service/price_service_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/services/security_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/security_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/security_service/security_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/security_service/security_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/security_service/security_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/services/transaction_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/transaction_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/transaction_service/transaction_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/transaction_service/transaction_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/transaction_service/transaction_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/services/valuation_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/valuation_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/valuation_service/valuation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/valuation_service/valuation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/services/valuation_service/valuation_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/security_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/tenor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/util/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/util/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/util/fintekkers_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/util/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/requests/security.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/requests/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/fintekkers/wrappers/services/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/fintekkers_ledger_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-12 14:48:12.000000 fintekkers-ledger-models-0.1.50/fintekkers_ledger_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-06-12 14:48:12.000000 fintekkers-ledger-models-0.1.50/fintekkers_ledger_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:48:12.000000 fintekkers-ledger-models-0.1.50/fintekkers_ledger_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 14:48:12.000000 fintekkers-ledger-models-0.1.50/fintekkers_ledger_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 14:48:12.504071 fintekkers-ledger-models-0.1.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-12 14:48:11.000000 fintekkers-ledger-models-0.1.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.927176 fintekkers-ledger-models-0.1.51/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-03 15:22:53.927176 fintekkers-ledger-models-0.1.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.895176 fintekkers-ledger-models-0.1.51/fintekkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.895176 fintekkers-ledger-models-0.1.51/fintekkers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.895176 fintekkers-ledger-models-0.1.51/fintekkers/models/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/portfolio/portfolio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/portfolio/portfolio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/portfolio/portfolio_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.899176 fintekkers-ledger-models-0.1.51/fintekkers/models/position/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/field_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/field_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/field_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/measure_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/measure_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/measure_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_filter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_filter_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_filter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_util_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_util_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_util_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.899176 fintekkers-ledger-models-0.1.51/fintekkers/models/price/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/price/price_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/price/price_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/price/price_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.903176 fintekkers-ledger-models-0.1.51/fintekkers/models/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/coupon_frequency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/coupon_frequency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/coupon_frequency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/coupon_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/coupon_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/coupon_type_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.903176 fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/identifier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/identifier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/identifier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/identifier_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/identifier_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/identifier_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_quantity_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_quantity_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_quantity_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/tenor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/tenor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/tenor_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/tenor_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/tenor_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/security/tenor_type_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.903176 fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/strategy_allocation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/strategy_allocation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/strategy_allocation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/strategy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/strategy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/strategy_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.903176 fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/transaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/transaction_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/transaction_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/transaction_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/transaction_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/transaction_type_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.907176 fintekkers-ledger-models-0.1.51/fintekkers/models/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/decimal_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/decimal_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/decimal_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/endpoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/endpoint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/endpoint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/local_date_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/local_date_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/local_date_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/local_timestamp_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/local_timestamp_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/local_timestamp_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.907176 fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/node_partition_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/node_partition_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/node_partition_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/node_state_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/node_state_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/node_state_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/uuid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/uuid_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/models/util/uuid_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.907176 fintekkers-ledger-models-0.1.51/fintekkers/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.911176 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/create_portfolio_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/create_portfolio_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/create_portfolio_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/create_portfolio_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/create_portfolio_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/create_portfolio_response_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/query_portfolio_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/query_portfolio_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/query_portfolio_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/query_portfolio_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/query_portfolio_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/query_portfolio_response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.911176 fintekkers-ledger-models-0.1.51/fintekkers/requests/position/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/position/query_position_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/position/query_position_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/position/query_position_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/position/query_position_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/position/query_position_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/position/query_position_response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.911176 fintekkers-ledger-models-0.1.51/fintekkers/requests/price/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/price/create_price_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/price/create_price_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/price/query_price_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/price/query_price_response_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.915176 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/create_security_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/create_security_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/create_security_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/create_security_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/create_security_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/create_security_response_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/query_security_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/query_security_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/query_security_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/query_security_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/query_security_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/security/query_security_response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.915176 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/create_transaction_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/create_transaction_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/create_transaction_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/create_transaction_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/create_transaction_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/create_transaction_response_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/query_transaction_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/query_transaction_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/query_transaction_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/query_transaction_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/query_transaction_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/query_transaction_response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.915176 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.919176 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/error_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/error_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/message_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/summary_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/summary_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.919176 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/lock_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/lock_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/lock_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/lock_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/lock_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/lock_response_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/operation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/util/operation_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.919176 fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/valuation_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/valuation_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/valuation_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/valuation_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/valuation_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/valuation_response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.919176 fintekkers-ledger-models-0.1.51/fintekkers/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.919176 fintekkers-ledger-models-0.1.51/fintekkers/services/lock_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/lock_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/lock_service/lock_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/lock_service/lock_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/lock_service/lock_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.923176 fintekkers-ledger-models-0.1.51/fintekkers/services/portfolio_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/portfolio_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/portfolio_service/portfolio_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/portfolio_service/portfolio_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/portfolio_service/portfolio_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.923176 fintekkers-ledger-models-0.1.51/fintekkers/services/position_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/position_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/position_service/position_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/position_service/position_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/position_service/position_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.923176 fintekkers-ledger-models-0.1.51/fintekkers/services/price_service/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/price_service/price_service_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.923176 fintekkers-ledger-models-0.1.51/fintekkers/services/security_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/security_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/security_service/security_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/security_service/security_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/security_service/security_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.923176 fintekkers-ledger-models-0.1.51/fintekkers/services/transaction_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/transaction_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/transaction_service/transaction_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/transaction_service/transaction_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/transaction_service/transaction_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.923176 fintekkers-ledger-models-0.1.51/fintekkers/services/valuation_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/valuation_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/valuation_service/valuation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/valuation_service/valuation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/services/valuation_service/valuation_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.923176 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.923176 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/security_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/tenor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.927176 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/util/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/util/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/util/fintekkers_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/util/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.927176 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/requests/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/requests/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.927176 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/fintekkers/wrappers/services/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:22:53.927176 fintekkers-ledger-models-0.1.51/fintekkers_ledger_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-03 15:22:53.000000 fintekkers-ledger-models-0.1.51/fintekkers_ledger_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-08-03 15:22:53.000000 fintekkers-ledger-models-0.1.51/fintekkers_ledger_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:22:53.000000 fintekkers-ledger-models-0.1.51/fintekkers_ledger_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 15:22:53.000000 fintekkers-ledger-models-0.1.51/fintekkers_ledger_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-03 15:22:53.927176 fintekkers-ledger-models-0.1.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-03 15:22:52.000000 fintekkers-ledger-models-0.1.51/setup.py
```

### Comparing `fintekkers-ledger-models-0.1.50/PKG-INFO` & `fintekkers-ledger-models-0.1.51/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fintekkers-ledger-models
-Version: 0.1.50
+Version: 0.1.51
 Summary: Fintekkers Ledger Models python package
 Home-page: https://github.com/fintekkers/ledger-models
 Author: David Doherty
 Author-email: dave@fintekkers.org
 License: MIT
 Keywords: fintekkers ledger models
 Platform: UNKNOWN
```

### Comparing `fintekkers-ledger-models-0.1.50/README.rst` & `fintekkers-ledger-models-0.1.51/README.rst`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/portfolio/portfolio_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/portfolio/portfolio_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 _sym_db = _symbol_database.Default()
 
 
 from fintekkers.models.util import local_timestamp_pb2 as fintekkers_dot_models_dot_util_dot_local__timestamp__pb2
 from fintekkers.models.util import uuid_pb2 as fintekkers_dot_models_dot_util_dot_uuid__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+fintekkers/models/portfolio/portfolio.proto\x12\x1b\x66intekkers.models.portfolio\x1a,fintekkers/models/util/local_timestamp.proto\x1a!fintekkers/models/util/uuid.proto\"\xcd\x01\n\x0ePortfolioProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x04uuid\x18\x05 \x01(\x0b\x32!.fintekkers.models.util.UUIDProto\x12:\n\x05\x61s_of\x18\x06 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x0f\n\x07is_link\x18\x07 \x01(\x08\x12\x16\n\x0eportfolio_name\x18\n \x01(\tB\x13\x42\x0fPortfolioProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+fintekkers/models/portfolio/portfolio.proto\x12\x1b\x66intekkers.models.portfolio\x1a,fintekkers/models/util/local_timestamp.proto\x1a!fintekkers/models/util/uuid.proto\"\xcd\x02\n\x0ePortfolioProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x04uuid\x18\x05 \x01(\x0b\x32!.fintekkers.models.util.UUIDProto\x12:\n\x05\x61s_of\x18\x06 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x0f\n\x07is_link\x18\x07 \x01(\x08\x12?\n\nvalid_from\x18\x08 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12=\n\x08valid_to\x18\t \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x16\n\x0eportfolio_name\x18\n \x01(\tB\x13\x42\x0fPortfolioProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.models.portfolio.portfolio_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\017PortfolioProtosP\001'
   _PORTFOLIOPROTO._serialized_start=158
-  _PORTFOLIOPROTO._serialized_end=363
+  _PORTFOLIOPROTO._serialized_end=491
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/portfolio/portfolio_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/query_portfolio_request_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from fintekkers.models.util import local_timestamp_pb2 as _local_timestamp_pb2
 from fintekkers.models.util import uuid_pb2 as _uuid_pb2
+from fintekkers.models.util import local_timestamp_pb2 as _local_timestamp_pb2
+from fintekkers.models.position import position_filter_pb2 as _position_filter_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class PortfolioProto(_message.Message):
-    __slots__ = ["as_of", "is_link", "object_class", "portfolio_name", "uuid", "version"]
+class QueryPortfolioRequestProto(_message.Message):
+    __slots__ = ["as_of", "object_class", "search_portfolio_input", "uuIds", "version"]
     AS_OF_FIELD_NUMBER: _ClassVar[int]
-    IS_LINK_FIELD_NUMBER: _ClassVar[int]
     OBJECT_CLASS_FIELD_NUMBER: _ClassVar[int]
-    PORTFOLIO_NAME_FIELD_NUMBER: _ClassVar[int]
-    UUID_FIELD_NUMBER: _ClassVar[int]
+    SEARCH_PORTFOLIO_INPUT_FIELD_NUMBER: _ClassVar[int]
+    UUIDS_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     as_of: _local_timestamp_pb2.LocalTimestampProto
-    is_link: bool
     object_class: str
-    portfolio_name: str
-    uuid: _uuid_pb2.UUIDProto
+    search_portfolio_input: _position_filter_pb2.PositionFilterProto
+    uuIds: _containers.RepeatedCompositeFieldContainer[_uuid_pb2.UUIDProto]
     version: str
-    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuid: _Optional[_Union[_uuid_pb2.UUIDProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., is_link: bool = ..., portfolio_name: _Optional[str] = ...) -> None: ...
+    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuIds: _Optional[_Iterable[_Union[_uuid_pb2.UUIDProto, _Mapping]]] = ..., search_portfolio_input: _Optional[_Union[_position_filter_pb2.PositionFilterProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ...) -> None: ...
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/field_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/field_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/field_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/field_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/measure_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/measure_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/measure_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/measure_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_filter_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_filter_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_status_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_status_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_util_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_util_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from fintekkers.models.position import field_pb2 as fintekkers_dot_models_dot_position_dot_field__pb2
 from fintekkers.models.position import measure_pb2 as fintekkers_dot_models_dot_position_dot_measure__pb2
 from fintekkers.models.util import decimal_value_pb2 as fintekkers_dot_models_dot_util_dot_decimal__value__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.fintekkers/models/position/position_util.proto\x12\x1a\x66intekkers.models.position\x1a\x19google/protobuf/any.proto\x1a&fintekkers/models/position/field.proto\x1a(fintekkers/models/position/measure.proto\x1a*fintekkers/models/util/decimal_value.proto\"\x96\x01\n\x0fMeasureMapEntry\x12\x39\n\x07measure\x18\x01 \x01(\x0e\x32(.fintekkers.models.position.MeasureProto\x12H\n\x15measure_decimal_value\x18\x02 \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\"\xec\x01\n\rFieldMapEntry\x12\x35\n\x05\x66ield\x18\x01 \x01(\x0e\x32&.fintekkers.models.position.FieldProto\x12\x32\n\x12\x66ield_value_packed\x18\x04 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x12\x14\n\nenum_value\x18\x05 \x01(\x05H\x00\x12\x44\n\x08operator\x18\x14 \x01(\x0e\x32\x32.fintekkers.models.position.PositionFilterOperatorB\x14\n\x12\x46ieldMapValueOneOf*\x9a\x01\n\x16PositionFilterOperator\x12\x14\n\x10UNKNOWN_OPERATOR\x10\x00\x12\n\n\x06\x45QUALS\x10\x01\x12\x0e\n\nNOT_EQUALS\x10\x02\x12\r\n\tLESS_THAN\x10\x03\x12\x17\n\x13LESS_THAN_OR_EQUALS\x10\x04\x12\r\n\tMORE_THAN\x10\x05\x12\x17\n\x13MORE_THAN_OR_EQUALS\x10\x06\x42\x16\x42\x12PositionUtilProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.fintekkers/models/position/position_util.proto\x12\x1a\x66intekkers.models.position\x1a\x19google/protobuf/any.proto\x1a&fintekkers/models/position/field.proto\x1a(fintekkers/models/position/measure.proto\x1a*fintekkers/models/util/decimal_value.proto\"\x96\x01\n\x0fMeasureMapEntry\x12\x39\n\x07measure\x18\x01 \x01(\x0e\x32(.fintekkers.models.position.MeasureProto\x12H\n\x15measure_decimal_value\x18\x02 \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\"\x84\x02\n\rFieldMapEntry\x12\x35\n\x05\x66ield\x18\x01 \x01(\x0e\x32&.fintekkers.models.position.FieldProto\x12\x32\n\x12\x66ield_value_packed\x18\x04 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x12\x14\n\nenum_value\x18\x05 \x01(\x05H\x00\x12\x16\n\x0cstring_value\x18\x06 \x01(\tH\x00\x12\x44\n\x08operator\x18\x14 \x01(\x0e\x32\x32.fintekkers.models.position.PositionFilterOperatorB\x14\n\x12\x46ieldMapValueOneOf*\x9a\x01\n\x16PositionFilterOperator\x12\x14\n\x10UNKNOWN_OPERATOR\x10\x00\x12\n\n\x06\x45QUALS\x10\x01\x12\x0e\n\nNOT_EQUALS\x10\x02\x12\r\n\tLESS_THAN\x10\x03\x12\x17\n\x13LESS_THAN_OR_EQUALS\x10\x04\x12\r\n\tMORE_THAN\x10\x05\x12\x17\n\x13MORE_THAN_OR_EQUALS\x10\x06\x42\x16\x42\x12PositionUtilProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.models.position.position_util_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\022PositionUtilProtosP\001'
-  _POSITIONFILTEROPERATOR._serialized_start=624
-  _POSITIONFILTEROPERATOR._serialized_end=778
+  _POSITIONFILTEROPERATOR._serialized_start=648
+  _POSITIONFILTEROPERATOR._serialized_end=802
   _MEASUREMAPENTRY._serialized_start=232
   _MEASUREMAPENTRY._serialized_end=382
   _FIELDMAPENTRY._serialized_start=385
-  _FIELDMAPENTRY._serialized_end=621
+  _FIELDMAPENTRY._serialized_end=645
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/position/position_util_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/position/position_util_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 LESS_THAN_OR_EQUALS: PositionFilterOperator
 MORE_THAN: PositionFilterOperator
 MORE_THAN_OR_EQUALS: PositionFilterOperator
 NOT_EQUALS: PositionFilterOperator
 UNKNOWN_OPERATOR: PositionFilterOperator
 
 class FieldMapEntry(_message.Message):
-    __slots__ = ["enum_value", "field", "field_value_packed", "operator"]
+    __slots__ = ["enum_value", "field", "field_value_packed", "operator", "string_value"]
     ENUM_VALUE_FIELD_NUMBER: _ClassVar[int]
     FIELD_FIELD_NUMBER: _ClassVar[int]
     FIELD_VALUE_PACKED_FIELD_NUMBER: _ClassVar[int]
     OPERATOR_FIELD_NUMBER: _ClassVar[int]
+    STRING_VALUE_FIELD_NUMBER: _ClassVar[int]
     enum_value: int
     field: _field_pb2.FieldProto
     field_value_packed: _any_pb2.Any
     operator: PositionFilterOperator
-    def __init__(self, field: _Optional[_Union[_field_pb2.FieldProto, str]] = ..., field_value_packed: _Optional[_Union[_any_pb2.Any, _Mapping]] = ..., enum_value: _Optional[int] = ..., operator: _Optional[_Union[PositionFilterOperator, str]] = ...) -> None: ...
+    string_value: str
+    def __init__(self, field: _Optional[_Union[_field_pb2.FieldProto, str]] = ..., field_value_packed: _Optional[_Union[_any_pb2.Any, _Mapping]] = ..., enum_value: _Optional[int] = ..., string_value: _Optional[str] = ..., operator: _Optional[_Union[PositionFilterOperator, str]] = ...) -> None: ...
 
 class MeasureMapEntry(_message.Message):
     __slots__ = ["measure", "measure_decimal_value"]
     MEASURE_DECIMAL_VALUE_FIELD_NUMBER: _ClassVar[int]
     MEASURE_FIELD_NUMBER: _ClassVar[int]
     measure: _measure_pb2.MeasureProto
     measure_decimal_value: _decimal_value_pb2.DecimalValueProto
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/price/price_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/price/price_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 from fintekkers.models.util import decimal_value_pb2 as fintekkers_dot_models_dot_util_dot_decimal__value__pb2
 from fintekkers.models.util import local_timestamp_pb2 as fintekkers_dot_models_dot_util_dot_local__timestamp__pb2
 from fintekkers.models.util import uuid_pb2 as fintekkers_dot_models_dot_util_dot_uuid__pb2
 from fintekkers.models.security import security_pb2 as fintekkers_dot_models_dot_security_dot_security__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#fintekkers/models/price/price.proto\x12\x17\x66intekkers.models.price\x1a*fintekkers/models/util/decimal_value.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a!fintekkers/models/util/uuid.proto\x1a)fintekkers/models/security/security.proto\"\xa8\x02\n\nPriceProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x04uuid\x18\x05 \x01(\x0b\x32!.fintekkers.models.util.UUIDProto\x12:\n\x05\x61s_of\x18\x06 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x0f\n\x07is_link\x18\x07 \x01(\x08\x12\x38\n\x05price\x18\n \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\x12;\n\x08security\x18\x0b \x01(\x0b\x32).fintekkers.models.security.SecurityProtoB\x0f\x42\x0bPriceProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#fintekkers/models/price/price.proto\x12\x17\x66intekkers.models.price\x1a*fintekkers/models/util/decimal_value.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a!fintekkers/models/util/uuid.proto\x1a)fintekkers/models/security/security.proto\"\xa8\x03\n\nPriceProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x04uuid\x18\x05 \x01(\x0b\x32!.fintekkers.models.util.UUIDProto\x12:\n\x05\x61s_of\x18\x06 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x0f\n\x07is_link\x18\x07 \x01(\x08\x12?\n\nvalid_from\x18\x08 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12=\n\x08valid_to\x18\t \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x38\n\x05price\x18\n \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\x12;\n\x08security\x18\x0b \x01(\x0b\x32).fintekkers.models.security.SecurityProtoB\x0f\x42\x0bPriceProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.models.price.price_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\013PriceProtosP\001'
   _PRICEPROTO._serialized_start=233
-  _PRICEPROTO._serialized_end=529
+  _PRICEPROTO._serialized_end=657
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/price/price_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/security/query_security_request_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-from fintekkers.models.util import decimal_value_pb2 as _decimal_value_pb2
-from fintekkers.models.util import local_timestamp_pb2 as _local_timestamp_pb2
 from fintekkers.models.util import uuid_pb2 as _uuid_pb2
-from fintekkers.models.security import security_pb2 as _security_pb2
+from fintekkers.models.util import local_timestamp_pb2 as _local_timestamp_pb2
+from fintekkers.models.position import position_filter_pb2 as _position_filter_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class PriceProto(_message.Message):
-    __slots__ = ["as_of", "is_link", "object_class", "price", "security", "uuid", "version"]
+class QuerySecurityRequestProto(_message.Message):
+    __slots__ = ["as_of", "object_class", "search_security_input", "uuIds", "version"]
     AS_OF_FIELD_NUMBER: _ClassVar[int]
-    IS_LINK_FIELD_NUMBER: _ClassVar[int]
     OBJECT_CLASS_FIELD_NUMBER: _ClassVar[int]
-    PRICE_FIELD_NUMBER: _ClassVar[int]
-    SECURITY_FIELD_NUMBER: _ClassVar[int]
-    UUID_FIELD_NUMBER: _ClassVar[int]
+    SEARCH_SECURITY_INPUT_FIELD_NUMBER: _ClassVar[int]
+    UUIDS_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     as_of: _local_timestamp_pb2.LocalTimestampProto
-    is_link: bool
     object_class: str
-    price: _decimal_value_pb2.DecimalValueProto
-    security: _security_pb2.SecurityProto
-    uuid: _uuid_pb2.UUIDProto
+    search_security_input: _position_filter_pb2.PositionFilterProto
+    uuIds: _containers.RepeatedCompositeFieldContainer[_uuid_pb2.UUIDProto]
     version: str
-    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuid: _Optional[_Union[_uuid_pb2.UUIDProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., is_link: bool = ..., price: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ..., security: _Optional[_Union[_security_pb2.SecurityProto, _Mapping]] = ...) -> None: ...
+    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuIds: _Optional[_Iterable[_Union[_uuid_pb2.UUIDProto, _Mapping]]] = ..., search_security_input: _Optional[_Union[_position_filter_pb2.PositionFilterProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ...) -> None: ...
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/coupon_frequency_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/coupon_frequency_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/coupon_frequency_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/coupon_frequency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/coupon_type_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/coupon_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/identifier_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/identifier_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/identifier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/identifier_type_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/identifier_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/identifier/identifier_type_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/identifier/identifier_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from fintekkers.models.security.identifier import identifier_pb2 as fintekkers_dot_models_dot_security_dot_identifier_dot_identifier__pb2
 from fintekkers.models.security import security_type_pb2 as fintekkers_dot_models_dot_security_dot_security__type__pb2
 from fintekkers.models.security import security_quantity_type_pb2 as fintekkers_dot_models_dot_security_dot_security__quantity__type__pb2
 from fintekkers.models.security import coupon_frequency_pb2 as fintekkers_dot_models_dot_security_dot_coupon__frequency__pb2
 from fintekkers.models.security import coupon_type_pb2 as fintekkers_dot_models_dot_security_dot_coupon__type__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)fintekkers/models/security/security.proto\x12\x1a\x66intekkers.models.security\x1a*fintekkers/models/util/decimal_value.proto\x1a\'fintekkers/models/util/local_date.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a!fintekkers/models/util/uuid.proto\x1a\x36\x66intekkers/models/security/identifier/identifier.proto\x1a.fintekkers/models/security/security_type.proto\x1a\x37\x66intekkers/models/security/security_quantity_type.proto\x1a\x31\x66intekkers/models/security/coupon_frequency.proto\x1a,fintekkers/models/security/coupon_type.proto\"\xe5\x07\n\rSecurityProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x04uuid\x18\x05 \x01(\x0b\x32!.fintekkers.models.util.UUIDProto\x12:\n\x05\x61s_of\x18\x06 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x0f\n\x07is_link\x18\x07 \x01(\x08\x12\x44\n\rsecurity_type\x18\n \x01(\x0e\x32-.fintekkers.models.security.SecurityTypeProto\x12\x13\n\x0b\x61sset_class\x18\x0b \x01(\t\x12\x13\n\x0bissuer_name\x18\x0c \x01(\t\x12\x46\n\x13settlement_currency\x18\r \x01(\x0b\x32).fintekkers.models.security.SecurityProto\x12L\n\rquantity_type\x18\x0e \x01(\x0e\x32\x35.fintekkers.models.security.SecurityQuantityTypeProto\x12?\n\nidentifier\x18( \x01(\x0b\x32+.fintekkers.models.security.IdentifierProto\x12\x13\n\x0b\x64\x65scription\x18) \x01(\t\x12\x0f\n\x07\x63\x61sh_id\x18\x32 \x01(\t\x12>\n\x0b\x63oupon_rate\x18< \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\x12@\n\x0b\x63oupon_type\x18= \x01(\x0e\x32+.fintekkers.models.security.CouponTypeProto\x12J\n\x10\x63oupon_frequency\x18> \x01(\x0e\x32\x30.fintekkers.models.security.CouponFrequencyProto\x12:\n\ndated_date\x18? \x01(\x0b\x32&.fintekkers.models.util.LocalDateProto\x12=\n\nface_value\x18@ \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\x12:\n\nissue_date\x18\x41 \x01(\x0b\x32&.fintekkers.models.util.LocalDateProto\x12=\n\rmaturity_date\x18\x42 \x01(\x0b\x32&.fintekkers.models.util.LocalDateProtoB\x12\x42\x0eSecurityProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)fintekkers/models/security/security.proto\x12\x1a\x66intekkers.models.security\x1a*fintekkers/models/util/decimal_value.proto\x1a\'fintekkers/models/util/local_date.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a!fintekkers/models/util/uuid.proto\x1a\x36\x66intekkers/models/security/identifier/identifier.proto\x1a.fintekkers/models/security/security_type.proto\x1a\x37\x66intekkers/models/security/security_quantity_type.proto\x1a\x31\x66intekkers/models/security/coupon_frequency.proto\x1a,fintekkers/models/security/coupon_type.proto\"\xe5\x08\n\rSecurityProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x04uuid\x18\x05 \x01(\x0b\x32!.fintekkers.models.util.UUIDProto\x12:\n\x05\x61s_of\x18\x06 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x0f\n\x07is_link\x18\x07 \x01(\x08\x12?\n\nvalid_from\x18\x08 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12=\n\x08valid_to\x18\t \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x44\n\rsecurity_type\x18\n \x01(\x0e\x32-.fintekkers.models.security.SecurityTypeProto\x12\x13\n\x0b\x61sset_class\x18\x0b \x01(\t\x12\x13\n\x0bissuer_name\x18\x0c \x01(\t\x12\x46\n\x13settlement_currency\x18\r \x01(\x0b\x32).fintekkers.models.security.SecurityProto\x12L\n\rquantity_type\x18\x0e \x01(\x0e\x32\x35.fintekkers.models.security.SecurityQuantityTypeProto\x12?\n\nidentifier\x18( \x01(\x0b\x32+.fintekkers.models.security.IdentifierProto\x12\x13\n\x0b\x64\x65scription\x18) \x01(\t\x12\x0f\n\x07\x63\x61sh_id\x18\x32 \x01(\t\x12>\n\x0b\x63oupon_rate\x18< \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\x12@\n\x0b\x63oupon_type\x18= \x01(\x0e\x32+.fintekkers.models.security.CouponTypeProto\x12J\n\x10\x63oupon_frequency\x18> \x01(\x0e\x32\x30.fintekkers.models.security.CouponFrequencyProto\x12:\n\ndated_date\x18? \x01(\x0b\x32&.fintekkers.models.util.LocalDateProto\x12=\n\nface_value\x18@ \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\x12:\n\nissue_date\x18\x41 \x01(\x0b\x32&.fintekkers.models.util.LocalDateProto\x12=\n\rmaturity_date\x18\x42 \x01(\x0b\x32&.fintekkers.models.util.LocalDateProtoB\x12\x42\x0eSecurityProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.models.security.security_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\016SecurityProtosP\001'
   _SECURITYPROTO._serialized_start=498
-  _SECURITYPROTO._serialized_end=1495
+  _SECURITYPROTO._serialized_end=1623
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class SecurityProto(_message.Message):
-    __slots__ = ["as_of", "asset_class", "cash_id", "coupon_frequency", "coupon_rate", "coupon_type", "dated_date", "description", "face_value", "identifier", "is_link", "issue_date", "issuer_name", "maturity_date", "object_class", "quantity_type", "security_type", "settlement_currency", "uuid", "version"]
+    __slots__ = ["as_of", "asset_class", "cash_id", "coupon_frequency", "coupon_rate", "coupon_type", "dated_date", "description", "face_value", "identifier", "is_link", "issue_date", "issuer_name", "maturity_date", "object_class", "quantity_type", "security_type", "settlement_currency", "uuid", "valid_from", "valid_to", "version"]
     ASSET_CLASS_FIELD_NUMBER: _ClassVar[int]
     AS_OF_FIELD_NUMBER: _ClassVar[int]
     CASH_ID_FIELD_NUMBER: _ClassVar[int]
     COUPON_FREQUENCY_FIELD_NUMBER: _ClassVar[int]
     COUPON_RATE_FIELD_NUMBER: _ClassVar[int]
     COUPON_TYPE_FIELD_NUMBER: _ClassVar[int]
     DATED_DATE_FIELD_NUMBER: _ClassVar[int]
@@ -30,14 +30,16 @@
     IS_LINK_FIELD_NUMBER: _ClassVar[int]
     MATURITY_DATE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_CLASS_FIELD_NUMBER: _ClassVar[int]
     QUANTITY_TYPE_FIELD_NUMBER: _ClassVar[int]
     SECURITY_TYPE_FIELD_NUMBER: _ClassVar[int]
     SETTLEMENT_CURRENCY_FIELD_NUMBER: _ClassVar[int]
     UUID_FIELD_NUMBER: _ClassVar[int]
+    VALID_FROM_FIELD_NUMBER: _ClassVar[int]
+    VALID_TO_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     as_of: _local_timestamp_pb2.LocalTimestampProto
     asset_class: str
     cash_id: str
     coupon_frequency: _coupon_frequency_pb2.CouponFrequencyProto
     coupon_rate: _decimal_value_pb2.DecimalValueProto
     coupon_type: _coupon_type_pb2.CouponTypeProto
@@ -50,9 +52,11 @@
     issuer_name: str
     maturity_date: _local_date_pb2.LocalDateProto
     object_class: str
     quantity_type: _security_quantity_type_pb2.SecurityQuantityTypeProto
     security_type: _security_type_pb2.SecurityTypeProto
     settlement_currency: SecurityProto
     uuid: _uuid_pb2.UUIDProto
+    valid_from: _local_timestamp_pb2.LocalTimestampProto
+    valid_to: _local_timestamp_pb2.LocalTimestampProto
     version: str
-    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuid: _Optional[_Union[_uuid_pb2.UUIDProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., is_link: bool = ..., security_type: _Optional[_Union[_security_type_pb2.SecurityTypeProto, str]] = ..., asset_class: _Optional[str] = ..., issuer_name: _Optional[str] = ..., settlement_currency: _Optional[_Union[SecurityProto, _Mapping]] = ..., quantity_type: _Optional[_Union[_security_quantity_type_pb2.SecurityQuantityTypeProto, str]] = ..., identifier: _Optional[_Union[_identifier_pb2.IdentifierProto, _Mapping]] = ..., description: _Optional[str] = ..., cash_id: _Optional[str] = ..., coupon_rate: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ..., coupon_type: _Optional[_Union[_coupon_type_pb2.CouponTypeProto, str]] = ..., coupon_frequency: _Optional[_Union[_coupon_frequency_pb2.CouponFrequencyProto, str]] = ..., dated_date: _Optional[_Union[_local_date_pb2.LocalDateProto, _Mapping]] = ..., face_value: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ..., issue_date: _Optional[_Union[_local_date_pb2.LocalDateProto, _Mapping]] = ..., maturity_date: _Optional[_Union[_local_date_pb2.LocalDateProto, _Mapping]] = ...) -> None: ...
+    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuid: _Optional[_Union[_uuid_pb2.UUIDProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., is_link: bool = ..., valid_from: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., valid_to: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., security_type: _Optional[_Union[_security_type_pb2.SecurityTypeProto, str]] = ..., asset_class: _Optional[str] = ..., issuer_name: _Optional[str] = ..., settlement_currency: _Optional[_Union[SecurityProto, _Mapping]] = ..., quantity_type: _Optional[_Union[_security_quantity_type_pb2.SecurityQuantityTypeProto, str]] = ..., identifier: _Optional[_Union[_identifier_pb2.IdentifierProto, _Mapping]] = ..., description: _Optional[str] = ..., cash_id: _Optional[str] = ..., coupon_rate: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ..., coupon_type: _Optional[_Union[_coupon_type_pb2.CouponTypeProto, str]] = ..., coupon_frequency: _Optional[_Union[_coupon_frequency_pb2.CouponFrequencyProto, str]] = ..., dated_date: _Optional[_Union[_local_date_pb2.LocalDateProto, _Mapping]] = ..., face_value: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ..., issue_date: _Optional[_Union[_local_date_pb2.LocalDateProto, _Mapping]] = ..., maturity_date: _Optional[_Union[_local_date_pb2.LocalDateProto, _Mapping]] = ...) -> None: ...
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_quantity_type_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_quantity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/security_type_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/security_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/tenor_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/tenor_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/tenor_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/tenor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/security/tenor_type_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/security/tenor_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/strategy_allocation_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/strategy_allocation_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/strategy_allocation_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/strategy_allocation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/strategy_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/strategy_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 _sym_db = _symbol_database.Default()
 
 
 from fintekkers.models.util import local_timestamp_pb2 as fintekkers_dot_models_dot_util_dot_local__timestamp__pb2
 from fintekkers.models.util import uuid_pb2 as fintekkers_dot_models_dot_util_dot_uuid__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)fintekkers/models/strategy/strategy.proto\x12\x1a\x66intekkers.models.strategy\x1a,fintekkers/models/util/local_timestamp.proto\x1a!fintekkers/models/util/uuid.proto\"\x86\x02\n\rStrategyProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x04uuid\x18\x05 \x01(\x0b\x32!.fintekkers.models.util.UUIDProto\x12:\n\x05\x61s_of\x18\x06 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x0f\n\x07is_link\x18\x07 \x01(\x08\x12\x15\n\rstrategy_name\x18\n \x01(\t\x12\x39\n\x06parent\x18\x0b \x01(\x0b\x32).fintekkers.models.strategy.StrategyProtoB\x12\x42\x0eStrategyProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)fintekkers/models/strategy/strategy.proto\x12\x1a\x66intekkers.models.strategy\x1a,fintekkers/models/util/local_timestamp.proto\x1a!fintekkers/models/util/uuid.proto\"\x86\x03\n\rStrategyProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x04uuid\x18\x05 \x01(\x0b\x32!.fintekkers.models.util.UUIDProto\x12:\n\x05\x61s_of\x18\x06 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x0f\n\x07is_link\x18\x07 \x01(\x08\x12?\n\nvalid_from\x18\x08 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12=\n\x08valid_to\x18\t \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x15\n\rstrategy_name\x18\n \x01(\t\x12\x39\n\x06parent\x18\x0b \x01(\x0b\x32).fintekkers.models.strategy.StrategyProtoB\x12\x42\x0eStrategyProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.models.strategy.strategy_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\016StrategyProtosP\001'
   _STRATEGYPROTO._serialized_start=155
-  _STRATEGYPROTO._serialized_end=417
+  _STRATEGYPROTO._serialized_end=545
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/strategy/strategy_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/price/query_price_request_pb2.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from fintekkers.models.util import local_timestamp_pb2 as _local_timestamp_pb2
 from fintekkers.models.util import uuid_pb2 as _uuid_pb2
+from fintekkers.models.util import local_timestamp_pb2 as _local_timestamp_pb2
+from fintekkers.models.position import position_filter_pb2 as _position_filter_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class StrategyProto(_message.Message):
-    __slots__ = ["as_of", "is_link", "object_class", "parent", "strategy_name", "uuid", "version"]
+class QueryPriceRequestProto(_message.Message):
+    __slots__ = ["as_of", "object_class", "search_price_input", "uuIds", "version"]
     AS_OF_FIELD_NUMBER: _ClassVar[int]
-    IS_LINK_FIELD_NUMBER: _ClassVar[int]
     OBJECT_CLASS_FIELD_NUMBER: _ClassVar[int]
-    PARENT_FIELD_NUMBER: _ClassVar[int]
-    STRATEGY_NAME_FIELD_NUMBER: _ClassVar[int]
-    UUID_FIELD_NUMBER: _ClassVar[int]
+    SEARCH_PRICE_INPUT_FIELD_NUMBER: _ClassVar[int]
+    UUIDS_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     as_of: _local_timestamp_pb2.LocalTimestampProto
-    is_link: bool
     object_class: str
-    parent: StrategyProto
-    strategy_name: str
-    uuid: _uuid_pb2.UUIDProto
+    search_price_input: _position_filter_pb2.PositionFilterProto
+    uuIds: _containers.RepeatedCompositeFieldContainer[_uuid_pb2.UUIDProto]
     version: str
-    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuid: _Optional[_Union[_uuid_pb2.UUIDProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., is_link: bool = ..., strategy_name: _Optional[str] = ..., parent: _Optional[_Union[StrategyProto, _Mapping]] = ...) -> None: ...
+    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuIds: _Optional[_Iterable[_Union[_uuid_pb2.UUIDProto, _Mapping]]] = ..., search_price_input: _Optional[_Union[_position_filter_pb2.PositionFilterProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ...) -> None: ...
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/transaction_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/transaction_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 from fintekkers.models.strategy import strategy_allocation_pb2 as fintekkers_dot_models_dot_strategy_dot_strategy__allocation__pb2
 from fintekkers.models.security import security_pb2 as fintekkers_dot_models_dot_security_dot_security__pb2
 from fintekkers.models.price import price_pb2 as fintekkers_dot_models_dot_price_dot_price__pb2
 from fintekkers.models.position import position_status_pb2 as fintekkers_dot_models_dot_position_dot_position__status__pb2
 from fintekkers.models.transaction import transaction_type_pb2 as fintekkers_dot_models_dot_transaction_dot_transaction__type__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/fintekkers/models/transaction/transaction.proto\x12\x1d\x66intekkers.models.transaction\x1a*fintekkers/models/util/decimal_value.proto\x1a\'fintekkers/models/util/local_date.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a!fintekkers/models/util/uuid.proto\x1a+fintekkers/models/portfolio/portfolio.proto\x1a\x34\x66intekkers/models/strategy/strategy_allocation.proto\x1a)fintekkers/models/security/security.proto\x1a#fintekkers/models/price/price.proto\x1a\x30\x66intekkers/models/position/position_status.proto\x1a\x34\x66intekkers/models/transaction/transaction_type.proto\"\x83\x07\n\x10TransactionProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x04uuid\x18\x05 \x01(\x0b\x32!.fintekkers.models.util.UUIDProto\x12:\n\x05\x61s_of\x18\x06 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x0f\n\x07is_link\x18\x07 \x01(\x08\x12>\n\tportfolio\x18\n \x01(\x0b\x32+.fintekkers.models.portfolio.PortfolioProto\x12;\n\x08security\x18\x0b \x01(\x0b\x32).fintekkers.models.security.SecurityProto\x12M\n\x10transaction_type\x18\x0c \x01(\x0e\x32\x33.fintekkers.models.transaction.TransactionTypeProto\x12;\n\x08quantity\x18\r \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\x12\x32\n\x05price\x18\x0e \x01(\x0b\x32#.fintekkers.models.price.PriceProto\x12:\n\ntrade_date\x18\x0f \x01(\x0b\x32&.fintekkers.models.util.LocalDateProto\x12?\n\x0fsettlement_date\x18\x10 \x01(\x0b\x32&.fintekkers.models.util.LocalDateProto\x12J\n\x11\x63hildTransactions\x18\x14 \x03(\x0b\x32/.fintekkers.models.transaction.TransactionProto\x12H\n\x0fposition_status\x18\x19 \x01(\x0e\x32/.fintekkers.models.position.PositionStatusProto\x12\x12\n\ntrade_name\x18\x1a \x01(\t\x12P\n\x13strategy_allocation\x18\x1b \x01(\x0b\x32\x33.fintekkers.models.strategy.StrategyAllocationProto\x12\x14\n\x0cis_cancelled\x18\x1e \x01(\x08\x42\x15\x42\x11TransactionProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/fintekkers/models/transaction/transaction.proto\x12\x1d\x66intekkers.models.transaction\x1a*fintekkers/models/util/decimal_value.proto\x1a\'fintekkers/models/util/local_date.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a!fintekkers/models/util/uuid.proto\x1a+fintekkers/models/portfolio/portfolio.proto\x1a\x34\x66intekkers/models/strategy/strategy_allocation.proto\x1a)fintekkers/models/security/security.proto\x1a#fintekkers/models/price/price.proto\x1a\x30\x66intekkers/models/position/position_status.proto\x1a\x34\x66intekkers/models/transaction/transaction_type.proto\"\x83\x08\n\x10TransactionProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12/\n\x04uuid\x18\x05 \x01(\x0b\x32!.fintekkers.models.util.UUIDProto\x12:\n\x05\x61s_of\x18\x06 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12\x0f\n\x07is_link\x18\x07 \x01(\x08\x12?\n\nvalid_from\x18\x08 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12=\n\x08valid_to\x18\t \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProto\x12>\n\tportfolio\x18\n \x01(\x0b\x32+.fintekkers.models.portfolio.PortfolioProto\x12;\n\x08security\x18\x0b \x01(\x0b\x32).fintekkers.models.security.SecurityProto\x12M\n\x10transaction_type\x18\x0c \x01(\x0e\x32\x33.fintekkers.models.transaction.TransactionTypeProto\x12;\n\x08quantity\x18\r \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\x12\x32\n\x05price\x18\x0e \x01(\x0b\x32#.fintekkers.models.price.PriceProto\x12:\n\ntrade_date\x18\x0f \x01(\x0b\x32&.fintekkers.models.util.LocalDateProto\x12?\n\x0fsettlement_date\x18\x10 \x01(\x0b\x32&.fintekkers.models.util.LocalDateProto\x12J\n\x11\x63hildTransactions\x18\x14 \x03(\x0b\x32/.fintekkers.models.transaction.TransactionProto\x12H\n\x0fposition_status\x18\x19 \x01(\x0e\x32/.fintekkers.models.position.PositionStatusProto\x12\x12\n\ntrade_name\x18\x1a \x01(\t\x12P\n\x13strategy_allocation\x18\x1b \x01(\x0b\x32\x33.fintekkers.models.strategy.StrategyAllocationProto\x12\x14\n\x0cis_cancelled\x18\x1e \x01(\x08\x42\x15\x42\x11TransactionProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.models.transaction.transaction_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\021TransactionProtosP\001'
   _TRANSACTIONPROTO._serialized_start=532
-  _TRANSACTIONPROTO._serialized_end=1431
+  _TRANSACTIONPROTO._serialized_end=1559
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/transaction_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/transaction_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class TransactionProto(_message.Message):
-    __slots__ = ["as_of", "childTransactions", "is_cancelled", "is_link", "object_class", "portfolio", "position_status", "price", "quantity", "security", "settlement_date", "strategy_allocation", "trade_date", "trade_name", "transaction_type", "uuid", "version"]
+    __slots__ = ["as_of", "childTransactions", "is_cancelled", "is_link", "object_class", "portfolio", "position_status", "price", "quantity", "security", "settlement_date", "strategy_allocation", "trade_date", "trade_name", "transaction_type", "uuid", "valid_from", "valid_to", "version"]
     AS_OF_FIELD_NUMBER: _ClassVar[int]
     CHILDTRANSACTIONS_FIELD_NUMBER: _ClassVar[int]
     IS_CANCELLED_FIELD_NUMBER: _ClassVar[int]
     IS_LINK_FIELD_NUMBER: _ClassVar[int]
     OBJECT_CLASS_FIELD_NUMBER: _ClassVar[int]
     PORTFOLIO_FIELD_NUMBER: _ClassVar[int]
     POSITION_STATUS_FIELD_NUMBER: _ClassVar[int]
@@ -29,14 +29,16 @@
     SECURITY_FIELD_NUMBER: _ClassVar[int]
     SETTLEMENT_DATE_FIELD_NUMBER: _ClassVar[int]
     STRATEGY_ALLOCATION_FIELD_NUMBER: _ClassVar[int]
     TRADE_DATE_FIELD_NUMBER: _ClassVar[int]
     TRADE_NAME_FIELD_NUMBER: _ClassVar[int]
     TRANSACTION_TYPE_FIELD_NUMBER: _ClassVar[int]
     UUID_FIELD_NUMBER: _ClassVar[int]
+    VALID_FROM_FIELD_NUMBER: _ClassVar[int]
+    VALID_TO_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     as_of: _local_timestamp_pb2.LocalTimestampProto
     childTransactions: _containers.RepeatedCompositeFieldContainer[TransactionProto]
     is_cancelled: bool
     is_link: bool
     object_class: str
     portfolio: _portfolio_pb2.PortfolioProto
@@ -46,9 +48,11 @@
     security: _security_pb2.SecurityProto
     settlement_date: _local_date_pb2.LocalDateProto
     strategy_allocation: _strategy_allocation_pb2.StrategyAllocationProto
     trade_date: _local_date_pb2.LocalDateProto
     trade_name: str
     transaction_type: _transaction_type_pb2.TransactionTypeProto
     uuid: _uuid_pb2.UUIDProto
+    valid_from: _local_timestamp_pb2.LocalTimestampProto
+    valid_to: _local_timestamp_pb2.LocalTimestampProto
     version: str
-    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuid: _Optional[_Union[_uuid_pb2.UUIDProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., is_link: bool = ..., portfolio: _Optional[_Union[_portfolio_pb2.PortfolioProto, _Mapping]] = ..., security: _Optional[_Union[_security_pb2.SecurityProto, _Mapping]] = ..., transaction_type: _Optional[_Union[_transaction_type_pb2.TransactionTypeProto, str]] = ..., quantity: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ..., price: _Optional[_Union[_price_pb2.PriceProto, _Mapping]] = ..., trade_date: _Optional[_Union[_local_date_pb2.LocalDateProto, _Mapping]] = ..., settlement_date: _Optional[_Union[_local_date_pb2.LocalDateProto, _Mapping]] = ..., childTransactions: _Optional[_Iterable[_Union[TransactionProto, _Mapping]]] = ..., position_status: _Optional[_Union[_position_status_pb2.PositionStatusProto, str]] = ..., trade_name: _Optional[str] = ..., strategy_allocation: _Optional[_Union[_strategy_allocation_pb2.StrategyAllocationProto, _Mapping]] = ..., is_cancelled: bool = ...) -> None: ...
+    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuid: _Optional[_Union[_uuid_pb2.UUIDProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., is_link: bool = ..., valid_from: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., valid_to: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., portfolio: _Optional[_Union[_portfolio_pb2.PortfolioProto, _Mapping]] = ..., security: _Optional[_Union[_security_pb2.SecurityProto, _Mapping]] = ..., transaction_type: _Optional[_Union[_transaction_type_pb2.TransactionTypeProto, str]] = ..., quantity: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ..., price: _Optional[_Union[_price_pb2.PriceProto, _Mapping]] = ..., trade_date: _Optional[_Union[_local_date_pb2.LocalDateProto, _Mapping]] = ..., settlement_date: _Optional[_Union[_local_date_pb2.LocalDateProto, _Mapping]] = ..., childTransactions: _Optional[_Iterable[_Union[TransactionProto, _Mapping]]] = ..., position_status: _Optional[_Union[_position_status_pb2.PositionStatusProto, str]] = ..., trade_name: _Optional[str] = ..., strategy_allocation: _Optional[_Union[_strategy_allocation_pb2.StrategyAllocationProto, _Mapping]] = ..., is_cancelled: bool = ...) -> None: ...
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/transaction_type_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/transaction_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/transaction/transaction_type_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/transaction/transaction_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/decimal_value_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/decimal_value_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/endpoint_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/endpoint_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/endpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/local_date_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/local_date_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/local_date_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/local_date_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/local_timestamp_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/local_timestamp_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/local_timestamp_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/local_timestamp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/node_partition_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/node_partition_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/node_partition_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/node_partition_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/node_state_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/node_state_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/lock/node_state_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/lock/node_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/models/util/uuid_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/models/util/uuid_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/create_portfolio_request_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/create_portfolio_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/create_portfolio_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/create_portfolio_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/create_portfolio_response_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/create_portfolio_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/create_portfolio_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/create_portfolio_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/query_portfolio_request_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/query_portfolio_request_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from fintekkers.models.util import uuid_pb2 as fintekkers_dot_models_dot_util_dot_uuid__pb2
 from fintekkers.models.util import local_timestamp_pb2 as fintekkers_dot_models_dot_util_dot_local__timestamp__pb2
 from fintekkers.models.position import position_filter_pb2 as fintekkers_dot_models_dot_position_dot_position__filter__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;fintekkers/requests/portfolio/query_portfolio_request.proto\x12\x1d\x66intekkers.requests.portfolio\x1a!fintekkers/models/util/uuid.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a\x30\x66intekkers/models/position/position_filter.proto\"\x82\x02\n\x1aQueryPortfolioRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x30\n\x05uuids\x18\x15 \x03(\x0b\x32!.fintekkers.models.util.UUIDProto\x12O\n\x16search_portfolio_input\x18\x16 \x01(\x0b\x32/.fintekkers.models.position.PositionFilterProto\x12:\n\x05\x61s_of\x18\x17 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProtoB\x1f\x42\x1bQueryPortfolioRequestProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;fintekkers/requests/portfolio/query_portfolio_request.proto\x12\x1d\x66intekkers.requests.portfolio\x1a!fintekkers/models/util/uuid.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a\x30\x66intekkers/models/position/position_filter.proto\"\x82\x02\n\x1aQueryPortfolioRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x30\n\x05uuIds\x18\x15 \x03(\x0b\x32!.fintekkers.models.util.UUIDProto\x12O\n\x16search_portfolio_input\x18\x16 \x01(\x0b\x32/.fintekkers.models.position.PositionFilterProto\x12:\n\x05\x61s_of\x18\x17 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProtoB\x1f\x42\x1bQueryPortfolioRequestProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.requests.portfolio.query_portfolio_request_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\033QueryPortfolioRequestProtosP\001'
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/query_portfolio_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/query_transaction_request_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class QueryPortfolioRequestProto(_message.Message):
-    __slots__ = ["as_of", "object_class", "search_portfolio_input", "uuids", "version"]
+class QueryTransactionRequestProto(_message.Message):
+    __slots__ = ["as_of", "object_class", "search_transaction_input", "uuIds", "version"]
     AS_OF_FIELD_NUMBER: _ClassVar[int]
     OBJECT_CLASS_FIELD_NUMBER: _ClassVar[int]
-    SEARCH_PORTFOLIO_INPUT_FIELD_NUMBER: _ClassVar[int]
+    SEARCH_TRANSACTION_INPUT_FIELD_NUMBER: _ClassVar[int]
     UUIDS_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     as_of: _local_timestamp_pb2.LocalTimestampProto
     object_class: str
-    search_portfolio_input: _position_filter_pb2.PositionFilterProto
-    uuids: _containers.RepeatedCompositeFieldContainer[_uuid_pb2.UUIDProto]
+    search_transaction_input: _position_filter_pb2.PositionFilterProto
+    uuIds: _containers.RepeatedCompositeFieldContainer[_uuid_pb2.UUIDProto]
     version: str
-    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuids: _Optional[_Iterable[_Union[_uuid_pb2.UUIDProto, _Mapping]]] = ..., search_portfolio_input: _Optional[_Union[_position_filter_pb2.PositionFilterProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ...) -> None: ...
+    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuIds: _Optional[_Iterable[_Union[_uuid_pb2.UUIDProto, _Mapping]]] = ..., search_transaction_input: _Optional[_Union[_position_filter_pb2.PositionFilterProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ...) -> None: ...
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/query_portfolio_response_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/query_portfolio_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/portfolio/query_portfolio_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/portfolio/query_portfolio_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/position/query_position_request_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/position/query_position_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/position/query_position_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/position/query_position_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/position/query_position_response_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/position/query_position_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/position/query_position_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/position/query_position_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/price/create_price_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/price/create_price_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/price/create_price_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/price/create_price_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/price/query_price_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/price/price_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,31 @@
-from fintekkers.models.util import uuid_pb2 as _uuid_pb2
+from fintekkers.models.util import decimal_value_pb2 as _decimal_value_pb2
 from fintekkers.models.util import local_timestamp_pb2 as _local_timestamp_pb2
-from fintekkers.models.position import position_filter_pb2 as _position_filter_pb2
-from google.protobuf.internal import containers as _containers
+from fintekkers.models.util import uuid_pb2 as _uuid_pb2
+from fintekkers.models.security import security_pb2 as _security_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class QueryPriceRequestProto(_message.Message):
-    __slots__ = ["as_of", "object_class", "search_price_input", "uuids", "version"]
+class PriceProto(_message.Message):
+    __slots__ = ["as_of", "is_link", "object_class", "price", "security", "uuid", "valid_from", "valid_to", "version"]
     AS_OF_FIELD_NUMBER: _ClassVar[int]
+    IS_LINK_FIELD_NUMBER: _ClassVar[int]
     OBJECT_CLASS_FIELD_NUMBER: _ClassVar[int]
-    SEARCH_PRICE_INPUT_FIELD_NUMBER: _ClassVar[int]
-    UUIDS_FIELD_NUMBER: _ClassVar[int]
+    PRICE_FIELD_NUMBER: _ClassVar[int]
+    SECURITY_FIELD_NUMBER: _ClassVar[int]
+    UUID_FIELD_NUMBER: _ClassVar[int]
+    VALID_FROM_FIELD_NUMBER: _ClassVar[int]
+    VALID_TO_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     as_of: _local_timestamp_pb2.LocalTimestampProto
+    is_link: bool
     object_class: str
-    search_price_input: _position_filter_pb2.PositionFilterProto
-    uuids: _containers.RepeatedCompositeFieldContainer[_uuid_pb2.UUIDProto]
+    price: _decimal_value_pb2.DecimalValueProto
+    security: _security_pb2.SecurityProto
+    uuid: _uuid_pb2.UUIDProto
+    valid_from: _local_timestamp_pb2.LocalTimestampProto
+    valid_to: _local_timestamp_pb2.LocalTimestampProto
     version: str
-    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuids: _Optional[_Iterable[_Union[_uuid_pb2.UUIDProto, _Mapping]]] = ..., search_price_input: _Optional[_Union[_position_filter_pb2.PositionFilterProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ...) -> None: ...
+    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuid: _Optional[_Union[_uuid_pb2.UUIDProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., is_link: bool = ..., valid_from: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., valid_to: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., price: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ..., security: _Optional[_Union[_security_pb2.SecurityProto, _Mapping]] = ...) -> None: ...
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/price/query_price_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/price/query_price_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/security/create_security_request_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/security/create_security_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/security/create_security_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/security/create_security_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/security/create_security_response_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/security/create_security_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/security/create_security_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/security/create_security_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/security/query_security_request_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/security/query_security_request_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from fintekkers.models.util import uuid_pb2 as fintekkers_dot_models_dot_util_dot_uuid__pb2
 from fintekkers.models.util import local_timestamp_pb2 as fintekkers_dot_models_dot_util_dot_local__timestamp__pb2
 from fintekkers.models.position import position_filter_pb2 as fintekkers_dot_models_dot_position_dot_position__filter__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9fintekkers/requests/security/query_security_request.proto\x12\x1c\x66intekkers.requests.security\x1a!fintekkers/models/util/uuid.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a\x30\x66intekkers/models/position/position_filter.proto\"\x80\x02\n\x19QuerySecurityRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x30\n\x05uuids\x18\x15 \x03(\x0b\x32!.fintekkers.models.util.UUIDProto\x12N\n\x15search_security_input\x18\x16 \x01(\x0b\x32/.fintekkers.models.position.PositionFilterProto\x12:\n\x05\x61s_of\x18\x17 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProtoB\x1e\x42\x1aQuerySecurityRequestProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9fintekkers/requests/security/query_security_request.proto\x12\x1c\x66intekkers.requests.security\x1a!fintekkers/models/util/uuid.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a\x30\x66intekkers/models/position/position_filter.proto\"\x80\x02\n\x19QuerySecurityRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x30\n\x05uuIds\x18\x15 \x03(\x0b\x32!.fintekkers.models.util.UUIDProto\x12N\n\x15search_security_input\x18\x16 \x01(\x0b\x32/.fintekkers.models.position.PositionFilterProto\x12:\n\x05\x61s_of\x18\x17 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProtoB\x1e\x42\x1aQuerySecurityRequestProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.requests.security.query_security_request_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\032QuerySecurityRequestProtosP\001'
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/security/query_security_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/strategy/strategy_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-from fintekkers.models.util import uuid_pb2 as _uuid_pb2
 from fintekkers.models.util import local_timestamp_pb2 as _local_timestamp_pb2
-from fintekkers.models.position import position_filter_pb2 as _position_filter_pb2
-from google.protobuf.internal import containers as _containers
+from fintekkers.models.util import uuid_pb2 as _uuid_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class QuerySecurityRequestProto(_message.Message):
-    __slots__ = ["as_of", "object_class", "search_security_input", "uuids", "version"]
+class StrategyProto(_message.Message):
+    __slots__ = ["as_of", "is_link", "object_class", "parent", "strategy_name", "uuid", "valid_from", "valid_to", "version"]
     AS_OF_FIELD_NUMBER: _ClassVar[int]
+    IS_LINK_FIELD_NUMBER: _ClassVar[int]
     OBJECT_CLASS_FIELD_NUMBER: _ClassVar[int]
-    SEARCH_SECURITY_INPUT_FIELD_NUMBER: _ClassVar[int]
-    UUIDS_FIELD_NUMBER: _ClassVar[int]
+    PARENT_FIELD_NUMBER: _ClassVar[int]
+    STRATEGY_NAME_FIELD_NUMBER: _ClassVar[int]
+    UUID_FIELD_NUMBER: _ClassVar[int]
+    VALID_FROM_FIELD_NUMBER: _ClassVar[int]
+    VALID_TO_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     as_of: _local_timestamp_pb2.LocalTimestampProto
+    is_link: bool
     object_class: str
-    search_security_input: _position_filter_pb2.PositionFilterProto
-    uuids: _containers.RepeatedCompositeFieldContainer[_uuid_pb2.UUIDProto]
+    parent: StrategyProto
+    strategy_name: str
+    uuid: _uuid_pb2.UUIDProto
+    valid_from: _local_timestamp_pb2.LocalTimestampProto
+    valid_to: _local_timestamp_pb2.LocalTimestampProto
     version: str
-    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuids: _Optional[_Iterable[_Union[_uuid_pb2.UUIDProto, _Mapping]]] = ..., search_security_input: _Optional[_Union[_position_filter_pb2.PositionFilterProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ...) -> None: ...
+    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuid: _Optional[_Union[_uuid_pb2.UUIDProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., is_link: bool = ..., valid_from: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., valid_to: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., strategy_name: _Optional[str] = ..., parent: _Optional[_Union[StrategyProto, _Mapping]] = ...) -> None: ...
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/security/query_security_response_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/security/query_security_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/security/query_security_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/security/query_security_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/create_transaction_request_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/create_transaction_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/create_transaction_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/create_transaction_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/create_transaction_response_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/create_transaction_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/create_transaction_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/create_transaction_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/query_transaction_request_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/query_transaction_request_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from fintekkers.models.util import uuid_pb2 as fintekkers_dot_models_dot_util_dot_uuid__pb2
 from fintekkers.models.util import local_timestamp_pb2 as fintekkers_dot_models_dot_util_dot_local__timestamp__pb2
 from fintekkers.models.position import position_filter_pb2 as fintekkers_dot_models_dot_position_dot_position__filter__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n?fintekkers/requests/transaction/query_transaction_request.proto\x12\x1f\x66intekkers.requests.transaction\x1a!fintekkers/models/util/uuid.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a\x30\x66intekkers/models/position/position_filter.proto\"\x86\x02\n\x1cQueryTransactionRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x30\n\x05uuids\x18\x15 \x03(\x0b\x32!.fintekkers.models.util.UUIDProto\x12Q\n\x18search_transaction_input\x18\x16 \x01(\x0b\x32/.fintekkers.models.position.PositionFilterProto\x12:\n\x05\x61s_of\x18\x17 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProtoB!B\x1dQueryTransactionRequestProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n?fintekkers/requests/transaction/query_transaction_request.proto\x12\x1f\x66intekkers.requests.transaction\x1a!fintekkers/models/util/uuid.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a\x30\x66intekkers/models/position/position_filter.proto\"\x86\x02\n\x1cQueryTransactionRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x30\n\x05uuIds\x18\x15 \x03(\x0b\x32!.fintekkers.models.util.UUIDProto\x12Q\n\x18search_transaction_input\x18\x16 \x01(\x0b\x32/.fintekkers.models.position.PositionFilterProto\x12:\n\x05\x61s_of\x18\x17 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProtoB!B\x1dQueryTransactionRequestProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.requests.transaction.query_transaction_request_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\035QueryTransactionRequestProtosP\001'
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/query_transaction_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/models/portfolio/portfolio_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from fintekkers.models.util import uuid_pb2 as _uuid_pb2
 from fintekkers.models.util import local_timestamp_pb2 as _local_timestamp_pb2
-from fintekkers.models.position import position_filter_pb2 as _position_filter_pb2
-from google.protobuf.internal import containers as _containers
+from fintekkers.models.util import uuid_pb2 as _uuid_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class QueryTransactionRequestProto(_message.Message):
-    __slots__ = ["as_of", "object_class", "search_transaction_input", "uuids", "version"]
+class PortfolioProto(_message.Message):
+    __slots__ = ["as_of", "is_link", "object_class", "portfolio_name", "uuid", "valid_from", "valid_to", "version"]
     AS_OF_FIELD_NUMBER: _ClassVar[int]
+    IS_LINK_FIELD_NUMBER: _ClassVar[int]
     OBJECT_CLASS_FIELD_NUMBER: _ClassVar[int]
-    SEARCH_TRANSACTION_INPUT_FIELD_NUMBER: _ClassVar[int]
-    UUIDS_FIELD_NUMBER: _ClassVar[int]
+    PORTFOLIO_NAME_FIELD_NUMBER: _ClassVar[int]
+    UUID_FIELD_NUMBER: _ClassVar[int]
+    VALID_FROM_FIELD_NUMBER: _ClassVar[int]
+    VALID_TO_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     as_of: _local_timestamp_pb2.LocalTimestampProto
+    is_link: bool
     object_class: str
-    search_transaction_input: _position_filter_pb2.PositionFilterProto
-    uuids: _containers.RepeatedCompositeFieldContainer[_uuid_pb2.UUIDProto]
+    portfolio_name: str
+    uuid: _uuid_pb2.UUIDProto
+    valid_from: _local_timestamp_pb2.LocalTimestampProto
+    valid_to: _local_timestamp_pb2.LocalTimestampProto
     version: str
-    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuids: _Optional[_Iterable[_Union[_uuid_pb2.UUIDProto, _Mapping]]] = ..., search_transaction_input: _Optional[_Union[_position_filter_pb2.PositionFilterProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ...) -> None: ...
+    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., uuid: _Optional[_Union[_uuid_pb2.UUIDProto, _Mapping]] = ..., as_of: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., is_link: bool = ..., valid_from: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., valid_to: _Optional[_Union[_local_timestamp_pb2.LocalTimestampProto, _Mapping]] = ..., portfolio_name: _Optional[str] = ...) -> None: ...
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/query_transaction_response_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/query_transaction_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/transaction/query_transaction_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/transaction/query_transaction_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/error_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/error_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/error_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/message_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/message_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/message_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/summary_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/errors/summary_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/errors/summary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/lock_request_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/lock_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/lock_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/lock_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/lock_response_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/lock_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/lock/lock_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/lock/lock_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/util/operation_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/util/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/valuation_request_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/valuation_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/valuation_request_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/valuation_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/valuation_response_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/valuation_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/requests/valuation/valuation_response_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/requests/valuation/valuation_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/lock_service/lock_service_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/lock_service/lock_service_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/lock_service/lock_service_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/services/lock_service/lock_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/lock_service/lock_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/lock_service/lock_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/portfolio_service/portfolio_service_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/portfolio_service/portfolio_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from fintekkers.requests.portfolio import create_portfolio_request_pb2 as fintekkers_dot_requests_dot_portfolio_dot_create__portfolio__request__pb2
 from fintekkers.requests.portfolio import create_portfolio_response_pb2 as fintekkers_dot_requests_dot_portfolio_dot_create__portfolio__response__pb2
 from fintekkers.requests.portfolio import query_portfolio_request_pb2 as fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__request__pb2
 from fintekkers.requests.portfolio import query_portfolio_response_pb2 as fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__response__pb2
 from fintekkers.requests.util.errors import summary_pb2 as fintekkers_dot_requests_dot_util_dot_errors_dot_summary__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n=fintekkers/services/portfolio-service/portfolio_service.proto\x12%fintekkers.services.portfolio_service\x1a<fintekkers/requests/portfolio/create_portfolio_request.proto\x1a=fintekkers/requests/portfolio/create_portfolio_response.proto\x1a;fintekkers/requests/portfolio/query_portfolio_request.proto\x1a<fintekkers/requests/portfolio/query_portfolio_response.proto\x1a-fintekkers/requests/util/errors/summary.proto2\xab\x06\n\tPortfolio\x12\x89\x01\n\x0e\x43reateOrUpdate\x12:.fintekkers.requests.portfolio.CreatePortfolioRequestProto\x1a;.fintekkers.requests.portfolio.CreatePortfolioResponseProto\x12\x81\x01\n\x08GetByIDs\x12\x39.fintekkers.requests.portfolio.QueryPortfolioRequestProto\x1a:.fintekkers.requests.portfolio.QueryPortfolioResponseProto\x12\x81\x01\n\x06Search\x12\x39.fintekkers.requests.portfolio.QueryPortfolioRequestProto\x1a:.fintekkers.requests.portfolio.QueryPortfolioResponseProto0\x01\x12\x80\x01\n\x07ListIDs\x12\x39.fintekkers.requests.portfolio.QueryPortfolioRequestProto\x1a:.fintekkers.requests.portfolio.QueryPortfolioResponseProto\x12\x83\x01\n\x16ValidateCreateOrUpdate\x12:.fintekkers.requests.portfolio.CreatePortfolioRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProto\x12\x80\x01\n\x14ValidateQueryRequest\x12\x39.fintekkers.requests.portfolio.QueryPortfolioRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProtoB\x06\x88\x01\x01\x90\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n=fintekkers/services/portfolio-service/portfolio_service.proto\x12%fintekkers.services.portfolio_service\x1a<fintekkers/requests/portfolio/create_portfolio_request.proto\x1a=fintekkers/requests/portfolio/create_portfolio_response.proto\x1a;fintekkers/requests/portfolio/query_portfolio_request.proto\x1a<fintekkers/requests/portfolio/query_portfolio_response.proto\x1a-fintekkers/requests/util/errors/summary.proto2\xab\x06\n\tPortfolio\x12\x89\x01\n\x0e\x43reateOrUpdate\x12:.fintekkers.requests.portfolio.CreatePortfolioRequestProto\x1a;.fintekkers.requests.portfolio.CreatePortfolioResponseProto\x12\x81\x01\n\x08GetByIds\x12\x39.fintekkers.requests.portfolio.QueryPortfolioRequestProto\x1a:.fintekkers.requests.portfolio.QueryPortfolioResponseProto\x12\x81\x01\n\x06Search\x12\x39.fintekkers.requests.portfolio.QueryPortfolioRequestProto\x1a:.fintekkers.requests.portfolio.QueryPortfolioResponseProto0\x01\x12\x80\x01\n\x07ListIds\x12\x39.fintekkers.requests.portfolio.QueryPortfolioRequestProto\x1a:.fintekkers.requests.portfolio.QueryPortfolioResponseProto\x12\x83\x01\n\x16ValidateCreateOrUpdate\x12:.fintekkers.requests.portfolio.CreatePortfolioRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProto\x12\x80\x01\n\x14ValidateQueryRequest\x12\x39.fintekkers.requests.portfolio.QueryPortfolioRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProtoB\x06\x88\x01\x01\x90\x01\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.services.portfolio_service.portfolio_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\210\001\001\220\001\001'
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/portfolio_service/portfolio_service_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/services/portfolio_service/portfolio_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/portfolio_service/portfolio_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/portfolio_service/portfolio_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,26 @@
             channel: A grpc.Channel.
         """
         self.CreateOrUpdate = channel.unary_unary(
                 '/fintekkers.services.portfolio_service.Portfolio/CreateOrUpdate',
                 request_serializer=fintekkers_dot_requests_dot_portfolio_dot_create__portfolio__request__pb2.CreatePortfolioRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_portfolio_dot_create__portfolio__response__pb2.CreatePortfolioResponseProto.FromString,
                 )
-        self.GetByIDs = channel.unary_unary(
-                '/fintekkers.services.portfolio_service.Portfolio/GetByIDs',
+        self.GetByIds = channel.unary_unary(
+                '/fintekkers.services.portfolio_service.Portfolio/GetByIds',
                 request_serializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__request__pb2.QueryPortfolioRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__response__pb2.QueryPortfolioResponseProto.FromString,
                 )
         self.Search = channel.unary_stream(
                 '/fintekkers.services.portfolio_service.Portfolio/Search',
                 request_serializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__request__pb2.QueryPortfolioRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__response__pb2.QueryPortfolioResponseProto.FromString,
                 )
-        self.ListIDs = channel.unary_unary(
-                '/fintekkers.services.portfolio_service.Portfolio/ListIDs',
+        self.ListIds = channel.unary_unary(
+                '/fintekkers.services.portfolio_service.Portfolio/ListIds',
                 request_serializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__request__pb2.QueryPortfolioRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__response__pb2.QueryPortfolioResponseProto.FromString,
                 )
         self.ValidateCreateOrUpdate = channel.unary_unary(
                 '/fintekkers.services.portfolio_service.Portfolio/ValidateCreateOrUpdate',
                 request_serializer=fintekkers_dot_requests_dot_portfolio_dot_create__portfolio__request__pb2.CreatePortfolioRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_util_dot_errors_dot_summary__pb2.SummaryProto.FromString,
@@ -55,27 +55,27 @@
 
     def CreateOrUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetByIDs(self, request, context):
+    def GetByIds(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Search(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListIDs(self, request, context):
+    def ListIds(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ValidateCreateOrUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -93,26 +93,26 @@
 def add_PortfolioServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateOrUpdate': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateOrUpdate,
                     request_deserializer=fintekkers_dot_requests_dot_portfolio_dot_create__portfolio__request__pb2.CreatePortfolioRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_portfolio_dot_create__portfolio__response__pb2.CreatePortfolioResponseProto.SerializeToString,
             ),
-            'GetByIDs': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetByIDs,
+            'GetByIds': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetByIds,
                     request_deserializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__request__pb2.QueryPortfolioRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__response__pb2.QueryPortfolioResponseProto.SerializeToString,
             ),
             'Search': grpc.unary_stream_rpc_method_handler(
                     servicer.Search,
                     request_deserializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__request__pb2.QueryPortfolioRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__response__pb2.QueryPortfolioResponseProto.SerializeToString,
             ),
-            'ListIDs': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListIDs,
+            'ListIds': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListIds,
                     request_deserializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__request__pb2.QueryPortfolioRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__response__pb2.QueryPortfolioResponseProto.SerializeToString,
             ),
             'ValidateCreateOrUpdate': grpc.unary_unary_rpc_method_handler(
                     servicer.ValidateCreateOrUpdate,
                     request_deserializer=fintekkers_dot_requests_dot_portfolio_dot_create__portfolio__request__pb2.CreatePortfolioRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_util_dot_errors_dot_summary__pb2.SummaryProto.SerializeToString,
@@ -146,25 +146,25 @@
         return grpc.experimental.unary_unary(request, target, '/fintekkers.services.portfolio_service.Portfolio/CreateOrUpdate',
             fintekkers_dot_requests_dot_portfolio_dot_create__portfolio__request__pb2.CreatePortfolioRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_portfolio_dot_create__portfolio__response__pb2.CreatePortfolioResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetByIDs(request,
+    def GetByIds(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.portfolio_service.Portfolio/GetByIDs',
+        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.portfolio_service.Portfolio/GetByIds',
             fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__request__pb2.QueryPortfolioRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__response__pb2.QueryPortfolioResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Search(request,
@@ -180,25 +180,25 @@
         return grpc.experimental.unary_stream(request, target, '/fintekkers.services.portfolio_service.Portfolio/Search',
             fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__request__pb2.QueryPortfolioRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__response__pb2.QueryPortfolioResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListIDs(request,
+    def ListIds(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.portfolio_service.Portfolio/ListIDs',
+        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.portfolio_service.Portfolio/ListIds',
             fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__request__pb2.QueryPortfolioRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_portfolio_dot_query__portfolio__response__pb2.QueryPortfolioResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ValidateCreateOrUpdate(request,
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/position_service/position_service_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/position_service/position_service_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/position_service/position_service_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/services/position_service/position_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/position_service/position_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/position_service/position_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
                 )
 
 
 class PositionServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Search(self, request, context):
-        """rpc GetByIDs (position.QueryPositionRequestProto) returns (position.QueryPositionResponseProto);
-        rpc ListIDs (transaction.QueryTransactionRequestProto) returns (transaction.QueryTransactionResponseProto);
+        """rpc GetByIds (position.QueryPositionRequestProto) returns (position.QueryPositionResponseProto);
+        rpc ListIds (transaction.QueryTransactionRequestProto) returns (transaction.QueryTransactionResponseProto);
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ValidateQueryRequest(self, request, context):
         """rpc ValidateCreateOrUpdate (transaction.CreateTransactionRequestProto) returns (util.errors.SummaryProto);
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/price_service/price_service_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/services/price_service/price_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/security_service/security_service_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/security_service/security_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from fintekkers.requests.security import query_security_request_pb2 as fintekkers_dot_requests_dot_security_dot_query__security__request__pb2
 from fintekkers.requests.security import query_security_response_pb2 as fintekkers_dot_requests_dot_security_dot_query__security__response__pb2
 from fintekkers.requests.security import create_security_request_pb2 as fintekkers_dot_requests_dot_security_dot_create__security__request__pb2
 from fintekkers.requests.security import create_security_response_pb2 as fintekkers_dot_requests_dot_security_dot_create__security__response__pb2
 from fintekkers.requests.util.errors import summary_pb2 as fintekkers_dot_requests_dot_util_dot_errors_dot_summary__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;fintekkers/services/security-service/security_service.proto\x12$fintekkers.services.security_service\x1a\x39\x66intekkers/requests/security/query_security_request.proto\x1a:fintekkers/requests/security/query_security_response.proto\x1a:fintekkers/requests/security/create_security_request.proto\x1a;fintekkers/requests/security/create_security_response.proto\x1a-fintekkers/requests/util/errors/summary.proto2\x92\x06\n\x08Security\x12\x85\x01\n\x0e\x43reateOrUpdate\x12\x38.fintekkers.requests.security.CreateSecurityRequestProto\x1a\x39.fintekkers.requests.security.CreateSecurityResponseProto\x12}\n\x08GetByIDs\x12\x37.fintekkers.requests.security.QuerySecurityRequestProto\x1a\x38.fintekkers.requests.security.QuerySecurityResponseProto\x12}\n\x06Search\x12\x37.fintekkers.requests.security.QuerySecurityRequestProto\x1a\x38.fintekkers.requests.security.QuerySecurityResponseProto0\x01\x12|\n\x07ListIDs\x12\x37.fintekkers.requests.security.QuerySecurityRequestProto\x1a\x38.fintekkers.requests.security.QuerySecurityResponseProto\x12\x81\x01\n\x16ValidateCreateOrUpdate\x12\x38.fintekkers.requests.security.CreateSecurityRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProto\x12~\n\x14ValidateQueryRequest\x12\x37.fintekkers.requests.security.QuerySecurityRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProtoB\x06\x88\x01\x01\x90\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;fintekkers/services/security-service/security_service.proto\x12$fintekkers.services.security_service\x1a\x39\x66intekkers/requests/security/query_security_request.proto\x1a:fintekkers/requests/security/query_security_response.proto\x1a:fintekkers/requests/security/create_security_request.proto\x1a;fintekkers/requests/security/create_security_response.proto\x1a-fintekkers/requests/util/errors/summary.proto2\x92\x06\n\x08Security\x12\x85\x01\n\x0e\x43reateOrUpdate\x12\x38.fintekkers.requests.security.CreateSecurityRequestProto\x1a\x39.fintekkers.requests.security.CreateSecurityResponseProto\x12}\n\x08GetByIds\x12\x37.fintekkers.requests.security.QuerySecurityRequestProto\x1a\x38.fintekkers.requests.security.QuerySecurityResponseProto\x12}\n\x06Search\x12\x37.fintekkers.requests.security.QuerySecurityRequestProto\x1a\x38.fintekkers.requests.security.QuerySecurityResponseProto0\x01\x12|\n\x07ListIds\x12\x37.fintekkers.requests.security.QuerySecurityRequestProto\x1a\x38.fintekkers.requests.security.QuerySecurityResponseProto\x12\x81\x01\n\x16ValidateCreateOrUpdate\x12\x38.fintekkers.requests.security.CreateSecurityRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProto\x12~\n\x14ValidateQueryRequest\x12\x37.fintekkers.requests.security.QuerySecurityRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProtoB\x06\x88\x01\x01\x90\x01\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.services.security_service.security_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\210\001\001\220\001\001'
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/security_service/security_service_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/services/security_service/security_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/security_service/security_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/security_service/security_service_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,26 +19,26 @@
             channel: A grpc.Channel.
         """
         self.CreateOrUpdate = channel.unary_unary(
                 '/fintekkers.services.security_service.Security/CreateOrUpdate',
                 request_serializer=fintekkers_dot_requests_dot_security_dot_create__security__request__pb2.CreateSecurityRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_security_dot_create__security__response__pb2.CreateSecurityResponseProto.FromString,
                 )
-        self.GetByIDs = channel.unary_unary(
-                '/fintekkers.services.security_service.Security/GetByIDs',
+        self.GetByIds = channel.unary_unary(
+                '/fintekkers.services.security_service.Security/GetByIds',
                 request_serializer=fintekkers_dot_requests_dot_security_dot_query__security__request__pb2.QuerySecurityRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_security_dot_query__security__response__pb2.QuerySecurityResponseProto.FromString,
                 )
         self.Search = channel.unary_stream(
                 '/fintekkers.services.security_service.Security/Search',
                 request_serializer=fintekkers_dot_requests_dot_security_dot_query__security__request__pb2.QuerySecurityRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_security_dot_query__security__response__pb2.QuerySecurityResponseProto.FromString,
                 )
-        self.ListIDs = channel.unary_unary(
-                '/fintekkers.services.security_service.Security/ListIDs',
+        self.ListIds = channel.unary_unary(
+                '/fintekkers.services.security_service.Security/ListIds',
                 request_serializer=fintekkers_dot_requests_dot_security_dot_query__security__request__pb2.QuerySecurityRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_security_dot_query__security__response__pb2.QuerySecurityResponseProto.FromString,
                 )
         self.ValidateCreateOrUpdate = channel.unary_unary(
                 '/fintekkers.services.security_service.Security/ValidateCreateOrUpdate',
                 request_serializer=fintekkers_dot_requests_dot_security_dot_create__security__request__pb2.CreateSecurityRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_util_dot_errors_dot_summary__pb2.SummaryProto.FromString,
@@ -55,27 +55,27 @@
 
     def CreateOrUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetByIDs(self, request, context):
+    def GetByIds(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Search(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListIDs(self, request, context):
+    def ListIds(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ValidateCreateOrUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -93,26 +93,26 @@
 def add_SecurityServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateOrUpdate': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateOrUpdate,
                     request_deserializer=fintekkers_dot_requests_dot_security_dot_create__security__request__pb2.CreateSecurityRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_security_dot_create__security__response__pb2.CreateSecurityResponseProto.SerializeToString,
             ),
-            'GetByIDs': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetByIDs,
+            'GetByIds': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetByIds,
                     request_deserializer=fintekkers_dot_requests_dot_security_dot_query__security__request__pb2.QuerySecurityRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_security_dot_query__security__response__pb2.QuerySecurityResponseProto.SerializeToString,
             ),
             'Search': grpc.unary_stream_rpc_method_handler(
                     servicer.Search,
                     request_deserializer=fintekkers_dot_requests_dot_security_dot_query__security__request__pb2.QuerySecurityRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_security_dot_query__security__response__pb2.QuerySecurityResponseProto.SerializeToString,
             ),
-            'ListIDs': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListIDs,
+            'ListIds': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListIds,
                     request_deserializer=fintekkers_dot_requests_dot_security_dot_query__security__request__pb2.QuerySecurityRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_security_dot_query__security__response__pb2.QuerySecurityResponseProto.SerializeToString,
             ),
             'ValidateCreateOrUpdate': grpc.unary_unary_rpc_method_handler(
                     servicer.ValidateCreateOrUpdate,
                     request_deserializer=fintekkers_dot_requests_dot_security_dot_create__security__request__pb2.CreateSecurityRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_util_dot_errors_dot_summary__pb2.SummaryProto.SerializeToString,
@@ -146,25 +146,25 @@
         return grpc.experimental.unary_unary(request, target, '/fintekkers.services.security_service.Security/CreateOrUpdate',
             fintekkers_dot_requests_dot_security_dot_create__security__request__pb2.CreateSecurityRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_security_dot_create__security__response__pb2.CreateSecurityResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetByIDs(request,
+    def GetByIds(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.security_service.Security/GetByIDs',
+        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.security_service.Security/GetByIds',
             fintekkers_dot_requests_dot_security_dot_query__security__request__pb2.QuerySecurityRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_security_dot_query__security__response__pb2.QuerySecurityResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Search(request,
@@ -180,25 +180,25 @@
         return grpc.experimental.unary_stream(request, target, '/fintekkers.services.security_service.Security/Search',
             fintekkers_dot_requests_dot_security_dot_query__security__request__pb2.QuerySecurityRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_security_dot_query__security__response__pb2.QuerySecurityResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListIDs(request,
+    def ListIds(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.security_service.Security/ListIDs',
+        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.security_service.Security/ListIds',
             fintekkers_dot_requests_dot_security_dot_query__security__request__pb2.QuerySecurityRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_security_dot_query__security__response__pb2.QuerySecurityResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ValidateCreateOrUpdate(request,
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/transaction_service/transaction_service_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/transaction_service/transaction_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from fintekkers.requests.transaction import create_transaction_request_pb2 as fintekkers_dot_requests_dot_transaction_dot_create__transaction__request__pb2
 from fintekkers.requests.transaction import create_transaction_response_pb2 as fintekkers_dot_requests_dot_transaction_dot_create__transaction__response__pb2
 from fintekkers.requests.transaction import query_transaction_request_pb2 as fintekkers_dot_requests_dot_transaction_dot_query__transaction__request__pb2
 from fintekkers.requests.transaction import query_transaction_response_pb2 as fintekkers_dot_requests_dot_transaction_dot_query__transaction__response__pb2
 from fintekkers.requests.util.errors import summary_pb2 as fintekkers_dot_requests_dot_util_dot_errors_dot_summary__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAfintekkers/services/transaction-service/transaction_service.proto\x12\'fintekkers.services.transaction_service\x1a@fintekkers/requests/transaction/create_transaction_request.proto\x1a\x41\x66intekkers/requests/transaction/create_transaction_response.proto\x1a?fintekkers/requests/transaction/query_transaction_request.proto\x1a@fintekkers/requests/transaction/query_transaction_response.proto\x1a-fintekkers/requests/util/errors/summary.proto2\xd5\x06\n\x0bTransaction\x12\x91\x01\n\x0e\x43reateOrUpdate\x12>.fintekkers.requests.transaction.CreateTransactionRequestProto\x1a?.fintekkers.requests.transaction.CreateTransactionResponseProto\x12\x89\x01\n\x08GetByIDs\x12=.fintekkers.requests.transaction.QueryTransactionRequestProto\x1a>.fintekkers.requests.transaction.QueryTransactionResponseProto\x12\x89\x01\n\x06Search\x12=.fintekkers.requests.transaction.QueryTransactionRequestProto\x1a>.fintekkers.requests.transaction.QueryTransactionResponseProto0\x01\x12\x88\x01\n\x07ListIDs\x12=.fintekkers.requests.transaction.QueryTransactionRequestProto\x1a>.fintekkers.requests.transaction.QueryTransactionResponseProto\x12\x87\x01\n\x16ValidateCreateOrUpdate\x12>.fintekkers.requests.transaction.CreateTransactionRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProto\x12\x84\x01\n\x14ValidateQueryRequest\x12=.fintekkers.requests.transaction.QueryTransactionRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProtoB\x06\x88\x01\x01\x90\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAfintekkers/services/transaction-service/transaction_service.proto\x12\'fintekkers.services.transaction_service\x1a@fintekkers/requests/transaction/create_transaction_request.proto\x1a\x41\x66intekkers/requests/transaction/create_transaction_response.proto\x1a?fintekkers/requests/transaction/query_transaction_request.proto\x1a@fintekkers/requests/transaction/query_transaction_response.proto\x1a-fintekkers/requests/util/errors/summary.proto2\xd5\x06\n\x0bTransaction\x12\x91\x01\n\x0e\x43reateOrUpdate\x12>.fintekkers.requests.transaction.CreateTransactionRequestProto\x1a?.fintekkers.requests.transaction.CreateTransactionResponseProto\x12\x89\x01\n\x08GetByIds\x12=.fintekkers.requests.transaction.QueryTransactionRequestProto\x1a>.fintekkers.requests.transaction.QueryTransactionResponseProto\x12\x89\x01\n\x06Search\x12=.fintekkers.requests.transaction.QueryTransactionRequestProto\x1a>.fintekkers.requests.transaction.QueryTransactionResponseProto0\x01\x12\x88\x01\n\x07ListIds\x12=.fintekkers.requests.transaction.QueryTransactionRequestProto\x1a>.fintekkers.requests.transaction.QueryTransactionResponseProto\x12\x87\x01\n\x16ValidateCreateOrUpdate\x12>.fintekkers.requests.transaction.CreateTransactionRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProto\x12\x84\x01\n\x14ValidateQueryRequest\x12=.fintekkers.requests.transaction.QueryTransactionRequestProto\x1a-.fintekkers.requests.util.errors.SummaryProtoB\x06\x88\x01\x01\x90\x01\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.services.transaction_service.transaction_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\210\001\001\220\001\001'
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/transaction_service/transaction_service_pb2.pyi` & `fintekkers-ledger-models-0.1.51/fintekkers/services/transaction_service/transaction_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/transaction_service/transaction_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/transaction_service/transaction_service_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,26 +19,26 @@
             channel: A grpc.Channel.
         """
         self.CreateOrUpdate = channel.unary_unary(
                 '/fintekkers.services.transaction_service.Transaction/CreateOrUpdate',
                 request_serializer=fintekkers_dot_requests_dot_transaction_dot_create__transaction__request__pb2.CreateTransactionRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_transaction_dot_create__transaction__response__pb2.CreateTransactionResponseProto.FromString,
                 )
-        self.GetByIDs = channel.unary_unary(
-                '/fintekkers.services.transaction_service.Transaction/GetByIDs',
+        self.GetByIds = channel.unary_unary(
+                '/fintekkers.services.transaction_service.Transaction/GetByIds',
                 request_serializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__request__pb2.QueryTransactionRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__response__pb2.QueryTransactionResponseProto.FromString,
                 )
         self.Search = channel.unary_stream(
                 '/fintekkers.services.transaction_service.Transaction/Search',
                 request_serializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__request__pb2.QueryTransactionRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__response__pb2.QueryTransactionResponseProto.FromString,
                 )
-        self.ListIDs = channel.unary_unary(
-                '/fintekkers.services.transaction_service.Transaction/ListIDs',
+        self.ListIds = channel.unary_unary(
+                '/fintekkers.services.transaction_service.Transaction/ListIds',
                 request_serializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__request__pb2.QueryTransactionRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__response__pb2.QueryTransactionResponseProto.FromString,
                 )
         self.ValidateCreateOrUpdate = channel.unary_unary(
                 '/fintekkers.services.transaction_service.Transaction/ValidateCreateOrUpdate',
                 request_serializer=fintekkers_dot_requests_dot_transaction_dot_create__transaction__request__pb2.CreateTransactionRequestProto.SerializeToString,
                 response_deserializer=fintekkers_dot_requests_dot_util_dot_errors_dot_summary__pb2.SummaryProto.FromString,
@@ -55,27 +55,27 @@
 
     def CreateOrUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetByIDs(self, request, context):
+    def GetByIds(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Search(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListIDs(self, request, context):
+    def ListIds(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ValidateCreateOrUpdate(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -93,26 +93,26 @@
 def add_TransactionServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateOrUpdate': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateOrUpdate,
                     request_deserializer=fintekkers_dot_requests_dot_transaction_dot_create__transaction__request__pb2.CreateTransactionRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_transaction_dot_create__transaction__response__pb2.CreateTransactionResponseProto.SerializeToString,
             ),
-            'GetByIDs': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetByIDs,
+            'GetByIds': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetByIds,
                     request_deserializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__request__pb2.QueryTransactionRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__response__pb2.QueryTransactionResponseProto.SerializeToString,
             ),
             'Search': grpc.unary_stream_rpc_method_handler(
                     servicer.Search,
                     request_deserializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__request__pb2.QueryTransactionRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__response__pb2.QueryTransactionResponseProto.SerializeToString,
             ),
-            'ListIDs': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListIDs,
+            'ListIds': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListIds,
                     request_deserializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__request__pb2.QueryTransactionRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_transaction_dot_query__transaction__response__pb2.QueryTransactionResponseProto.SerializeToString,
             ),
             'ValidateCreateOrUpdate': grpc.unary_unary_rpc_method_handler(
                     servicer.ValidateCreateOrUpdate,
                     request_deserializer=fintekkers_dot_requests_dot_transaction_dot_create__transaction__request__pb2.CreateTransactionRequestProto.FromString,
                     response_serializer=fintekkers_dot_requests_dot_util_dot_errors_dot_summary__pb2.SummaryProto.SerializeToString,
@@ -146,25 +146,25 @@
         return grpc.experimental.unary_unary(request, target, '/fintekkers.services.transaction_service.Transaction/CreateOrUpdate',
             fintekkers_dot_requests_dot_transaction_dot_create__transaction__request__pb2.CreateTransactionRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_transaction_dot_create__transaction__response__pb2.CreateTransactionResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetByIDs(request,
+    def GetByIds(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.transaction_service.Transaction/GetByIDs',
+        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.transaction_service.Transaction/GetByIds',
             fintekkers_dot_requests_dot_transaction_dot_query__transaction__request__pb2.QueryTransactionRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_transaction_dot_query__transaction__response__pb2.QueryTransactionResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Search(request,
@@ -180,25 +180,25 @@
         return grpc.experimental.unary_stream(request, target, '/fintekkers.services.transaction_service.Transaction/Search',
             fintekkers_dot_requests_dot_transaction_dot_query__transaction__request__pb2.QueryTransactionRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_transaction_dot_query__transaction__response__pb2.QueryTransactionResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListIDs(request,
+    def ListIds(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.transaction_service.Transaction/ListIDs',
+        return grpc.experimental.unary_unary(request, target, '/fintekkers.services.transaction_service.Transaction/ListIds',
             fintekkers_dot_requests_dot_transaction_dot_query__transaction__request__pb2.QueryTransactionRequestProto.SerializeToString,
             fintekkers_dot_requests_dot_transaction_dot_query__transaction__response__pb2.QueryTransactionResponseProto.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ValidateCreateOrUpdate(request,
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/valuation_service/valuation_service_pb2.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/valuation_service/valuation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/services/valuation_service/valuation_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.51/fintekkers/services/valuation_service/valuation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/portfolio.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/portfolio.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/position.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/position.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,21 +98,21 @@
     
     def __str__(self):
         out:StringIO = StringIO()
         
         for field in self.get_fields():
             out.write(FieldProto.Name(number=field.field))
             out.write(',')
-            out.write(self.get_field_display(field.field))
+            out.write(self.get_field_display(field))
             out.write(';')
 
         for measure in self.get_measures():
             out.write(MeasureProto.Name(number=measure.measure))
             out.write(',')
-            tmp:Decimal = self.get_measure(measure.measure)
+            tmp:Decimal = self.get_measure(measure)
             out.write(str(tmp))
             out.write(';')
         
         return out.getvalue()
 
     @staticmethod
     def wrap_string_to_any(my_string:str):
@@ -182,8 +182,8 @@
 
     from fintekkers.models.util.decimal_value_pb2 import DecimalValueProto
     @staticmethod
     def unpack_measure(measure_to_unpack:MeasureProto) -> DecimalValueProto:
         if measure_to_unpack.measure == MeasureProto.DIRECTED_QUANTITY:
             return measure_to_unpack.measure_decimal_value
         
-        raise ValueError(f"Field not found. Could not unpack {MeasureProto.Name(measure_to_unpack.measure)}")
+        raise ValueError(f"Field not found. Could not unpack {MeasureProto.Name(measure_to_unpack.measure)}")
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/security.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/security.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/tenor.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/tenor.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/transaction.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/transaction.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/util/date_utils.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/util/date_utils.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/util/environment.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/util/environment.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/util/fintekkers_uuid.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/util/fintekkers_uuid.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/models/util/serialization.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/models/util/serialization.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/requests/security.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/requests/security.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/requests/transaction.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/requests/transaction.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers/wrappers/services/security.py` & `fintekkers-ledger-models-0.1.51/fintekkers/wrappers/services/security.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers_ledger_models.egg-info/PKG-INFO` & `fintekkers-ledger-models-0.1.51/fintekkers_ledger_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fintekkers-ledger-models
-Version: 0.1.50
+Version: 0.1.51
 Summary: Fintekkers Ledger Models python package
 Home-page: https://github.com/fintekkers/ledger-models
 Author: David Doherty
 Author-email: dave@fintekkers.org
 License: MIT
 Keywords: fintekkers ledger models
 Platform: UNKNOWN
```

### Comparing `fintekkers-ledger-models-0.1.50/fintekkers_ledger_models.egg-info/SOURCES.txt` & `fintekkers-ledger-models-0.1.51/fintekkers_ledger_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.50/setup.py` & `fintekkers-ledger-models-0.1.51/setup.py`

 * *Files identical despite different names*

