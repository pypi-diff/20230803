# Comparing `tmp/omni-pro-0.1.33.tar.gz` & `tmp/omni-pro-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omni-pro-0.1.33.tar", last modified: Tue Aug  1 23:03:07 2023, max compression
+gzip compressed data, was "omni-pro-0.1.34.tar", last modified: Thu Aug  3 15:57:08 2023, max compression
```

## Comparing `omni-pro-0.1.33.tar` & `omni-pro-0.1.34.tar`

### file list

```diff
@@ -1,327 +1,327 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.837713 omni-pro-0.1.33/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-01 23:02:42.000000 omni-pro-0.1.33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-08-01 23:03:07.833713 omni-pro-0.1.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-01 23:02:42.000000 omni-pro-0.1.33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.781712 omni-pro-0.1.33/omni/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.785712 omni-pro-0.1.33/omni/pro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/cloudmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.785712 omni-pro-0.1.33/omni/pro/data/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/data/models.user.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/database_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.785712 omni-pro-0.1.33/omni/pro/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.785712 omni-pro-0.1.33/omni/pro/models/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/common/ms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.785712 omni-pro-0.1.33/omni/pro/models/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/custom_fields/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.785712 omni-pro-0.1.33/omni/pro/models/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.785712 omni-pro-0.1.33/omni/pro/models/sql/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/catalog/category.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.785712 omni-pro-0.1.33/omni/pro/models/sql/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/common/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.789712 omni-pro-0.1.33/omni/pro/models/sql/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_category_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_locality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_method_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_method_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/schedule_work.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/schedule_work_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/rules/warehouse_hierarchy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.789712 omni-pro-0.1.33/omni/pro/models/sql/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/stock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.789712 omni-pro-0.1.33/omni/pro/models/sql/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/utilities/country.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/utilities/territory_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/sql/utilities/territory_matrix_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.789712 omni-pro-0.1.33/omni/pro/models/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/models/utilities/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.789712 omni-pro-0.1.33/omni/pro/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.789712 omni-pro-0.1.33/omni/pro/protos/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/common/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/common/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/common/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/grpc_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.789712 omni-pro-0.1.33/omni/pro/protos/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.789712 omni-pro-0.1.33/omni/pro/protos/v1/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/catalogs/family_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/catalogs/family_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/catalogs/family_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/catalogs/template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/catalogs/template_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/catalogs/template_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.793712 omni-pro-0.1.33/omni/pro/protos/v1/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/clients/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/clients/address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/clients/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/clients/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/clients/client_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/clients/client_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.809713 omni-pro-0.1.33/omni/pro/protos/v1/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/calendar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/calendar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/calendar_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_schedule_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/location_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/location_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/location_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.813712 omni-pro-0.1.33/omni/pro/protos/v1/sales/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/carrier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/carrier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/carrier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/channel_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/channel_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/client_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/client_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/currency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/currency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/currency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/order_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/order_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/order_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/order_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/order_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/order_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/payment_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/payment_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_order_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_order_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/product_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/product_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/product_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/sale_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/sale_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/sale_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/tax_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/tax_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/tax_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.825713 omni-pro-0.1.33/omni/pro/protos/v1/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/attachment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/attachment_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/attachment_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/carrier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/carrier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/carrier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/location_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/location_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/location_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/procurement_group_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/procurement_group_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/product_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/product_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/product_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/quant_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/quant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/quant_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/route_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/route_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/route_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/rule_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/rule_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/rule_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/sequence_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/sequence_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/sequence_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.825713 omni-pro-0.1.33/omni/pro/protos/v1/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/users/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31841 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/users/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    43955 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/users/user_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.833713 omni-pro-0.1.33/omni/pro/protos/v1/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/currency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/currency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/currency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/document_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/document_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/language_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/language_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/language_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/model_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/payment_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/payment_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/sequence_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/sequence_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/sequence_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/tax_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/tax_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/tax_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/timezone_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/timezone_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/protos/v1/utilities/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.833713 omni-pro-0.1.33/omni/pro/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/user/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-01 23:02:42.000000 omni-pro-0.1.33/omni/pro/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:03:07.833713 omni-pro-0.1.33/omni_pro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-08-01 23:03:07.000000 omni-pro-0.1.33/omni_pro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-08-01 23:03:07.000000 omni-pro-0.1.33/omni_pro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:03:07.000000 omni-pro-0.1.33/omni_pro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-01 23:03:07.000000 omni-pro-0.1.33/omni_pro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 23:03:07.000000 omni-pro-0.1.33/omni_pro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 23:03:07.837713 omni-pro-0.1.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-01 23:03:01.000000 omni-pro-0.1.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.163500 omni-pro-0.1.34/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-03 15:56:41.000000 omni-pro-0.1.34/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-08-03 15:57:08.163500 omni-pro-0.1.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-03 15:56:41.000000 omni-pro-0.1.34/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.131500 omni-pro-0.1.34/omni/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.131500 omni-pro-0.1.34/omni/pro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/cloudmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.131500 omni-pro-0.1.34/omni/pro/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/data/models.user.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21990 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/database_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.131500 omni-pro-0.1.34/omni/pro/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.131500 omni-pro-0.1.34/omni/pro/models/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/common/ms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.131500 omni-pro-0.1.34/omni/pro/models/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/custom_fields/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.131500 omni-pro-0.1.34/omni/pro/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.131500 omni-pro-0.1.34/omni/pro/models/sql/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/catalog/category.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.131500 omni-pro-0.1.34/omni/pro/models/sql/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/common/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.135500 omni-pro-0.1.34/omni/pro/models/sql/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_category_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_locality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_method_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_method_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/schedule_work.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/schedule_work_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/rules/warehouse_hierarchy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.135500 omni-pro-0.1.34/omni/pro/models/sql/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/stock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.135500 omni-pro-0.1.34/omni/pro/models/sql/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/utilities/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/utilities/territory_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/sql/utilities/territory_matrix_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.135500 omni-pro-0.1.34/omni/pro/models/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/models/utilities/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.135500 omni-pro-0.1.34/omni/pro/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.135500 omni-pro-0.1.34/omni/pro/protos/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/common/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/common/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/common/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/grpc_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.135500 omni-pro-0.1.34/omni/pro/protos/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.135500 omni-pro-0.1.34/omni/pro/protos/v1/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/catalogs/family_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/catalogs/family_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/catalogs/family_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/catalogs/template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/catalogs/template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/catalogs/template_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.139500 omni-pro-0.1.34/omni/pro/protos/v1/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/clients/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/clients/address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/clients/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/clients/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/clients/client_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/clients/client_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.147500 omni-pro-0.1.34/omni/pro/protos/v1/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/calendar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/calendar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/calendar_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_schedule_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/location_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/location_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/location_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.151500 omni-pro-0.1.34/omni/pro/protos/v1/sales/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/carrier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/carrier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/carrier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/channel_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/client_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/client_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/currency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/currency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/currency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/order_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/order_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/order_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/order_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/order_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/order_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/payment_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/payment_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_order_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_order_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/product_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/product_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/product_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/sale_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/sale_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/sale_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/tax_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/tax_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/tax_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.159500 omni-pro-0.1.34/omni/pro/protos/v1/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/attachment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/attachment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/attachment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/carrier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/carrier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/carrier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/location_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/location_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/location_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/procurement_group_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/procurement_group_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/product_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/product_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/product_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/quant_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/quant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/quant_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/route_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/route_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/route_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/rule_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/rule_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/rule_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/sequence_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/sequence_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/sequence_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.159500 omni-pro-0.1.34/omni/pro/protos/v1/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/users/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31841 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/users/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    43955 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/users/user_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.163500 omni-pro-0.1.34/omni/pro/protos/v1/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/currency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/currency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/currency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/document_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/document_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/language_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/language_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/language_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/model_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/payment_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/payment_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/sequence_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/sequence_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/sequence_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/tax_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/tax_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/tax_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/timezone_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/timezone_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/protos/v1/utilities/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.163500 omni-pro-0.1.34/omni/pro/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/user/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-03 15:56:41.000000 omni-pro-0.1.34/omni/pro/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:57:08.163500 omni-pro-0.1.34/omni_pro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-08-03 15:57:08.000000 omni-pro-0.1.34/omni_pro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-08-03 15:57:08.000000 omni-pro-0.1.34/omni_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:57:08.000000 omni-pro-0.1.34/omni_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-03 15:57:08.000000 omni-pro-0.1.34/omni_pro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 15:57:08.000000 omni-pro-0.1.34/omni_pro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:57:08.163500 omni-pro-0.1.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-03 15:57:01.000000 omni-pro-0.1.34/setup.py
```

### Comparing `omni-pro-0.1.33/LICENSE` & `omni-pro-0.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/PKG-INFO` & `omni-pro-0.1.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-pro
-Version: 0.1.33
+Version: 0.1.34
 Summary: Python library designed to be a utility for OMS microservices
 Home-page: https://github.com/Omnipro-Solutions/saas-ms-library
 Author: OMNI.PRO
 Author-email: development@omni.pro
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `omni-pro-0.1.33/README.md` & `omni-pro-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/aws.py` & `omni-pro-0.1.34/omni/pro/aws.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/cloudmap.py` & `omni-pro-0.1.34/omni/pro/cloudmap.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/config.py` & `omni-pro-0.1.34/omni/pro/config.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/database.py` & `omni-pro-0.1.34/omni/pro/database.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/database_connection.py` & `omni-pro-0.1.34/omni/pro/database_connection.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/decorators.py` & `omni-pro-0.1.34/omni/pro/decorators.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/initial.py` & `omni-pro-0.1.34/omni/pro/initial.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/logger.py` & `omni-pro-0.1.34/omni/pro/logger.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/base.py` & `omni-pro-0.1.34/omni/pro/models/base.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/custom_fields/enum.py` & `omni-pro-0.1.34/omni/pro/models/custom_fields/enum.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/common/country.py` & `omni-pro-0.1.34/omni/pro/models/sql/common/country.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_category.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_category.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_category_category.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_category_category.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_locality.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_locality.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_method.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_method.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_method_ref.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_method_ref.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_method_warehouse.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_method_warehouse.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/delivery_schedule.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/delivery_schedule.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/schedule_work.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/schedule_work.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/schedule_work_line.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/schedule_work_line.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/sql/rules/warehouse_hierarchy.py` & `omni-pro-0.1.34/omni/pro/models/sql/rules/warehouse_hierarchy.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/models/utilities/country.py` & `omni-pro-0.1.34/omni/pro/models/utilities/country.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/common/base_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/common/base_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/common/base_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/common/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/grpc_connector.py` & `omni-pro-0.1.34/omni/pro/protos/grpc_connector.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/response.py` & `omni-pro-0.1.34/omni/pro/protos/response.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/util.py` & `omni-pro-0.1.34/omni/pro/protos/util.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/catalogs/family_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/catalogs/family_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/catalogs/family_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/catalogs/family_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/catalogs/family_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/catalogs/family_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/catalogs/template_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/catalogs/template_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/catalogs/template_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/catalogs/template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/catalogs/template_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/catalogs/template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/clients/address_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/clients/address_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/clients/address_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/clients/address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/clients/address_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/clients/address_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/clients/client_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/clients/client_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/clients/client_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/clients/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/clients/client_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/clients/client_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/calendar_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/calendar_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/calendar_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/calendar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/calendar_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/calendar_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/category_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/category_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/category_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/country_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/country_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/country_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_category_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_category_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_method_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_method_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_schedule_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_warehouse_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_warehouse_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delivery_warehouse_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delivery_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/location_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/location_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x17v1/rules/location.proto\x12"pro.omni.oms.api.v1.rules.location\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb8\x01\n\x08Location\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x17\n\x0flocation_sql_id\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"]\n\x15LocationCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16LocationCreateResponse\x12>\n\x08Location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf1\x02\n\x13LocationReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdd\x01\n\x14LocationReadResponse\x12?\n\tLocations\x18\x01 \x03(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8f\x01\n\x15LocationUpdateRequest\x12>\n\x08Location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16LocationUpdateResponse\x12>\n\x08Location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"[\n\x15LocationDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16LocationDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0fLocationService\x12\x89\x01\n\x0eLocationCreate\x12\x39.pro.omni.oms.api.v1.rules.location.LocationCreateRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationCreateResponse"\x00\x12\x83\x01\n\x0cLocationRead\x12\x37.pro.omni.oms.api.v1.rules.location.LocationReadRequest\x1a\x38.pro.omni.oms.api.v1.rules.location.LocationReadResponse"\x00\x12\x89\x01\n\x0eLocationUpdate\x12\x39.pro.omni.oms.api.v1.rules.location.LocationUpdateRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationUpdateResponse"\x00\x12\x89\x01\n\x0eLocationDelete\x12\x39.pro.omni.oms.api.v1.rules.location.LocationDeleteRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x17v1/rules/location.proto\x12"pro.omni.oms.api.v1.rules.location\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb8\x01\n\x08Location\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x17\n\x0flocation_sql_id\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x84\x01\n\x15LocationCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x17\n\x0flocation_sql_id\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16LocationCreateResponse\x12>\n\x08location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf1\x02\n\x13LocationReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\t\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xdd\x01\n\x14LocationReadResponse\x12?\n\tlocations\x18\x01 \x03(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8f\x01\n\x15LocationUpdateRequest\x12>\n\x08location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16LocationUpdateResponse\x12>\n\x08location\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.rules.location.Location\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"[\n\x15LocationDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16LocationDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0fLocationService\x12\x89\x01\n\x0eLocationCreate\x12\x39.pro.omni.oms.api.v1.rules.location.LocationCreateRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationCreateResponse"\x00\x12\x83\x01\n\x0cLocationRead\x12\x37.pro.omni.oms.api.v1.rules.location.LocationReadRequest\x1a\x38.pro.omni.oms.api.v1.rules.location.LocationReadResponse"\x00\x12\x89\x01\n\x0eLocationUpdate\x12\x39.pro.omni.oms.api.v1.rules.location.LocationUpdateRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationUpdateResponse"\x00\x12\x89\x01\n\x0eLocationDelete\x12\x39.pro.omni.oms.api.v1.rules.location.LocationDeleteRequest\x1a:.pro.omni.oms.api.v1.rules.location.LocationDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.rules.location_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     _globals["_LOCATION"]._serialized_start = 115
     _globals["_LOCATION"]._serialized_end = 299
-    _globals["_LOCATIONCREATEREQUEST"]._serialized_start = 301
-    _globals["_LOCATIONCREATEREQUEST"]._serialized_end = 394
-    _globals["_LOCATIONCREATERESPONSE"]._serialized_start = 397
-    _globals["_LOCATIONCREATERESPONSE"]._serialized_end = 560
-    _globals["_LOCATIONREADREQUEST"]._serialized_start = 563
-    _globals["_LOCATIONREADREQUEST"]._serialized_end = 932
-    _globals["_LOCATIONREADRESPONSE"]._serialized_start = 935
-    _globals["_LOCATIONREADRESPONSE"]._serialized_end = 1156
-    _globals["_LOCATIONUPDATEREQUEST"]._serialized_start = 1159
-    _globals["_LOCATIONUPDATEREQUEST"]._serialized_end = 1302
-    _globals["_LOCATIONUPDATERESPONSE"]._serialized_start = 1305
-    _globals["_LOCATIONUPDATERESPONSE"]._serialized_end = 1468
-    _globals["_LOCATIONDELETEREQUEST"]._serialized_start = 1470
-    _globals["_LOCATIONDELETEREQUEST"]._serialized_end = 1561
-    _globals["_LOCATIONDELETERESPONSE"]._serialized_start = 1563
-    _globals["_LOCATIONDELETERESPONSE"]._serialized_end = 1662
-    _globals["_LOCATIONSERVICE"]._serialized_start = 1665
-    _globals["_LOCATIONSERVICE"]._serialized_end = 2236
+    _globals["_LOCATIONCREATEREQUEST"]._serialized_start = 302
+    _globals["_LOCATIONCREATEREQUEST"]._serialized_end = 434
+    _globals["_LOCATIONCREATERESPONSE"]._serialized_start = 437
+    _globals["_LOCATIONCREATERESPONSE"]._serialized_end = 600
+    _globals["_LOCATIONREADREQUEST"]._serialized_start = 603
+    _globals["_LOCATIONREADREQUEST"]._serialized_end = 972
+    _globals["_LOCATIONREADRESPONSE"]._serialized_start = 975
+    _globals["_LOCATIONREADRESPONSE"]._serialized_end = 1196
+    _globals["_LOCATIONUPDATEREQUEST"]._serialized_start = 1199
+    _globals["_LOCATIONUPDATEREQUEST"]._serialized_end = 1342
+    _globals["_LOCATIONUPDATERESPONSE"]._serialized_start = 1345
+    _globals["_LOCATIONUPDATERESPONSE"]._serialized_end = 1508
+    _globals["_LOCATIONDELETEREQUEST"]._serialized_start = 1510
+    _globals["_LOCATIONDELETEREQUEST"]._serialized_end = 1601
+    _globals["_LOCATIONDELETERESPONSE"]._serialized_start = 1603
+    _globals["_LOCATIONDELETERESPONSE"]._serialized_end = 1702
+    _globals["_LOCATIONSERVICE"]._serialized_start = 1705
+    _globals["_LOCATIONSERVICE"]._serialized_end = 2276
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/location_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/location_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,64 +2,101 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Location(_message.Message):
-    __slots__ = ["id", "name", "code", "location_sql_id", "active", "object_audit"]
+    __slots__ = [
+        "id",
+        "name",
+        "parent_id",
+        "code",
+        "type_location",
+        "barcode",
+        "warehouse_id",
+        "active",
+        "object_audit",
+    ]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    PARENT_ID_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_SQL_ID_FIELD_NUMBER: _ClassVar[int]
+    TYPE_LOCATION_FIELD_NUMBER: _ClassVar[int]
+    BARCODE_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: str
+    id: int
     name: str
+    parent_id: int
     code: str
-    location_sql_id: str
+    type_location: str
+    barcode: str
+    warehouse_id: int
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[str] = ...,
+        id: _Optional[int] = ...,
         name: _Optional[str] = ...,
+        parent_id: _Optional[int] = ...,
         code: _Optional[str] = ...,
-        location_sql_id: _Optional[str] = ...,
+        type_location: _Optional[str] = ...,
+        barcode: _Optional[str] = ...,
+        warehouse_id: _Optional[int] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class LocationCreateRequest(_message.Message):
-    __slots__ = ["name", "context"]
+    __slots__ = ["name", "parent_id", "code", "type_location", "barcode", "warehouse_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    PARENT_ID_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    TYPE_LOCATION_FIELD_NUMBER: _ClassVar[int]
+    BARCODE_FIELD_NUMBER: _ClassVar[int]
+    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
+    parent_id: int
+    code: str
+    type_location: str
+    barcode: str
+    warehouse_id: int
     context: _base_pb2.Context
     def __init__(
-        self, name: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self,
+        name: _Optional[str] = ...,
+        parent_id: _Optional[int] = ...,
+        code: _Optional[str] = ...,
+        type_location: _Optional[str] = ...,
+        barcode: _Optional[str] = ...,
+        warehouse_id: _Optional[int] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class LocationCreateResponse(_message.Message):
-    __slots__ = ["Location", "response_standard"]
-    LOCATION_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["response_standard", "location"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    Location: Location
+    LOCATION_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    location: Location
     def __init__(
         self,
-        Location: _Optional[_Union[Location, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        location: _Optional[_Union[Location, _Mapping]] = ...,
     ) -> None: ...
 
 class LocationReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
@@ -68,74 +105,74 @@
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: str
+    id: int
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[str] = ...,
+        id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class LocationReadResponse(_message.Message):
-    __slots__ = ["Locations", "meta_data", "response_standard"]
-    LOCATIONS_FIELD_NUMBER: _ClassVar[int]
-    META_DATA_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["response_standard", "meta_data", "locations"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    Locations: _containers.RepeatedCompositeFieldContainer[Location]
-    meta_data: _base_pb2.MetaData
+    META_DATA_FIELD_NUMBER: _ClassVar[int]
+    LOCATIONS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    meta_data: _base_pb2.MetaData
+    locations: _containers.RepeatedCompositeFieldContainer[Location]
     def __init__(
         self,
-        Locations: _Optional[_Iterable[_Union[Location, _Mapping]]] = ...,
-        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        locations: _Optional[_Iterable[_Union[Location, _Mapping]]] = ...,
     ) -> None: ...
 
 class LocationUpdateRequest(_message.Message):
-    __slots__ = ["Location", "context"]
+    __slots__ = ["location", "context"]
     LOCATION_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    Location: Location
+    location: Location
     context: _base_pb2.Context
     def __init__(
         self,
-        Location: _Optional[_Union[Location, _Mapping]] = ...,
+        location: _Optional[_Union[Location, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class LocationUpdateResponse(_message.Message):
-    __slots__ = ["Location", "response_standard"]
-    LOCATION_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["response_standard", "location"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    Location: Location
+    LOCATION_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    location: Location
     def __init__(
         self,
-        Location: _Optional[_Union[Location, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        location: _Optional[_Union[Location, _Mapping]] = ...,
     ) -> None: ...
 
 class LocationDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: str
+    id: int
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
 class LocationDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/location_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/location_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_line_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/address_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/address_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/sales/address.proto\x12!pro.omni.oms.api.v1.sales.address\x1a\x11\x63ommon/base.proto"\xad\x01\n\x07\x41\x64\x64ress\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x11\n\tclient_id\x18\x02 \x01(\x05\x12\x16\n\x0e\x61\x64\x64ress_doc_id\x18\x03 \x01(\t\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x06 \x01(\x08\x12?\n\x0cobject_audit\x18\x07 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x95\x01\n\x14\x41\x64\x64ressCreateRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x61\x64\x64ress_doc_id\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x36\n\x07\x63ontext\x18\x05 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x41\x64\x64ressCreateResponse\x12;\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.address.Address\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12\x41\x64\x64ressReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xda\x01\n\x13\x41\x64\x64ressReadResponse\x12=\n\taddresses\x18\x01 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.address.Address\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8b\x01\n\x14\x41\x64\x64ressUpdateRequest\x12;\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.address.Address\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x41\x64\x64ressUpdateResponse\x12;\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.address.Address\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14\x41\x64\x64ressDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x41\x64\x64ressDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0e\x41\x64\x64ressService\x12\x84\x01\n\rAddressCreate\x12\x37.pro.omni.oms.api.v1.sales.address.AddressCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.address.AddressCreateResponse"\x00\x12~\n\x0b\x41\x64\x64ressRead\x12\x35.pro.omni.oms.api.v1.sales.address.AddressReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.address.AddressReadResponse"\x00\x12\x84\x01\n\rAddressUpdate\x12\x37.pro.omni.oms.api.v1.sales.address.AddressUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.address.AddressUpdateResponse"\x00\x12\x84\x01\n\rAddressDelete\x12\x37.pro.omni.oms.api.v1.sales.address.AddressDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.address.AddressDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/sales/address.proto\x12!pro.omni.oms.api.v1.sales.address\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xc9\x01\n\x07\x41\x64\x64ress\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x11\n\tclient_id\x18\x02 \x01(\x05\x12\x16\n\x0e\x61\x64\x64ress_doc_id\x18\x03 \x01(\t\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12*\n\x06\x61\x63tive\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x07 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x95\x01\n\x14\x41\x64\x64ressCreateRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x61\x64\x64ress_doc_id\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x36\n\x07\x63ontext\x18\x05 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x41\x64\x64ressCreateResponse\x12;\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.address.Address\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12\x41\x64\x64ressReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xda\x01\n\x13\x41\x64\x64ressReadResponse\x12=\n\taddresses\x18\x01 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.address.Address\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8b\x01\n\x14\x41\x64\x64ressUpdateRequest\x12;\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.address.Address\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x41\x64\x64ressUpdateResponse\x12;\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.address.Address\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14\x41\x64\x64ressDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x41\x64\x64ressDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0e\x41\x64\x64ressService\x12\x84\x01\n\rAddressCreate\x12\x37.pro.omni.oms.api.v1.sales.address.AddressCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.address.AddressCreateResponse"\x00\x12~\n\x0b\x41\x64\x64ressRead\x12\x35.pro.omni.oms.api.v1.sales.address.AddressReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.address.AddressReadResponse"\x00\x12\x84\x01\n\rAddressUpdate\x12\x37.pro.omni.oms.api.v1.sales.address.AddressUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.address.AddressUpdateResponse"\x00\x12\x84\x01\n\rAddressDelete\x12\x37.pro.omni.oms.api.v1.sales.address.AddressDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.address.AddressDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.address_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_ADDRESS"]._serialized_start = 81
-    _globals["_ADDRESS"]._serialized_end = 254
-    _globals["_ADDRESSCREATEREQUEST"]._serialized_start = 257
-    _globals["_ADDRESSCREATEREQUEST"]._serialized_end = 406
-    _globals["_ADDRESSCREATERESPONSE"]._serialized_start = 409
-    _globals["_ADDRESSCREATERESPONSE"]._serialized_end = 568
-    _globals["_ADDRESSREADREQUEST"]._serialized_start = 571
-    _globals["_ADDRESSREADREQUEST"]._serialized_end = 939
-    _globals["_ADDRESSREADRESPONSE"]._serialized_start = 942
-    _globals["_ADDRESSREADRESPONSE"]._serialized_end = 1160
-    _globals["_ADDRESSUPDATEREQUEST"]._serialized_start = 1163
-    _globals["_ADDRESSUPDATEREQUEST"]._serialized_end = 1302
-    _globals["_ADDRESSUPDATERESPONSE"]._serialized_start = 1305
-    _globals["_ADDRESSUPDATERESPONSE"]._serialized_end = 1464
-    _globals["_ADDRESSDELETEREQUEST"]._serialized_start = 1466
-    _globals["_ADDRESSDELETEREQUEST"]._serialized_end = 1556
-    _globals["_ADDRESSDELETERESPONSE"]._serialized_start = 1558
-    _globals["_ADDRESSDELETERESPONSE"]._serialized_end = 1656
-    _globals["_ADDRESSSERVICE"]._serialized_start = 1659
-    _globals["_ADDRESSSERVICE"]._serialized_end = 2208
+    _globals["_ADDRESS"]._serialized_start = 113
+    _globals["_ADDRESS"]._serialized_end = 314
+    _globals["_ADDRESSCREATEREQUEST"]._serialized_start = 317
+    _globals["_ADDRESSCREATEREQUEST"]._serialized_end = 466
+    _globals["_ADDRESSCREATERESPONSE"]._serialized_start = 469
+    _globals["_ADDRESSCREATERESPONSE"]._serialized_end = 628
+    _globals["_ADDRESSREADREQUEST"]._serialized_start = 631
+    _globals["_ADDRESSREADREQUEST"]._serialized_end = 999
+    _globals["_ADDRESSREADRESPONSE"]._serialized_start = 1002
+    _globals["_ADDRESSREADRESPONSE"]._serialized_end = 1220
+    _globals["_ADDRESSUPDATEREQUEST"]._serialized_start = 1223
+    _globals["_ADDRESSUPDATEREQUEST"]._serialized_end = 1362
+    _globals["_ADDRESSUPDATERESPONSE"]._serialized_start = 1365
+    _globals["_ADDRESSUPDATERESPONSE"]._serialized_end = 1524
+    _globals["_ADDRESSDELETEREQUEST"]._serialized_start = 1526
+    _globals["_ADDRESSDELETEREQUEST"]._serialized_end = 1616
+    _globals["_ADDRESSDELETERESPONSE"]._serialized_start = 1618
+    _globals["_ADDRESSDELETERESPONSE"]._serialized_end = 1716
+    _globals["_ADDRESSSERVICE"]._serialized_start = 1719
+    _globals["_ADDRESSSERVICE"]._serialized_end = 2268
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/address_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/address_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Address(_message.Message):
     __slots__ = ["id", "client_id", "address_doc_id", "code", "name", "active", "object_audit"]
@@ -21,24 +22,24 @@
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     client_id: int
     address_doc_id: str
     code: str
     name: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         client_id: _Optional[int] = ...,
         address_doc_id: _Optional[str] = ...,
         code: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class AddressCreateRequest(_message.Message):
     __slots__ = ["client_id", "address_doc_id", "code", "name", "context"]
     CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
     ADDRESS_DOC_ID_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/address_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/address_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/carrier_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/carrier_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/sales/carrier.proto\x12!pro.omni.oms.api.v1.sales.carrier\x1a\x11\x63ommon/base.proto"\x9a\x01\n\x07\x43\x61rrier\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x16\n\x0e\x63\x61rrier_sql_id\x18\x04 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x82\x01\n\x14\x43\x61rrierCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x16\n\x0e\x63\x61rrier_sql_id\x18\x03 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43\x61rrierCreateResponse\x12;\n\x07\x63\x61rrier\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.carrier.Carrier\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12\x43\x61rrierReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13\x43\x61rrierReadResponse\x12<\n\x08\x63\x61rriers\x18\x01 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.carrier.Carrier\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8b\x01\n\x14\x43\x61rrierUpdateRequest\x12;\n\x07\x63\x61rrier\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.carrier.Carrier\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43\x61rrierUpdateResponse\x12;\n\x07\x63\x61rrier\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.carrier.Carrier\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14\x43\x61rrierDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43\x61rrierDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0e\x43\x61rrierService\x12\x84\x01\n\rCarrierCreate\x12\x37.pro.omni.oms.api.v1.sales.carrier.CarrierCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.carrier.CarrierCreateResponse"\x00\x12~\n\x0b\x43\x61rrierRead\x12\x35.pro.omni.oms.api.v1.sales.carrier.CarrierReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.carrier.CarrierReadResponse"\x00\x12\x84\x01\n\rCarrierUpdate\x12\x37.pro.omni.oms.api.v1.sales.carrier.CarrierUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.carrier.CarrierUpdateResponse"\x00\x12\x84\x01\n\rCarrierDelete\x12\x37.pro.omni.oms.api.v1.sales.carrier.CarrierDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.carrier.CarrierDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/sales/carrier.proto\x12!pro.omni.oms.api.v1.sales.carrier\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb6\x01\n\x07\x43\x61rrier\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x16\n\x0e\x63\x61rrier_sql_id\x18\x04 \x01(\x05\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x82\x01\n\x14\x43\x61rrierCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x16\n\x0e\x63\x61rrier_sql_id\x18\x03 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43\x61rrierCreateResponse\x12;\n\x07\x63\x61rrier\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.carrier.Carrier\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12\x43\x61rrierReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13\x43\x61rrierReadResponse\x12<\n\x08\x63\x61rriers\x18\x01 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.carrier.Carrier\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x8b\x01\n\x14\x43\x61rrierUpdateRequest\x12;\n\x07\x63\x61rrier\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.carrier.Carrier\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43\x61rrierUpdateResponse\x12;\n\x07\x63\x61rrier\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.carrier.Carrier\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14\x43\x61rrierDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43\x61rrierDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0e\x43\x61rrierService\x12\x84\x01\n\rCarrierCreate\x12\x37.pro.omni.oms.api.v1.sales.carrier.CarrierCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.carrier.CarrierCreateResponse"\x00\x12~\n\x0b\x43\x61rrierRead\x12\x35.pro.omni.oms.api.v1.sales.carrier.CarrierReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.carrier.CarrierReadResponse"\x00\x12\x84\x01\n\rCarrierUpdate\x12\x37.pro.omni.oms.api.v1.sales.carrier.CarrierUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.carrier.CarrierUpdateResponse"\x00\x12\x84\x01\n\rCarrierDelete\x12\x37.pro.omni.oms.api.v1.sales.carrier.CarrierDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.carrier.CarrierDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.carrier_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_CARRIER"]._serialized_start = 81
-    _globals["_CARRIER"]._serialized_end = 235
-    _globals["_CARRIERCREATEREQUEST"]._serialized_start = 238
-    _globals["_CARRIERCREATEREQUEST"]._serialized_end = 368
-    _globals["_CARRIERCREATERESPONSE"]._serialized_start = 371
-    _globals["_CARRIERCREATERESPONSE"]._serialized_end = 530
-    _globals["_CARRIERREADREQUEST"]._serialized_start = 533
-    _globals["_CARRIERREADREQUEST"]._serialized_end = 901
-    _globals["_CARRIERREADRESPONSE"]._serialized_start = 904
-    _globals["_CARRIERREADRESPONSE"]._serialized_end = 1121
-    _globals["_CARRIERUPDATEREQUEST"]._serialized_start = 1124
-    _globals["_CARRIERUPDATEREQUEST"]._serialized_end = 1263
-    _globals["_CARRIERUPDATERESPONSE"]._serialized_start = 1266
-    _globals["_CARRIERUPDATERESPONSE"]._serialized_end = 1425
-    _globals["_CARRIERDELETEREQUEST"]._serialized_start = 1427
-    _globals["_CARRIERDELETEREQUEST"]._serialized_end = 1517
-    _globals["_CARRIERDELETERESPONSE"]._serialized_start = 1519
-    _globals["_CARRIERDELETERESPONSE"]._serialized_end = 1617
-    _globals["_CARRIERSERVICE"]._serialized_start = 1620
-    _globals["_CARRIERSERVICE"]._serialized_end = 2169
+    _globals["_CARRIER"]._serialized_start = 113
+    _globals["_CARRIER"]._serialized_end = 295
+    _globals["_CARRIERCREATEREQUEST"]._serialized_start = 298
+    _globals["_CARRIERCREATEREQUEST"]._serialized_end = 428
+    _globals["_CARRIERCREATERESPONSE"]._serialized_start = 431
+    _globals["_CARRIERCREATERESPONSE"]._serialized_end = 590
+    _globals["_CARRIERREADREQUEST"]._serialized_start = 593
+    _globals["_CARRIERREADREQUEST"]._serialized_end = 961
+    _globals["_CARRIERREADRESPONSE"]._serialized_start = 964
+    _globals["_CARRIERREADRESPONSE"]._serialized_end = 1181
+    _globals["_CARRIERUPDATEREQUEST"]._serialized_start = 1184
+    _globals["_CARRIERUPDATEREQUEST"]._serialized_end = 1323
+    _globals["_CARRIERUPDATERESPONSE"]._serialized_start = 1326
+    _globals["_CARRIERUPDATERESPONSE"]._serialized_end = 1485
+    _globals["_CARRIERDELETEREQUEST"]._serialized_start = 1487
+    _globals["_CARRIERDELETEREQUEST"]._serialized_end = 1577
+    _globals["_CARRIERDELETERESPONSE"]._serialized_start = 1579
+    _globals["_CARRIERDELETERESPONSE"]._serialized_end = 1677
+    _globals["_CARRIERSERVICE"]._serialized_start = 1680
+    _globals["_CARRIERSERVICE"]._serialized_end = 2229
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/carrier_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/carrier_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,71 +2,67 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Carrier(_message.Message):
-    __slots__ = ["id", "name", "code", "carrier_sql_id", "active", "object_audit"]
+    __slots__ = ["id", "name", "code", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CARRIER_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     name: str
     code: str
-    carrier_sql_id: int
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        carrier_sql_id: _Optional[int] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class CarrierCreateRequest(_message.Message):
-    __slots__ = ["name", "code", "carrier_sql_id", "context"]
+    __slots__ = ["name", "code", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    CARRIER_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     code: str
-    carrier_sql_id: int
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        carrier_sql_id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class CarrierCreateResponse(_message.Message):
-    __slots__ = ["carrier", "response_standard"]
-    CARRIER_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["response_standard", "carrier"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    carrier: Carrier
+    CARRIER_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    carrier: Carrier
     def __init__(
         self,
-        carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
     ) -> None: ...
 
 class CarrierReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
@@ -89,26 +85,26 @@
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class CarrierReadResponse(_message.Message):
-    __slots__ = ["carriers", "meta_data", "response_standard"]
-    CARRIERS_FIELD_NUMBER: _ClassVar[int]
-    META_DATA_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["response_standard", "meta_data", "carriers"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    carriers: _containers.RepeatedCompositeFieldContainer[Carrier]
-    meta_data: _base_pb2.MetaData
+    META_DATA_FIELD_NUMBER: _ClassVar[int]
+    CARRIERS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    meta_data: _base_pb2.MetaData
+    carriers: _containers.RepeatedCompositeFieldContainer[Carrier]
     def __init__(
         self,
-        carriers: _Optional[_Iterable[_Union[Carrier, _Mapping]]] = ...,
-        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        carriers: _Optional[_Iterable[_Union[Carrier, _Mapping]]] = ...,
     ) -> None: ...
 
 class CarrierUpdateRequest(_message.Message):
     __slots__ = ["carrier", "context"]
     CARRIER_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     carrier: Carrier
@@ -116,23 +112,23 @@
     def __init__(
         self,
         carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class CarrierUpdateResponse(_message.Message):
-    __slots__ = ["carrier", "response_standard"]
-    CARRIER_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["response_standard", "carrier"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    carrier: Carrier
+    CARRIER_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    carrier: Carrier
     def __init__(
         self,
-        carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
     ) -> None: ...
 
 class CarrierDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/carrier_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/carrier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/channel_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/channel_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/sales/channel.proto\x12!pro.omni.oms.api.v1.sales.channel\x1a\x11\x63ommon/base.proto"\x82\x01\n\x07\x43hannel\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"j\n\x14\x43hannelCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43hannelCreateResponse\x12;\n\x07\x63hannel\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.channel.Channel\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12\x43hannelReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13\x43hannelReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12<\n\x08\x63hannels\x18\x03 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.channel.Channel"\x8b\x01\n\x14\x43hannelUpdateRequest\x12;\n\x07\x63hannel\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.channel.Channel\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43hannelUpdateResponse\x12;\n\x07\x63hannel\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.channel.Channel\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14\x43hannelDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43hannelDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x9d\x04\n\x0e\x43hannelService\x12\x82\x01\n\rChannelCreate\x12\x37.pro.omni.oms.api.v1.sales.channel.ChannelCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.channel.ChannelCreateResponse\x12|\n\x0b\x43hannelRead\x12\x35.pro.omni.oms.api.v1.sales.channel.ChannelReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.channel.ChannelReadResponse\x12\x82\x01\n\rChannelUpdate\x12\x37.pro.omni.oms.api.v1.sales.channel.ChannelUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.channel.ChannelUpdateResponse\x12\x82\x01\n\rChannelDelete\x12\x37.pro.omni.oms.api.v1.sales.channel.ChannelDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.channel.ChannelDeleteResponseb\x06proto3'
+    b'\n\x16v1/sales/channel.proto\x12!pro.omni.oms.api.v1.sales.channel\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\x9e\x01\n\x07\x43hannel\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"j\n\x14\x43hannelCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43hannelCreateResponse\x12;\n\x07\x63hannel\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.channel.Channel\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12\x43hannelReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13\x43hannelReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12<\n\x08\x63hannels\x18\x03 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.channel.Channel"\x8b\x01\n\x14\x43hannelUpdateRequest\x12;\n\x07\x63hannel\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.channel.Channel\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43hannelUpdateResponse\x12;\n\x07\x63hannel\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.channel.Channel\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14\x43hannelDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43hannelDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x9d\x04\n\x0e\x43hannelService\x12\x82\x01\n\rChannelCreate\x12\x37.pro.omni.oms.api.v1.sales.channel.ChannelCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.channel.ChannelCreateResponse\x12|\n\x0b\x43hannelRead\x12\x35.pro.omni.oms.api.v1.sales.channel.ChannelReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.channel.ChannelReadResponse\x12\x82\x01\n\rChannelUpdate\x12\x37.pro.omni.oms.api.v1.sales.channel.ChannelUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.channel.ChannelUpdateResponse\x12\x82\x01\n\rChannelDelete\x12\x37.pro.omni.oms.api.v1.sales.channel.ChannelDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.channel.ChannelDeleteResponseb\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.channel_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_CHANNEL"]._serialized_start = 81
-    _globals["_CHANNEL"]._serialized_end = 211
-    _globals["_CHANNELCREATEREQUEST"]._serialized_start = 213
-    _globals["_CHANNELCREATEREQUEST"]._serialized_end = 319
-    _globals["_CHANNELCREATERESPONSE"]._serialized_start = 322
-    _globals["_CHANNELCREATERESPONSE"]._serialized_end = 481
-    _globals["_CHANNELREADREQUEST"]._serialized_start = 484
-    _globals["_CHANNELREADREQUEST"]._serialized_end = 852
-    _globals["_CHANNELREADRESPONSE"]._serialized_start = 855
-    _globals["_CHANNELREADRESPONSE"]._serialized_end = 1072
-    _globals["_CHANNELUPDATEREQUEST"]._serialized_start = 1075
-    _globals["_CHANNELUPDATEREQUEST"]._serialized_end = 1214
-    _globals["_CHANNELUPDATERESPONSE"]._serialized_start = 1217
-    _globals["_CHANNELUPDATERESPONSE"]._serialized_end = 1376
-    _globals["_CHANNELDELETEREQUEST"]._serialized_start = 1378
-    _globals["_CHANNELDELETEREQUEST"]._serialized_end = 1468
-    _globals["_CHANNELDELETERESPONSE"]._serialized_start = 1470
-    _globals["_CHANNELDELETERESPONSE"]._serialized_end = 1568
-    _globals["_CHANNELSERVICE"]._serialized_start = 1571
-    _globals["_CHANNELSERVICE"]._serialized_end = 2112
+    _globals["_CHANNEL"]._serialized_start = 113
+    _globals["_CHANNEL"]._serialized_end = 271
+    _globals["_CHANNELCREATEREQUEST"]._serialized_start = 273
+    _globals["_CHANNELCREATEREQUEST"]._serialized_end = 379
+    _globals["_CHANNELCREATERESPONSE"]._serialized_start = 382
+    _globals["_CHANNELCREATERESPONSE"]._serialized_end = 541
+    _globals["_CHANNELREADREQUEST"]._serialized_start = 544
+    _globals["_CHANNELREADREQUEST"]._serialized_end = 912
+    _globals["_CHANNELREADRESPONSE"]._serialized_start = 915
+    _globals["_CHANNELREADRESPONSE"]._serialized_end = 1132
+    _globals["_CHANNELUPDATEREQUEST"]._serialized_start = 1135
+    _globals["_CHANNELUPDATEREQUEST"]._serialized_end = 1274
+    _globals["_CHANNELUPDATERESPONSE"]._serialized_start = 1277
+    _globals["_CHANNELUPDATERESPONSE"]._serialized_end = 1436
+    _globals["_CHANNELDELETEREQUEST"]._serialized_start = 1438
+    _globals["_CHANNELDELETEREQUEST"]._serialized_end = 1528
+    _globals["_CHANNELDELETERESPONSE"]._serialized_start = 1530
+    _globals["_CHANNELDELETERESPONSE"]._serialized_end = 1628
+    _globals["_CHANNELSERVICE"]._serialized_start = 1631
+    _globals["_CHANNELSERVICE"]._serialized_end = 2172
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/channel_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/channel_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Channel(_message.Message):
     __slots__ = ["id", "name", "code", "active", "object_audit"]
@@ -17,22 +18,22 @@
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     name: str
     code: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class ChannelCreateRequest(_message.Message):
     __slots__ = ["name", "code", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/channel_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/client_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/client_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x15v1/sales/client.proto\x12 pro.omni.oms.api.v1.sales.client\x1a\x11\x63ommon/base.proto"\x8a\x01\n\x06\x43lient\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rclient_doc_id\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"r\n\x13\x43lientCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rclient_doc_id\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9b\x01\n\x14\x43lientCreateResponse\x12\x38\n\x06\x63lient\x18\x01 \x01(\x0b\x32(.pro.omni.oms.api.v1.sales.client.Client\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xef\x02\n\x11\x43lientReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd5\x01\n\x12\x43lientReadResponse\x12\x39\n\x07\x63lients\x18\x01 \x03(\x0b\x32(.pro.omni.oms.api.v1.sales.client.Client\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x87\x01\n\x13\x43lientUpdateRequest\x12\x38\n\x06\x63lient\x18\x01 \x01(\x0b\x32(.pro.omni.oms.api.v1.sales.client.Client\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9b\x01\n\x14\x43lientUpdateResponse\x12\x38\n\x06\x63lient\x18\x01 \x01(\x0b\x32(.pro.omni.oms.api.v1.sales.client.Client\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Y\n\x13\x43lientDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"a\n\x14\x43lientDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x8d\x04\n\rClientService\x12\x7f\n\x0c\x43lientCreate\x12\x35.pro.omni.oms.api.v1.sales.client.ClientCreateRequest\x1a\x36.pro.omni.oms.api.v1.sales.client.ClientCreateResponse"\x00\x12y\n\nClientRead\x12\x33.pro.omni.oms.api.v1.sales.client.ClientReadRequest\x1a\x34.pro.omni.oms.api.v1.sales.client.ClientReadResponse"\x00\x12\x7f\n\x0c\x43lientUpdate\x12\x35.pro.omni.oms.api.v1.sales.client.ClientUpdateRequest\x1a\x36.pro.omni.oms.api.v1.sales.client.ClientUpdateResponse"\x00\x12\x7f\n\x0c\x43lientDelete\x12\x35.pro.omni.oms.api.v1.sales.client.ClientDeleteRequest\x1a\x36.pro.omni.oms.api.v1.sales.client.ClientDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x15v1/sales/client.proto\x12 pro.omni.oms.api.v1.sales.client\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xa6\x01\n\x06\x43lient\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rclient_doc_id\x18\x03 \x01(\t\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"r\n\x13\x43lientCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rclient_doc_id\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9b\x01\n\x14\x43lientCreateResponse\x12\x38\n\x06\x63lient\x18\x01 \x01(\x0b\x32(.pro.omni.oms.api.v1.sales.client.Client\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xef\x02\n\x11\x43lientReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd5\x01\n\x12\x43lientReadResponse\x12\x39\n\x07\x63lients\x18\x01 \x03(\x0b\x32(.pro.omni.oms.api.v1.sales.client.Client\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x87\x01\n\x13\x43lientUpdateRequest\x12\x38\n\x06\x63lient\x18\x01 \x01(\x0b\x32(.pro.omni.oms.api.v1.sales.client.Client\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9b\x01\n\x14\x43lientUpdateResponse\x12\x38\n\x06\x63lient\x18\x01 \x01(\x0b\x32(.pro.omni.oms.api.v1.sales.client.Client\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Y\n\x13\x43lientDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"a\n\x14\x43lientDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x8d\x04\n\rClientService\x12\x7f\n\x0c\x43lientCreate\x12\x35.pro.omni.oms.api.v1.sales.client.ClientCreateRequest\x1a\x36.pro.omni.oms.api.v1.sales.client.ClientCreateResponse"\x00\x12y\n\nClientRead\x12\x33.pro.omni.oms.api.v1.sales.client.ClientReadRequest\x1a\x34.pro.omni.oms.api.v1.sales.client.ClientReadResponse"\x00\x12\x7f\n\x0c\x43lientUpdate\x12\x35.pro.omni.oms.api.v1.sales.client.ClientUpdateRequest\x1a\x36.pro.omni.oms.api.v1.sales.client.ClientUpdateResponse"\x00\x12\x7f\n\x0c\x43lientDelete\x12\x35.pro.omni.oms.api.v1.sales.client.ClientDeleteRequest\x1a\x36.pro.omni.oms.api.v1.sales.client.ClientDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.client_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_CLIENT"]._serialized_start = 79
-    _globals["_CLIENT"]._serialized_end = 217
-    _globals["_CLIENTCREATEREQUEST"]._serialized_start = 219
-    _globals["_CLIENTCREATEREQUEST"]._serialized_end = 333
-    _globals["_CLIENTCREATERESPONSE"]._serialized_start = 336
-    _globals["_CLIENTCREATERESPONSE"]._serialized_end = 491
-    _globals["_CLIENTREADREQUEST"]._serialized_start = 494
-    _globals["_CLIENTREADREQUEST"]._serialized_end = 861
-    _globals["_CLIENTREADRESPONSE"]._serialized_start = 864
-    _globals["_CLIENTREADRESPONSE"]._serialized_end = 1077
-    _globals["_CLIENTUPDATEREQUEST"]._serialized_start = 1080
-    _globals["_CLIENTUPDATEREQUEST"]._serialized_end = 1215
-    _globals["_CLIENTUPDATERESPONSE"]._serialized_start = 1218
-    _globals["_CLIENTUPDATERESPONSE"]._serialized_end = 1373
-    _globals["_CLIENTDELETEREQUEST"]._serialized_start = 1375
-    _globals["_CLIENTDELETEREQUEST"]._serialized_end = 1464
-    _globals["_CLIENTDELETERESPONSE"]._serialized_start = 1466
-    _globals["_CLIENTDELETERESPONSE"]._serialized_end = 1563
-    _globals["_CLIENTSERVICE"]._serialized_start = 1566
-    _globals["_CLIENTSERVICE"]._serialized_end = 2091
+    _globals["_CLIENT"]._serialized_start = 111
+    _globals["_CLIENT"]._serialized_end = 277
+    _globals["_CLIENTCREATEREQUEST"]._serialized_start = 279
+    _globals["_CLIENTCREATEREQUEST"]._serialized_end = 393
+    _globals["_CLIENTCREATERESPONSE"]._serialized_start = 396
+    _globals["_CLIENTCREATERESPONSE"]._serialized_end = 551
+    _globals["_CLIENTREADREQUEST"]._serialized_start = 554
+    _globals["_CLIENTREADREQUEST"]._serialized_end = 921
+    _globals["_CLIENTREADRESPONSE"]._serialized_start = 924
+    _globals["_CLIENTREADRESPONSE"]._serialized_end = 1137
+    _globals["_CLIENTUPDATEREQUEST"]._serialized_start = 1140
+    _globals["_CLIENTUPDATEREQUEST"]._serialized_end = 1275
+    _globals["_CLIENTUPDATERESPONSE"]._serialized_start = 1278
+    _globals["_CLIENTUPDATERESPONSE"]._serialized_end = 1433
+    _globals["_CLIENTDELETEREQUEST"]._serialized_start = 1435
+    _globals["_CLIENTDELETEREQUEST"]._serialized_end = 1524
+    _globals["_CLIENTDELETERESPONSE"]._serialized_start = 1526
+    _globals["_CLIENTDELETERESPONSE"]._serialized_end = 1623
+    _globals["_CLIENTSERVICE"]._serialized_start = 1626
+    _globals["_CLIENTSERVICE"]._serialized_end = 2151
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/client_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/client_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Client(_message.Message):
     __slots__ = ["id", "name", "client_doc_id", "active", "object_audit"]
@@ -17,22 +18,22 @@
     NAME_FIELD_NUMBER: _ClassVar[int]
     CLIENT_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     name: str
     client_doc_id: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         name: _Optional[str] = ...,
         client_doc_id: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class ClientCreateRequest(_message.Message):
     __slots__ = ["name", "client_doc_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CLIENT_DOC_ID_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/client_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/client_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/country_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/country_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/sales/country.proto\x12!pro.omni.oms.api.v1.sales.country\x1a\x11\x63ommon/base.proto"\x8c\x01\n\x07\x43ountry\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ountry_doc_id\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"t\n\x14\x43ountryCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0e\x63ountry_doc_id\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43ountryCreateResponse\x12;\n\x07\x63ountry\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.country.Country\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12\x43ountryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xda\x01\n\x13\x43ountryReadResponse\x12=\n\tcountries\x18\x01 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.country.Country\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x8b\x01\n\x14\x43ountryUpdateRequest\x12;\n\x07\x63ountry\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.country.Country\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43ountryUpdateResponse\x12;\n\x07\x63ountry\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.country.Country\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14\x43ountryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43ountryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0e\x43ountryService\x12\x84\x01\n\rCountryCreate\x12\x37.pro.omni.oms.api.v1.sales.country.CountryCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.country.CountryCreateResponse"\x00\x12~\n\x0b\x43ountryRead\x12\x35.pro.omni.oms.api.v1.sales.country.CountryReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.country.CountryReadResponse"\x00\x12\x84\x01\n\rCountryUpdate\x12\x37.pro.omni.oms.api.v1.sales.country.CountryUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.country.CountryUpdateResponse"\x00\x12\x84\x01\n\rCountryDelete\x12\x37.pro.omni.oms.api.v1.sales.country.CountryDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.country.CountryDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/sales/country.proto\x12!pro.omni.oms.api.v1.sales.country\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xa8\x01\n\x07\x43ountry\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ountry_doc_id\x18\x03 \x01(\t\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"t\n\x14\x43ountryCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0e\x63ountry_doc_id\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43ountryCreateResponse\x12;\n\x07\x63ountry\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.country.Country\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12\x43ountryReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xda\x01\n\x13\x43ountryReadResponse\x12=\n\tcountries\x18\x01 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.country.Country\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x8b\x01\n\x14\x43ountryUpdateRequest\x12;\n\x07\x63ountry\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.country.Country\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15\x43ountryUpdateResponse\x12;\n\x07\x63ountry\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.country.Country\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14\x43ountryDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15\x43ountryDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0e\x43ountryService\x12\x84\x01\n\rCountryCreate\x12\x37.pro.omni.oms.api.v1.sales.country.CountryCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.country.CountryCreateResponse"\x00\x12~\n\x0b\x43ountryRead\x12\x35.pro.omni.oms.api.v1.sales.country.CountryReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.country.CountryReadResponse"\x00\x12\x84\x01\n\rCountryUpdate\x12\x37.pro.omni.oms.api.v1.sales.country.CountryUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.country.CountryUpdateResponse"\x00\x12\x84\x01\n\rCountryDelete\x12\x37.pro.omni.oms.api.v1.sales.country.CountryDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.country.CountryDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.country_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_COUNTRY"]._serialized_start = 81
-    _globals["_COUNTRY"]._serialized_end = 221
-    _globals["_COUNTRYCREATEREQUEST"]._serialized_start = 223
-    _globals["_COUNTRYCREATEREQUEST"]._serialized_end = 339
-    _globals["_COUNTRYCREATERESPONSE"]._serialized_start = 342
-    _globals["_COUNTRYCREATERESPONSE"]._serialized_end = 501
-    _globals["_COUNTRYREADREQUEST"]._serialized_start = 504
-    _globals["_COUNTRYREADREQUEST"]._serialized_end = 872
-    _globals["_COUNTRYREADRESPONSE"]._serialized_start = 875
-    _globals["_COUNTRYREADRESPONSE"]._serialized_end = 1093
-    _globals["_COUNTRYUPDATEREQUEST"]._serialized_start = 1096
-    _globals["_COUNTRYUPDATEREQUEST"]._serialized_end = 1235
-    _globals["_COUNTRYUPDATERESPONSE"]._serialized_start = 1238
-    _globals["_COUNTRYUPDATERESPONSE"]._serialized_end = 1397
-    _globals["_COUNTRYDELETEREQUEST"]._serialized_start = 1399
-    _globals["_COUNTRYDELETEREQUEST"]._serialized_end = 1489
-    _globals["_COUNTRYDELETERESPONSE"]._serialized_start = 1491
-    _globals["_COUNTRYDELETERESPONSE"]._serialized_end = 1589
-    _globals["_COUNTRYSERVICE"]._serialized_start = 1592
-    _globals["_COUNTRYSERVICE"]._serialized_end = 2141
+    _globals["_COUNTRY"]._serialized_start = 113
+    _globals["_COUNTRY"]._serialized_end = 281
+    _globals["_COUNTRYCREATEREQUEST"]._serialized_start = 283
+    _globals["_COUNTRYCREATEREQUEST"]._serialized_end = 399
+    _globals["_COUNTRYCREATERESPONSE"]._serialized_start = 402
+    _globals["_COUNTRYCREATERESPONSE"]._serialized_end = 561
+    _globals["_COUNTRYREADREQUEST"]._serialized_start = 564
+    _globals["_COUNTRYREADREQUEST"]._serialized_end = 932
+    _globals["_COUNTRYREADRESPONSE"]._serialized_start = 935
+    _globals["_COUNTRYREADRESPONSE"]._serialized_end = 1153
+    _globals["_COUNTRYUPDATEREQUEST"]._serialized_start = 1156
+    _globals["_COUNTRYUPDATEREQUEST"]._serialized_end = 1295
+    _globals["_COUNTRYUPDATERESPONSE"]._serialized_start = 1298
+    _globals["_COUNTRYUPDATERESPONSE"]._serialized_end = 1457
+    _globals["_COUNTRYDELETEREQUEST"]._serialized_start = 1459
+    _globals["_COUNTRYDELETEREQUEST"]._serialized_end = 1549
+    _globals["_COUNTRYDELETERESPONSE"]._serialized_start = 1551
+    _globals["_COUNTRYDELETERESPONSE"]._serialized_end = 1649
+    _globals["_COUNTRYSERVICE"]._serialized_start = 1652
+    _globals["_COUNTRYSERVICE"]._serialized_end = 2201
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/country_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/country_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Country(_message.Message):
     __slots__ = ["id", "name", "country_doc_id", "active", "object_audit"]
@@ -17,22 +18,22 @@
     NAME_FIELD_NUMBER: _ClassVar[int]
     COUNTRY_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     name: str
     country_doc_id: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         name: _Optional[str] = ...,
         country_doc_id: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class CountryCreateRequest(_message.Message):
     __slots__ = ["name", "country_doc_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     COUNTRY_DOC_ID_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/country_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/currency_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/currency_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x17v1/sales/currency.proto\x12"pro.omni.oms.api.v1.sales.currency\x1a\x11\x63ommon/base.proto"\x9c\x01\n\x08\x43urrency\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x17\n\x0f\x63urrency_doc_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x84\x01\n\x15\x43urrencyCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x17\n\x0f\x63urrency_doc_id\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43urrencyCreateResponse\x12>\n\x08\x63urrency\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.sales.currency.Currency\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf1\x02\n\x13\x43urrencyReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xde\x01\n\x14\x43urrencyReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12@\n\ncurrencies\x18\x03 \x03(\x0b\x32,.pro.omni.oms.api.v1.sales.currency.Currency"\x8f\x01\n\x15\x43urrencyUpdateRequest\x12>\n\x08\x63urrency\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.sales.currency.Currency\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43urrencyUpdateResponse\x12>\n\x08\x63urrency\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.sales.currency.Currency\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"[\n\x15\x43urrencyDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16\x43urrencyDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0f\x43urrencyService\x12\x89\x01\n\x0e\x43urrencyCreate\x12\x39.pro.omni.oms.api.v1.sales.currency.CurrencyCreateRequest\x1a:.pro.omni.oms.api.v1.sales.currency.CurrencyCreateResponse"\x00\x12\x83\x01\n\x0c\x43urrencyRead\x12\x37.pro.omni.oms.api.v1.sales.currency.CurrencyReadRequest\x1a\x38.pro.omni.oms.api.v1.sales.currency.CurrencyReadResponse"\x00\x12\x89\x01\n\x0e\x43urrencyUpdate\x12\x39.pro.omni.oms.api.v1.sales.currency.CurrencyUpdateRequest\x1a:.pro.omni.oms.api.v1.sales.currency.CurrencyUpdateResponse"\x00\x12\x89\x01\n\x0e\x43urrencyDelete\x12\x39.pro.omni.oms.api.v1.sales.currency.CurrencyDeleteRequest\x1a:.pro.omni.oms.api.v1.sales.currency.CurrencyDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x17v1/sales/currency.proto\x12"pro.omni.oms.api.v1.sales.currency\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb8\x01\n\x08\x43urrency\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x17\n\x0f\x63urrency_doc_id\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x84\x01\n\x15\x43urrencyCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x17\n\x0f\x63urrency_doc_id\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43urrencyCreateResponse\x12>\n\x08\x63urrency\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.sales.currency.Currency\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf1\x02\n\x13\x43urrencyReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xde\x01\n\x14\x43urrencyReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12@\n\ncurrencies\x18\x03 \x03(\x0b\x32,.pro.omni.oms.api.v1.sales.currency.Currency"\x8f\x01\n\x15\x43urrencyUpdateRequest\x12>\n\x08\x63urrency\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.sales.currency.Currency\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa3\x01\n\x16\x43urrencyUpdateResponse\x12>\n\x08\x63urrency\x18\x01 \x01(\x0b\x32,.pro.omni.oms.api.v1.sales.currency.Currency\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"[\n\x15\x43urrencyDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"c\n\x16\x43urrencyDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xbb\x04\n\x0f\x43urrencyService\x12\x89\x01\n\x0e\x43urrencyCreate\x12\x39.pro.omni.oms.api.v1.sales.currency.CurrencyCreateRequest\x1a:.pro.omni.oms.api.v1.sales.currency.CurrencyCreateResponse"\x00\x12\x83\x01\n\x0c\x43urrencyRead\x12\x37.pro.omni.oms.api.v1.sales.currency.CurrencyReadRequest\x1a\x38.pro.omni.oms.api.v1.sales.currency.CurrencyReadResponse"\x00\x12\x89\x01\n\x0e\x43urrencyUpdate\x12\x39.pro.omni.oms.api.v1.sales.currency.CurrencyUpdateRequest\x1a:.pro.omni.oms.api.v1.sales.currency.CurrencyUpdateResponse"\x00\x12\x89\x01\n\x0e\x43urrencyDelete\x12\x39.pro.omni.oms.api.v1.sales.currency.CurrencyDeleteRequest\x1a:.pro.omni.oms.api.v1.sales.currency.CurrencyDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.currency_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_CURRENCY"]._serialized_start = 83
-    _globals["_CURRENCY"]._serialized_end = 239
-    _globals["_CURRENCYCREATEREQUEST"]._serialized_start = 242
-    _globals["_CURRENCYCREATEREQUEST"]._serialized_end = 374
-    _globals["_CURRENCYCREATERESPONSE"]._serialized_start = 377
-    _globals["_CURRENCYCREATERESPONSE"]._serialized_end = 540
-    _globals["_CURRENCYREADREQUEST"]._serialized_start = 543
-    _globals["_CURRENCYREADREQUEST"]._serialized_end = 912
-    _globals["_CURRENCYREADRESPONSE"]._serialized_start = 915
-    _globals["_CURRENCYREADRESPONSE"]._serialized_end = 1137
-    _globals["_CURRENCYUPDATEREQUEST"]._serialized_start = 1140
-    _globals["_CURRENCYUPDATEREQUEST"]._serialized_end = 1283
-    _globals["_CURRENCYUPDATERESPONSE"]._serialized_start = 1286
-    _globals["_CURRENCYUPDATERESPONSE"]._serialized_end = 1449
-    _globals["_CURRENCYDELETEREQUEST"]._serialized_start = 1451
-    _globals["_CURRENCYDELETEREQUEST"]._serialized_end = 1542
-    _globals["_CURRENCYDELETERESPONSE"]._serialized_start = 1544
-    _globals["_CURRENCYDELETERESPONSE"]._serialized_end = 1643
-    _globals["_CURRENCYSERVICE"]._serialized_start = 1646
-    _globals["_CURRENCYSERVICE"]._serialized_end = 2217
+    _globals["_CURRENCY"]._serialized_start = 115
+    _globals["_CURRENCY"]._serialized_end = 299
+    _globals["_CURRENCYCREATEREQUEST"]._serialized_start = 302
+    _globals["_CURRENCYCREATEREQUEST"]._serialized_end = 434
+    _globals["_CURRENCYCREATERESPONSE"]._serialized_start = 437
+    _globals["_CURRENCYCREATERESPONSE"]._serialized_end = 600
+    _globals["_CURRENCYREADREQUEST"]._serialized_start = 603
+    _globals["_CURRENCYREADREQUEST"]._serialized_end = 972
+    _globals["_CURRENCYREADRESPONSE"]._serialized_start = 975
+    _globals["_CURRENCYREADRESPONSE"]._serialized_end = 1197
+    _globals["_CURRENCYUPDATEREQUEST"]._serialized_start = 1200
+    _globals["_CURRENCYUPDATEREQUEST"]._serialized_end = 1343
+    _globals["_CURRENCYUPDATERESPONSE"]._serialized_start = 1346
+    _globals["_CURRENCYUPDATERESPONSE"]._serialized_end = 1509
+    _globals["_CURRENCYDELETEREQUEST"]._serialized_start = 1511
+    _globals["_CURRENCYDELETEREQUEST"]._serialized_end = 1602
+    _globals["_CURRENCYDELETERESPONSE"]._serialized_start = 1604
+    _globals["_CURRENCYDELETERESPONSE"]._serialized_end = 1703
+    _globals["_CURRENCYSERVICE"]._serialized_start = 1706
+    _globals["_CURRENCYSERVICE"]._serialized_end = 2277
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/currency_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/currency_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Currency(_message.Message):
     __slots__ = ["id", "name", "code", "currency_doc_id", "active", "object_audit"]
@@ -19,23 +20,23 @@
     CURRENCY_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     name: str
     code: str
     currency_doc_id: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
         currency_doc_id: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class CurrencyCreateRequest(_message.Message):
     __slots__ = ["name", "code", "currency_doc_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/currency_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/currency_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/delivery_method_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/delivery_method_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1ev1/sales/delivery_method.proto\x12)pro.omni.oms.api.v1.sales.delivery.method\x1a\x11\x63ommon/base.proto"\x89\x01\n\x0e\x44\x65liveryMethod\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"q\n\x1b\x44\x65liveryMethodCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodCreateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf7\x02\n\x19\x44\x65liveryMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf7\x01\n\x1a\x44\x65liveryMethodReadResponse\x12S\n\x10\x64\x65livery_methods\x18\x01 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa9\x01\n\x1b\x44\x65liveryMethodUpdateRequest\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodUpdateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"a\n\x1b\x44\x65liveryMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"i\n\x1c\x44\x65liveryMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xc5\x05\n\x15\x44\x65liveryMethodService\x12\xaa\x01\n\x15\x44\x65liveryServiceCreate\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodCreateRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodCreateResponse"\x00\x12\xa4\x01\n\x13\x44\x65liveryServiceRead\x12\x44.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodReadRequest\x1a\x45.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodReadResponse"\x00\x12\xaa\x01\n\x15\x44\x65liveryServiceUpdate\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodUpdateRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodUpdateResponse"\x00\x12\xaa\x01\n\x15\x44\x65liveryServiceDelete\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodDeleteRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1ev1/sales/delivery_method.proto\x12)pro.omni.oms.api.v1.sales.delivery.method\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xa5\x01\n\x0e\x44\x65liveryMethod\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"q\n\x1b\x44\x65liveryMethodCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodCreateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf7\x02\n\x19\x44\x65liveryMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf7\x01\n\x1a\x44\x65liveryMethodReadResponse\x12S\n\x10\x64\x65livery_methods\x18\x01 \x03(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xa9\x01\n\x1b\x44\x65liveryMethodUpdateRequest\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xbd\x01\n\x1c\x44\x65liveryMethodUpdateResponse\x12R\n\x0f\x64\x65livery_method\x18\x01 \x01(\x0b\x32\x39.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"a\n\x1b\x44\x65liveryMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"i\n\x1c\x44\x65liveryMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xc5\x05\n\x15\x44\x65liveryMethodService\x12\xaa\x01\n\x15\x44\x65liveryServiceCreate\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodCreateRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodCreateResponse"\x00\x12\xa4\x01\n\x13\x44\x65liveryServiceRead\x12\x44.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodReadRequest\x1a\x45.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodReadResponse"\x00\x12\xaa\x01\n\x15\x44\x65liveryServiceUpdate\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodUpdateRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodUpdateResponse"\x00\x12\xaa\x01\n\x15\x44\x65liveryServiceDelete\x12\x46.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodDeleteRequest\x1aG.pro.omni.oms.api.v1.sales.delivery.method.DeliveryMethodDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.delivery_method_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_DELIVERYMETHOD"]._serialized_start = 97
-    _globals["_DELIVERYMETHOD"]._serialized_end = 234
-    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_start = 236
-    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_end = 349
-    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_start = 352
-    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_end = 541
-    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_start = 544
-    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_end = 919
-    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_start = 922
-    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_end = 1169
-    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_start = 1172
-    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_end = 1341
-    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_start = 1344
-    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_end = 1533
-    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_start = 1535
-    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_end = 1632
-    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_start = 1634
-    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_end = 1739
-    _globals["_DELIVERYMETHODSERVICE"]._serialized_start = 1742
-    _globals["_DELIVERYMETHODSERVICE"]._serialized_end = 2451
+    _globals["_DELIVERYMETHOD"]._serialized_start = 129
+    _globals["_DELIVERYMETHOD"]._serialized_end = 294
+    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_start = 296
+    _globals["_DELIVERYMETHODCREATEREQUEST"]._serialized_end = 409
+    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_start = 412
+    _globals["_DELIVERYMETHODCREATERESPONSE"]._serialized_end = 601
+    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_start = 604
+    _globals["_DELIVERYMETHODREADREQUEST"]._serialized_end = 979
+    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_start = 982
+    _globals["_DELIVERYMETHODREADRESPONSE"]._serialized_end = 1229
+    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_start = 1232
+    _globals["_DELIVERYMETHODUPDATEREQUEST"]._serialized_end = 1401
+    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_start = 1404
+    _globals["_DELIVERYMETHODUPDATERESPONSE"]._serialized_end = 1593
+    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_start = 1595
+    _globals["_DELIVERYMETHODDELETEREQUEST"]._serialized_end = 1692
+    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_start = 1694
+    _globals["_DELIVERYMETHODDELETERESPONSE"]._serialized_end = 1799
+    _globals["_DELIVERYMETHODSERVICE"]._serialized_start = 1802
+    _globals["_DELIVERYMETHODSERVICE"]._serialized_end = 2511
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/delivery_method_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/delivery_method_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class DeliveryMethod(_message.Message):
     __slots__ = ["id", "name", "code", "active", "object_audit"]
@@ -17,22 +18,22 @@
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     code: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class DeliveryMethodCreateRequest(_message.Message):
     __slots__ = ["name", "code", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/order_line_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/order_line_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x19v1/sales/order_line.proto\x12$pro.omni.oms.api.v1.sales.order.line\x1a\x11\x63ommon/base.proto"\x93\x02\n\tOrderLine\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x10\n\x08order_id\x18\x02 \x01(\x05\x12\x12\n\nproduct_id\x18\x03 \x01(\x05\x12\x10\n\x08quantity\x18\x04 \x01(\x02\x12\x0e\n\x06uom_id\x18\x05 \x01(\x05\x12\x12\n\nprice_unit\x18\x06 \x01(\x02\x12\x0e\n\x06tax_id\x18\x07 \x01(\x05\x12\x10\n\x08\x64iscount\x18\x08 \x01(\x02\x12\x16\n\x0eprice_subtotal\x18\t \x01(\x02\x12\x13\n\x0bprice_total\x18\n \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x0b \x01(\x08\x12?\n\x0cobject_audit\x18\x0c \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xfb\x01\n\x16OrderLineCreateRequest\x12\x10\n\x08order_id\x18\x01 \x01(\x05\x12\x12\n\nproduct_id\x18\x02 \x01(\x05\x12\x10\n\x08quantity\x18\x03 \x01(\x02\x12\x0e\n\x06uom_id\x18\x04 \x01(\x05\x12\x12\n\nprice_unit\x18\x05 \x01(\x02\x12\x0e\n\x06tax_id\x18\x06 \x01(\x05\x12\x10\n\x08\x64iscount\x18\x07 \x01(\x02\x12\x16\n\x0eprice_subtotal\x18\x08 \x01(\x02\x12\x13\n\x0bprice_total\x18\t \x01(\x02\x12\x36\n\x07\x63ontext\x18\n \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17OrderLineCreateResponse\x12\x43\n\norder_line\x18\x01 \x01(\x0b\x32/.pro.omni.oms.api.v1.sales.order.line.OrderLine\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf2\x02\n\x14OrderLineReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe3\x01\n\x15OrderLineReadResponse\x12\x44\n\x0border_lines\x18\x01 \x03(\x0b\x32/.pro.omni.oms.api.v1.sales.order.line.OrderLine\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x95\x01\n\x16OrderLineUpdateRequest\x12\x43\n\norder_line\x18\x01 \x01(\x0b\x32/.pro.omni.oms.api.v1.sales.order.line.OrderLine\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17OrderLineUpdateResponse\x12\x43\n\norder_line\x18\x01 \x01(\x0b\x32/.pro.omni.oms.api.v1.sales.order.line.OrderLine\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\\\n\x16OrderLineDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17OrderLineDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd8\x04\n\x10OrderLineService\x12\x90\x01\n\x0fOrderLineCreate\x12<.pro.omni.oms.api.v1.sales.order.line.OrderLineCreateRequest\x1a=.pro.omni.oms.api.v1.sales.order.line.OrderLineCreateResponse"\x00\x12\x8a\x01\n\rOrderLineRead\x12:.pro.omni.oms.api.v1.sales.order.line.OrderLineReadRequest\x1a;.pro.omni.oms.api.v1.sales.order.line.OrderLineReadResponse"\x00\x12\x90\x01\n\x0fOrderLineUpdate\x12<.pro.omni.oms.api.v1.sales.order.line.OrderLineUpdateRequest\x1a=.pro.omni.oms.api.v1.sales.order.line.OrderLineUpdateResponse"\x00\x12\x90\x01\n\x0fOrderLineDelete\x12<.pro.omni.oms.api.v1.sales.order.line.OrderLineDeleteRequest\x1a=.pro.omni.oms.api.v1.sales.order.line.OrderLineDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x19v1/sales/order_line.proto\x12$pro.omni.oms.api.v1.sales.order.line\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\x97\x02\n\tOrderLine\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x10\n\x08order_id\x18\x02 \x01(\x05\x12\x12\n\nproduct_id\x18\x03 \x01(\x05\x12\x10\n\x08quantity\x18\x04 \x01(\x02\x12\x0e\n\x06uom_id\x18\x05 \x01(\x05\x12\x12\n\nprice_unit\x18\x06 \x01(\x02\x12\x0e\n\x06tax_id\x18\x07 \x01(\x05\x12\x10\n\x08\x64iscount\x18\x08 \x01(\x02\x12\x13\n\x0bprice_total\x18\t \x01(\x02\x12*\n\x06\x61\x63tive\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0b \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xe3\x01\n\x16OrderLineCreateRequest\x12\x10\n\x08order_id\x18\x01 \x01(\x05\x12\x12\n\nproduct_id\x18\x02 \x01(\x05\x12\x10\n\x08quantity\x18\x03 \x01(\x02\x12\x0e\n\x06uom_id\x18\x04 \x01(\x05\x12\x12\n\nprice_unit\x18\x05 \x01(\x02\x12\x0e\n\x06tax_id\x18\x06 \x01(\x05\x12\x10\n\x08\x64iscount\x18\x07 \x01(\x02\x12\x13\n\x0bprice_total\x18\x08 \x01(\x02\x12\x36\n\x07\x63ontext\x18\t \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17OrderLineCreateResponse\x12\x43\n\norder_line\x18\x01 \x01(\x0b\x32/.pro.omni.oms.api.v1.sales.order.line.OrderLine\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf2\x02\n\x14OrderLineReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe3\x01\n\x15OrderLineReadResponse\x12\x44\n\x0border_lines\x18\x01 \x03(\x0b\x32/.pro.omni.oms.api.v1.sales.order.line.OrderLine\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x95\x01\n\x16OrderLineUpdateRequest\x12\x43\n\norder_line\x18\x01 \x01(\x0b\x32/.pro.omni.oms.api.v1.sales.order.line.OrderLine\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa9\x01\n\x17OrderLineUpdateResponse\x12\x43\n\norder_line\x18\x01 \x01(\x0b\x32/.pro.omni.oms.api.v1.sales.order.line.OrderLine\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\\\n\x16OrderLineDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17OrderLineDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd8\x04\n\x10OrderLineService\x12\x90\x01\n\x0fOrderLineCreate\x12<.pro.omni.oms.api.v1.sales.order.line.OrderLineCreateRequest\x1a=.pro.omni.oms.api.v1.sales.order.line.OrderLineCreateResponse"\x00\x12\x8a\x01\n\rOrderLineRead\x12:.pro.omni.oms.api.v1.sales.order.line.OrderLineReadRequest\x1a;.pro.omni.oms.api.v1.sales.order.line.OrderLineReadResponse"\x00\x12\x90\x01\n\x0fOrderLineUpdate\x12<.pro.omni.oms.api.v1.sales.order.line.OrderLineUpdateRequest\x1a=.pro.omni.oms.api.v1.sales.order.line.OrderLineUpdateResponse"\x00\x12\x90\x01\n\x0fOrderLineDelete\x12<.pro.omni.oms.api.v1.sales.order.line.OrderLineDeleteRequest\x1a=.pro.omni.oms.api.v1.sales.order.line.OrderLineDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.order_line_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_ORDERLINE"]._serialized_start = 87
-    _globals["_ORDERLINE"]._serialized_end = 362
-    _globals["_ORDERLINECREATEREQUEST"]._serialized_start = 365
-    _globals["_ORDERLINECREATEREQUEST"]._serialized_end = 616
-    _globals["_ORDERLINECREATERESPONSE"]._serialized_start = 619
-    _globals["_ORDERLINECREATERESPONSE"]._serialized_end = 788
-    _globals["_ORDERLINEREADREQUEST"]._serialized_start = 791
-    _globals["_ORDERLINEREADREQUEST"]._serialized_end = 1161
-    _globals["_ORDERLINEREADRESPONSE"]._serialized_start = 1164
-    _globals["_ORDERLINEREADRESPONSE"]._serialized_end = 1391
-    _globals["_ORDERLINEUPDATEREQUEST"]._serialized_start = 1394
-    _globals["_ORDERLINEUPDATEREQUEST"]._serialized_end = 1543
-    _globals["_ORDERLINEUPDATERESPONSE"]._serialized_start = 1546
-    _globals["_ORDERLINEUPDATERESPONSE"]._serialized_end = 1715
-    _globals["_ORDERLINEDELETEREQUEST"]._serialized_start = 1717
-    _globals["_ORDERLINEDELETEREQUEST"]._serialized_end = 1809
-    _globals["_ORDERLINEDELETERESPONSE"]._serialized_start = 1811
-    _globals["_ORDERLINEDELETERESPONSE"]._serialized_end = 1911
-    _globals["_ORDERLINESERVICE"]._serialized_start = 1914
-    _globals["_ORDERLINESERVICE"]._serialized_end = 2514
+    _globals["_ORDERLINE"]._serialized_start = 119
+    _globals["_ORDERLINE"]._serialized_end = 398
+    _globals["_ORDERLINECREATEREQUEST"]._serialized_start = 401
+    _globals["_ORDERLINECREATEREQUEST"]._serialized_end = 628
+    _globals["_ORDERLINECREATERESPONSE"]._serialized_start = 631
+    _globals["_ORDERLINECREATERESPONSE"]._serialized_end = 800
+    _globals["_ORDERLINEREADREQUEST"]._serialized_start = 803
+    _globals["_ORDERLINEREADREQUEST"]._serialized_end = 1173
+    _globals["_ORDERLINEREADRESPONSE"]._serialized_start = 1176
+    _globals["_ORDERLINEREADRESPONSE"]._serialized_end = 1403
+    _globals["_ORDERLINEUPDATEREQUEST"]._serialized_start = 1406
+    _globals["_ORDERLINEUPDATEREQUEST"]._serialized_end = 1555
+    _globals["_ORDERLINEUPDATERESPONSE"]._serialized_start = 1558
+    _globals["_ORDERLINEUPDATERESPONSE"]._serialized_end = 1727
+    _globals["_ORDERLINEDELETEREQUEST"]._serialized_start = 1729
+    _globals["_ORDERLINEDELETEREQUEST"]._serialized_end = 1821
+    _globals["_ORDERLINEDELETERESPONSE"]._serialized_start = 1823
+    _globals["_ORDERLINEDELETERESPONSE"]._serialized_end = 1923
+    _globals["_ORDERLINESERVICE"]._serialized_start = 1926
+    _globals["_ORDERLINESERVICE"]._serialized_end = 2526
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/order_line_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/order_line_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class OrderLine(_message.Message):
     __slots__ = [
@@ -17,102 +18,94 @@
         "order_id",
         "product_id",
         "quantity",
         "uom_id",
         "price_unit",
         "tax_id",
         "discount",
-        "price_subtotal",
         "price_total",
         "active",
         "object_audit",
     ]
     ID_FIELD_NUMBER: _ClassVar[int]
     ORDER_ID_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_ID_FIELD_NUMBER: _ClassVar[int]
     QUANTITY_FIELD_NUMBER: _ClassVar[int]
     UOM_ID_FIELD_NUMBER: _ClassVar[int]
     PRICE_UNIT_FIELD_NUMBER: _ClassVar[int]
     TAX_ID_FIELD_NUMBER: _ClassVar[int]
     DISCOUNT_FIELD_NUMBER: _ClassVar[int]
-    PRICE_SUBTOTAL_FIELD_NUMBER: _ClassVar[int]
     PRICE_TOTAL_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     order_id: int
     product_id: int
     quantity: float
     uom_id: int
     price_unit: float
     tax_id: int
     discount: float
-    price_subtotal: float
     price_total: float
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         order_id: _Optional[int] = ...,
         product_id: _Optional[int] = ...,
         quantity: _Optional[float] = ...,
         uom_id: _Optional[int] = ...,
         price_unit: _Optional[float] = ...,
         tax_id: _Optional[int] = ...,
         discount: _Optional[float] = ...,
-        price_subtotal: _Optional[float] = ...,
         price_total: _Optional[float] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class OrderLineCreateRequest(_message.Message):
     __slots__ = [
         "order_id",
         "product_id",
         "quantity",
         "uom_id",
         "price_unit",
         "tax_id",
         "discount",
-        "price_subtotal",
         "price_total",
         "context",
     ]
     ORDER_ID_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_ID_FIELD_NUMBER: _ClassVar[int]
     QUANTITY_FIELD_NUMBER: _ClassVar[int]
     UOM_ID_FIELD_NUMBER: _ClassVar[int]
     PRICE_UNIT_FIELD_NUMBER: _ClassVar[int]
     TAX_ID_FIELD_NUMBER: _ClassVar[int]
     DISCOUNT_FIELD_NUMBER: _ClassVar[int]
-    PRICE_SUBTOTAL_FIELD_NUMBER: _ClassVar[int]
     PRICE_TOTAL_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     order_id: int
     product_id: int
     quantity: float
     uom_id: int
     price_unit: float
     tax_id: int
     discount: float
-    price_subtotal: float
     price_total: float
     context: _base_pb2.Context
     def __init__(
         self,
         order_id: _Optional[int] = ...,
         product_id: _Optional[int] = ...,
         quantity: _Optional[float] = ...,
         uom_id: _Optional[int] = ...,
         price_unit: _Optional[float] = ...,
         tax_id: _Optional[int] = ...,
         discount: _Optional[float] = ...,
-        price_subtotal: _Optional[float] = ...,
         price_total: _Optional[float] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class OrderLineCreateResponse(_message.Message):
     __slots__ = ["order_line", "response_standard"]
     ORDER_LINE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/order_line_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/order_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/order_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/order_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x14v1/sales/order.proto\x12\x1fpro.omni.oms.api.v1.sales.order\x1a\x11\x63ommon/base.proto"\x9b\x02\n\x05Order\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07sale_id\x18\x03 \x01(\x05\x12\x17\n\x0fship_address_id\x18\x04 \x01(\x05\x12\x1a\n\x12\x64\x65livery_method_id\x18\x05 \x01(\x05\x12\x12\n\ncarrier_id\x18\x06 \x01(\x05\x12\x19\n\x11payment_method_id\x18\x07 \x01(\x05\x12\x11\n\ttax_total\x18\x08 \x01(\x02\x12\x10\n\x08subtotal\x18\t \x01(\x02\x12\r\n\x05total\x18\n \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x0b \x01(\x08\x12?\n\x0cobject_audit\x18\x0c \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x83\x02\n\x12OrderCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07sale_id\x18\x02 \x01(\x05\x12\x17\n\x0fship_address_id\x18\x03 \x01(\x05\x12\x1a\n\x12\x64\x65livery_method_id\x18\x04 \x01(\x05\x12\x12\n\ncarrier_id\x18\x05 \x01(\x05\x12\x19\n\x11payment_method_id\x18\x06 \x01(\x05\x12\x11\n\ttax_total\x18\x07 \x01(\x02\x12\x10\n\x08subtotal\x18\x08 \x01(\x02\x12\r\n\x05total\x18\t \x01(\x02\x12\x36\n\x07\x63ontext\x18\n \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x97\x01\n\x13OrderCreateResponse\x12\x35\n\x05order\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.sales.order.Order\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xee\x02\n\x10OrderReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd0\x01\n\x11OrderReadResponse\x12\x35\n\x05order\x18\x01 \x03(\x0b\x32&.pro.omni.oms.api.v1.sales.order.Order\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x83\x01\n\x12OrderUpdateRequest\x12\x35\n\x05order\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.sales.order.Order\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x97\x01\n\x13OrderUpdateResponse\x12\x35\n\x05order\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.sales.order.Order\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"X\n\x12OrderDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"`\n\x13OrderDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xf8\x03\n\x0cOrderService\x12z\n\x0bOrderCreate\x12\x33.pro.omni.oms.api.v1.sales.order.OrderCreateRequest\x1a\x34.pro.omni.oms.api.v1.sales.order.OrderCreateResponse"\x00\x12t\n\tOrderRead\x12\x31.pro.omni.oms.api.v1.sales.order.OrderReadRequest\x1a\x32.pro.omni.oms.api.v1.sales.order.OrderReadResponse"\x00\x12z\n\x0bOrderUpdate\x12\x33.pro.omni.oms.api.v1.sales.order.OrderUpdateRequest\x1a\x34.pro.omni.oms.api.v1.sales.order.OrderUpdateResponse"\x00\x12z\n\x0bOrderDelete\x12\x33.pro.omni.oms.api.v1.sales.order.OrderDeleteRequest\x1a\x34.pro.omni.oms.api.v1.sales.order.OrderDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x14v1/sales/order.proto\x12\x1fpro.omni.oms.api.v1.sales.order\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xb7\x02\n\x05Order\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07sale_id\x18\x03 \x01(\x05\x12\x17\n\x0fship_address_id\x18\x04 \x01(\x05\x12\x1a\n\x12\x64\x65livery_method_id\x18\x05 \x01(\x05\x12\x12\n\ncarrier_id\x18\x06 \x01(\x05\x12\x19\n\x11payment_method_id\x18\x07 \x01(\x05\x12\x11\n\ttax_total\x18\x08 \x01(\x02\x12\x10\n\x08subtotal\x18\t \x01(\x02\x12\r\n\x05total\x18\n \x01(\x02\x12*\n\x06\x61\x63tive\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0c \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x83\x02\n\x12OrderCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07sale_id\x18\x02 \x01(\x05\x12\x17\n\x0fship_address_id\x18\x03 \x01(\x05\x12\x1a\n\x12\x64\x65livery_method_id\x18\x04 \x01(\x05\x12\x12\n\ncarrier_id\x18\x05 \x01(\x05\x12\x19\n\x11payment_method_id\x18\x06 \x01(\x05\x12\x11\n\ttax_total\x18\x07 \x01(\x02\x12\x10\n\x08subtotal\x18\x08 \x01(\x02\x12\r\n\x05total\x18\t \x01(\x02\x12\x36\n\x07\x63ontext\x18\n \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x97\x01\n\x13OrderCreateResponse\x12\x35\n\x05order\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.sales.order.Order\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xee\x02\n\x10OrderReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd0\x01\n\x11OrderReadResponse\x12\x35\n\x05order\x18\x01 \x03(\x0b\x32&.pro.omni.oms.api.v1.sales.order.Order\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x83\x01\n\x12OrderUpdateRequest\x12\x35\n\x05order\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.sales.order.Order\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x97\x01\n\x13OrderUpdateResponse\x12\x35\n\x05order\x18\x01 \x01(\x0b\x32&.pro.omni.oms.api.v1.sales.order.Order\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"X\n\x12OrderDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"`\n\x13OrderDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xf8\x03\n\x0cOrderService\x12z\n\x0bOrderCreate\x12\x33.pro.omni.oms.api.v1.sales.order.OrderCreateRequest\x1a\x34.pro.omni.oms.api.v1.sales.order.OrderCreateResponse"\x00\x12t\n\tOrderRead\x12\x31.pro.omni.oms.api.v1.sales.order.OrderReadRequest\x1a\x32.pro.omni.oms.api.v1.sales.order.OrderReadResponse"\x00\x12z\n\x0bOrderUpdate\x12\x33.pro.omni.oms.api.v1.sales.order.OrderUpdateRequest\x1a\x34.pro.omni.oms.api.v1.sales.order.OrderUpdateResponse"\x00\x12z\n\x0bOrderDelete\x12\x33.pro.omni.oms.api.v1.sales.order.OrderDeleteRequest\x1a\x34.pro.omni.oms.api.v1.sales.order.OrderDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.order_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_ORDER"]._serialized_start = 77
-    _globals["_ORDER"]._serialized_end = 360
-    _globals["_ORDERCREATEREQUEST"]._serialized_start = 363
-    _globals["_ORDERCREATEREQUEST"]._serialized_end = 622
-    _globals["_ORDERCREATERESPONSE"]._serialized_start = 625
-    _globals["_ORDERCREATERESPONSE"]._serialized_end = 776
-    _globals["_ORDERREADREQUEST"]._serialized_start = 779
-    _globals["_ORDERREADREQUEST"]._serialized_end = 1145
-    _globals["_ORDERREADRESPONSE"]._serialized_start = 1148
-    _globals["_ORDERREADRESPONSE"]._serialized_end = 1356
-    _globals["_ORDERUPDATEREQUEST"]._serialized_start = 1359
-    _globals["_ORDERUPDATEREQUEST"]._serialized_end = 1490
-    _globals["_ORDERUPDATERESPONSE"]._serialized_start = 1493
-    _globals["_ORDERUPDATERESPONSE"]._serialized_end = 1644
-    _globals["_ORDERDELETEREQUEST"]._serialized_start = 1646
-    _globals["_ORDERDELETEREQUEST"]._serialized_end = 1734
-    _globals["_ORDERDELETERESPONSE"]._serialized_start = 1736
-    _globals["_ORDERDELETERESPONSE"]._serialized_end = 1832
-    _globals["_ORDERSERVICE"]._serialized_start = 1835
-    _globals["_ORDERSERVICE"]._serialized_end = 2339
+    _globals["_ORDER"]._serialized_start = 109
+    _globals["_ORDER"]._serialized_end = 420
+    _globals["_ORDERCREATEREQUEST"]._serialized_start = 423
+    _globals["_ORDERCREATEREQUEST"]._serialized_end = 682
+    _globals["_ORDERCREATERESPONSE"]._serialized_start = 685
+    _globals["_ORDERCREATERESPONSE"]._serialized_end = 836
+    _globals["_ORDERREADREQUEST"]._serialized_start = 839
+    _globals["_ORDERREADREQUEST"]._serialized_end = 1205
+    _globals["_ORDERREADRESPONSE"]._serialized_start = 1208
+    _globals["_ORDERREADRESPONSE"]._serialized_end = 1416
+    _globals["_ORDERUPDATEREQUEST"]._serialized_start = 1419
+    _globals["_ORDERUPDATEREQUEST"]._serialized_end = 1550
+    _globals["_ORDERUPDATERESPONSE"]._serialized_start = 1553
+    _globals["_ORDERUPDATERESPONSE"]._serialized_end = 1704
+    _globals["_ORDERDELETEREQUEST"]._serialized_start = 1706
+    _globals["_ORDERDELETEREQUEST"]._serialized_end = 1794
+    _globals["_ORDERDELETERESPONSE"]._serialized_start = 1796
+    _globals["_ORDERDELETERESPONSE"]._serialized_end = 1892
+    _globals["_ORDERSERVICE"]._serialized_start = 1895
+    _globals["_ORDERSERVICE"]._serialized_end = 2399
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/order_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/tax_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,207 +2,164 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Order(_message.Message):
-    __slots__ = [
-        "id",
-        "name",
-        "sale_id",
-        "ship_address_id",
-        "delivery_method_id",
-        "carrier_id",
-        "payment_method_id",
-        "tax_total",
-        "subtotal",
-        "total",
-        "active",
-        "object_audit",
-    ]
+class Tax(_message.Message):
+    __slots__ = ["id", "name", "code", "rate", "rounding", "decimal_places", "position", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    SALE_ID_FIELD_NUMBER: _ClassVar[int]
-    SHIP_ADDRESS_ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
-    CARRIER_ID_FIELD_NUMBER: _ClassVar[int]
-    PAYMENT_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
-    TAX_TOTAL_FIELD_NUMBER: _ClassVar[int]
-    SUBTOTAL_FIELD_NUMBER: _ClassVar[int]
-    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    RATE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
+    DECIMAL_PLACES_FIELD_NUMBER: _ClassVar[int]
+    POSITION_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     name: str
-    sale_id: int
-    ship_address_id: int
-    delivery_method_id: int
-    carrier_id: int
-    payment_method_id: int
-    tax_total: float
-    subtotal: float
-    total: float
-    active: bool
+    code: str
+    rate: float
+    rounding: float
+    decimal_places: int
+    position: str
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        sale_id: _Optional[int] = ...,
-        ship_address_id: _Optional[int] = ...,
-        delivery_method_id: _Optional[int] = ...,
-        carrier_id: _Optional[int] = ...,
-        payment_method_id: _Optional[int] = ...,
-        tax_total: _Optional[float] = ...,
-        subtotal: _Optional[float] = ...,
-        total: _Optional[float] = ...,
-        active: bool = ...,
+        code: _Optional[str] = ...,
+        rate: _Optional[float] = ...,
+        rounding: _Optional[float] = ...,
+        decimal_places: _Optional[int] = ...,
+        position: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderCreateRequest(_message.Message):
-    __slots__ = [
-        "name",
-        "sale_id",
-        "ship_address_id",
-        "delivery_method_id",
-        "carrier_id",
-        "payment_method_id",
-        "tax_total",
-        "subtotal",
-        "total",
-        "context",
-    ]
+class TaxAddRequest(_message.Message):
+    __slots__ = ["name", "code", "rate", "rounding", "decimal_places", "position", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    SALE_ID_FIELD_NUMBER: _ClassVar[int]
-    SHIP_ADDRESS_ID_FIELD_NUMBER: _ClassVar[int]
-    DELIVERY_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
-    CARRIER_ID_FIELD_NUMBER: _ClassVar[int]
-    PAYMENT_METHOD_ID_FIELD_NUMBER: _ClassVar[int]
-    TAX_TOTAL_FIELD_NUMBER: _ClassVar[int]
-    SUBTOTAL_FIELD_NUMBER: _ClassVar[int]
-    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    RATE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
+    DECIMAL_PLACES_FIELD_NUMBER: _ClassVar[int]
+    POSITION_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
-    sale_id: int
-    ship_address_id: int
-    delivery_method_id: int
-    carrier_id: int
-    payment_method_id: int
-    tax_total: float
-    subtotal: float
-    total: float
+    code: str
+    rate: float
+    rounding: float
+    decimal_places: int
+    position: str
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
-        sale_id: _Optional[int] = ...,
-        ship_address_id: _Optional[int] = ...,
-        delivery_method_id: _Optional[int] = ...,
-        carrier_id: _Optional[int] = ...,
-        payment_method_id: _Optional[int] = ...,
-        tax_total: _Optional[float] = ...,
-        subtotal: _Optional[float] = ...,
-        total: _Optional[float] = ...,
+        code: _Optional[str] = ...,
+        rate: _Optional[float] = ...,
+        rounding: _Optional[float] = ...,
+        decimal_places: _Optional[int] = ...,
+        position: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderCreateResponse(_message.Message):
-    __slots__ = ["order", "response_standard"]
-    ORDER_FIELD_NUMBER: _ClassVar[int]
+class TaxAddResponse(_message.Message):
+    __slots__ = ["response_standard", "tax"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    order: Order
+    TAX_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    tax: Tax
     def __init__(
         self,
-        order: _Optional[_Union[Order, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        tax: _Optional[_Union[Tax, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderReadRequest(_message.Message):
+class TaxReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderReadResponse(_message.Message):
-    __slots__ = ["order", "response_standard", "meta_data"]
-    ORDER_FIELD_NUMBER: _ClassVar[int]
+class TaxReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "taxes"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    order: _containers.RepeatedCompositeFieldContainer[Order]
+    TAXES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
+    taxes: _containers.RepeatedCompositeFieldContainer[Tax]
     def __init__(
         self,
-        order: _Optional[_Iterable[_Union[Order, _Mapping]]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        taxes: _Optional[_Iterable[_Union[Tax, _Mapping]]] = ...,
     ) -> None: ...
 
-class OrderUpdateRequest(_message.Message):
-    __slots__ = ["order", "context"]
-    ORDER_FIELD_NUMBER: _ClassVar[int]
+class TaxUpdateRequest(_message.Message):
+    __slots__ = ["tax", "context"]
+    TAX_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    order: Order
+    tax: Tax
     context: _base_pb2.Context
     def __init__(
-        self,
-        order: _Optional[_Union[Order, _Mapping]] = ...,
-        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+        self, tax: _Optional[_Union[Tax, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class OrderUpdateResponse(_message.Message):
-    __slots__ = ["order", "response_standard"]
-    ORDER_FIELD_NUMBER: _ClassVar[int]
+class TaxUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "tax"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    order: Order
+    TAX_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    tax: Tax
     def __init__(
         self,
-        order: _Optional[_Union[Order, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        tax: _Optional[_Union[Tax, _Mapping]] = ...,
     ) -> None: ...
 
-class OrderDeleteRequest(_message.Message):
+class TaxDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class OrderDeleteResponse(_message.Message):
+class TaxDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/order_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/order_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/payment_method_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/payment_method_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1dv1/sales/payment_method.proto\x12(pro.omni.oms.api.v1.sales.payment.method\x1a\x11\x63ommon/base.proto"\xa7\x01\n\rPaymentMethod\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x1d\n\x15payment_method_doc_id\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x8f\x01\n\x1aPaymentMethodCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x1d\n\x15payment_method_doc_id\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb9\x01\n\x1bPaymentMethodCreateResponse\x12O\n\x0epayment_method\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.sales.payment.method.PaymentMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf6\x02\n\x18PaymentMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf3\x01\n\x19PaymentMethodReadResponse\x12P\n\x0fpayment_methods\x18\x01 \x03(\x0b\x32\x37.pro.omni.oms.api.v1.sales.payment.method.PaymentMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\xa5\x01\n\x1aPaymentMethodUpdateRequest\x12O\n\x0epayment_method\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.sales.payment.method.PaymentMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb9\x01\n\x1bPaymentMethodUpdateResponse\x12O\n\x0epayment_method\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.sales.payment.method.PaymentMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"`\n\x1aPaymentMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1bPaymentMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xac\x05\n\x14PaymentMethodService\x12\xa4\x01\n\x13PaymentMethodCreate\x12\x44.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodCreateRequest\x1a\x45.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodCreateResponse"\x00\x12\x9e\x01\n\x11PaymentMethodRead\x12\x42.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodReadRequest\x1a\x43.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodReadResponse"\x00\x12\xa4\x01\n\x13PaymentMethodUpdate\x12\x44.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodUpdateRequest\x1a\x45.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodUpdateResponse"\x00\x12\xa4\x01\n\x13PaymentMethodDelete\x12\x44.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodDeleteRequest\x1a\x45.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1dv1/sales/payment_method.proto\x12(pro.omni.oms.api.v1.sales.payment.method\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xc3\x01\n\rPaymentMethod\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x1d\n\x15payment_method_doc_id\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x8f\x01\n\x1aPaymentMethodCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x1d\n\x15payment_method_doc_id\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb9\x01\n\x1bPaymentMethodCreateResponse\x12O\n\x0epayment_method\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.sales.payment.method.PaymentMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf6\x02\n\x18PaymentMethodReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xf3\x01\n\x19PaymentMethodReadResponse\x12P\n\x0fpayment_methods\x18\x01 \x03(\x0b\x32\x37.pro.omni.oms.api.v1.sales.payment.method.PaymentMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\xa5\x01\n\x1aPaymentMethodUpdateRequest\x12O\n\x0epayment_method\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.sales.payment.method.PaymentMethod\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb9\x01\n\x1bPaymentMethodUpdateResponse\x12O\n\x0epayment_method\x18\x01 \x01(\x0b\x32\x37.pro.omni.oms.api.v1.sales.payment.method.PaymentMethod\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"`\n\x1aPaymentMethodDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"h\n\x1bPaymentMethodDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xac\x05\n\x14PaymentMethodService\x12\xa4\x01\n\x13PaymentMethodCreate\x12\x44.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodCreateRequest\x1a\x45.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodCreateResponse"\x00\x12\x9e\x01\n\x11PaymentMethodRead\x12\x42.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodReadRequest\x1a\x43.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodReadResponse"\x00\x12\xa4\x01\n\x13PaymentMethodUpdate\x12\x44.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodUpdateRequest\x1a\x45.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodUpdateResponse"\x00\x12\xa4\x01\n\x13PaymentMethodDelete\x12\x44.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodDeleteRequest\x1a\x45.pro.omni.oms.api.v1.sales.payment.method.PaymentMethodDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.payment_method_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_PAYMENTMETHOD"]._serialized_start = 95
-    _globals["_PAYMENTMETHOD"]._serialized_end = 262
-    _globals["_PAYMENTMETHODCREATEREQUEST"]._serialized_start = 265
-    _globals["_PAYMENTMETHODCREATEREQUEST"]._serialized_end = 408
-    _globals["_PAYMENTMETHODCREATERESPONSE"]._serialized_start = 411
-    _globals["_PAYMENTMETHODCREATERESPONSE"]._serialized_end = 596
-    _globals["_PAYMENTMETHODREADREQUEST"]._serialized_start = 599
-    _globals["_PAYMENTMETHODREADREQUEST"]._serialized_end = 973
-    _globals["_PAYMENTMETHODREADRESPONSE"]._serialized_start = 976
-    _globals["_PAYMENTMETHODREADRESPONSE"]._serialized_end = 1219
-    _globals["_PAYMENTMETHODUPDATEREQUEST"]._serialized_start = 1222
-    _globals["_PAYMENTMETHODUPDATEREQUEST"]._serialized_end = 1387
-    _globals["_PAYMENTMETHODUPDATERESPONSE"]._serialized_start = 1390
-    _globals["_PAYMENTMETHODUPDATERESPONSE"]._serialized_end = 1575
-    _globals["_PAYMENTMETHODDELETEREQUEST"]._serialized_start = 1577
-    _globals["_PAYMENTMETHODDELETEREQUEST"]._serialized_end = 1673
-    _globals["_PAYMENTMETHODDELETERESPONSE"]._serialized_start = 1675
-    _globals["_PAYMENTMETHODDELETERESPONSE"]._serialized_end = 1779
-    _globals["_PAYMENTMETHODSERVICE"]._serialized_start = 1782
-    _globals["_PAYMENTMETHODSERVICE"]._serialized_end = 2466
+    _globals["_PAYMENTMETHOD"]._serialized_start = 127
+    _globals["_PAYMENTMETHOD"]._serialized_end = 322
+    _globals["_PAYMENTMETHODCREATEREQUEST"]._serialized_start = 325
+    _globals["_PAYMENTMETHODCREATEREQUEST"]._serialized_end = 468
+    _globals["_PAYMENTMETHODCREATERESPONSE"]._serialized_start = 471
+    _globals["_PAYMENTMETHODCREATERESPONSE"]._serialized_end = 656
+    _globals["_PAYMENTMETHODREADREQUEST"]._serialized_start = 659
+    _globals["_PAYMENTMETHODREADREQUEST"]._serialized_end = 1033
+    _globals["_PAYMENTMETHODREADRESPONSE"]._serialized_start = 1036
+    _globals["_PAYMENTMETHODREADRESPONSE"]._serialized_end = 1279
+    _globals["_PAYMENTMETHODUPDATEREQUEST"]._serialized_start = 1282
+    _globals["_PAYMENTMETHODUPDATEREQUEST"]._serialized_end = 1447
+    _globals["_PAYMENTMETHODUPDATERESPONSE"]._serialized_start = 1450
+    _globals["_PAYMENTMETHODUPDATERESPONSE"]._serialized_end = 1635
+    _globals["_PAYMENTMETHODDELETEREQUEST"]._serialized_start = 1637
+    _globals["_PAYMENTMETHODDELETEREQUEST"]._serialized_end = 1733
+    _globals["_PAYMENTMETHODDELETERESPONSE"]._serialized_start = 1735
+    _globals["_PAYMENTMETHODDELETERESPONSE"]._serialized_end = 1839
+    _globals["_PAYMENTMETHODSERVICE"]._serialized_start = 1842
+    _globals["_PAYMENTMETHODSERVICE"]._serialized_end = 2526
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/payment_method_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/tax_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,74 +2,75 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class PaymentMethod(_message.Message):
-    __slots__ = ["id", "name", "code", "payment_method_doc_id", "active", "object_audit"]
+class Tax(_message.Message):
+    __slots__ = ["id", "tax_doc_id", "code", "name", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+    TAX_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    PAYMENT_METHOD_DOC_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
-    name: str
+    tax_doc_id: str
     code: str
-    payment_method_doc_id: str
-    active: bool
+    name: str
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
-        name: _Optional[str] = ...,
+        tax_doc_id: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        payment_method_doc_id: _Optional[str] = ...,
-        active: bool = ...,
+        name: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodCreateRequest(_message.Message):
-    __slots__ = ["name", "code", "payment_method_doc_id", "context"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+class TaxCreateRequest(_message.Message):
+    __slots__ = ["tax_doc_id", "code", "name", "context"]
+    TAX_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    PAYMENT_METHOD_DOC_ID_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    name: str
+    tax_doc_id: str
     code: str
-    payment_method_doc_id: str
+    name: str
     context: _base_pb2.Context
     def __init__(
         self,
-        name: _Optional[str] = ...,
+        tax_doc_id: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        payment_method_doc_id: _Optional[str] = ...,
+        name: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodCreateResponse(_message.Message):
-    __slots__ = ["payment_method", "response_standard"]
-    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
+class TaxCreateResponse(_message.Message):
+    __slots__ = ["tax", "response_standard"]
+    TAX_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    payment_method: PaymentMethod
+    tax: Tax
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
+        tax: _Optional[_Union[Tax, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodReadRequest(_message.Message):
+class TaxReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -88,61 +89,59 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodReadResponse(_message.Message):
-    __slots__ = ["payment_methods", "response_standard", "meta_data"]
-    PAYMENT_METHODS_FIELD_NUMBER: _ClassVar[int]
+class TaxReadResponse(_message.Message):
+    __slots__ = ["tax", "response_standard", "meta_data"]
+    TAX_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    payment_methods: _containers.RepeatedCompositeFieldContainer[PaymentMethod]
+    tax: _containers.RepeatedCompositeFieldContainer[Tax]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
     def __init__(
         self,
-        payment_methods: _Optional[_Iterable[_Union[PaymentMethod, _Mapping]]] = ...,
+        tax: _Optional[_Iterable[_Union[Tax, _Mapping]]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodUpdateRequest(_message.Message):
-    __slots__ = ["payment_method", "context"]
-    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
+class TaxUpdateRequest(_message.Message):
+    __slots__ = ["tax", "context"]
+    TAX_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    payment_method: PaymentMethod
+    tax: Tax
     context: _base_pb2.Context
     def __init__(
-        self,
-        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
-        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+        self, tax: _Optional[_Union[Tax, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class PaymentMethodUpdateResponse(_message.Message):
-    __slots__ = ["payment_method", "response_standard"]
-    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
+class TaxUpdateResponse(_message.Message):
+    __slots__ = ["tax", "response_standard"]
+    TAX_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    payment_method: PaymentMethod
+    tax: Tax
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
+        tax: _Optional[_Union[Tax, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class PaymentMethodDeleteRequest(_message.Message):
+class TaxDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class PaymentMethodDeleteResponse(_message.Message):
+class TaxDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_order_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_order_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1cv1/sales/picking_order.proto\x12\'pro.omni.oms.api.v1.sales.picking.order\x1a\x11\x63ommon/base.proto"\x91\x01\n\x0cPickingOrder\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x10\n\x08order_id\x18\x02 \x01(\x05\x12\x12\n\npicking_id\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"y\n\x19PickingOrderCreateRequest\x12\x10\n\x08order_id\x18\x01 \x01(\x05\x12\x12\n\npicking_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1aPickingOrderCreateResponse\x12L\n\rpicking_order\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.sales.picking.order.PickingOrder\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf5\x02\n\x17PickingOrderReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xef\x01\n\x18PickingOrderReadResponse\x12M\n\x0epicking_orders\x18\x01 \x03(\x0b\x32\x35.pro.omni.oms.api.v1.sales.picking.order.PickingOrder\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\xa1\x01\n\x19PickingOrderUpdateRequest\x12L\n\rpicking_order\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.sales.picking.order.PickingOrder\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1aPickingOrderUpdateResponse\x12L\n\rpicking_order\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.sales.picking.order.PickingOrder\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"_\n\x19PickingOrderDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1aPickingOrderDeleteResponse\x12L\n\rpicking_order\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.sales.picking.order.PickingOrder\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x97\x05\n\x13PickingOrderService\x12\x9f\x01\n\x12PickingOrderCreate\x12\x42.pro.omni.oms.api.v1.sales.picking.order.PickingOrderCreateRequest\x1a\x43.pro.omni.oms.api.v1.sales.picking.order.PickingOrderCreateResponse"\x00\x12\x99\x01\n\x10PickingOrderRead\x12@.pro.omni.oms.api.v1.sales.picking.order.PickingOrderReadRequest\x1a\x41.pro.omni.oms.api.v1.sales.picking.order.PickingOrderReadResponse"\x00\x12\x9f\x01\n\x12PickingOrderUpdate\x12\x42.pro.omni.oms.api.v1.sales.picking.order.PickingOrderUpdateRequest\x1a\x43.pro.omni.oms.api.v1.sales.picking.order.PickingOrderUpdateResponse"\x00\x12\x9f\x01\n\x12PickingOrderDelete\x12\x42.pro.omni.oms.api.v1.sales.picking.order.PickingOrderDeleteRequest\x1a\x43.pro.omni.oms.api.v1.sales.picking.order.PickingOrderDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x1cv1/sales/picking_order.proto\x12\'pro.omni.oms.api.v1.sales.picking.order\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xad\x01\n\x0cPickingOrder\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x10\n\x08order_id\x18\x02 \x01(\x05\x12\x12\n\npicking_id\x18\x03 \x01(\x05\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"y\n\x19PickingOrderCreateRequest\x12\x10\n\x08order_id\x18\x01 \x01(\x05\x12\x12\n\npicking_id\x18\x02 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1aPickingOrderCreateResponse\x12L\n\rpicking_order\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.sales.picking.order.PickingOrder\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf5\x02\n\x17PickingOrderReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xef\x01\n\x18PickingOrderReadResponse\x12M\n\x0epicking_orders\x18\x01 \x03(\x0b\x32\x35.pro.omni.oms.api.v1.sales.picking.order.PickingOrder\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\xa1\x01\n\x19PickingOrderUpdateRequest\x12L\n\rpicking_order\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.sales.picking.order.PickingOrder\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1aPickingOrderUpdateResponse\x12L\n\rpicking_order\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.sales.picking.order.PickingOrder\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"_\n\x19PickingOrderDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xb5\x01\n\x1aPickingOrderDeleteResponse\x12L\n\rpicking_order\x18\x01 \x01(\x0b\x32\x35.pro.omni.oms.api.v1.sales.picking.order.PickingOrder\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\x97\x05\n\x13PickingOrderService\x12\x9f\x01\n\x12PickingOrderCreate\x12\x42.pro.omni.oms.api.v1.sales.picking.order.PickingOrderCreateRequest\x1a\x43.pro.omni.oms.api.v1.sales.picking.order.PickingOrderCreateResponse"\x00\x12\x99\x01\n\x10PickingOrderRead\x12@.pro.omni.oms.api.v1.sales.picking.order.PickingOrderReadRequest\x1a\x41.pro.omni.oms.api.v1.sales.picking.order.PickingOrderReadResponse"\x00\x12\x9f\x01\n\x12PickingOrderUpdate\x12\x42.pro.omni.oms.api.v1.sales.picking.order.PickingOrderUpdateRequest\x1a\x43.pro.omni.oms.api.v1.sales.picking.order.PickingOrderUpdateResponse"\x00\x12\x9f\x01\n\x12PickingOrderDelete\x12\x42.pro.omni.oms.api.v1.sales.picking.order.PickingOrderDeleteRequest\x1a\x43.pro.omni.oms.api.v1.sales.picking.order.PickingOrderDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.picking_order_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_PICKINGORDER"]._serialized_start = 93
-    _globals["_PICKINGORDER"]._serialized_end = 238
-    _globals["_PICKINGORDERCREATEREQUEST"]._serialized_start = 240
-    _globals["_PICKINGORDERCREATEREQUEST"]._serialized_end = 361
-    _globals["_PICKINGORDERCREATERESPONSE"]._serialized_start = 364
-    _globals["_PICKINGORDERCREATERESPONSE"]._serialized_end = 545
-    _globals["_PICKINGORDERREADREQUEST"]._serialized_start = 548
-    _globals["_PICKINGORDERREADREQUEST"]._serialized_end = 921
-    _globals["_PICKINGORDERREADRESPONSE"]._serialized_start = 924
-    _globals["_PICKINGORDERREADRESPONSE"]._serialized_end = 1163
-    _globals["_PICKINGORDERUPDATEREQUEST"]._serialized_start = 1166
-    _globals["_PICKINGORDERUPDATEREQUEST"]._serialized_end = 1327
-    _globals["_PICKINGORDERUPDATERESPONSE"]._serialized_start = 1330
-    _globals["_PICKINGORDERUPDATERESPONSE"]._serialized_end = 1511
-    _globals["_PICKINGORDERDELETEREQUEST"]._serialized_start = 1513
-    _globals["_PICKINGORDERDELETEREQUEST"]._serialized_end = 1608
-    _globals["_PICKINGORDERDELETERESPONSE"]._serialized_start = 1611
-    _globals["_PICKINGORDERDELETERESPONSE"]._serialized_end = 1792
-    _globals["_PICKINGORDERSERVICE"]._serialized_start = 1795
-    _globals["_PICKINGORDERSERVICE"]._serialized_end = 2458
+    _globals["_PICKINGORDER"]._serialized_start = 125
+    _globals["_PICKINGORDER"]._serialized_end = 298
+    _globals["_PICKINGORDERCREATEREQUEST"]._serialized_start = 300
+    _globals["_PICKINGORDERCREATEREQUEST"]._serialized_end = 421
+    _globals["_PICKINGORDERCREATERESPONSE"]._serialized_start = 424
+    _globals["_PICKINGORDERCREATERESPONSE"]._serialized_end = 605
+    _globals["_PICKINGORDERREADREQUEST"]._serialized_start = 608
+    _globals["_PICKINGORDERREADREQUEST"]._serialized_end = 981
+    _globals["_PICKINGORDERREADRESPONSE"]._serialized_start = 984
+    _globals["_PICKINGORDERREADRESPONSE"]._serialized_end = 1223
+    _globals["_PICKINGORDERUPDATEREQUEST"]._serialized_start = 1226
+    _globals["_PICKINGORDERUPDATEREQUEST"]._serialized_end = 1387
+    _globals["_PICKINGORDERUPDATERESPONSE"]._serialized_start = 1390
+    _globals["_PICKINGORDERUPDATERESPONSE"]._serialized_end = 1571
+    _globals["_PICKINGORDERDELETEREQUEST"]._serialized_start = 1573
+    _globals["_PICKINGORDERDELETEREQUEST"]._serialized_end = 1668
+    _globals["_PICKINGORDERDELETERESPONSE"]._serialized_start = 1671
+    _globals["_PICKINGORDERDELETERESPONSE"]._serialized_end = 1852
+    _globals["_PICKINGORDERSERVICE"]._serialized_start = 1855
+    _globals["_PICKINGORDERSERVICE"]._serialized_end = 2518
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_order_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_order_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class PickingOrder(_message.Message):
     __slots__ = ["id", "order_id", "picking_id", "active", "object_audit"]
@@ -17,22 +18,22 @@
     ORDER_ID_FIELD_NUMBER: _ClassVar[int]
     PICKING_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     order_id: int
     picking_id: int
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         order_id: _Optional[int] = ...,
         picking_id: _Optional[int] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class PickingOrderCreateRequest(_message.Message):
     __slots__ = ["order_id", "picking_id", "context"]
     ORDER_ID_FIELD_NUMBER: _ClassVar[int]
     PICKING_ID_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,39 +9,40 @@
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/sales/picking.proto\x12!pro.omni.oms.api.v1.sales.picking\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x11\x63ommon/base.proto"\xd3\x04\n\x07Picking\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x03 \x01(\x05\x12\x13\n\x0blocation_id\x18\x04 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x05 \x01(\x05\x12\x0f\n\x07user_id\x18\x06 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x07 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x08 \x01(\x05\x12\x0e\n\x06origin\x18\t \x01(\t\x12-\n\tdate_done\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\x0c \x01(\x02\x12\x15\n\rtime_assigned\x18\r \x01(\x02\x12\x12\n\ncarrier_id\x18\x0e \x01(\x05\x12\x31\n\rdate_delivery\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x10 \x01(\t\x12\x10\n\x08group_id\x18\x11 \x01(\x05\x12\x0e\n\x06weight\x18\x12 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x13 \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x14 \x01(\x08\x12?\n\x0cobject_audit\x18\x15 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xbb\x04\n\x14PickingCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x02 \x01(\x05\x12\x13\n\x0blocation_id\x18\x03 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x04 \x01(\x05\x12\x0f\n\x07user_id\x18\x05 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x06 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x07 \x01(\x05\x12\x0e\n\x06origin\x18\x08 \x01(\t\x12-\n\tdate_done\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\x0b \x01(\x02\x12\x15\n\rtime_assigned\x18\x0c \x01(\x02\x12\x12\n\ncarrier_id\x18\r \x01(\x05\x12\x31\n\rdate_delivery\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x0f \x01(\t\x12\x10\n\x08group_id\x18\x10 \x01(\x05\x12\x0e\n\x06weight\x18\x11 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x12 \x01(\x02\x12\x36\n\x07\x63ontext\x18\x13 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"\xf0\x02\n\x12PickingReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13PickingReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12<\n\x08pickings\x18\x03 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"\x8b\x01\n\x14PickingUpdateRequest\x12;\n\x07picking\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"Z\n\x14PickingDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15PickingDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0ePickingService\x12\x84\x01\n\rPickingCreate\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingCreateResponse"\x00\x12~\n\x0bPickingRead\x12\x35.pro.omni.oms.api.v1.sales.picking.PickingReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.picking.PickingReadResponse"\x00\x12\x84\x01\n\rPickingUpdate\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingUpdateResponse"\x00\x12\x84\x01\n\rPickingDelete\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/sales/picking.proto\x12!pro.omni.oms.api.v1.sales.picking\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x11\x63ommon/base.proto"\xef\x04\n\x07Picking\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x03 \x01(\x05\x12\x13\n\x0blocation_id\x18\x04 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x05 \x01(\x05\x12\x0f\n\x07user_id\x18\x06 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x07 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x08 \x01(\x05\x12\x0e\n\x06origin\x18\t \x01(\t\x12-\n\tdate_done\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\x0c \x01(\x02\x12\x15\n\rtime_assigned\x18\r \x01(\x02\x12\x12\n\ncarrier_id\x18\x0e \x01(\x05\x12\x31\n\rdate_delivery\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x10 \x01(\t\x12\x10\n\x08group_id\x18\x11 \x01(\x05\x12\x0e\n\x06weight\x18\x12 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x13 \x01(\x02\x12*\n\x06\x61\x63tive\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x15 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xbb\x04\n\x14PickingCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x17\n\x0fpicking_type_id\x18\x02 \x01(\x05\x12\x13\n\x0blocation_id\x18\x03 \x01(\x05\x12\x18\n\x10location_dest_id\x18\x04 \x01(\x05\x12\x0f\n\x07user_id\x18\x05 \x01(\x05\x12\x1b\n\x13\x61ttachment_guide_id\x18\x06 \x01(\x05\x12\x1d\n\x15\x61ttachment_invoice_id\x18\x07 \x01(\x05\x12\x0e\n\x06origin\x18\x08 \x01(\t\x12-\n\tdate_done\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0escheduled_date\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16time_total_preparation\x18\x0b \x01(\x02\x12\x15\n\rtime_assigned\x18\x0c \x01(\x02\x12\x12\n\ncarrier_id\x18\r \x01(\x05\x12\x31\n\rdate_delivery\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14\x63\x61rrier_tracking_ref\x18\x0f \x01(\t\x12\x10\n\x08group_id\x18\x10 \x01(\x05\x12\x0e\n\x06weight\x18\x11 \x01(\x02\x12\x17\n\x0fshipping_weight\x18\x12 \x01(\x02\x12\x36\n\x07\x63ontext\x18\x13 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingCreateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"\xf0\x02\n\x12PickingReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13PickingReadResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12<\n\x08pickings\x18\x03 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"\x8b\x01\n\x14PickingUpdateRequest\x12;\n\x07picking\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15PickingUpdateResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12;\n\x07picking\x18\x02 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.picking.Picking"Z\n\x14PickingDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15PickingDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0ePickingService\x12\x84\x01\n\rPickingCreate\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingCreateResponse"\x00\x12~\n\x0bPickingRead\x12\x35.pro.omni.oms.api.v1.sales.picking.PickingReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.picking.PickingReadResponse"\x00\x12\x84\x01\n\rPickingUpdate\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingUpdateResponse"\x00\x12\x84\x01\n\rPickingDelete\x12\x37.pro.omni.oms.api.v1.sales.picking.PickingDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.picking.PickingDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.picking_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_PICKING"]._serialized_start = 114
-    _globals["_PICKING"]._serialized_end = 709
-    _globals["_PICKINGCREATEREQUEST"]._serialized_start = 712
-    _globals["_PICKINGCREATEREQUEST"]._serialized_end = 1283
-    _globals["_PICKINGCREATERESPONSE"]._serialized_start = 1286
-    _globals["_PICKINGCREATERESPONSE"]._serialized_end = 1445
-    _globals["_PICKINGREADREQUEST"]._serialized_start = 1448
-    _globals["_PICKINGREADREQUEST"]._serialized_end = 1816
-    _globals["_PICKINGREADRESPONSE"]._serialized_start = 1819
-    _globals["_PICKINGREADRESPONSE"]._serialized_end = 2036
-    _globals["_PICKINGUPDATEREQUEST"]._serialized_start = 2039
-    _globals["_PICKINGUPDATEREQUEST"]._serialized_end = 2178
-    _globals["_PICKINGUPDATERESPONSE"]._serialized_start = 2181
-    _globals["_PICKINGUPDATERESPONSE"]._serialized_end = 2340
-    _globals["_PICKINGDELETEREQUEST"]._serialized_start = 2342
-    _globals["_PICKINGDELETEREQUEST"]._serialized_end = 2432
-    _globals["_PICKINGDELETERESPONSE"]._serialized_start = 2434
-    _globals["_PICKINGDELETERESPONSE"]._serialized_end = 2532
-    _globals["_PICKINGSERVICE"]._serialized_start = 2535
-    _globals["_PICKINGSERVICE"]._serialized_end = 3084
+    _globals["_PICKING"]._serialized_start = 146
+    _globals["_PICKING"]._serialized_end = 769
+    _globals["_PICKINGCREATEREQUEST"]._serialized_start = 772
+    _globals["_PICKINGCREATEREQUEST"]._serialized_end = 1343
+    _globals["_PICKINGCREATERESPONSE"]._serialized_start = 1346
+    _globals["_PICKINGCREATERESPONSE"]._serialized_end = 1505
+    _globals["_PICKINGREADREQUEST"]._serialized_start = 1508
+    _globals["_PICKINGREADREQUEST"]._serialized_end = 1876
+    _globals["_PICKINGREADRESPONSE"]._serialized_start = 1879
+    _globals["_PICKINGREADRESPONSE"]._serialized_end = 2096
+    _globals["_PICKINGUPDATEREQUEST"]._serialized_start = 2099
+    _globals["_PICKINGUPDATEREQUEST"]._serialized_end = 2238
+    _globals["_PICKINGUPDATERESPONSE"]._serialized_start = 2241
+    _globals["_PICKINGUPDATERESPONSE"]._serialized_end = 2400
+    _globals["_PICKINGDELETEREQUEST"]._serialized_start = 2402
+    _globals["_PICKINGDELETEREQUEST"]._serialized_end = 2492
+    _globals["_PICKINGDELETERESPONSE"]._serialized_start = 2494
+    _globals["_PICKINGDELETERESPONSE"]._serialized_end = 2592
+    _globals["_PICKINGSERVICE"]._serialized_start = 2595
+    _globals["_PICKINGSERVICE"]._serialized_end = 3144
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Picking(_message.Message):
     __slots__ = [
@@ -72,15 +73,15 @@
     time_assigned: float
     carrier_id: int
     date_delivery: _timestamp_pb2.Timestamp
     carrier_tracking_ref: str
     group_id: int
     weight: float
     shipping_weight: float
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         name: _Optional[str] = ...,
         picking_type_id: _Optional[int] = ...,
         location_id: _Optional[int] = ...,
@@ -95,15 +96,15 @@
         time_assigned: _Optional[float] = ...,
         carrier_id: _Optional[int] = ...,
         date_delivery: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
         carrier_tracking_ref: _Optional[str] = ...,
         group_id: _Optional[int] = ...,
         weight: _Optional[float] = ...,
         shipping_weight: _Optional[float] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class PickingCreateRequest(_message.Message):
     __slots__ = [
         "name",
         "picking_type_id",
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/picking_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/picking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/product_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/product_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16v1/sales/product.proto\x12!pro.omni.oms.api.v1.sales.product\x1a\x11\x63ommon/base.proto"\xa5\x01\n\x07Product\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x16\n\x0eproduct_doc_id\x18\x02 \x01(\t\x12\x17\n\x0ftemplate_doc_id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x8d\x01\n\x14ProductCreateRequest\x12\x16\n\x0eproduct_doc_id\x18\x01 \x01(\t\x12\x17\n\x0ftemplate_doc_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15ProductCreateResponse\x12;\n\x07product\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.product.Product\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12ProductReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13ProductReadResponse\x12<\n\x08products\x18\x01 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.product.Product\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x8b\x01\n\x14ProductUpdateRequest\x12;\n\x07product\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.product.Product\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15ProductUpdateResponse\x12;\n\x07product\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.product.Product\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14ProductDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15ProductDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0eProductService\x12\x84\x01\n\rProductCreate\x12\x37.pro.omni.oms.api.v1.sales.product.ProductCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.product.ProductCreateResponse"\x00\x12~\n\x0bProductRead\x12\x35.pro.omni.oms.api.v1.sales.product.ProductReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.product.ProductReadResponse"\x00\x12\x84\x01\n\rProductUpdate\x12\x37.pro.omni.oms.api.v1.sales.product.ProductUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.product.ProductUpdateResponse"\x00\x12\x84\x01\n\rProductDelete\x12\x37.pro.omni.oms.api.v1.sales.product.ProductDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.product.ProductDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x16v1/sales/product.proto\x12!pro.omni.oms.api.v1.sales.product\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xc1\x01\n\x07Product\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x16\n\x0eproduct_doc_id\x18\x02 \x01(\t\x12\x17\n\x0ftemplate_doc_id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x8d\x01\n\x14ProductCreateRequest\x12\x16\n\x0eproduct_doc_id\x18\x01 \x01(\t\x12\x17\n\x0ftemplate_doc_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15ProductCreateResponse\x12;\n\x07product\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.product.Product\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf0\x02\n\x12ProductReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xd9\x01\n\x13ProductReadResponse\x12<\n\x08products\x18\x01 \x03(\x0b\x32*.pro.omni.oms.api.v1.sales.product.Product\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x8b\x01\n\x14ProductUpdateRequest\x12;\n\x07product\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.product.Product\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x9f\x01\n\x15ProductUpdateResponse\x12;\n\x07product\x18\x01 \x01(\x0b\x32*.pro.omni.oms.api.v1.sales.product.Product\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"Z\n\x14ProductDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"b\n\x15ProductDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xa5\x04\n\x0eProductService\x12\x84\x01\n\rProductCreate\x12\x37.pro.omni.oms.api.v1.sales.product.ProductCreateRequest\x1a\x38.pro.omni.oms.api.v1.sales.product.ProductCreateResponse"\x00\x12~\n\x0bProductRead\x12\x35.pro.omni.oms.api.v1.sales.product.ProductReadRequest\x1a\x36.pro.omni.oms.api.v1.sales.product.ProductReadResponse"\x00\x12\x84\x01\n\rProductUpdate\x12\x37.pro.omni.oms.api.v1.sales.product.ProductUpdateRequest\x1a\x38.pro.omni.oms.api.v1.sales.product.ProductUpdateResponse"\x00\x12\x84\x01\n\rProductDelete\x12\x37.pro.omni.oms.api.v1.sales.product.ProductDeleteRequest\x1a\x38.pro.omni.oms.api.v1.sales.product.ProductDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.product_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_PRODUCT"]._serialized_start = 81
-    _globals["_PRODUCT"]._serialized_end = 246
-    _globals["_PRODUCTCREATEREQUEST"]._serialized_start = 249
-    _globals["_PRODUCTCREATEREQUEST"]._serialized_end = 390
-    _globals["_PRODUCTCREATERESPONSE"]._serialized_start = 393
-    _globals["_PRODUCTCREATERESPONSE"]._serialized_end = 552
-    _globals["_PRODUCTREADREQUEST"]._serialized_start = 555
-    _globals["_PRODUCTREADREQUEST"]._serialized_end = 923
-    _globals["_PRODUCTREADRESPONSE"]._serialized_start = 926
-    _globals["_PRODUCTREADRESPONSE"]._serialized_end = 1143
-    _globals["_PRODUCTUPDATEREQUEST"]._serialized_start = 1146
-    _globals["_PRODUCTUPDATEREQUEST"]._serialized_end = 1285
-    _globals["_PRODUCTUPDATERESPONSE"]._serialized_start = 1288
-    _globals["_PRODUCTUPDATERESPONSE"]._serialized_end = 1447
-    _globals["_PRODUCTDELETEREQUEST"]._serialized_start = 1449
-    _globals["_PRODUCTDELETEREQUEST"]._serialized_end = 1539
-    _globals["_PRODUCTDELETERESPONSE"]._serialized_start = 1541
-    _globals["_PRODUCTDELETERESPONSE"]._serialized_end = 1639
-    _globals["_PRODUCTSERVICE"]._serialized_start = 1642
-    _globals["_PRODUCTSERVICE"]._serialized_end = 2191
+    _globals["_PRODUCT"]._serialized_start = 113
+    _globals["_PRODUCT"]._serialized_end = 306
+    _globals["_PRODUCTCREATEREQUEST"]._serialized_start = 309
+    _globals["_PRODUCTCREATEREQUEST"]._serialized_end = 450
+    _globals["_PRODUCTCREATERESPONSE"]._serialized_start = 453
+    _globals["_PRODUCTCREATERESPONSE"]._serialized_end = 612
+    _globals["_PRODUCTREADREQUEST"]._serialized_start = 615
+    _globals["_PRODUCTREADREQUEST"]._serialized_end = 983
+    _globals["_PRODUCTREADRESPONSE"]._serialized_start = 986
+    _globals["_PRODUCTREADRESPONSE"]._serialized_end = 1203
+    _globals["_PRODUCTUPDATEREQUEST"]._serialized_start = 1206
+    _globals["_PRODUCTUPDATEREQUEST"]._serialized_end = 1345
+    _globals["_PRODUCTUPDATERESPONSE"]._serialized_start = 1348
+    _globals["_PRODUCTUPDATERESPONSE"]._serialized_end = 1507
+    _globals["_PRODUCTDELETEREQUEST"]._serialized_start = 1509
+    _globals["_PRODUCTDELETEREQUEST"]._serialized_end = 1599
+    _globals["_PRODUCTDELETERESPONSE"]._serialized_start = 1601
+    _globals["_PRODUCTDELETERESPONSE"]._serialized_end = 1699
+    _globals["_PRODUCTSERVICE"]._serialized_start = 1702
+    _globals["_PRODUCTSERVICE"]._serialized_end = 2251
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/product_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/carrier_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,74 +2,75 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Product(_message.Message):
-    __slots__ = ["id", "product_doc_id", "template_doc_id", "name", "active", "object_audit"]
+class Carrier(_message.Message):
+    __slots__ = ["id", "name", "code", "carrier_sql_id", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    PRODUCT_DOC_ID_FIELD_NUMBER: _ClassVar[int]
-    TEMPLATE_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    CARRIER_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
-    product_doc_id: str
-    template_doc_id: str
     name: str
-    active: bool
+    code: str
+    carrier_sql_id: int
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
-        product_doc_id: _Optional[str] = ...,
-        template_doc_id: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        active: bool = ...,
+        code: _Optional[str] = ...,
+        carrier_sql_id: _Optional[int] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class ProductCreateRequest(_message.Message):
-    __slots__ = ["product_doc_id", "template_doc_id", "name", "context"]
-    PRODUCT_DOC_ID_FIELD_NUMBER: _ClassVar[int]
-    TEMPLATE_DOC_ID_FIELD_NUMBER: _ClassVar[int]
+class CarrierCreateRequest(_message.Message):
+    __slots__ = ["name", "code", "carrier_sql_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    CARRIER_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    product_doc_id: str
-    template_doc_id: str
     name: str
+    code: str
+    carrier_sql_id: int
     context: _base_pb2.Context
     def __init__(
         self,
-        product_doc_id: _Optional[str] = ...,
-        template_doc_id: _Optional[str] = ...,
         name: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        carrier_sql_id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ProductCreateResponse(_message.Message):
-    __slots__ = ["product", "response_standard"]
-    PRODUCT_FIELD_NUMBER: _ClassVar[int]
+class CarrierCreateResponse(_message.Message):
+    __slots__ = ["carrier", "response_standard"]
+    CARRIER_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    product: Product
+    carrier: Carrier
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        product: _Optional[_Union[Product, _Mapping]] = ...,
+        carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class ProductReadRequest(_message.Message):
+class CarrierReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -88,61 +89,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ProductReadResponse(_message.Message):
-    __slots__ = ["products", "response_standard", "meta_data"]
-    PRODUCTS_FIELD_NUMBER: _ClassVar[int]
-    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+class CarrierReadResponse(_message.Message):
+    __slots__ = ["carriers", "meta_data", "response_standard"]
+    CARRIERS_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    products: _containers.RepeatedCompositeFieldContainer[Product]
-    response_standard: _base_pb2.ResponseStandard
+    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    carriers: _containers.RepeatedCompositeFieldContainer[Carrier]
     meta_data: _base_pb2.MetaData
+    response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        products: _Optional[_Iterable[_Union[Product, _Mapping]]] = ...,
-        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        carriers: _Optional[_Iterable[_Union[Carrier, _Mapping]]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class ProductUpdateRequest(_message.Message):
-    __slots__ = ["product", "context"]
-    PRODUCT_FIELD_NUMBER: _ClassVar[int]
+class CarrierUpdateRequest(_message.Message):
+    __slots__ = ["carrier", "context"]
+    CARRIER_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    product: Product
+    carrier: Carrier
     context: _base_pb2.Context
     def __init__(
         self,
-        product: _Optional[_Union[Product, _Mapping]] = ...,
+        carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ProductUpdateResponse(_message.Message):
-    __slots__ = ["product", "response_standard"]
-    PRODUCT_FIELD_NUMBER: _ClassVar[int]
+class CarrierUpdateResponse(_message.Message):
+    __slots__ = ["carrier", "response_standard"]
+    CARRIER_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    product: Product
+    carrier: Carrier
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        product: _Optional[_Union[Product, _Mapping]] = ...,
+        carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class ProductDeleteRequest(_message.Message):
+class CarrierDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class ProductDeleteResponse(_message.Message):
+class CarrierDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/product_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/sale_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/sale_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,39 +9,40 @@
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x13v1/sales/sale.proto\x12\x1epro.omni.oms.api.v1.sales.sale\x1a\x11\x63ommon/base.proto\x1a\x1fgoogle/protobuf/timestamp.proto"\xf6\x02\n\x04Sale\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12.\n\ndate_order\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x04 \x01(\t\x12\x12\n\nchannel_id\x18\x05 \x01(\x05\x12\x13\n\x0b\x63urrency_id\x18\x06 \x01(\x05\x12\x30\n\x0c\x63onfirm_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tclient_id\x18\x08 \x01(\x05\x12\x17\n\x0f\x62ill_address_id\x18\t \x01(\x05\x12\x12\n\ncountry_id\x18\n \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x0b \x01(\x05\x12\x12\n\njson_order\x18\x0c \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\r \x01(\x08\x12?\n\x0cobject_audit\x18\x0e \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xde\x02\n\x11SaleCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\ndate_order\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x03 \x01(\t\x12\x12\n\nchannel_id\x18\x04 \x01(\x05\x12\x13\n\x0b\x63urrency_id\x18\x05 \x01(\x05\x12\x30\n\x0c\x63onfirm_date\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tclient_id\x18\x07 \x01(\x05\x12\x17\n\x0f\x62ill_address_id\x18\x08 \x01(\x05\x12\x12\n\ncountry_id\x18\t \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\n \x01(\x05\x12\x12\n\njson_order\x18\x0b \x01(\t\x12\x36\n\x07\x63ontext\x18\x0c \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x12SaleCreateResponse\x12\x32\n\x04sale\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.sale.Sale\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xed\x02\n\x0fSaleReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcc\x01\n\x10SaleReadResponse\x12\x32\n\x04sale\x18\x01 \x03(\x0b\x32$.pro.omni.oms.api.v1.sales.sale.Sale\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x7f\n\x11SaleUpdateRequest\x12\x32\n\x04sale\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.sale.Sale\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x12SaleUpdateResponse\x12\x32\n\x04sale\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.sale.Sale\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"W\n\x11SaleDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"_\n\x12SaleDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xe3\x03\n\x0bSaleService\x12u\n\nSaleCreate\x12\x31.pro.omni.oms.api.v1.sales.sale.SaleCreateRequest\x1a\x32.pro.omni.oms.api.v1.sales.sale.SaleCreateResponse"\x00\x12o\n\x08SaleRead\x12/.pro.omni.oms.api.v1.sales.sale.SaleReadRequest\x1a\x30.pro.omni.oms.api.v1.sales.sale.SaleReadResponse"\x00\x12u\n\nSaleUpdate\x12\x31.pro.omni.oms.api.v1.sales.sale.SaleUpdateRequest\x1a\x32.pro.omni.oms.api.v1.sales.sale.SaleUpdateResponse"\x00\x12u\n\nSaleDelete\x12\x31.pro.omni.oms.api.v1.sales.sale.SaleDeleteRequest\x1a\x32.pro.omni.oms.api.v1.sales.sale.SaleDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x13v1/sales/sale.proto\x12\x1epro.omni.oms.api.v1.sales.sale\x1a\x11\x63ommon/base.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto"\x92\x03\n\x04Sale\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12.\n\ndate_order\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x04 \x01(\t\x12\x12\n\nchannel_id\x18\x05 \x01(\x05\x12\x13\n\x0b\x63urrency_id\x18\x06 \x01(\x05\x12\x30\n\x0c\x63onfirm_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tclient_id\x18\x08 \x01(\x05\x12\x17\n\x0f\x62ill_address_id\x18\t \x01(\x05\x12\x12\n\ncountry_id\x18\n \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\x0b \x01(\x05\x12\x12\n\njson_order\x18\x0c \x01(\t\x12*\n\x06\x61\x63tive\x18\r \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x0e \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\xde\x02\n\x11SaleCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\ndate_order\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x03 \x01(\t\x12\x12\n\nchannel_id\x18\x04 \x01(\x05\x12\x13\n\x0b\x63urrency_id\x18\x05 \x01(\x05\x12\x30\n\x0c\x63onfirm_date\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tclient_id\x18\x07 \x01(\x05\x12\x17\n\x0f\x62ill_address_id\x18\x08 \x01(\x05\x12\x12\n\ncountry_id\x18\t \x01(\x05\x12\x14\n\x0cwarehouse_id\x18\n \x01(\x05\x12\x12\n\njson_order\x18\x0b \x01(\t\x12\x36\n\x07\x63ontext\x18\x0c \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x12SaleCreateResponse\x12\x32\n\x04sale\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.sale.Sale\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xed\x02\n\x0fSaleReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcc\x01\n\x10SaleReadResponse\x12\x32\n\x04sale\x18\x01 \x03(\x0b\x32$.pro.omni.oms.api.v1.sales.sale.Sale\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x7f\n\x11SaleUpdateRequest\x12\x32\n\x04sale\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.sale.Sale\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x12SaleUpdateResponse\x12\x32\n\x04sale\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.sale.Sale\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"W\n\x11SaleDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"_\n\x12SaleDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xe3\x03\n\x0bSaleService\x12u\n\nSaleCreate\x12\x31.pro.omni.oms.api.v1.sales.sale.SaleCreateRequest\x1a\x32.pro.omni.oms.api.v1.sales.sale.SaleCreateResponse"\x00\x12o\n\x08SaleRead\x12/.pro.omni.oms.api.v1.sales.sale.SaleReadRequest\x1a\x30.pro.omni.oms.api.v1.sales.sale.SaleReadResponse"\x00\x12u\n\nSaleUpdate\x12\x31.pro.omni.oms.api.v1.sales.sale.SaleUpdateRequest\x1a\x32.pro.omni.oms.api.v1.sales.sale.SaleUpdateResponse"\x00\x12u\n\nSaleDelete\x12\x31.pro.omni.oms.api.v1.sales.sale.SaleDeleteRequest\x1a\x32.pro.omni.oms.api.v1.sales.sale.SaleDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.sale_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_SALE"]._serialized_start = 108
-    _globals["_SALE"]._serialized_end = 482
-    _globals["_SALECREATEREQUEST"]._serialized_start = 485
-    _globals["_SALECREATEREQUEST"]._serialized_end = 835
-    _globals["_SALECREATERESPONSE"]._serialized_start = 838
-    _globals["_SALECREATERESPONSE"]._serialized_end = 985
-    _globals["_SALEREADREQUEST"]._serialized_start = 988
-    _globals["_SALEREADREQUEST"]._serialized_end = 1353
-    _globals["_SALEREADRESPONSE"]._serialized_start = 1356
-    _globals["_SALEREADRESPONSE"]._serialized_end = 1560
-    _globals["_SALEUPDATEREQUEST"]._serialized_start = 1562
-    _globals["_SALEUPDATEREQUEST"]._serialized_end = 1689
-    _globals["_SALEUPDATERESPONSE"]._serialized_start = 1692
-    _globals["_SALEUPDATERESPONSE"]._serialized_end = 1839
-    _globals["_SALEDELETEREQUEST"]._serialized_start = 1841
-    _globals["_SALEDELETEREQUEST"]._serialized_end = 1928
-    _globals["_SALEDELETERESPONSE"]._serialized_start = 1930
-    _globals["_SALEDELETERESPONSE"]._serialized_end = 2025
-    _globals["_SALESERVICE"]._serialized_start = 2028
-    _globals["_SALESERVICE"]._serialized_end = 2511
+    _globals["_SALE"]._serialized_start = 140
+    _globals["_SALE"]._serialized_end = 542
+    _globals["_SALECREATEREQUEST"]._serialized_start = 545
+    _globals["_SALECREATEREQUEST"]._serialized_end = 895
+    _globals["_SALECREATERESPONSE"]._serialized_start = 898
+    _globals["_SALECREATERESPONSE"]._serialized_end = 1045
+    _globals["_SALEREADREQUEST"]._serialized_start = 1048
+    _globals["_SALEREADREQUEST"]._serialized_end = 1413
+    _globals["_SALEREADRESPONSE"]._serialized_start = 1416
+    _globals["_SALEREADRESPONSE"]._serialized_end = 1620
+    _globals["_SALEUPDATEREQUEST"]._serialized_start = 1622
+    _globals["_SALEUPDATEREQUEST"]._serialized_end = 1749
+    _globals["_SALEUPDATERESPONSE"]._serialized_start = 1752
+    _globals["_SALEUPDATERESPONSE"]._serialized_end = 1899
+    _globals["_SALEDELETEREQUEST"]._serialized_start = 1901
+    _globals["_SALEDELETEREQUEST"]._serialized_end = 1988
+    _globals["_SALEDELETERESPONSE"]._serialized_start = 1990
+    _globals["_SALEDELETERESPONSE"]._serialized_end = 2085
+    _globals["_SALESERVICE"]._serialized_start = 2088
+    _globals["_SALESERVICE"]._serialized_end = 2571
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/sale_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/sale_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Sale(_message.Message):
     __slots__ = [
@@ -51,15 +52,15 @@
     currency_id: int
     confirm_date: _timestamp_pb2.Timestamp
     client_id: int
     bill_address_id: int
     country_id: int
     warehouse_id: int
     json_order: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         name: _Optional[str] = ...,
         date_order: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
         origin: _Optional[str] = ...,
@@ -67,15 +68,15 @@
         currency_id: _Optional[int] = ...,
         confirm_date: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
         client_id: _Optional[int] = ...,
         bill_address_id: _Optional[int] = ...,
         country_id: _Optional[int] = ...,
         warehouse_id: _Optional[int] = ...,
         json_order: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class SaleCreateRequest(_message.Message):
     __slots__ = [
         "name",
         "date_order",
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/sale_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/sale_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/tax_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/tax_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x12v1/sales/tax.proto\x12\x1dpro.omni.oms.api.v1.sales.tax\x1a\x11\x63ommon/base.proto"\x92\x01\n\x03Tax\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\ntax_doc_id\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"z\n\x10TaxCreateRequest\x12\x12\n\ntax_doc_id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8f\x01\n\x11TaxCreateResponse\x12/\n\x03tax\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.tax.Tax\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xec\x02\n\x0eTaxReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc8\x01\n\x0fTaxReadResponse\x12/\n\x03tax\x18\x01 \x03(\x0b\x32".pro.omni.oms.api.v1.sales.tax.Tax\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"{\n\x10TaxUpdateRequest\x12/\n\x03tax\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.tax.Tax\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8f\x01\n\x11TaxUpdateResponse\x12/\n\x03tax\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.tax.Tax\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"V\n\x10TaxDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11TaxDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xce\x03\n\nTaxService\x12p\n\tTaxCreate\x12/.pro.omni.oms.api.v1.sales.tax.TaxCreateRequest\x1a\x30.pro.omni.oms.api.v1.sales.tax.TaxCreateResponse"\x00\x12j\n\x07TaxRead\x12-.pro.omni.oms.api.v1.sales.tax.TaxReadRequest\x1a..pro.omni.oms.api.v1.sales.tax.TaxReadResponse"\x00\x12p\n\tTaxUpdate\x12/.pro.omni.oms.api.v1.sales.tax.TaxUpdateRequest\x1a\x30.pro.omni.oms.api.v1.sales.tax.TaxUpdateResponse"\x00\x12p\n\tTaxDelete\x12/.pro.omni.oms.api.v1.sales.tax.TaxDeleteRequest\x1a\x30.pro.omni.oms.api.v1.sales.tax.TaxDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x12v1/sales/tax.proto\x12\x1dpro.omni.oms.api.v1.sales.tax\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xae\x01\n\x03Tax\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\ntax_doc_id\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"z\n\x10TaxCreateRequest\x12\x12\n\ntax_doc_id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8f\x01\n\x11TaxCreateResponse\x12/\n\x03tax\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.tax.Tax\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xec\x02\n\x0eTaxReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc8\x01\n\x0fTaxReadResponse\x12/\n\x03tax\x18\x01 \x03(\x0b\x32".pro.omni.oms.api.v1.sales.tax.Tax\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"{\n\x10TaxUpdateRequest\x12/\n\x03tax\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.tax.Tax\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8f\x01\n\x11TaxUpdateResponse\x12/\n\x03tax\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.tax.Tax\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"V\n\x10TaxDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11TaxDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xce\x03\n\nTaxService\x12p\n\tTaxCreate\x12/.pro.omni.oms.api.v1.sales.tax.TaxCreateRequest\x1a\x30.pro.omni.oms.api.v1.sales.tax.TaxCreateResponse"\x00\x12j\n\x07TaxRead\x12-.pro.omni.oms.api.v1.sales.tax.TaxReadRequest\x1a..pro.omni.oms.api.v1.sales.tax.TaxReadResponse"\x00\x12p\n\tTaxUpdate\x12/.pro.omni.oms.api.v1.sales.tax.TaxUpdateRequest\x1a\x30.pro.omni.oms.api.v1.sales.tax.TaxUpdateResponse"\x00\x12p\n\tTaxDelete\x12/.pro.omni.oms.api.v1.sales.tax.TaxDeleteRequest\x1a\x30.pro.omni.oms.api.v1.sales.tax.TaxDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.tax_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_TAX"]._serialized_start = 73
-    _globals["_TAX"]._serialized_end = 219
-    _globals["_TAXCREATEREQUEST"]._serialized_start = 221
-    _globals["_TAXCREATEREQUEST"]._serialized_end = 343
-    _globals["_TAXCREATERESPONSE"]._serialized_start = 346
-    _globals["_TAXCREATERESPONSE"]._serialized_end = 489
-    _globals["_TAXREADREQUEST"]._serialized_start = 492
-    _globals["_TAXREADREQUEST"]._serialized_end = 856
-    _globals["_TAXREADRESPONSE"]._serialized_start = 859
-    _globals["_TAXREADRESPONSE"]._serialized_end = 1059
-    _globals["_TAXUPDATEREQUEST"]._serialized_start = 1061
-    _globals["_TAXUPDATEREQUEST"]._serialized_end = 1184
-    _globals["_TAXUPDATERESPONSE"]._serialized_start = 1187
-    _globals["_TAXUPDATERESPONSE"]._serialized_end = 1330
-    _globals["_TAXDELETEREQUEST"]._serialized_start = 1332
-    _globals["_TAXDELETEREQUEST"]._serialized_end = 1418
-    _globals["_TAXDELETERESPONSE"]._serialized_start = 1420
-    _globals["_TAXDELETERESPONSE"]._serialized_end = 1514
-    _globals["_TAXSERVICE"]._serialized_start = 1517
-    _globals["_TAXSERVICE"]._serialized_end = 1979
+    _globals["_TAX"]._serialized_start = 105
+    _globals["_TAX"]._serialized_end = 279
+    _globals["_TAXCREATEREQUEST"]._serialized_start = 281
+    _globals["_TAXCREATEREQUEST"]._serialized_end = 403
+    _globals["_TAXCREATERESPONSE"]._serialized_start = 406
+    _globals["_TAXCREATERESPONSE"]._serialized_end = 549
+    _globals["_TAXREADREQUEST"]._serialized_start = 552
+    _globals["_TAXREADREQUEST"]._serialized_end = 916
+    _globals["_TAXREADRESPONSE"]._serialized_start = 919
+    _globals["_TAXREADRESPONSE"]._serialized_end = 1119
+    _globals["_TAXUPDATEREQUEST"]._serialized_start = 1121
+    _globals["_TAXUPDATEREQUEST"]._serialized_end = 1244
+    _globals["_TAXUPDATERESPONSE"]._serialized_start = 1247
+    _globals["_TAXUPDATERESPONSE"]._serialized_end = 1390
+    _globals["_TAXDELETEREQUEST"]._serialized_start = 1392
+    _globals["_TAXDELETEREQUEST"]._serialized_end = 1478
+    _globals["_TAXDELETERESPONSE"]._serialized_start = 1480
+    _globals["_TAXDELETERESPONSE"]._serialized_end = 1574
+    _globals["_TAXSERVICE"]._serialized_start = 1577
+    _globals["_TAXSERVICE"]._serialized_end = 2039
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/tax_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/uom_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,74 +2,75 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Tax(_message.Message):
-    __slots__ = ["id", "tax_doc_id", "code", "name", "active", "object_audit"]
+class Uom(_message.Message):
+    __slots__ = ["id", "uom_doc_id", "code", "name", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    TAX_DOC_ID_FIELD_NUMBER: _ClassVar[int]
+    UOM_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
-    tax_doc_id: str
+    uom_doc_id: str
     code: str
     name: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
-        tax_doc_id: _Optional[str] = ...,
+        uom_doc_id: _Optional[str] = ...,
         code: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxCreateRequest(_message.Message):
-    __slots__ = ["tax_doc_id", "code", "name", "context"]
-    TAX_DOC_ID_FIELD_NUMBER: _ClassVar[int]
+class UomCreateRequest(_message.Message):
+    __slots__ = ["uom_doc_id", "code", "name", "context"]
+    UOM_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    tax_doc_id: str
+    uom_doc_id: str
     code: str
     name: str
     context: _base_pb2.Context
     def __init__(
         self,
-        tax_doc_id: _Optional[str] = ...,
+        uom_doc_id: _Optional[str] = ...,
         code: _Optional[str] = ...,
         name: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxCreateResponse(_message.Message):
-    __slots__ = ["tax", "response_standard"]
-    TAX_FIELD_NUMBER: _ClassVar[int]
+class UomCreateResponse(_message.Message):
+    __slots__ = ["uom", "response_standard"]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    tax: Tax
+    uom: Uom
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        tax: _Optional[_Union[Tax, _Mapping]] = ...,
+        uom: _Optional[_Union[Uom, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxReadRequest(_message.Message):
+class UomReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -88,59 +89,59 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxReadResponse(_message.Message):
-    __slots__ = ["tax", "response_standard", "meta_data"]
-    TAX_FIELD_NUMBER: _ClassVar[int]
+class UomReadResponse(_message.Message):
+    __slots__ = ["uom", "response_standard", "meta_data"]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    tax: _containers.RepeatedCompositeFieldContainer[Tax]
+    uom: _containers.RepeatedCompositeFieldContainer[Uom]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
     def __init__(
         self,
-        tax: _Optional[_Iterable[_Union[Tax, _Mapping]]] = ...,
+        uom: _Optional[_Iterable[_Union[Uom, _Mapping]]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxUpdateRequest(_message.Message):
-    __slots__ = ["tax", "context"]
-    TAX_FIELD_NUMBER: _ClassVar[int]
+class UomUpdateRequest(_message.Message):
+    __slots__ = ["uom", "context"]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    tax: Tax
+    uom: Uom
     context: _base_pb2.Context
     def __init__(
-        self, tax: _Optional[_Union[Tax, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, uom: _Optional[_Union[Uom, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class TaxUpdateResponse(_message.Message):
-    __slots__ = ["tax", "response_standard"]
-    TAX_FIELD_NUMBER: _ClassVar[int]
+class UomUpdateResponse(_message.Message):
+    __slots__ = ["uom", "response_standard"]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    tax: Tax
+    uom: Uom
     response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        tax: _Optional[_Union[Tax, _Mapping]] = ...,
+        uom: _Optional[_Union[Uom, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxDeleteRequest(_message.Message):
+class UomDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class TaxDeleteResponse(_message.Message):
+class UomDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/tax_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/tax_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/uom_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/uom_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x12v1/sales/uom.proto\x12\x1dpro.omni.oms.api.v1.sales.uom\x1a\x11\x63ommon/base.proto"\x92\x01\n\x03Uom\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\nuom_doc_id\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"z\n\x10UomCreateRequest\x12\x12\n\nuom_doc_id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8f\x01\n\x11UomCreateResponse\x12/\n\x03uom\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.uom.Uom\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xec\x02\n\x0eUomReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc8\x01\n\x0fUomReadResponse\x12/\n\x03uom\x18\x01 \x03(\x0b\x32".pro.omni.oms.api.v1.sales.uom.Uom\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"{\n\x10UomUpdateRequest\x12/\n\x03uom\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.uom.Uom\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8f\x01\n\x11UomUpdateResponse\x12/\n\x03uom\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.uom.Uom\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"V\n\x10UomDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11UomDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xce\x03\n\nUomService\x12p\n\tUomCreate\x12/.pro.omni.oms.api.v1.sales.uom.UomCreateRequest\x1a\x30.pro.omni.oms.api.v1.sales.uom.UomCreateResponse"\x00\x12j\n\x07UomRead\x12-.pro.omni.oms.api.v1.sales.uom.UomReadRequest\x1a..pro.omni.oms.api.v1.sales.uom.UomReadResponse"\x00\x12p\n\tUomUpdate\x12/.pro.omni.oms.api.v1.sales.uom.UomUpdateRequest\x1a\x30.pro.omni.oms.api.v1.sales.uom.UomUpdateResponse"\x00\x12p\n\tUomDelete\x12/.pro.omni.oms.api.v1.sales.uom.UomDeleteRequest\x1a\x30.pro.omni.oms.api.v1.sales.uom.UomDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x12v1/sales/uom.proto\x12\x1dpro.omni.oms.api.v1.sales.uom\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xae\x01\n\x03Uom\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\nuom_doc_id\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"z\n\x10UomCreateRequest\x12\x12\n\nuom_doc_id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8f\x01\n\x11UomCreateResponse\x12/\n\x03uom\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.uom.Uom\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xec\x02\n\x0eUomReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xc8\x01\n\x0fUomReadResponse\x12/\n\x03uom\x18\x01 \x03(\x0b\x32".pro.omni.oms.api.v1.sales.uom.Uom\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"{\n\x10UomUpdateRequest\x12/\n\x03uom\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.uom.Uom\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x8f\x01\n\x11UomUpdateResponse\x12/\n\x03uom\x18\x01 \x01(\x0b\x32".pro.omni.oms.api.v1.sales.uom.Uom\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"V\n\x10UomDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"^\n\x11UomDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xce\x03\n\nUomService\x12p\n\tUomCreate\x12/.pro.omni.oms.api.v1.sales.uom.UomCreateRequest\x1a\x30.pro.omni.oms.api.v1.sales.uom.UomCreateResponse"\x00\x12j\n\x07UomRead\x12-.pro.omni.oms.api.v1.sales.uom.UomReadRequest\x1a..pro.omni.oms.api.v1.sales.uom.UomReadResponse"\x00\x12p\n\tUomUpdate\x12/.pro.omni.oms.api.v1.sales.uom.UomUpdateRequest\x1a\x30.pro.omni.oms.api.v1.sales.uom.UomUpdateResponse"\x00\x12p\n\tUomDelete\x12/.pro.omni.oms.api.v1.sales.uom.UomDeleteRequest\x1a\x30.pro.omni.oms.api.v1.sales.uom.UomDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.uom_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_UOM"]._serialized_start = 73
-    _globals["_UOM"]._serialized_end = 219
-    _globals["_UOMCREATEREQUEST"]._serialized_start = 221
-    _globals["_UOMCREATEREQUEST"]._serialized_end = 343
-    _globals["_UOMCREATERESPONSE"]._serialized_start = 346
-    _globals["_UOMCREATERESPONSE"]._serialized_end = 489
-    _globals["_UOMREADREQUEST"]._serialized_start = 492
-    _globals["_UOMREADREQUEST"]._serialized_end = 856
-    _globals["_UOMREADRESPONSE"]._serialized_start = 859
-    _globals["_UOMREADRESPONSE"]._serialized_end = 1059
-    _globals["_UOMUPDATEREQUEST"]._serialized_start = 1061
-    _globals["_UOMUPDATEREQUEST"]._serialized_end = 1184
-    _globals["_UOMUPDATERESPONSE"]._serialized_start = 1187
-    _globals["_UOMUPDATERESPONSE"]._serialized_end = 1330
-    _globals["_UOMDELETEREQUEST"]._serialized_start = 1332
-    _globals["_UOMDELETEREQUEST"]._serialized_end = 1418
-    _globals["_UOMDELETERESPONSE"]._serialized_start = 1420
-    _globals["_UOMDELETERESPONSE"]._serialized_end = 1514
-    _globals["_UOMSERVICE"]._serialized_start = 1517
-    _globals["_UOMSERVICE"]._serialized_end = 1979
+    _globals["_UOM"]._serialized_start = 105
+    _globals["_UOM"]._serialized_end = 279
+    _globals["_UOMCREATEREQUEST"]._serialized_start = 281
+    _globals["_UOMCREATEREQUEST"]._serialized_end = 403
+    _globals["_UOMCREATERESPONSE"]._serialized_start = 406
+    _globals["_UOMCREATERESPONSE"]._serialized_end = 549
+    _globals["_UOMREADREQUEST"]._serialized_start = 552
+    _globals["_UOMREADREQUEST"]._serialized_end = 916
+    _globals["_UOMREADRESPONSE"]._serialized_start = 919
+    _globals["_UOMREADRESPONSE"]._serialized_end = 1119
+    _globals["_UOMUPDATEREQUEST"]._serialized_start = 1121
+    _globals["_UOMUPDATEREQUEST"]._serialized_end = 1244
+    _globals["_UOMUPDATERESPONSE"]._serialized_start = 1247
+    _globals["_UOMUPDATERESPONSE"]._serialized_end = 1390
+    _globals["_UOMDELETEREQUEST"]._serialized_start = 1392
+    _globals["_UOMDELETEREQUEST"]._serialized_end = 1478
+    _globals["_UOMDELETERESPONSE"]._serialized_start = 1480
+    _globals["_UOMDELETERESPONSE"]._serialized_end = 1574
+    _globals["_UOMSERVICE"]._serialized_start = 1577
+    _globals["_UOMSERVICE"]._serialized_end = 2039
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/uom_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/uom_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Uom(_message.Message):
     __slots__ = ["id", "uom_doc_id", "code", "name", "active", "object_audit"]
@@ -19,23 +20,23 @@
     NAME_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     uom_doc_id: str
     code: str
     name: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         uom_doc_id: _Optional[str] = ...,
         code: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class UomCreateRequest(_message.Message):
     __slots__ = ["uom_doc_id", "code", "name", "context"]
     UOM_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
@@ -50,23 +51,23 @@
         uom_doc_id: _Optional[str] = ...,
         code: _Optional[str] = ...,
         name: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class UomCreateResponse(_message.Message):
-    __slots__ = ["uom", "response_standard"]
+    __slots__ = ["response", "uom"]
+    RESPONSE_FIELD_NUMBER: _ClassVar[int]
     UOM_FIELD_NUMBER: _ClassVar[int]
-    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    response: _base_pb2.ResponseStandard
     uom: Uom
-    response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
+        response: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         uom: _Optional[_Union[Uom, _Mapping]] = ...,
-        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
 class UomReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
@@ -89,58 +90,58 @@
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class UomReadResponse(_message.Message):
-    __slots__ = ["uom", "response_standard", "meta_data"]
-    UOM_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["response_standard", "meta_data", "uoms"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    uom: _containers.RepeatedCompositeFieldContainer[Uom]
+    UOMS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
+    uoms: _containers.RepeatedCompositeFieldContainer[Uom]
     def __init__(
         self,
-        uom: _Optional[_Iterable[_Union[Uom, _Mapping]]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        uoms: _Optional[_Iterable[_Union[Uom, _Mapping]]] = ...,
     ) -> None: ...
 
 class UomUpdateRequest(_message.Message):
     __slots__ = ["uom", "context"]
     UOM_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     uom: Uom
     context: _base_pb2.Context
     def __init__(
         self, uom: _Optional[_Union[Uom, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
 class UomUpdateResponse(_message.Message):
-    __slots__ = ["uom", "response_standard"]
+    __slots__ = ["response", "uom"]
+    RESPONSE_FIELD_NUMBER: _ClassVar[int]
     UOM_FIELD_NUMBER: _ClassVar[int]
-    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    response: _base_pb2.ResponseStandard
     uom: Uom
-    response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
+        response: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         uom: _Optional[_Union[Uom, _Mapping]] = ...,
-        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
 class UomDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
 class UomDeleteResponse(_message.Message):
-    __slots__ = ["response_standard"]
-    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    response_standard: _base_pb2.ResponseStandard
-    def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
+    __slots__ = ["response"]
+    RESPONSE_FIELD_NUMBER: _ClassVar[int]
+    response: _base_pb2.ResponseStandard
+    def __init__(self, response: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/uom_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/uom_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/user_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/user_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x13v1/sales/user.proto\x12\x1epro.omni.oms.api.v1.sales.user\x1a\x11\x63ommon/base.proto"\x86\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x13\n\x0buser_doc_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"n\n\x11UserCreateRequest\x12\x13\n\x0buser_doc_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x12UserCreateResponse\x12\x32\n\x04user\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.user.User\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xed\x02\n\x0fUserReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcc\x01\n\x10UserReadResponse\x12\x32\n\x04user\x18\x01 \x03(\x0b\x32$.pro.omni.oms.api.v1.sales.user.User\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x7f\n\x11UserUpdateRequest\x12\x32\n\x04user\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.user.User\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x12UserUpdateResponse\x12\x32\n\x04user\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.user.User\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"W\n\x11UserDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"_\n\x12UserDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xe3\x03\n\x0bUserService\x12u\n\nUserCreate\x12\x31.pro.omni.oms.api.v1.sales.user.UserCreateRequest\x1a\x32.pro.omni.oms.api.v1.sales.user.UserCreateResponse"\x00\x12o\n\x08UserRead\x12/.pro.omni.oms.api.v1.sales.user.UserReadRequest\x1a\x30.pro.omni.oms.api.v1.sales.user.UserReadResponse"\x00\x12u\n\nUserUpdate\x12\x31.pro.omni.oms.api.v1.sales.user.UserUpdateRequest\x1a\x32.pro.omni.oms.api.v1.sales.user.UserUpdateResponse"\x00\x12u\n\nUserDelete\x12\x31.pro.omni.oms.api.v1.sales.user.UserDeleteRequest\x1a\x32.pro.omni.oms.api.v1.sales.user.UserDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x13v1/sales/user.proto\x12\x1epro.omni.oms.api.v1.sales.user\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xa2\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x13\n\x0buser_doc_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12*\n\x06\x61\x63tive\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"n\n\x11UserCreateRequest\x12\x13\n\x0buser_doc_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x36\n\x07\x63ontext\x18\x03 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x12UserCreateResponse\x12\x32\n\x04user\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.user.User\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xed\x02\n\x0fUserReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xcc\x01\n\x10UserReadResponse\x12\x32\n\x04user\x18\x01 \x03(\x0b\x32$.pro.omni.oms.api.v1.sales.user.User\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard\x12\x39\n\tmeta_data\x18\x03 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData"\x7f\n\x11UserUpdateRequest\x12\x32\n\x04user\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.user.User\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\x93\x01\n\x12UserUpdateResponse\x12\x32\n\x04user\x18\x01 \x01(\x0b\x32$.pro.omni.oms.api.v1.sales.user.User\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"W\n\x11UserDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"_\n\x12UserDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xe3\x03\n\x0bUserService\x12u\n\nUserCreate\x12\x31.pro.omni.oms.api.v1.sales.user.UserCreateRequest\x1a\x32.pro.omni.oms.api.v1.sales.user.UserCreateResponse"\x00\x12o\n\x08UserRead\x12/.pro.omni.oms.api.v1.sales.user.UserReadRequest\x1a\x30.pro.omni.oms.api.v1.sales.user.UserReadResponse"\x00\x12u\n\nUserUpdate\x12\x31.pro.omni.oms.api.v1.sales.user.UserUpdateRequest\x1a\x32.pro.omni.oms.api.v1.sales.user.UserUpdateResponse"\x00\x12u\n\nUserDelete\x12\x31.pro.omni.oms.api.v1.sales.user.UserDeleteRequest\x1a\x32.pro.omni.oms.api.v1.sales.user.UserDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.user_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_USER"]._serialized_start = 75
-    _globals["_USER"]._serialized_end = 209
-    _globals["_USERCREATEREQUEST"]._serialized_start = 211
-    _globals["_USERCREATEREQUEST"]._serialized_end = 321
-    _globals["_USERCREATERESPONSE"]._serialized_start = 324
-    _globals["_USERCREATERESPONSE"]._serialized_end = 471
-    _globals["_USERREADREQUEST"]._serialized_start = 474
-    _globals["_USERREADREQUEST"]._serialized_end = 839
-    _globals["_USERREADRESPONSE"]._serialized_start = 842
-    _globals["_USERREADRESPONSE"]._serialized_end = 1046
-    _globals["_USERUPDATEREQUEST"]._serialized_start = 1048
-    _globals["_USERUPDATEREQUEST"]._serialized_end = 1175
-    _globals["_USERUPDATERESPONSE"]._serialized_start = 1178
-    _globals["_USERUPDATERESPONSE"]._serialized_end = 1325
-    _globals["_USERDELETEREQUEST"]._serialized_start = 1327
-    _globals["_USERDELETEREQUEST"]._serialized_end = 1414
-    _globals["_USERDELETERESPONSE"]._serialized_start = 1416
-    _globals["_USERDELETERESPONSE"]._serialized_end = 1511
-    _globals["_USERSERVICE"]._serialized_start = 1514
-    _globals["_USERSERVICE"]._serialized_end = 1997
+    _globals["_USER"]._serialized_start = 107
+    _globals["_USER"]._serialized_end = 269
+    _globals["_USERCREATEREQUEST"]._serialized_start = 271
+    _globals["_USERCREATEREQUEST"]._serialized_end = 381
+    _globals["_USERCREATERESPONSE"]._serialized_start = 384
+    _globals["_USERCREATERESPONSE"]._serialized_end = 531
+    _globals["_USERREADREQUEST"]._serialized_start = 534
+    _globals["_USERREADREQUEST"]._serialized_end = 899
+    _globals["_USERREADRESPONSE"]._serialized_start = 902
+    _globals["_USERREADRESPONSE"]._serialized_end = 1106
+    _globals["_USERUPDATEREQUEST"]._serialized_start = 1108
+    _globals["_USERUPDATEREQUEST"]._serialized_end = 1235
+    _globals["_USERUPDATERESPONSE"]._serialized_start = 1238
+    _globals["_USERUPDATERESPONSE"]._serialized_end = 1385
+    _globals["_USERDELETEREQUEST"]._serialized_start = 1387
+    _globals["_USERDELETEREQUEST"]._serialized_end = 1474
+    _globals["_USERDELETERESPONSE"]._serialized_start = 1476
+    _globals["_USERDELETERESPONSE"]._serialized_end = 1571
+    _globals["_USERSERVICE"]._serialized_start = 1574
+    _globals["_USERSERVICE"]._serialized_end = 2057
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/user_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/user_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class User(_message.Message):
     __slots__ = ["id", "user_doc_id", "name", "active", "object_audit"]
@@ -17,22 +18,22 @@
     USER_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     user_doc_id: str
     name: str
-    active: bool
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         user_doc_id: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        active: bool = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class UserCreateRequest(_message.Message):
     __slots__ = ["user_doc_id", "name", "context"]
     USER_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
@@ -44,23 +45,23 @@
         self,
         user_doc_id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class UserCreateResponse(_message.Message):
-    __slots__ = ["user", "response_standard"]
-    USER_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["response_standard", "user"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    user: User
+    USER_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    user: User
     def __init__(
         self,
-        user: _Optional[_Union[User, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        user: _Optional[_Union[User, _Mapping]] = ...,
     ) -> None: ...
 
 class UserReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
@@ -83,26 +84,26 @@
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class UserReadResponse(_message.Message):
-    __slots__ = ["user", "response_standard", "meta_data"]
-    USER_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["response_standard", "meta_data", "users"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    user: _containers.RepeatedCompositeFieldContainer[User]
+    USERS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
+    users: _containers.RepeatedCompositeFieldContainer[User]
     def __init__(
         self,
-        user: _Optional[_Iterable[_Union[User, _Mapping]]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
+        users: _Optional[_Iterable[_Union[User, _Mapping]]] = ...,
     ) -> None: ...
 
 class UserUpdateRequest(_message.Message):
     __slots__ = ["user", "context"]
     USER_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     user: User
@@ -110,23 +111,23 @@
     def __init__(
         self,
         user: _Optional[_Union[User, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class UserUpdateResponse(_message.Message):
-    __slots__ = ["user", "response_standard"]
-    USER_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["response_standard", "user"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    user: User
+    USER_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
+    user: User
     def __init__(
         self,
-        user: _Optional[_Union[User, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        user: _Optional[_Union[User, _Mapping]] = ...,
     ) -> None: ...
 
 class UserDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/user_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/warehouse_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/warehouse_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from omni.pro.protos.common import base_pb2 as common_dot_base__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x18v1/sales/warehouse.proto\x12#pro.omni.oms.api.v1.sales.warehouse\x1a\x11\x63ommon/base.proto"\x8e\x01\n\tWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x18\n\x10warehouse_sql_id\x18\x04 \x01(\x05\x12?\n\x0cobject_audit\x18\x05 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x86\x01\n\x16WarehouseCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x18\n\x10warehouse_sql_id\x18\x03 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseCreateResponse\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.sales.warehouse.Warehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf2\x02\n\x14WarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe1\x01\n\x15WarehouseReadResponse\x12\x42\n\nwarehouses\x18\x01 \x03(\x0b\x32..pro.omni.oms.api.v1.sales.warehouse.Warehouse\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x93\x01\n\x16WarehouseUpdateRequest\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.sales.warehouse.Warehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseUpdateResponse\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.sales.warehouse.Warehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\\\n\x16WarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17WarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd0\x04\n\x10WarehouseService\x12\x8e\x01\n\x0fWarehouseCreate\x12;.pro.omni.oms.api.v1.sales.warehouse.WarehouseCreateRequest\x1a<.pro.omni.oms.api.v1.sales.warehouse.WarehouseCreateResponse"\x00\x12\x88\x01\n\rWarehouseRead\x12\x39.pro.omni.oms.api.v1.sales.warehouse.WarehouseReadRequest\x1a:.pro.omni.oms.api.v1.sales.warehouse.WarehouseReadResponse"\x00\x12\x8e\x01\n\x0fWarehouseUpdate\x12;.pro.omni.oms.api.v1.sales.warehouse.WarehouseUpdateRequest\x1a<.pro.omni.oms.api.v1.sales.warehouse.WarehouseUpdateResponse"\x00\x12\x8e\x01\n\x0fWarehouseDelete\x12;.pro.omni.oms.api.v1.sales.warehouse.WarehouseDeleteRequest\x1a<.pro.omni.oms.api.v1.sales.warehouse.WarehouseDeleteResponse"\x00\x62\x06proto3'
+    b'\n\x18v1/sales/warehouse.proto\x12#pro.omni.oms.api.v1.sales.warehouse\x1a\x11\x63ommon/base.proto\x1a\x1egoogle/protobuf/wrappers.proto"\xba\x01\n\tWarehouse\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x18\n\x10warehouse_sql_id\x18\x04 \x01(\x05\x12*\n\x06\x61\x63tive\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x0cobject_audit\x18\x06 \x01(\x0b\x32).pro.omni.oms.api.common.base.ObjectAudit"\x86\x01\n\x16WarehouseCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x18\n\x10warehouse_sql_id\x18\x03 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x04 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseCreateResponse\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.sales.warehouse.Warehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\xf2\x02\n\x14WarehouseReadRequest\x12\x37\n\x08group_by\x18\x01 \x03(\x0b\x32%.pro.omni.oms.api.common.base.GroupBy\x12\x35\n\x07sort_by\x18\x02 \x01(\x0b\x32$.pro.omni.oms.api.common.base.SortBy\x12\x34\n\x06\x66ields\x18\x03 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Fields\x12\x34\n\x06\x66ilter\x18\x04 \x01(\x0b\x32$.pro.omni.oms.api.common.base.Filter\x12:\n\tpaginated\x18\x05 \x01(\x0b\x32\'.pro.omni.oms.api.common.base.Paginated\x12\n\n\x02id\x18\x06 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x07 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xe1\x01\n\x15WarehouseReadResponse\x12\x42\n\nwarehouses\x18\x01 \x03(\x0b\x32..pro.omni.oms.api.v1.sales.warehouse.Warehouse\x12\x39\n\tmeta_data\x18\x02 \x01(\x0b\x32&.pro.omni.oms.api.common.base.MetaData\x12I\n\x11response_standard\x18\x03 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\x93\x01\n\x16WarehouseUpdateRequest\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.sales.warehouse.Warehouse\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"\xa7\x01\n\x17WarehouseUpdateResponse\x12\x41\n\twarehouse\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.v1.sales.warehouse.Warehouse\x12I\n\x11response_standard\x18\x02 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard"\\\n\x16WarehouseDeleteRequest\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x36\n\x07\x63ontext\x18\x02 \x01(\x0b\x32%.pro.omni.oms.api.common.base.Context"d\n\x17WarehouseDeleteResponse\x12I\n\x11response_standard\x18\x01 \x01(\x0b\x32..pro.omni.oms.api.common.base.ResponseStandard2\xd0\x04\n\x10WarehouseService\x12\x8e\x01\n\x0fWarehouseCreate\x12;.pro.omni.oms.api.v1.sales.warehouse.WarehouseCreateRequest\x1a<.pro.omni.oms.api.v1.sales.warehouse.WarehouseCreateResponse"\x00\x12\x88\x01\n\rWarehouseRead\x12\x39.pro.omni.oms.api.v1.sales.warehouse.WarehouseReadRequest\x1a:.pro.omni.oms.api.v1.sales.warehouse.WarehouseReadResponse"\x00\x12\x8e\x01\n\x0fWarehouseUpdate\x12;.pro.omni.oms.api.v1.sales.warehouse.WarehouseUpdateRequest\x1a<.pro.omni.oms.api.v1.sales.warehouse.WarehouseUpdateResponse"\x00\x12\x8e\x01\n\x0fWarehouseDelete\x12;.pro.omni.oms.api.v1.sales.warehouse.WarehouseDeleteRequest\x1a<.pro.omni.oms.api.v1.sales.warehouse.WarehouseDeleteResponse"\x00\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.sales.warehouse_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_WAREHOUSE"]._serialized_start = 85
-    _globals["_WAREHOUSE"]._serialized_end = 227
-    _globals["_WAREHOUSECREATEREQUEST"]._serialized_start = 230
-    _globals["_WAREHOUSECREATEREQUEST"]._serialized_end = 364
-    _globals["_WAREHOUSECREATERESPONSE"]._serialized_start = 367
-    _globals["_WAREHOUSECREATERESPONSE"]._serialized_end = 534
-    _globals["_WAREHOUSEREADREQUEST"]._serialized_start = 537
-    _globals["_WAREHOUSEREADREQUEST"]._serialized_end = 907
-    _globals["_WAREHOUSEREADRESPONSE"]._serialized_start = 910
-    _globals["_WAREHOUSEREADRESPONSE"]._serialized_end = 1135
-    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_start = 1138
-    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_end = 1285
-    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_start = 1288
-    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_end = 1455
-    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_start = 1457
-    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_end = 1549
-    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_start = 1551
-    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_end = 1651
-    _globals["_WAREHOUSESERVICE"]._serialized_start = 1654
-    _globals["_WAREHOUSESERVICE"]._serialized_end = 2246
+    _globals["_WAREHOUSE"]._serialized_start = 117
+    _globals["_WAREHOUSE"]._serialized_end = 303
+    _globals["_WAREHOUSECREATEREQUEST"]._serialized_start = 306
+    _globals["_WAREHOUSECREATEREQUEST"]._serialized_end = 440
+    _globals["_WAREHOUSECREATERESPONSE"]._serialized_start = 443
+    _globals["_WAREHOUSECREATERESPONSE"]._serialized_end = 610
+    _globals["_WAREHOUSEREADREQUEST"]._serialized_start = 613
+    _globals["_WAREHOUSEREADREQUEST"]._serialized_end = 983
+    _globals["_WAREHOUSEREADRESPONSE"]._serialized_start = 986
+    _globals["_WAREHOUSEREADRESPONSE"]._serialized_end = 1211
+    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_start = 1214
+    _globals["_WAREHOUSEUPDATEREQUEST"]._serialized_end = 1361
+    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_start = 1364
+    _globals["_WAREHOUSEUPDATERESPONSE"]._serialized_end = 1531
+    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_start = 1533
+    _globals["_WAREHOUSEDELETEREQUEST"]._serialized_end = 1625
+    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_start = 1627
+    _globals["_WAREHOUSEDELETERESPONSE"]._serialized_end = 1727
+    _globals["_WAREHOUSESERVICE"]._serialized_start = 1730
+    _globals["_WAREHOUSESERVICE"]._serialized_end = 2322
 # @@protoc_insertion_point(module_scope)
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/warehouse_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/warehouse_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,41 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Warehouse(_message.Message):
-    __slots__ = ["id", "name", "code", "warehouse_sql_id", "object_audit"]
+    __slots__ = ["id", "name", "code", "warehouse_sql_id", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
     WAREHOUSE_SQL_ID_FIELD_NUMBER: _ClassVar[int]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
     name: str
     code: str
     warehouse_sql_id: int
+    active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
         warehouse_sql_id: _Optional[int] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
 class WarehouseCreateRequest(_message.Message):
     __slots__ = ["name", "code", "warehouse_sql_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/attachment_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/attachment_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/attachment_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/carrier_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/carrier_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/carrier_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/uom_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,70 +2,87 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Carrier(_message.Message):
-    __slots__ = ["id", "name", "code", "active", "object_audit"]
+class Uom(_message.Message):
+    __slots__ = ["id", "category", "code", "name", "type", "rounding", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+    CATEGORY_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
-    name: str
+    id: str
+    category: str
     code: str
+    name: str
+    type: str
+    rounding: float
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
-        name: _Optional[str] = ...,
+        id: _Optional[str] = ...,
+        category: _Optional[str] = ...,
         code: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        type: _Optional[str] = ...,
+        rounding: _Optional[float] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class CarrierCreateRequest(_message.Message):
-    __slots__ = ["name", "code", "context"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+class UomCreateRequest(_message.Message):
+    __slots__ = ["category", "code", "name", "type", "rounding", "context"]
+    CATEGORY_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    ROUNDING_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    name: str
+    category: str
     code: str
+    name: str
+    type: str
+    rounding: float
     context: _base_pb2.Context
     def __init__(
         self,
-        name: _Optional[str] = ...,
+        category: _Optional[str] = ...,
         code: _Optional[str] = ...,
+        name: _Optional[str] = ...,
+        type: _Optional[str] = ...,
+        rounding: _Optional[float] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class CarrierCreateResponse(_message.Message):
-    __slots__ = ["response_standard", "carrier"]
+class UomCreateResponse(_message.Message):
+    __slots__ = ["response_standard", "uom"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    CARRIER_FIELD_NUMBER: _ClassVar[int]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    carrier: Carrier
+    uom: Uom
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
+        uom: _Optional[_Union[Uom, _Mapping]] = ...,
     ) -> None: ...
 
-class CarrierReadRequest(_message.Message):
+class UomReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -84,61 +101,59 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class CarrierReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "carriers"]
+class UomReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "uoms"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    CARRIERS_FIELD_NUMBER: _ClassVar[int]
+    UOMS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    carriers: _containers.RepeatedCompositeFieldContainer[Carrier]
+    uoms: _containers.RepeatedCompositeFieldContainer[Uom]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        carriers: _Optional[_Iterable[_Union[Carrier, _Mapping]]] = ...,
+        uoms: _Optional[_Iterable[_Union[Uom, _Mapping]]] = ...,
     ) -> None: ...
 
-class CarrierUpdateRequest(_message.Message):
-    __slots__ = ["carrier", "context"]
-    CARRIER_FIELD_NUMBER: _ClassVar[int]
+class UomUpdateRequest(_message.Message):
+    __slots__ = ["uom", "context"]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    carrier: Carrier
+    uom: Uom
     context: _base_pb2.Context
     def __init__(
-        self,
-        carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
-        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
+        self, uom: _Optional[_Union[Uom, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class CarrierUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "carrier"]
+class UomUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "uom"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    CARRIER_FIELD_NUMBER: _ClassVar[int]
+    UOM_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    carrier: Carrier
+    uom: Uom
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        carrier: _Optional[_Union[Carrier, _Mapping]] = ...,
+        uom: _Optional[_Union[Uom, _Mapping]] = ...,
     ) -> None: ...
 
-class CarrierDeleteRequest(_message.Message):
+class UomDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class CarrierDeleteResponse(_message.Message):
+class UomDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/carrier_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/carrier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/country_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/country_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/country_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/location_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/location_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/location_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/model_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,177 +2,145 @@
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Location(_message.Message):
-    __slots__ = [
-        "id",
-        "name",
-        "parent_id",
-        "code",
-        "type_location",
-        "barcode",
-        "warehouse_id",
-        "active",
-        "object_audit",
-    ]
+class Model(_message.Message):
+    __slots__ = ["id", "name", "model", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    PARENT_ID_FIELD_NUMBER: _ClassVar[int]
-    CODE_FIELD_NUMBER: _ClassVar[int]
-    TYPE_LOCATION_FIELD_NUMBER: _ClassVar[int]
-    BARCODE_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
+    MODEL_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     name: str
-    parent_id: int
-    code: str
-    type_location: str
-    barcode: str
-    warehouse_id: int
+    model: str
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         name: _Optional[str] = ...,
-        parent_id: _Optional[int] = ...,
-        code: _Optional[str] = ...,
-        type_location: _Optional[str] = ...,
-        barcode: _Optional[str] = ...,
-        warehouse_id: _Optional[int] = ...,
+        model: _Optional[str] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class LocationCreateRequest(_message.Message):
-    __slots__ = ["name", "parent_id", "code", "type_location", "barcode", "warehouse_id", "context"]
+class ModelCreateRequest(_message.Message):
+    __slots__ = ["name", "model", "active", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    PARENT_ID_FIELD_NUMBER: _ClassVar[int]
-    CODE_FIELD_NUMBER: _ClassVar[int]
-    TYPE_LOCATION_FIELD_NUMBER: _ClassVar[int]
-    BARCODE_FIELD_NUMBER: _ClassVar[int]
-    WAREHOUSE_ID_FIELD_NUMBER: _ClassVar[int]
+    MODEL_FIELD_NUMBER: _ClassVar[int]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
-    parent_id: int
-    code: str
-    type_location: str
-    barcode: str
-    warehouse_id: int
+    model: str
+    active: _wrappers_pb2.BoolValue
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
-        parent_id: _Optional[int] = ...,
-        code: _Optional[str] = ...,
-        type_location: _Optional[str] = ...,
-        barcode: _Optional[str] = ...,
-        warehouse_id: _Optional[int] = ...,
+        model: _Optional[str] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class LocationCreateResponse(_message.Message):
-    __slots__ = ["response_standard", "location"]
+class ModelCreateResponse(_message.Message):
+    __slots__ = ["response_standard", "model"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_FIELD_NUMBER: _ClassVar[int]
+    MODEL_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    location: Location
+    model: Model
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        location: _Optional[_Union[Location, _Mapping]] = ...,
+        model: _Optional[_Union[Model, _Mapping]] = ...,
     ) -> None: ...
 
-class LocationReadRequest(_message.Message):
+class ModelReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[int] = ...,
+        id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class LocationReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "locations"]
+class ModelReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "models"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    LOCATIONS_FIELD_NUMBER: _ClassVar[int]
+    MODELS_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    locations: _containers.RepeatedCompositeFieldContainer[Location]
+    models: _containers.RepeatedCompositeFieldContainer[Model]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        locations: _Optional[_Iterable[_Union[Location, _Mapping]]] = ...,
+        models: _Optional[_Iterable[_Union[Model, _Mapping]]] = ...,
     ) -> None: ...
 
-class LocationUpdateRequest(_message.Message):
-    __slots__ = ["location", "context"]
-    LOCATION_FIELD_NUMBER: _ClassVar[int]
+class ModelUpdateRequest(_message.Message):
+    __slots__ = ["model", "context"]
+    MODEL_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    location: Location
+    model: Model
     context: _base_pb2.Context
     def __init__(
         self,
-        location: _Optional[_Union[Location, _Mapping]] = ...,
+        model: _Optional[_Union[Model, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class LocationUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "location"]
+class ModelUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "model"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_FIELD_NUMBER: _ClassVar[int]
+    MODEL_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    location: Location
+    model: Model
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        location: _Optional[_Union[Location, _Mapping]] = ...,
+        model: _Optional[_Union[Model, _Mapping]] = ...,
     ) -> None: ...
 
-class LocationDeleteRequest(_message.Message):
+class ModelDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: int
+    id: str
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class LocationDeleteResponse(_message.Message):
+class ModelDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/location_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/location_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_type_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_type_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_type_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/picking_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/procurement_group_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/procurement_group_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/procurement_group_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/procurement_group_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/procurement_group_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/product_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/product_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/product_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/product_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/product_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/quant_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/quant_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/quant_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/quant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/quant_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/quant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/route_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/route_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/route_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/route_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/route_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/route_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/rule_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/rule_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/rule_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/rule_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/rule_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/rule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/sequence_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/sequence_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/sequence_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/sequence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/sequence_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/sequence_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_line_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/uom_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/uom_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/uom_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/product_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -8,69 +8,69 @@
 from google.protobuf import message as _message
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Uom(_message.Message):
-    __slots__ = ["id", "uom_doc_id", "code", "name", "active", "object_audit"]
+class Product(_message.Message):
+    __slots__ = ["id", "product_doc_id", "template_doc_id", "name", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    UOM_DOC_ID_FIELD_NUMBER: _ClassVar[int]
-    CODE_FIELD_NUMBER: _ClassVar[int]
+    PRODUCT_DOC_ID_FIELD_NUMBER: _ClassVar[int]
+    TEMPLATE_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: int
-    uom_doc_id: str
-    code: str
+    product_doc_id: str
+    template_doc_id: str
     name: str
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[int] = ...,
-        uom_doc_id: _Optional[str] = ...,
-        code: _Optional[str] = ...,
+        product_doc_id: _Optional[str] = ...,
+        template_doc_id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class UomCreateRequest(_message.Message):
-    __slots__ = ["uom_doc_id", "code", "name", "context"]
-    UOM_DOC_ID_FIELD_NUMBER: _ClassVar[int]
-    CODE_FIELD_NUMBER: _ClassVar[int]
+class ProductCreateRequest(_message.Message):
+    __slots__ = ["product_doc_id", "template_doc_id", "name", "context"]
+    PRODUCT_DOC_ID_FIELD_NUMBER: _ClassVar[int]
+    TEMPLATE_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    uom_doc_id: str
-    code: str
+    product_doc_id: str
+    template_doc_id: str
     name: str
     context: _base_pb2.Context
     def __init__(
         self,
-        uom_doc_id: _Optional[str] = ...,
-        code: _Optional[str] = ...,
+        product_doc_id: _Optional[str] = ...,
+        template_doc_id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class UomCreateResponse(_message.Message):
-    __slots__ = ["response", "uom"]
-    RESPONSE_FIELD_NUMBER: _ClassVar[int]
-    UOM_FIELD_NUMBER: _ClassVar[int]
-    response: _base_pb2.ResponseStandard
-    uom: Uom
+class ProductCreateResponse(_message.Message):
+    __slots__ = ["product", "response_standard"]
+    PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    product: Product
+    response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        response: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        uom: _Optional[_Union[Uom, _Mapping]] = ...,
+        product: _Optional[_Union[Product, _Mapping]] = ...,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class UomReadRequest(_message.Message):
+class ProductReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -89,59 +89,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class UomReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "uoms"]
+class ProductReadResponse(_message.Message):
+    __slots__ = ["products", "response_standard", "meta_data"]
+    PRODUCTS_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    UOMS_FIELD_NUMBER: _ClassVar[int]
+    products: _containers.RepeatedCompositeFieldContainer[Product]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    uoms: _containers.RepeatedCompositeFieldContainer[Uom]
     def __init__(
         self,
+        products: _Optional[_Iterable[_Union[Product, _Mapping]]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        uoms: _Optional[_Iterable[_Union[Uom, _Mapping]]] = ...,
     ) -> None: ...
 
-class UomUpdateRequest(_message.Message):
-    __slots__ = ["uom", "context"]
-    UOM_FIELD_NUMBER: _ClassVar[int]
+class ProductUpdateRequest(_message.Message):
+    __slots__ = ["product", "context"]
+    PRODUCT_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    uom: Uom
+    product: Product
     context: _base_pb2.Context
     def __init__(
-        self, uom: _Optional[_Union[Uom, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self,
+        product: _Optional[_Union[Product, _Mapping]] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class UomUpdateResponse(_message.Message):
-    __slots__ = ["response", "uom"]
-    RESPONSE_FIELD_NUMBER: _ClassVar[int]
-    UOM_FIELD_NUMBER: _ClassVar[int]
-    response: _base_pb2.ResponseStandard
-    uom: Uom
+class ProductUpdateResponse(_message.Message):
+    __slots__ = ["product", "response_standard"]
+    PRODUCT_FIELD_NUMBER: _ClassVar[int]
+    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    product: Product
+    response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        response: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        uom: _Optional[_Union[Uom, _Mapping]] = ...,
+        product: _Optional[_Union[Product, _Mapping]] = ...,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class UomDeleteRequest(_message.Message):
+class ProductDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class UomDeleteResponse(_message.Message):
-    __slots__ = ["response"]
-    RESPONSE_FIELD_NUMBER: _ClassVar[int]
-    response: _base_pb2.ResponseStandard
-    def __init__(self, response: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
+class ProductDeleteResponse(_message.Message):
+    __slots__ = ["response_standard"]
+    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    response_standard: _base_pb2.ResponseStandard
+    def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/uom_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/uom_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/user_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/user_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/user_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,23 +45,23 @@
         self,
         user_doc_id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class UserCreateResponse(_message.Message):
-    __slots__ = ["response_standard", "user"]
-    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["user", "response_standard"]
     USER_FIELD_NUMBER: _ClassVar[int]
-    response_standard: _base_pb2.ResponseStandard
+    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     user: User
+    response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         user: _Optional[_Union[User, _Mapping]] = ...,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
 class UserReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
@@ -84,26 +84,26 @@
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class UserReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "users"]
+    __slots__ = ["user", "response_standard", "meta_data"]
+    USER_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    USERS_FIELD_NUMBER: _ClassVar[int]
+    user: _containers.RepeatedCompositeFieldContainer[User]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    users: _containers.RepeatedCompositeFieldContainer[User]
     def __init__(
         self,
+        user: _Optional[_Iterable[_Union[User, _Mapping]]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        users: _Optional[_Iterable[_Union[User, _Mapping]]] = ...,
     ) -> None: ...
 
 class UserUpdateRequest(_message.Message):
     __slots__ = ["user", "context"]
     USER_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     user: User
@@ -111,23 +111,23 @@
     def __init__(
         self,
         user: _Optional[_Union[User, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
 class UserUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "user"]
-    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["user", "response_standard"]
     USER_FIELD_NUMBER: _ClassVar[int]
-    response_standard: _base_pb2.ResponseStandard
+    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     user: User
+    response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         user: _Optional[_Union[User, _Mapping]] = ...,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
 class UserDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: int
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/user_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/warehouse_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/warehouse_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/stock/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/users/user_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/users/user_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/users/user_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/users/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/country_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/country_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/country_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/currency_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/currency_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/currency_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/currency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/currency_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/currency_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/document_type_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/document_type_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/document_type_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/document_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/language_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/language_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/language_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/language_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/language_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/language_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/model_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/model_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/model_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/sales/payment_method_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -8,139 +8,142 @@
 from google.protobuf import message as _message
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Model(_message.Message):
-    __slots__ = ["id", "name", "model", "active", "object_audit"]
+class PaymentMethod(_message.Message):
+    __slots__ = ["id", "name", "code", "payment_method_doc_id", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    MODEL_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    PAYMENT_METHOD_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
-    id: str
+    id: int
     name: str
-    model: str
+    code: str
+    payment_method_doc_id: str
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
-        id: _Optional[str] = ...,
+        id: _Optional[int] = ...,
         name: _Optional[str] = ...,
-        model: _Optional[str] = ...,
+        code: _Optional[str] = ...,
+        payment_method_doc_id: _Optional[str] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelCreateRequest(_message.Message):
-    __slots__ = ["name", "model", "active", "context"]
+class PaymentMethodCreateRequest(_message.Message):
+    __slots__ = ["name", "code", "payment_method_doc_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    MODEL_FIELD_NUMBER: _ClassVar[int]
-    ACTIVE_FIELD_NUMBER: _ClassVar[int]
+    CODE_FIELD_NUMBER: _ClassVar[int]
+    PAYMENT_METHOD_DOC_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
-    model: str
-    active: _wrappers_pb2.BoolValue
+    code: str
+    payment_method_doc_id: str
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
-        model: _Optional[str] = ...,
-        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
+        code: _Optional[str] = ...,
+        payment_method_doc_id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelCreateResponse(_message.Message):
-    __slots__ = ["response_standard", "model"]
+class PaymentMethodCreateResponse(_message.Message):
+    __slots__ = ["payment_method", "response_standard"]
+    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    MODEL_FIELD_NUMBER: _ClassVar[int]
+    payment_method: PaymentMethod
     response_standard: _base_pb2.ResponseStandard
-    model: Model
     def __init__(
         self,
+        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        model: _Optional[_Union[Model, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelReadRequest(_message.Message):
+class PaymentMethodReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     group_by: _containers.RepeatedCompositeFieldContainer[_base_pb2.GroupBy]
     sort_by: _base_pb2.SortBy
     fields: _base_pb2.Fields
     filter: _base_pb2.Filter
     paginated: _base_pb2.Paginated
-    id: str
+    id: int
     context: _base_pb2.Context
     def __init__(
         self,
         group_by: _Optional[_Iterable[_Union[_base_pb2.GroupBy, _Mapping]]] = ...,
         sort_by: _Optional[_Union[_base_pb2.SortBy, _Mapping]] = ...,
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
-        id: _Optional[str] = ...,
+        id: _Optional[int] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "models"]
+class PaymentMethodReadResponse(_message.Message):
+    __slots__ = ["payment_methods", "response_standard", "meta_data"]
+    PAYMENT_METHODS_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    MODELS_FIELD_NUMBER: _ClassVar[int]
+    payment_methods: _containers.RepeatedCompositeFieldContainer[PaymentMethod]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    models: _containers.RepeatedCompositeFieldContainer[Model]
     def __init__(
         self,
+        payment_methods: _Optional[_Iterable[_Union[PaymentMethod, _Mapping]]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        models: _Optional[_Iterable[_Union[Model, _Mapping]]] = ...,
     ) -> None: ...
 
-class ModelUpdateRequest(_message.Message):
-    __slots__ = ["model", "context"]
-    MODEL_FIELD_NUMBER: _ClassVar[int]
+class PaymentMethodUpdateRequest(_message.Message):
+    __slots__ = ["payment_method", "context"]
+    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    model: Model
+    payment_method: PaymentMethod
     context: _base_pb2.Context
     def __init__(
         self,
-        model: _Optional[_Union[Model, _Mapping]] = ...,
+        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "model"]
+class PaymentMethodUpdateResponse(_message.Message):
+    __slots__ = ["payment_method", "response_standard"]
+    PAYMENT_METHOD_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    MODEL_FIELD_NUMBER: _ClassVar[int]
+    payment_method: PaymentMethod
     response_standard: _base_pb2.ResponseStandard
-    model: Model
     def __init__(
         self,
+        payment_method: _Optional[_Union[PaymentMethod, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        model: _Optional[_Union[Model, _Mapping]] = ...,
     ) -> None: ...
 
-class ModelDeleteRequest(_message.Message):
+class PaymentMethodDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    id: str
+    id: int
     context: _base_pb2.Context
     def __init__(
-        self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self, id: _Optional[int] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class ModelDeleteResponse(_message.Message):
+class PaymentMethodDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/model_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/payment_method_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/payment_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/payment_method_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/payment_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/sequence_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/sequence_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/sequence_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/sequence_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/sequence_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/sequence_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/tax_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/tax_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/tax_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/timezone_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -8,87 +8,78 @@
 from google.protobuf import message as _message
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Tax(_message.Message):
-    __slots__ = ["id", "name", "code", "rate", "rounding", "decimal_places", "position", "active", "object_audit"]
+class Timezone(_message.Message):
+    __slots__ = ["id", "name", "code", "offset", "offset_dst", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    RATE_FIELD_NUMBER: _ClassVar[int]
-    ROUNDING_FIELD_NUMBER: _ClassVar[int]
-    DECIMAL_PLACES_FIELD_NUMBER: _ClassVar[int]
-    POSITION_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_DST_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     code: str
-    rate: float
-    rounding: float
-    decimal_places: int
-    position: str
+    offset: int
+    offset_dst: int
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        rate: _Optional[float] = ...,
-        rounding: _Optional[float] = ...,
-        decimal_places: _Optional[int] = ...,
-        position: _Optional[str] = ...,
+        offset: _Optional[int] = ...,
+        offset_dst: _Optional[int] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxAddRequest(_message.Message):
-    __slots__ = ["name", "code", "rate", "rounding", "decimal_places", "position", "context"]
+class TimezoneAddRequest(_message.Message):
+    __slots__ = ["name", "code", "offset", "offset_dst", "active", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    RATE_FIELD_NUMBER: _ClassVar[int]
-    ROUNDING_FIELD_NUMBER: _ClassVar[int]
-    DECIMAL_PLACES_FIELD_NUMBER: _ClassVar[int]
-    POSITION_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_FIELD_NUMBER: _ClassVar[int]
+    OFFSET_DST_FIELD_NUMBER: _ClassVar[int]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     code: str
-    rate: float
-    rounding: float
-    decimal_places: int
-    position: str
+    offset: int
+    offset_dst: int
+    active: _wrappers_pb2.BoolValue
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        rate: _Optional[float] = ...,
-        rounding: _Optional[float] = ...,
-        decimal_places: _Optional[int] = ...,
-        position: _Optional[str] = ...,
+        offset: _Optional[int] = ...,
+        offset_dst: _Optional[int] = ...,
+        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxAddResponse(_message.Message):
-    __slots__ = ["response_standard", "tax"]
+class TimezoneAddResponse(_message.Message):
+    __slots__ = ["response_standard", "timezone"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    TAX_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    tax: Tax
+    timezone: Timezone
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        tax: _Optional[_Union[Tax, _Mapping]] = ...,
+        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxReadRequest(_message.Message):
+class TimezoneReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -107,59 +98,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "taxes"]
+class TimezoneReadResponse(_message.Message):
+    __slots__ = ["response_standard", "meta_data", "timezones"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    TAXES_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONES_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     meta_data: _base_pb2.MetaData
-    taxes: _containers.RepeatedCompositeFieldContainer[Tax]
+    timezones: _containers.RepeatedCompositeFieldContainer[Timezone]
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        taxes: _Optional[_Iterable[_Union[Tax, _Mapping]]] = ...,
+        timezones: _Optional[_Iterable[_Union[Timezone, _Mapping]]] = ...,
     ) -> None: ...
 
-class TaxUpdateRequest(_message.Message):
-    __slots__ = ["tax", "context"]
-    TAX_FIELD_NUMBER: _ClassVar[int]
+class TimezoneUpdateRequest(_message.Message):
+    __slots__ = ["timezone", "context"]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    tax: Tax
+    timezone: Timezone
     context: _base_pb2.Context
     def __init__(
-        self, tax: _Optional[_Union[Tax, _Mapping]] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
+        self,
+        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
+        context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "tax"]
+class TimezoneUpdateResponse(_message.Message):
+    __slots__ = ["response_standard", "timezone"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    TAX_FIELD_NUMBER: _ClassVar[int]
+    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
-    tax: Tax
+    timezone: Timezone
     def __init__(
         self,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        tax: _Optional[_Union[Tax, _Mapping]] = ...,
+        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
     ) -> None: ...
 
-class TaxDeleteRequest(_message.Message):
+class TimezoneDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class TaxDeleteResponse(_message.Message):
+class TimezoneDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/tax_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/tax_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/timezone_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/timezone_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/timezone_pb2.pyi` & `omni-pro-0.1.34/omni/pro/protos/v1/rules/location_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -8,78 +8,69 @@
 from google.protobuf import message as _message
 from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from omni.pro.protos.common import base_pb2 as _base_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Timezone(_message.Message):
-    __slots__ = ["id", "name", "code", "offset", "offset_dst", "active", "object_audit"]
+class Location(_message.Message):
+    __slots__ = ["id", "name", "code", "location_sql_id", "active", "object_audit"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    OFFSET_FIELD_NUMBER: _ClassVar[int]
-    OFFSET_DST_FIELD_NUMBER: _ClassVar[int]
+    LOCATION_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_AUDIT_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     code: str
-    offset: int
-    offset_dst: int
+    location_sql_id: str
     active: _wrappers_pb2.BoolValue
     object_audit: _base_pb2.ObjectAudit
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        offset: _Optional[int] = ...,
-        offset_dst: _Optional[int] = ...,
+        location_sql_id: _Optional[str] = ...,
         active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
         object_audit: _Optional[_Union[_base_pb2.ObjectAudit, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneAddRequest(_message.Message):
-    __slots__ = ["name", "code", "offset", "offset_dst", "active", "context"]
+class LocationCreateRequest(_message.Message):
+    __slots__ = ["name", "code", "location_sql_id", "context"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
-    OFFSET_FIELD_NUMBER: _ClassVar[int]
-    OFFSET_DST_FIELD_NUMBER: _ClassVar[int]
-    ACTIVE_FIELD_NUMBER: _ClassVar[int]
+    LOCATION_SQL_ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     name: str
     code: str
-    offset: int
-    offset_dst: int
-    active: _wrappers_pb2.BoolValue
+    location_sql_id: str
     context: _base_pb2.Context
     def __init__(
         self,
         name: _Optional[str] = ...,
         code: _Optional[str] = ...,
-        offset: _Optional[int] = ...,
-        offset_dst: _Optional[int] = ...,
-        active: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...,
+        location_sql_id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneAddResponse(_message.Message):
-    __slots__ = ["response_standard", "timezone"]
+class LocationCreateResponse(_message.Message):
+    __slots__ = ["location", "response_standard"]
+    LOCATION_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
+    location: Location
     response_standard: _base_pb2.ResponseStandard
-    timezone: Timezone
     def __init__(
         self,
+        location: _Optional[_Union[Location, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneReadRequest(_message.Message):
+class LocationReadRequest(_message.Message):
     __slots__ = ["group_by", "sort_by", "fields", "filter", "paginated", "id", "context"]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_NUMBER: _ClassVar[int]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     PAGINATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -98,61 +89,61 @@
         fields: _Optional[_Union[_base_pb2.Fields, _Mapping]] = ...,
         filter: _Optional[_Union[_base_pb2.Filter, _Mapping]] = ...,
         paginated: _Optional[_Union[_base_pb2.Paginated, _Mapping]] = ...,
         id: _Optional[str] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneReadResponse(_message.Message):
-    __slots__ = ["response_standard", "meta_data", "timezones"]
-    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+class LocationReadResponse(_message.Message):
+    __slots__ = ["locations", "meta_data", "response_standard"]
+    LOCATIONS_FIELD_NUMBER: _ClassVar[int]
     META_DATA_FIELD_NUMBER: _ClassVar[int]
-    TIMEZONES_FIELD_NUMBER: _ClassVar[int]
-    response_standard: _base_pb2.ResponseStandard
+    RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
+    locations: _containers.RepeatedCompositeFieldContainer[Location]
     meta_data: _base_pb2.MetaData
-    timezones: _containers.RepeatedCompositeFieldContainer[Timezone]
+    response_standard: _base_pb2.ResponseStandard
     def __init__(
         self,
-        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
+        locations: _Optional[_Iterable[_Union[Location, _Mapping]]] = ...,
         meta_data: _Optional[_Union[_base_pb2.MetaData, _Mapping]] = ...,
-        timezones: _Optional[_Iterable[_Union[Timezone, _Mapping]]] = ...,
+        response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneUpdateRequest(_message.Message):
-    __slots__ = ["timezone", "context"]
-    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
+class LocationUpdateRequest(_message.Message):
+    __slots__ = ["location", "context"]
+    LOCATION_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    timezone: Timezone
+    location: Location
     context: _base_pb2.Context
     def __init__(
         self,
-        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
+        location: _Optional[_Union[Location, _Mapping]] = ...,
         context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneUpdateResponse(_message.Message):
-    __slots__ = ["response_standard", "timezone"]
+class LocationUpdateResponse(_message.Message):
+    __slots__ = ["location", "response_standard"]
+    LOCATION_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
-    TIMEZONE_FIELD_NUMBER: _ClassVar[int]
+    location: Location
     response_standard: _base_pb2.ResponseStandard
-    timezone: Timezone
     def __init__(
         self,
+        location: _Optional[_Union[Location, _Mapping]] = ...,
         response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...,
-        timezone: _Optional[_Union[Timezone, _Mapping]] = ...,
     ) -> None: ...
 
-class TimezoneDeleteRequest(_message.Message):
+class LocationDeleteRequest(_message.Message):
     __slots__ = ["id", "context"]
     ID_FIELD_NUMBER: _ClassVar[int]
     CONTEXT_FIELD_NUMBER: _ClassVar[int]
     id: str
     context: _base_pb2.Context
     def __init__(
         self, id: _Optional[str] = ..., context: _Optional[_Union[_base_pb2.Context, _Mapping]] = ...
     ) -> None: ...
 
-class TimezoneDeleteResponse(_message.Message):
+class LocationDeleteResponse(_message.Message):
     __slots__ = ["response_standard"]
     RESPONSE_STANDARD_FIELD_NUMBER: _ClassVar[int]
     response_standard: _base_pb2.ResponseStandard
     def __init__(self, response_standard: _Optional[_Union[_base_pb2.ResponseStandard, _Mapping]] = ...) -> None: ...
```

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/uom_pb2.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/uom_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/protos/v1/utilities/uom_pb2_grpc.py` & `omni-pro-0.1.34/omni/pro/protos/v1/utilities/uom_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/redis.py` & `omni-pro-0.1.34/omni/pro/redis.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/stack.py` & `omni-pro-0.1.34/omni/pro/stack.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/user/access.py` & `omni-pro-0.1.34/omni/pro/user/access.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/util.py` & `omni-pro-0.1.34/omni/pro/util.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni/pro/validators.py` & `omni-pro-0.1.34/omni/pro/validators.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/omni_pro.egg-info/PKG-INFO` & `omni-pro-0.1.34/omni_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-pro
-Version: 0.1.33
+Version: 0.1.34
 Summary: Python library designed to be a utility for OMS microservices
 Home-page: https://github.com/Omnipro-Solutions/saas-ms-library
 Author: OMNI.PRO
 Author-email: development@omni.pro
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `omni-pro-0.1.33/omni_pro.egg-info/SOURCES.txt` & `omni-pro-0.1.34/omni_pro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omni-pro-0.1.33/setup.py` & `omni-pro-0.1.34/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # The directory containing this file
 HERE = Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 DESCRIPTION = "Python library designed to be a utility for OMS microservices"
-VERSION = "0.1.33"
+VERSION = "0.1.34"
 PACKAGE_NAME = "omni-pro"
 AUTHOR = "OMNI.PRO"
 AUTHOR_EMAIL = "development@omni.pro"
 URL = "https://github.com/Omnipro-Solutions/saas-ms-library"
 
 INSTALL_REQUIRES = [
     "protobuf==4.23.4",
```

