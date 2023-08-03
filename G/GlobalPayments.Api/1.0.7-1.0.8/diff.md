# Comparing `tmp/GlobalPayments.Api-1.0.7.tar.gz` & `tmp/GlobalPayments.Api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GlobalPayments.Api-1.0.7.tar", last modified: Tue May  9 13:41:10 2023, max compression
+gzip compressed data, was "GlobalPayments.Api-1.0.8.tar", last modified: Thu Aug  3 14:24:37 2023, max compression
```

## Comparing `GlobalPayments.Api-1.0.7.tar` & `GlobalPayments.Api-1.0.8.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.166307 GlobalPayments.Api-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.836821 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/
--rw-rw-rw-   0        0        0      910 2023-05-09 13:41:09.000000 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2785 2023-05-09 13:41:09.000000 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 13:41:09.000000 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-05-09 13:41:09.000000 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-09 13:41:09.000000 GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15439 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/LICENSE.md
--rw-rw-rw-   0        0        0      910 2023-05-09 13:41:10.165304 GlobalPayments.Api-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      548 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.841580 GlobalPayments.Api-1.0.7/globalpayments/
--rw-rw-rw-   0        0        0       36 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.848567 GlobalPayments.Api-1.0.7/globalpayments/api/
--rw-rw-rw-   0        0        0    10064 2023-05-01 21:16:30.000000 GlobalPayments.Api-1.0.7/globalpayments/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.862867 GlobalPayments.Api-1.0.7/globalpayments/api/builders/
--rw-rw-rw-   0        0        0    13980 2023-05-08 13:15:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/__init__.py
--rw-rw-rw-   0        0        0     2807 2023-04-13 15:30:21.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/management_builder.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.901020 GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/
--rw-rw-rw-   0        0        0      322 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/__init__.py
--rw-rw-rw-   0        0        0     2742 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validation_clause.py
--rw-rw-rw-   0        0        0     1125 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validation_target.py
--rw-rw-rw-   0        0        0     2194 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validations.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:09.979662 GlobalPayments.Api-1.0.7/globalpayments/api/entities/
--rw-rw-rw-   0        0        0    15101 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/__init__.py
--rw-rw-rw-   0        0        0    18729 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/address.py
--rw-rw-rw-   0        0        0      176 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/batch_summary.py
--rw-rw-rw-   0        0        0      244 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/debit_mac.py
--rw-rw-rw-   0        0        0      658 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/ecommerce_info.py
--rw-rw-rw-   0        0        0      601 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/encryption_data.py
--rw-rw-rw-   0        0        0    12813 2023-05-08 13:15:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/enums.py
--rw-rw-rw-   0        0        0     1837 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/exceptions.py
--rw-rw-rw-   0        0        0      300 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/hosted_payment_data.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.004209 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/base_table_service_response.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/bump_status_collection.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/login_response.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/server_assignment_response.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/server_list_response.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/shift_assignments.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:40.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/table_service_response.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/table_service/ticket.py
--rw-rw-rw-   0        0        0      211 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/three_d_secure.py
--rw-rw-rw-   0        0        0      640 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/entities/transaction_summary.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.046097 GlobalPayments.Api-1.0.7/globalpayments/api/gateways/
--rw-rw-rw-   0        0        0   100405 2023-05-09 13:22:20.000000 GlobalPayments.Api-1.0.7/globalpayments/api/gateways/__init__.py
--rw-rw-rw-   0        0        0       81 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/gateways/gateway_response.py
--rw-rw-rw-   0        0        0       48 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/gateways/table_service_connector.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.108936 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/
--rw-rw-rw-   0        0        0      583 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/cash.py
--rw-rw-rw-   0        0        0     8601 2023-05-08 13:15:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/credit.py
--rw-rw-rw-   0        0        0     2256 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/debit.py
--rw-rw-rw-   0        0        0     2202 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/ebt.py
--rw-rw-rw-   0        0        0     1259 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/echeck.py
--rw-rw-rw-   0        0        0     3302 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/giftcard.py
--rw-rw-rw-   0        0        0     1274 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/payment_interfaces.py
--rw-rw-rw-   0        0        0      173 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/transaction_reference.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.155620 GlobalPayments.Api-1.0.7/globalpayments/api/services/
--rw-rw-rw-   0        0        0      220 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/__init__.py
--rw-rw-rw-   0        0        0      354 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/batch_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/credit_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/debit_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/device_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/ebt_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/gift_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/hosted_service.py
--rw-rw-rw-   0        0        0     1127 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/recurring_service.py
--rw-rw-rw-   0        0        0      589 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/reporting_service.py
--rw-rw-rw-   0        0        0        0 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/services/table_service.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:41:10.160301 GlobalPayments.Api-1.0.7/globalpayments/api/utils/
--rw-rw-rw-   0        0        0     6127 2023-04-13 00:13:41.000000 GlobalPayments.Api-1.0.7/globalpayments/api/utils/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-09 13:41:10.167305 GlobalPayments.Api-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1159 2023-05-09 13:22:20.000000 GlobalPayments.Api-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.192634 GlobalPayments.Api-1.0.8/
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.152473 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/
+-rw-rw-rw-   0        0        0      910 2023-08-03 14:24:37.000000 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2785 2023-08-03 14:24:37.000000 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 14:24:37.000000 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-08-03 14:24:37.000000 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-03 14:24:37.000000 GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15439 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0      910 2023-08-03 14:24:37.192634 GlobalPayments.Api-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/README.txt
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.152473 GlobalPayments.Api-1.0.8/globalpayments/
+-rw-rw-rw-   0        0        0       36 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.152473 GlobalPayments.Api-1.0.8/globalpayments/api/
+-rw-rw-rw-   0        0        0    10064 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.152473 GlobalPayments.Api-1.0.8/globalpayments/api/builders/
+-rw-rw-rw-   0        0        0    13980 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/__init__.py
+-rw-rw-rw-   0        0        0     2807 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/management_builder.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.164099 GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/
+-rw-rw-rw-   0        0        0      322 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/__init__.py
+-rw-rw-rw-   0        0        0     2742 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validation_clause.py
+-rw-rw-rw-   0        0        0     1125 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validation_target.py
+-rw-rw-rw-   0        0        0     2194 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validations.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.171340 GlobalPayments.Api-1.0.8/globalpayments/api/entities/
+-rw-rw-rw-   0        0        0    15101 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/__init__.py
+-rw-rw-rw-   0        0        0    18729 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/address.py
+-rw-rw-rw-   0        0        0      176 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/batch_summary.py
+-rw-rw-rw-   0        0        0      244 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/debit_mac.py
+-rw-rw-rw-   0        0        0      658 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/ecommerce_info.py
+-rw-rw-rw-   0        0        0      601 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/encryption_data.py
+-rw-rw-rw-   0        0        0    12813 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/enums.py
+-rw-rw-rw-   0        0        0     1837 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/exceptions.py
+-rw-rw-rw-   0        0        0      300 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/hosted_payment_data.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.177003 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/base_table_service_response.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/bump_status_collection.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/login_response.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/server_assignment_response.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/server_list_response.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/shift_assignments.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/table_service_response.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/table_service/ticket.py
+-rw-rw-rw-   0        0        0      211 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/three_d_secure.py
+-rw-rw-rw-   0        0        0      640 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/entities/transaction_summary.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.177003 GlobalPayments.Api-1.0.8/globalpayments/api/gateways/
+-rw-rw-rw-   0        0        0   100825 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/gateways/__init__.py
+-rw-rw-rw-   0        0        0       81 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/gateways/gateway_response.py
+-rw-rw-rw-   0        0        0       48 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/gateways/table_service_connector.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.177003 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/
+-rw-rw-rw-   0        0        0      583 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/cash.py
+-rw-rw-rw-   0        0        0     8601 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/credit.py
+-rw-rw-rw-   0        0        0     2256 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/debit.py
+-rw-rw-rw-   0        0        0     2202 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/ebt.py
+-rw-rw-rw-   0        0        0     1259 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/echeck.py
+-rw-rw-rw-   0        0        0     3302 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/giftcard.py
+-rw-rw-rw-   0        0        0     1274 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/payment_interfaces.py
+-rw-rw-rw-   0        0        0      173 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/transaction_reference.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.192634 GlobalPayments.Api-1.0.8/globalpayments/api/services/
+-rw-rw-rw-   0        0        0      220 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/batch_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/credit_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/debit_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/device_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/ebt_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/gift_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/hosted_service.py
+-rw-rw-rw-   0        0        0     1127 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/recurring_service.py
+-rw-rw-rw-   0        0        0      589 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/reporting_service.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/services/table_service.py
+drwxrwxrwx   0        0        0        0 2023-08-03 14:24:37.192634 GlobalPayments.Api-1.0.8/globalpayments/api/utils/
+-rw-rw-rw-   0        0        0     6127 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/globalpayments/api/utils/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 14:24:37.192634 GlobalPayments.Api-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1159 2023-08-03 14:24:00.000000 GlobalPayments.Api-1.0.8/setup.py
```

### Comparing `GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/PKG-INFO` & `GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlobalPayments.Api
-Version: 1.0.7
+Version: 1.0.8
 Summary: Global Payments Python SDK for integrating with Heartland and Global Payments merchant services APIs.
 Home-page: https://developer.heartlandpaymentsystems.com/
 Author: Heartland Payment Systems
 Author-email: EntApp_DevPortal@e-hps.com
 License: LICENSE.md
 License-File: LICENSE.md
```

### Comparing `GlobalPayments.Api-1.0.7/GlobalPayments.Api.egg-info/SOURCES.txt` & `GlobalPayments.Api-1.0.8/GlobalPayments.Api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/LICENSE.md` & `GlobalPayments.Api-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/PKG-INFO` & `GlobalPayments.Api-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlobalPayments.Api
-Version: 1.0.7
+Version: 1.0.8
 Summary: Global Payments Python SDK for integrating with Heartland and Global Payments merchant services APIs.
 Home-page: https://developer.heartlandpaymentsystems.com/
 Author: Heartland Payment Systems
 Author-email: EntApp_DevPortal@e-hps.com
 License: LICENSE.md
 License-File: LICENSE.md
```

### Comparing `GlobalPayments.Api-1.0.7/README.txt` & `GlobalPayments.Api-1.0.8/README.txt`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/__init__.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/builders/__init__.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/builders/management_builder.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/builders/management_builder.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validation_clause.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validation_clause.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validation_target.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validation_target.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/builders/validations/validations.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/builders/validations/validations.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/entities/__init__.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/entities/address.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/entities/address.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/entities/ecommerce_info.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/entities/ecommerce_info.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/entities/encryption_data.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/entities/encryption_data.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/entities/enums.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/entities/enums.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/entities/exceptions.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/entities/transaction_summary.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/entities/transaction_summary.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/gateways/__init__.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/gateways/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import re
 import certifi
 import jsonpickle
 import urllib3.contrib.pyopenssl
 import xmltodict
 import globalpayments as gp
 import datetime
+import pkg_resources
 from globalpayments.api.entities import (
     Address, BatchSummary, Customer, DebitMac, RecurringPaymentMethod,
     Schedule, ThreeDSecure, Transaction, TransactionSummary)
 from globalpayments.api.entities.enums import (
     AccountType, AddressType, AliasAction, CheckType, EmvChipCondition,
     EntryMethod, FraudFilterMode, HppVersion, PaymentMethodType,
     PaymentSchedule, ReportType, SecCode, TransactionType, TransactionModifier)
@@ -589,14 +590,15 @@
     license_id = None
     device_id = None
     username = None
     password = None
     secret_api_key = None
     developer_id = None
     version_number = None
+    sdkNameVersion = None
 
     @property
     def supports_hosted_payments(self):
         return False
 
     def __init__(self):
         XmlGateway.__init__(self)
@@ -1141,14 +1143,18 @@
             et.SubElement(header, 'Password').text = self.password
         if self.developer_id is not None:
             et.SubElement(header, 'DeveloperID').text = str(self.developer_id)
         if self.version_number is not None:
             et.SubElement(header, 'VersionNbr').text = str(self.version_number)
         if client_transaction_id is not None:
             et.SubElement(header, 'ClientTxnId').text = str(client_transaction_id)
+        if self.sdkNameVersion is not None:
+            et.SubElement(header, 'SDKNameVersion').text = str(self.sdkNameVersion)
+        else:
+            et.SubElement(header, 'SDKNameVersion').text = str('python;version=')+str(self._get_release_version())
 
         trans = et.SubElement(version1, 'Transaction')
         trans.append(transaction)
 
         return et.tostring(envelope)
 
     def _map_response(self, raw_response, payment_method):
@@ -1555,14 +1561,17 @@
             return False
 
         try:
             return getattr(obj, attr)
         except AttributeError as _exc:
             return False
 
+    def _get_release_version(self):
+        return pkg_resources.require("GlobalPayments.Api")[0].version
+
 
 class RealexConnector(XmlGateway):
     merchant_id = None
     account_id = None
     shared_secret = None
     channel = None
     rebate_password = None
```

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/__init__.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/credit.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/credit.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/debit.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/debit.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/ebt.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/ebt.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/echeck.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/echeck.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/giftcard.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/giftcard.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/payment_methods/payment_interfaces.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/payment_methods/payment_interfaces.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/services/recurring_service.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/services/recurring_service.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/services/reporting_service.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/services/reporting_service.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/globalpayments/api/utils/__init__.py` & `GlobalPayments.Api-1.0.8/globalpayments/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GlobalPayments.Api-1.0.7/setup.py` & `GlobalPayments.Api-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='GlobalPayments.Api',
-    version='1.0.7',
+    version='1.0.8',
     author='Heartland Payment Systems',
     author_email='EntApp_DevPortal@e-hps.com',
     packages=[
         'globalpayments', 'globalpayments.api', 'globalpayments.api.builders',
         'globalpayments.api.builders.validations',
         'globalpayments.api.entities',
         'globalpayments.api.entities.table_service',
```

