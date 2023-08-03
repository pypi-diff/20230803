# Comparing `tmp/modular_sdk-2.1.4.tar.gz` & `tmp/modular_sdk-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/onsha/Develop/EPAM/temp-modular-sdk/dist/.tmp-lau1mgvn/modular_sdk-2.1.4.tar", last modified: Fri Jun 30 09:15:25 2023, max compression
+gzip compressed data, was "/Users/onsha/Develop/EPAM/temp-modular-sdk/dist/.tmp-ft0tlbgk/modular_sdk-2.2.0.tar", last modified: Thu Aug  3 12:12:20 2023, max compression
```

## Comparing `modular_sdk-2.1.4.tar` & `modular_sdk-2.2.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.042288 modular_sdk-2.1.4/
--rw-r--r--   0 onsha      (501) staff       (20)    11357 2023-06-29 14:09:33.000000 modular_sdk-2.1.4/LICENSE
--rw-r--r--   0 onsha      (501) staff       (20)     4014 2023-06-30 09:15:25.042433 modular_sdk-2.1.4/PKG-INFO
--rw-r--r--   0 onsha      (501) staff       (20)     3507 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/README.md
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.000300 modular_sdk-2.1.4/modular_sdk/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/__init__.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.006476 modular_sdk-2.1.4/modular_sdk/commons/
--rw-r--r--   0 onsha      (501) staff       (20)     4869 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     4865 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/constants.py
--rw-r--r--   0 onsha      (501) staff       (20)     2045 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/error_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)      200 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/exception.py
--rw-r--r--   0 onsha      (501) staff       (20)      800 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/helpers.py
--rw-r--r--   0 onsha      (501) staff       (20)     2642 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/log_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)      951 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/time_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)     2458 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/commons/trace_helper.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.007818 modular_sdk-2.1.4/modular_sdk/connections/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/connections/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1754 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/connections/mongodb_connection.py
--rw-r--r--   0 onsha      (501) staff       (20)     4723 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/connections/rabbit_connection.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.008967 modular_sdk-2.1.4/modular_sdk/helpers/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/helpers/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)      985 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/helpers/response_helper.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.017760 modular_sdk-2.1.4/modular_sdk/models/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1579 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/application.py
--rw-r--r--   0 onsha      (501) staff       (20)      929 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/base_meta.py
--rw-r--r--   0 onsha      (501) staff       (20)      689 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/customer.py
--rw-r--r--   0 onsha      (501) staff       (20)     1050 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/execution_trace.py
--rw-r--r--   0 onsha      (501) staff       (20)      490 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/heartbeat.py
--rw-r--r--   0 onsha      (501) staff       (20)      712 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/job.py
--rw-r--r--   0 onsha      (501) staff       (20)      662 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/operation_mode.py
--rw-r--r--   0 onsha      (501) staff       (20)     1570 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/parent.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.022548 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)    22311 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_model.py
--rw-r--r--   0 onsha      (501) staff       (20)     2261 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_role_access_model.py
--rw-r--r--   0 onsha      (501) staff       (20)     7045 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_safe_update_model.py
--rw-r--r--   0 onsha      (501) staff       (20)    16520 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py
--rw-r--r--   0 onsha      (501) staff       (20)      811 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py
--rw-r--r--   0 onsha      (501) staff       (20)     2565 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/region.py
--rw-r--r--   0 onsha      (501) staff       (20)      476 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/setting.py
--rw-r--r--   0 onsha      (501) staff       (20)     4048 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/tenant.py
--rw-r--r--   0 onsha      (501) staff       (20)     1081 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/models/tenant_settings.py
--rw-r--r--   0 onsha      (501) staff       (20)    10963 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/modular.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.033396 modular_sdk-2.1.4/modular_sdk/services/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     4860 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/application_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     4559 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/aws_creds_provider.py
--rw-r--r--   0 onsha      (501) staff       (20)      803 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/customer_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     5073 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/environment_service.py
--rw-r--r--   0 onsha      (501) staff       (20)      618 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/events_service.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.035000 modular_sdk-2.1.4/modular_sdk/services/impl/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/impl/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)    25123 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/impl/maestro_credentials_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     9096 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/impl/maestro_rabbit_transport_service.py
--rw-r--r--   0 onsha      (501) staff       (20)      620 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/lambda_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     5862 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/parent_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     3751 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/rabbit_transport_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     2602 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/region_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     9806 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/settings_management_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     1488 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/sqs_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     7305 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/ssm_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     8390 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/sts_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     7165 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/tenant_service.py
--rw-r--r--   0 onsha      (501) staff       (20)     2143 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/services/tenant_settings_service.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.035638 modular_sdk-2.1.4/modular_sdk/utils/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/__init__.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.036775 modular_sdk-2.1.4/modular_sdk/utils/job_tracer/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/job_tracer/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)      354 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/job_tracer/abstract.py
--rw-r--r--   0 onsha      (501) staff       (20)     3832 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/job_tracer/generic.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.038279 modular_sdk-2.1.4/modular_sdk/utils/operation_mode/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/operation_mode/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)      776 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/operation_mode/abstract.py
--rw-r--r--   0 onsha      (501) staff       (20)     2171 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/operation_mode/generic.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.039420 modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1061 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/abstract.py
--rw-r--r--   0 onsha      (501) staff       (20)     4091 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/generic.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.002252 modular_sdk-2.1.4/modular_sdk.egg-info/
--rw-r--r--   0 onsha      (501) staff       (20)     4014 2023-06-30 09:15:24.000000 modular_sdk-2.1.4/modular_sdk.egg-info/PKG-INFO
--rw-r--r--   0 onsha      (501) staff       (20)     2945 2023-06-30 09:15:24.000000 modular_sdk-2.1.4/modular_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 onsha      (501) staff       (20)        1 2023-06-30 09:15:24.000000 modular_sdk-2.1.4/modular_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 onsha      (501) staff       (20)      271 2023-06-30 09:15:24.000000 modular_sdk-2.1.4/modular_sdk.egg-info/requires.txt
--rw-r--r--   0 onsha      (501) staff       (20)       18 2023-06-30 09:15:24.000000 modular_sdk-2.1.4/modular_sdk.egg-info/top_level.txt
--rw-r--r--   0 onsha      (501) staff       (20)       86 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/pyproject.toml
--rw-r--r--   0 onsha      (501) staff       (20)      923 2023-06-30 09:15:25.043102 modular_sdk-2.1.4/setup.cfg
--rw-r--r--   0 onsha      (501) staff       (20)       38 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/setup.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.039976 modular_sdk-2.1.4/tests/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/__init__.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.041232 modular_sdk-2.1.4/tests/test_commons/
--rw-r--r--   0 onsha      (501) staff       (20)      119 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/test_commons/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)     1852 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/test_commons/import_helper.py
--rw-r--r--   0 onsha      (501) staff       (20)     2846 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/test_commons/utils.py
-drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:25.041911 modular_sdk-2.1.4/tests/test_models/
--rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/test_models/__init__.py
--rw-r--r--   0 onsha      (501) staff       (20)    11617 2023-06-30 09:15:05.000000 modular_sdk-2.1.4/tests/test_models/test_base_safe_update_model.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.852361 modular_sdk-2.2.0/
+-rw-r--r--   0 onsha      (501) staff       (20)    11357 2023-06-29 14:09:33.000000 modular_sdk-2.2.0/LICENSE
+-rw-r--r--   0 onsha      (501) staff       (20)     4014 2023-08-03 12:12:20.852515 modular_sdk-2.2.0/PKG-INFO
+-rw-r--r--   0 onsha      (501) staff       (20)     3507 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/README.md
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.809026 modular_sdk-2.2.0/modular_sdk/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/__init__.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.815396 modular_sdk-2.2.0/modular_sdk/commons/
+-rw-r--r--   0 onsha      (501) staff       (20)     4869 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     5073 2023-08-03 12:11:18.000000 modular_sdk-2.2.0/modular_sdk/commons/constants.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2045 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/error_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)      200 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/exception.py
+-rw-r--r--   0 onsha      (501) staff       (20)      800 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/helpers.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2642 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/log_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)      951 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/time_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2458 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/commons/trace_helper.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.816547 modular_sdk-2.2.0/modular_sdk/connections/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/connections/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1754 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/connections/mongodb_connection.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4723 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/connections/rabbit_connection.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.817469 modular_sdk-2.2.0/modular_sdk/helpers/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/helpers/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)      985 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/helpers/response_helper.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.824546 modular_sdk-2.2.0/modular_sdk/models/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1579 2023-08-03 10:34:40.000000 modular_sdk-2.2.0/modular_sdk/models/application.py
+-rw-r--r--   0 onsha      (501) staff       (20)      929 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/base_meta.py
+-rw-r--r--   0 onsha      (501) staff       (20)      689 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/customer.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1050 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/execution_trace.py
+-rw-r--r--   0 onsha      (501) staff       (20)      490 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/heartbeat.py
+-rw-r--r--   0 onsha      (501) staff       (20)      712 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/job.py
+-rw-r--r--   0 onsha      (501) staff       (20)      662 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/operation_mode.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1570 2023-08-03 10:34:40.000000 modular_sdk-2.2.0/modular_sdk/models/parent.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.828651 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)    22311 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_model.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2261 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_role_access_model.py
+-rw-r--r--   0 onsha      (501) staff       (20)     7045 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_safe_update_model.py
+-rw-r--r--   0 onsha      (501) staff       (20)    16520 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py
+-rw-r--r--   0 onsha      (501) staff       (20)      811 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2565 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/region.py
+-rw-r--r--   0 onsha      (501) staff       (20)      476 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/setting.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4048 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/tenant.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1081 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/models/tenant_settings.py
+-rw-r--r--   0 onsha      (501) staff       (20)    10963 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/modular.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.838835 modular_sdk-2.2.0/modular_sdk/services/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4860 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/application_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4559 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/aws_creds_provider.py
+-rw-r--r--   0 onsha      (501) staff       (20)      803 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/customer_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     5073 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/environment_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)      618 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/events_service.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.841870 modular_sdk-2.2.0/modular_sdk/services/impl/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/impl/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)    25123 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/impl/maestro_credentials_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     9096 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/impl/maestro_rabbit_transport_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)      620 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/lambda_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     5862 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/parent_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     3751 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/rabbit_transport_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2602 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/region_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     9806 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/settings_management_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1488 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/sqs_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     7305 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/ssm_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     8390 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/sts_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     7445 2023-08-03 12:11:18.000000 modular_sdk-2.2.0/modular_sdk/services/tenant_service.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2143 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/services/tenant_settings_service.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.843060 modular_sdk-2.2.0/modular_sdk/utils/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/__init__.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.844500 modular_sdk-2.2.0/modular_sdk/utils/job_tracer/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/job_tracer/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)      354 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/job_tracer/abstract.py
+-rw-r--r--   0 onsha      (501) staff       (20)     3832 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/job_tracer/generic.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.846142 modular_sdk-2.2.0/modular_sdk/utils/operation_mode/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/operation_mode/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)      776 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/operation_mode/abstract.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2171 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/operation_mode/generic.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.847831 modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1061 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/abstract.py
+-rw-r--r--   0 onsha      (501) staff       (20)     4091 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/generic.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.810954 modular_sdk-2.2.0/modular_sdk.egg-info/
+-rw-r--r--   0 onsha      (501) staff       (20)     4014 2023-08-03 12:12:20.000000 modular_sdk-2.2.0/modular_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 onsha      (501) staff       (20)     2945 2023-08-03 12:12:20.000000 modular_sdk-2.2.0/modular_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 onsha      (501) staff       (20)        1 2023-08-03 12:12:20.000000 modular_sdk-2.2.0/modular_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 onsha      (501) staff       (20)      271 2023-08-03 12:12:20.000000 modular_sdk-2.2.0/modular_sdk.egg-info/requires.txt
+-rw-r--r--   0 onsha      (501) staff       (20)       18 2023-08-03 12:12:20.000000 modular_sdk-2.2.0/modular_sdk.egg-info/top_level.txt
+-rw-r--r--   0 onsha      (501) staff       (20)       86 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/pyproject.toml
+-rw-r--r--   0 onsha      (501) staff       (20)      923 2023-08-03 12:12:20.853168 modular_sdk-2.2.0/setup.cfg
+-rw-r--r--   0 onsha      (501) staff       (20)       38 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/setup.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.848585 modular_sdk-2.2.0/tests/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/__init__.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.850634 modular_sdk-2.2.0/tests/test_commons/
+-rw-r--r--   0 onsha      (501) staff       (20)      119 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/test_commons/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)     1852 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/test_commons/import_helper.py
+-rw-r--r--   0 onsha      (501) staff       (20)     2846 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/test_commons/utils.py
+drwxr-xr-x   0 onsha      (501) staff       (20)        0 2023-08-03 12:12:20.851827 modular_sdk-2.2.0/tests/test_models/
+-rw-r--r--   0 onsha      (501) staff       (20)        0 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/test_models/__init__.py
+-rw-r--r--   0 onsha      (501) staff       (20)    11617 2023-06-30 09:15:05.000000 modular_sdk-2.2.0/tests/test_models/test_base_safe_update_model.py
```

### Comparing `modular_sdk-2.1.4/LICENSE` & `modular_sdk-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/PKG-INFO` & `modular_sdk-2.2.0/modular_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: modular_sdk
-Version: 2.1.4
+Name: modular-sdk
+Version: 2.2.0
 Summary: Data level integration for services built atop of Modular Framework
 Home-page: https://github.com/epam/modular-sdk
 Author: EPAM Systems
 Author-email: support@syndicate.team
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `modular_sdk-2.1.4/README.md` & `modular_sdk-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/commons/__init__.py` & `modular_sdk-2.2.0/modular_sdk/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/commons/constants.py` & `modular_sdk-2.2.0/modular_sdk/commons/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,22 +37,24 @@
 AZURE_CSP_PARTNER = 'AZURE_CSP_PARTNER'
 AZURE_USAGE_DETAILS = 'AZURE_USAGE_DETAILS'
 GCP_BILLING_SERVICE = 'GCP_BILLING_SERVICE'
 AZURE_ENTERPRISE_BILLING = 'AZURE_ENTERPRISE_BILLING'
 CUSTODIAN_TYPE = 'CUSTODIAN'
 CUSTODIAN_LICENSES_TYPE = 'CUSTODIAN_LICENSES'
 RIGHTSIZER_PARENT_TYPE = 'RIGHTSIZER'
+RIGHTSIZER_LICENSES_PARENT_TYPE = 'RIGHTSIZER_LICENSES'
 SIEM_DEFECT_DOJO_TYPE = 'SIEM_DEFECT_DOJO'
 ALL_PARENT_TYPES = [
     AWS_MANAGEMENT, AWS_ATHENA, AWS_COST_EXPLORER,
     AZURE_ENTERPRISE_BILLING, AZURE_USAGE_DETAILS,
     AZURE_RATE_CARDS, AZURE_CSP_BILLING, AZURE_CSP_PARTNER,
     AZURE_MANAGEMENT, AZURE_AD_SSO, GCP_BILLING_SERVICE,
     GCP_SECURITY, GCP_MANAGEMENT, CUSTODIAN_TYPE,
-    RIGHTSIZER_PARENT_TYPE, SIEM_DEFECT_DOJO_TYPE, CUSTODIAN_LICENSES_TYPE
+    RIGHTSIZER_PARENT_TYPE, RIGHTSIZER_LICENSES_PARENT_TYPE,
+    SIEM_DEFECT_DOJO_TYPE, CUSTODIAN_LICENSES_TYPE
 ]
 
 AZURE_CLOUD = 'AZURE'
 YANDEX_CLOUD = 'YANDEX'
 GOOGLE_CLOUD = 'GOOGLE'
 AWS_CLOUD = 'AWS'
 OPENSTACK_CLOUD = 'OPEN_STACK'
@@ -109,22 +111,24 @@
 
 # Tenant parent map types
 TENANT_PARENT_MAP_BILLING_TYPE = 'BILLING'
 TENANT_PARENT_MAP_MANAGEMENT_TYPE = 'MANAGEMENT'
 TENANT_PARENT_MAP_CUSTODIAN_TYPE = CUSTODIAN_TYPE
 TENANT_PARENT_MAP_CUSTODIAN_LICENSES_TYPE = CUSTODIAN_LICENSES_TYPE
 TENANT_PARENT_MAP_RIGHTSIZER_TYPE = 'RIGHTSIZER'
+TENANT_PARENT_MAP_RIGHTSIZER_LICENSES_TYPE = 'RIGHTSIZER_LICENSES'
 TENANT_PARENT_MAP_SIEM_DEFECT_DOJO_TYPE = SIEM_DEFECT_DOJO_TYPE
 
 
 ALLOWED_TENANT_PARENT_MAP_KEYS = (
     TENANT_PARENT_MAP_BILLING_TYPE,
     TENANT_PARENT_MAP_MANAGEMENT_TYPE,
     TENANT_PARENT_MAP_CUSTODIAN_TYPE,
     TENANT_PARENT_MAP_RIGHTSIZER_TYPE,
+    TENANT_PARENT_MAP_RIGHTSIZER_LICENSES_TYPE,
     TENANT_PARENT_MAP_SIEM_DEFECT_DOJO_TYPE,
     TENANT_PARENT_MAP_CUSTODIAN_LICENSES_TYPE
 )
 
 DEFAULT_AWS_REGION = 'us-east-1'
 
 # native cloud credentials envs
```

### Comparing `modular_sdk-2.1.4/modular_sdk/commons/error_helper.py` & `modular_sdk-2.2.0/modular_sdk/commons/error_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/commons/helpers.py` & `modular_sdk-2.2.0/modular_sdk/commons/helpers.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/commons/log_helper.py` & `modular_sdk-2.2.0/modular_sdk/commons/log_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/commons/time_helper.py` & `modular_sdk-2.2.0/modular_sdk/commons/time_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/commons/trace_helper.py` & `modular_sdk-2.2.0/modular_sdk/commons/trace_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/connections/mongodb_connection.py` & `modular_sdk-2.2.0/modular_sdk/connections/mongodb_connection.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/connections/rabbit_connection.py` & `modular_sdk-2.2.0/modular_sdk/connections/rabbit_connection.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/helpers/response_helper.py` & `modular_sdk-2.2.0/modular_sdk/helpers/response_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/application.py` & `modular_sdk-2.2.0/modular_sdk/models/application.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/base_meta.py` & `modular_sdk-2.2.0/modular_sdk/models/base_meta.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/customer.py` & `modular_sdk-2.2.0/modular_sdk/models/customer.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/execution_trace.py` & `modular_sdk-2.2.0/modular_sdk/models/execution_trace.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/job.py` & `modular_sdk-2.2.0/modular_sdk/models/job.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/operation_mode.py` & `modular_sdk-2.2.0/modular_sdk/models/operation_mode.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/parent.py` & `modular_sdk-2.2.0/modular_sdk/models/parent.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_model.py` & `modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_role_access_model.py` & `modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_role_access_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/base_safe_update_model.py` & `modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/base_safe_update_model.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py` & `modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/pynamodb_to_pymongo_adapter.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py` & `modular_sdk-2.2.0/modular_sdk/models/pynamodb_extension/tenant_result_iterator.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/region.py` & `modular_sdk-2.2.0/modular_sdk/models/region.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/tenant.py` & `modular_sdk-2.2.0/modular_sdk/models/tenant.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/models/tenant_settings.py` & `modular_sdk-2.2.0/modular_sdk/models/tenant_settings.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/modular.py` & `modular_sdk-2.2.0/modular_sdk/modular.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/application_service.py` & `modular_sdk-2.2.0/modular_sdk/services/application_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/aws_creds_provider.py` & `modular_sdk-2.2.0/modular_sdk/services/aws_creds_provider.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/customer_service.py` & `modular_sdk-2.2.0/modular_sdk/services/customer_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/environment_service.py` & `modular_sdk-2.2.0/modular_sdk/services/environment_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/events_service.py` & `modular_sdk-2.2.0/modular_sdk/services/events_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/impl/maestro_credentials_service.py` & `modular_sdk-2.2.0/modular_sdk/services/impl/maestro_credentials_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/impl/maestro_rabbit_transport_service.py` & `modular_sdk-2.2.0/modular_sdk/services/impl/maestro_rabbit_transport_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/lambda_service.py` & `modular_sdk-2.2.0/modular_sdk/services/lambda_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/parent_service.py` & `modular_sdk-2.2.0/modular_sdk/services/parent_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/rabbit_transport_service.py` & `modular_sdk-2.2.0/modular_sdk/services/rabbit_transport_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/region_service.py` & `modular_sdk-2.2.0/modular_sdk/services/region_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/settings_management_service.py` & `modular_sdk-2.2.0/modular_sdk/services/settings_management_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/sqs_service.py` & `modular_sdk-2.2.0/modular_sdk/services/sqs_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/ssm_service.py` & `modular_sdk-2.2.0/modular_sdk/services/ssm_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/sts_service.py` & `modular_sdk-2.2.0/modular_sdk/services/sts_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/services/tenant_service.py` & `modular_sdk-2.2.0/modular_sdk/services/tenant_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,29 +67,37 @@
         )
 
     @staticmethod
     def i_get_tenant_by_customer(
             customer_id: str, active: Optional[bool] = None,
             tenant_name: Optional[str] = None, limit: int = None,
             last_evaluated_key: Union[dict, str] = None,
-            attributes_to_get: Optional[list] = None
+            cloud: Optional[str] = None,
+            attributes_to_get: Optional[list] = None,
+            rate_limit: Optional[int] = None
     ) -> Union[ResultIterator, Result]:
 
         condition = active if active is None else (Tenant.is_active == active)
         name = default_instance(tenant_name, str)
 
         if condition is not None and name:
             condition &= Tenant.name == name
         elif name:
             condition = Tenant.name == name
 
+        if condition is not None and cloud:
+            condition &= Tenant.cloud == cloud
+        elif cloud:
+            condition = Tenant.cloud == cloud
+
         return Tenant.customer_name_index.query(
             hash_key=customer_id, filter_condition=condition, limit=limit,
             last_evaluated_key=last_evaluated_key,
-            attributes_to_get=attributes_to_get
+            attributes_to_get=attributes_to_get,
+            rate_limit=rate_limit
         )
 
     @staticmethod
     def i_get_by_acc(acc: str, active: Optional[bool] = None,
                      limit: int = None,
                      last_evaluated_key: Union[dict, str] = None,
                      attributes_to_get: List[str] = None):
```

### Comparing `modular_sdk-2.1.4/modular_sdk/services/tenant_settings_service.py` & `modular_sdk-2.2.0/modular_sdk/services/tenant_settings_service.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/utils/job_tracer/generic.py` & `modular_sdk-2.2.0/modular_sdk/utils/job_tracer/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/utils/operation_mode/abstract.py` & `modular_sdk-2.2.0/modular_sdk/utils/operation_mode/abstract.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/utils/operation_mode/generic.py` & `modular_sdk-2.2.0/modular_sdk/utils/operation_mode/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/abstract.py` & `modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/abstract.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk/utils/runtime_tracer/generic.py` & `modular_sdk-2.2.0/modular_sdk/utils/runtime_tracer/generic.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/modular_sdk.egg-info/PKG-INFO` & `modular_sdk-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: modular-sdk
-Version: 2.1.4
+Name: modular_sdk
+Version: 2.2.0
 Summary: Data level integration for services built atop of Modular Framework
 Home-page: https://github.com/epam/modular-sdk
 Author: EPAM Systems
 Author-email: support@syndicate.team
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `modular_sdk-2.1.4/modular_sdk.egg-info/SOURCES.txt` & `modular_sdk-2.2.0/modular_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/setup.cfg` & `modular_sdk-2.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modular_sdk
-version = 2.1.4
+version = 2.2.0
 requires-python = >=3.8
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 license = Apache-2.0
 description = Data level integration for services built atop of Modular Framework
```

### Comparing `modular_sdk-2.1.4/tests/test_commons/import_helper.py` & `modular_sdk-2.2.0/tests/test_commons/import_helper.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/tests/test_commons/utils.py` & `modular_sdk-2.2.0/tests/test_commons/utils.py`

 * *Files identical despite different names*

### Comparing `modular_sdk-2.1.4/tests/test_models/test_base_safe_update_model.py` & `modular_sdk-2.2.0/tests/test_models/test_base_safe_update_model.py`

 * *Files identical despite different names*

