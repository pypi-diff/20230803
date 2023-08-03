# Comparing `tmp/clean-python-0.2.0b3.tar.gz` & `tmp/clean-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-python-0.2.0b3.tar", last modified: Wed Aug  2 11:59:52 2023, max compression
+gzip compressed data, was "clean-python-0.2.1.tar", last modified: Thu Aug  3 14:08:40 2023, max compression
```

## Comparing `clean-python-0.2.0b3.tar` & `clean-python-0.2.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.634187 clean-python-0.2.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-08-02 11:59:52.634187 clean-python-0.2.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/base/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/base/application/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/application/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/base/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/root_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/base/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/infrastructure/in_memory_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/infrastructure/internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/infrastructure/tmpdir_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/base/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/presentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/presentation/link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/celery/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/celery/celery_rmq_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/dramatiq/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/dramatiq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/dramatiq/async_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/dramatiq/dramatiq_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/dramatiq/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/error_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/fastapi_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/fluentbit/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fluentbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fluentbit/fluentbit_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/oauth2/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/sql/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/sql/sql_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/sql/sql_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/sql/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/testing/attr_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/testing/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/testing/profilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 11:59:52.634187 clean-python-0.2.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.634187 clean-python-0.2.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_async_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_celery_rmq_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_dramatiq_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_fastapi_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_root_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_sql_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.992662 clean-python-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-03 14:08:22.000000 clean-python-0.2.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-03 14:08:22.000000 clean-python-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-03 14:08:22.000000 clean-python-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-08-03 14:08:40.992662 clean-python-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-03 14:08:22.000000 clean-python-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.976662 clean-python-0.2.1/clean_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.976662 clean-python-0.2.1/clean_python/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.980661 clean-python-0.2.1/clean_python/base/application/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/application/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.980661 clean-python-0.2.1/clean_python/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/root_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/domain/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.980661 clean-python-0.2.1/clean_python/base/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/infrastructure/in_memory_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/infrastructure/internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/infrastructure/tmpdir_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.984661 clean-python-0.2.1/clean_python/base/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/presentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/base/presentation/link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.984661 clean-python-0.2.1/clean_python/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/celery/celery_rmq_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.984661 clean-python-0.2.1/clean_python/dramatiq/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/dramatiq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/dramatiq/async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/dramatiq/dramatiq_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/dramatiq/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.984661 clean-python-0.2.1/clean_python/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/fastapi/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/fastapi/error_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/fastapi/fastapi_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/fastapi/request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/fastapi/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/fastapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.984661 clean-python-0.2.1/clean_python/fluentbit/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/fluentbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/fluentbit/fluentbit_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.984661 clean-python-0.2.1/clean_python/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/oauth2/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/oauth2/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.988662 clean-python-0.2.1/clean_python/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/sql/sql_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/sql/sql_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/sql/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.988662 clean-python-0.2.1/clean_python/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/testing/attr_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/testing/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-03 14:08:22.000000 clean-python-0.2.1/clean_python/testing/profilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.976662 clean-python-0.2.1/clean_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-08-03 14:08:40.000000 clean-python-0.2.1/clean_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-08-03 14:08:40.000000 clean-python-0.2.1/clean_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:08:40.000000 clean-python-0.2.1/clean_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:08:40.000000 clean-python-0.2.1/clean_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-03 14:08:40.000000 clean-python-0.2.1/clean_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-03 14:08:40.000000 clean-python-0.2.1/clean_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-08-03 14:08:22.000000 clean-python-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-03 14:08:40.992662 clean-python-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:08:40.992662 clean-python-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_celery_rmq_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_dramatiq_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_fastapi_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_root_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_sql_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-03 14:08:22.000000 clean-python-0.2.1/tests/test_value_object.py
```

### Comparing `clean-python-0.2.0b3/CHANGES.md` & `clean-python-0.2.1/CHANGES.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # Changelog of clean-python
 
 
-0.2.0b3 (2023-08-02)
---------------------
-
-- Bugfix: remove bearer prefix from api-key
-
+0.2.1 (2023-08-03)
+------------------
 
-0.2.0b2 (2023-08-02)
---------------------
+- Add HTTP Bearer to OpenAPI security schema.
 
-- ApiKey authentication now uses `Authorization` header and `bearer` prefix by default.
+- Import debugpy at module level on setup_debugger import. Don't check for DEBUG
+  environment variable when setting up.
 
 
-0.1.2 (2023-07-31)
+0.2.0 (2023-08-03)
 ------------------
 
-- Added py.typed marker.
+- Pydantic 2.x support. Drops Pydantic 1.x support, use 0.1.x for Pydantic 1.x.
+  See https://docs.pydantic.dev/latest/migration/
 
+- `BadRequest` is a subclass of `Exception` instead of `ValidationError` / `ValueError`.
 
-0.2.0b1 (2023-07-25)
---------------------
+- `oauth2.OAuth2Settings` is split into two new objects: `TokenVerifierSettings` and
+  `OAuth2SPAClientSettings`. The associated call signature of `Service` was changed.
 
-- `BadRequest` needs `.errors()` method to be backwards compatible.
 
-- Added support for API key authentication.
+0.1.2 (2023-07-31)
+------------------
+
+- Added py.typed marker.
 
 
-0.2.0b0 (2023-07-23)
---------------------
 
-- Pydantic 2.x support. Drops Pydantic 1.x support, use 0.1.x for Pydantic 1.x.
 
 
 0.1.1 (2023-07-31)
 ------------------
 
 - Various import fixes.
```

### Comparing `clean-python-0.2.0b3/LICENSE` & `clean-python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/PKG-INFO` & `clean-python-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-python
-Version: 0.2.0b3
+Version: 0.2.1
 Summary: Clean architecture in Python
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: homepage, https://github.com/nens/clean-python
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `clean-python-0.2.0b3/README.md` & `clean-python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/base/application/manage.py` & `clean-python-0.2.1/clean_python/base/application/manage.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/base/domain/domain_event.py` & `clean-python-0.2.1/clean_python/base/domain/domain_event.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/base/domain/exceptions.py` & `clean-python-0.2.1/clean_python/base/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/base/domain/gateway.py` & `clean-python-0.2.1/clean_python/base/domain/gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/base/domain/repository.py` & `clean-python-0.2.1/clean_python/base/domain/repository.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/base/domain/root_entity.py` & `clean-python-0.2.1/clean_python/base/domain/root_entity.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/base/domain/value_object.py` & `clean-python-0.2.1/clean_python/base/domain/value_object.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/base/infrastructure/in_memory_gateway.py` & `clean-python-0.2.1/clean_python/base/infrastructure/in_memory_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/base/infrastructure/internal_gateway.py` & `clean-python-0.2.1/clean_python/base/infrastructure/internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/celery/celery_rmq_broker.py` & `clean-python-0.2.1/clean_python/celery/celery_rmq_broker.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/dramatiq/async_actor.py` & `clean-python-0.2.1/clean_python/dramatiq/async_actor.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/dramatiq/dramatiq_task_logger.py` & `clean-python-0.2.1/clean_python/dramatiq/dramatiq_task_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/dramatiq/testing.py` & `clean-python-0.2.1/clean_python/dramatiq/testing.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/fastapi/context.py` & `clean-python-0.2.1/clean_python/fastapi/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 # (c) Nelen & Schuurmans
 
 from contextvars import ContextVar
 
 from fastapi import Request
 
+from ..oauth2 import Claims
+
 __all__ = ["ctx", "RequestMiddleware"]
 
 
 class Context:
     def __init__(self):
         self._request_value: ContextVar[Request] = ContextVar("request_value")
+        self._claims_value: ContextVar[Claims] = ContextVar("claims_value")
 
     @property
     def request(self) -> Request:
         return self._request_value.get()
 
     @request.setter
     def request(self, value: Request) -> None:
         self._request_value.set(value)
 
+    @property
+    def claims(self) -> Claims:
+        return self._claims_value.get()
+
+    @claims.setter
+    def claims(self, value: Claims) -> None:
+        self._claims_value.set(value)
+
 
 ctx = Context()
 
 
 class RequestMiddleware:
     """Save the current request in a context variable.
```

### Comparing `clean-python-0.2.0b3/clean_python/fastapi/error_responses.py` & `clean-python-0.2.1/clean_python/fastapi/error_responses.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     )
 
 
 async def unauthorized_handler(request: Request, exc: Unauthorized):
     return JSONResponse(
         status_code=status.HTTP_401_UNAUTHORIZED,
         content={"message": "Unauthorized"},
+        headers={"WWW-Authenticate": "Bearer"},
     )
 
 
 async def permission_denied_handler(request: Request, exc: PermissionDenied):
     return JSONResponse(
         status_code=status.HTTP_403_FORBIDDEN,
         content={"message": "Permission denied"},
```

### Comparing `clean-python-0.2.0b3/clean_python/fastapi/fastapi_access_logger.py` & `clean-python-0.2.1/clean_python/fastapi/fastapi_access_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/fastapi/request_query.py` & `clean-python-0.2.1/clean_python/fastapi/request_query.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/fastapi/resource.py` & `clean-python-0.2.1/clean_python/fastapi/resource.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/fastapi/service.py` & `clean-python-0.2.1/clean_python/fastapi/service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 # (c) Nelen & Schuurmans
 
 import logging
 from typing import Any
 from typing import Callable
-from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
-from typing import Union
 
 from asgiref.sync import sync_to_async
 from fastapi import Depends
 from fastapi import FastAPI
 from fastapi import Request
-from fastapi import Security
-from fastapi.exceptions import HTTPException
 from fastapi.exceptions import RequestValidationError
+from fastapi.security import HTTPBearer
 from fastapi.security import OAuth2AuthorizationCodeBearer
-from fastapi.security.api_key import APIKeyHeader
-from starlette.status import HTTP_401_UNAUTHORIZED
-from starlette.status import HTTP_403_FORBIDDEN
 from starlette.types import ASGIApp
 
 from clean_python import Conflict
 from clean_python import DoesNotExist
 from clean_python import Gateway
 from clean_python import PermissionDenied
 from clean_python import Unauthorized
-from clean_python.oauth2 import AccessTokenVerifierSettings
-from clean_python.oauth2 import OAuth2AccessTokenVerifier
-from clean_python.oauth2 import OAuth2Settings
+from clean_python.oauth2 import OAuth2SPAClientSettings
+from clean_python.oauth2 import TokenVerifier
+from clean_python.oauth2 import TokenVerifierSettings
 
+from .context import ctx
 from .context import RequestMiddleware
 from .error_responses import BadRequest
 from .error_responses import conflict_handler
 from .error_responses import DefaultErrorResponse
 from .error_responses import not_found_handler
 from .error_responses import not_implemented_handler
 from .error_responses import permission_denied_handler
@@ -47,117 +42,71 @@
 from .resource import Resource
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["Service"]
 
 
-class OAuth2Dependable(OAuth2AuthorizationCodeBearer):
+class OAuth2WithClientDependable(OAuth2AuthorizationCodeBearer):
     """A fastapi 'dependable' configuring OAuth2.
 
     This does two things:
     - Verify the token in each request
     - (through FastAPI magic) add the scheme to the OpenAPI spec
     """
 
-    def __init__(self, scope, settings: OAuth2Settings):
-        self.verifier = sync_to_async(
-            OAuth2AccessTokenVerifier(
-                scope,
-                issuer=settings.issuer,
-                resource_server_id=settings.resource_server_id,
-                algorithms=settings.algorithms,
-                admin_users=settings.admin_users,
-            ),
-            thread_sensitive=False,
-        )
+    def __init__(
+        self, settings: TokenVerifierSettings, client: OAuth2SPAClientSettings
+    ):
+        self.verifier = sync_to_async(TokenVerifier(settings), thread_sensitive=False)
         super().__init__(
-            authorizationUrl=settings.authorization_url,
-            tokenUrl=settings.token_url,
-            scopes={
-                f"{settings.resource_server_id}*:readwrite": "Full read/write access"
-            },
+            scheme_name="OAuth2 Authorization Code Flow with PKCE",
+            authorizationUrl=str(client.authorization_url),
+            tokenUrl=str(client.token_url),
         )
 
     async def __call__(self, request: Request) -> None:
-        token = await super().__call__(request)
-        try:
-            await self.verifier(token)
-        except Unauthorized:
-            raise HTTPException(status_code=HTTP_401_UNAUTHORIZED)
-        except PermissionDenied:
-            raise HTTPException(status_code=HTTP_403_FORBIDDEN)
-
-
-def fastapi_oauth_kwargs(auth: OAuth2Settings) -> Dict:
-    return {
-        "dependencies": [Depends(OAuth2Dependable(scope="*:readwrite", settings=auth))],
-        "swagger_ui_init_oauth": {
-            "clientId": auth.client_id,
-            "usePkceWithAuthorizationCodeGrant": True,
-        },
-    }
-
-
-api_key_header = APIKeyHeader(name="Authorization", auto_error=True)
-
-
-class ApiKeyDependable:
-    def __init__(self, scope, settings: AccessTokenVerifierSettings):
-        self.verifier = sync_to_async(
-            OAuth2AccessTokenVerifier(
-                scope,
-                issuer=settings.issuer,
-                resource_server_id=settings.resource_server_id,
-                algorithms=settings.algorithms,
-                admin_users=settings.admin_users,
-                verify_scope_enabled=settings.scope_validation_enabled,
-            ),
-            thread_sensitive=False,
-        )
-        self.prefix = settings.prefix
+        ctx.claims = await self.verifier(request.headers.get("Authorization"))
 
-    async def __call__(
-        self, request: Request, api_key_header: str = Security(api_key_header)
-    ) -> None:
-        if not api_key_header.lower().startswith(self.prefix.lower()):
-            raise HTTPException(status_code=HTTP_401_UNAUTHORIZED)
-
-        # skip bearer part
-        api_key_header = api_key_header[len(self.prefix) + 1 :]
-        try:
-            claims = await self.verifier(api_key_header)
-            request.scope["user"] = claims
-        except Unauthorized:
-            raise HTTPException(status_code=HTTP_401_UNAUTHORIZED)
-        except PermissionDenied:
-            raise HTTPException(status_code=HTTP_403_FORBIDDEN)
-
-
-def fastapi_accesstoken_verifier_kwargs(auth: AccessTokenVerifierSettings) -> Dict:
-    return {
-        "dependencies": [Depends(ApiKeyDependable("", settings=auth))],
-    }
-
-
-class UnknownAuthSettings(Exception):
-    pass
-
-
-AUTH_MAPPING = {
-    OAuth2Settings: fastapi_oauth_kwargs,
-    AccessTokenVerifierSettings: fastapi_accesstoken_verifier_kwargs,
-}
-
-
-def get_auth_kwargs(auth: Any) -> None:
-    func = AUTH_MAPPING.get(type(auth), None)
-    if func is None:
-        raise UnknownAuthSettings(f"Unknown auth setting: {auth}")
-    return func(auth)
+
+class OAuth2WithoutClientDependable(HTTPBearer):
+    """A fastapi 'dependable' configuring OAuth2.
+
+    This does one thing:
+    - Verify the token in each request
+    """
+
+    def __init__(self, settings: TokenVerifierSettings):
+        self.verifier = sync_to_async(TokenVerifier(settings), thread_sensitive=False)
+        super().__init__(scheme_name="JWT Bearer token", bearerFormat="JWT")
+
+    async def __call__(self, request: Request) -> None:
+        ctx.claims = await self.verifier(request.headers.get("Authorization"))
+
+
+def get_auth_kwargs(
+    auth: Optional[TokenVerifierSettings],
+    auth_client: Optional[OAuth2SPAClientSettings],
+) -> None:
+    if auth is None:
+        return {}
+    if auth_client is None:
+        return {
+            "dependencies": [Depends(OAuth2WithoutClientDependable(settings=auth))],
+        }
+    else:
+        return {
+            "dependencies": [
+                Depends(OAuth2WithClientDependable(settings=auth, client=auth_client))
+            ],
+            "swagger_ui_init_oauth": {
+                "clientId": auth_client.client_id,
+                "usePkceWithAuthorizationCodeGrant": True,
+            },
+        }
 
 
 async def health_check():
     """Simple health check route"""
     return {"health": "OK"}
 
 
@@ -228,29 +177,30 @@
         return app
 
     def create_app(
         self,
         title: str,
         description: str,
         hostname: str,
-        auth: Optional[Union[OAuth2Settings, AccessTokenVerifierSettings]] = None,
+        auth: Optional[TokenVerifierSettings] = None,
+        auth_client: Optional[OAuth2SPAClientSettings] = None,
         on_startup: Optional[List[Callable[[], Any]]] = None,
         access_logger_gateway: Optional[Gateway] = None,
     ) -> ASGIApp:
         app = self._create_root_app(
             title=title,
             description=description,
             hostname=hostname,
             on_startup=on_startup,
             access_logger_gateway=access_logger_gateway,
         )
         kwargs = {
             "title": title,
             "description": description,
-            **get_auth_kwargs(auth),
+            **get_auth_kwargs(auth, auth_client),
         }
         versioned_apps = {
             v: self._create_versioned_app(v, **kwargs) for v in self.versions
         }
         for v, versioned_app in versioned_apps.items():
             app.mount("/" + v.prefix, versioned_app)
         return app
```

### Comparing `clean-python-0.2.0b3/clean_python/oauth2/oauth2.py` & `clean-python-0.2.1/clean_python/oauth2/oauth2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,129 @@
 # (c) Nelen & Schuurmans
 
 from typing import Dict
+from typing import FrozenSet
 from typing import List
+from typing import Optional
 
 import jwt
 from jwt import PyJWKClient
 from jwt.exceptions import PyJWTError
 from pydantic import AnyHttpUrl
 from pydantic import BaseModel
 
-from clean_python.base.domain.exceptions import PermissionDenied
-from clean_python.base.domain.exceptions import Unauthorized
+from clean_python import PermissionDenied
+from clean_python import Unauthorized
 
-__all__ = ["OAuth2Settings", "AccessTokenVerifierSettings", "OAuth2AccessTokenVerifier"]
+from .claims import Claims
+from .claims import Tenant
 
+__all__ = ["TokenVerifier", "TokenVerifierSettings", "OAuth2SPAClientSettings"]
 
-class OAuth2Settings(BaseModel):
-    client_id: str
+
+class TokenVerifierSettings(BaseModel):
     issuer: str
-    resource_server_id: str
-    token_url: AnyHttpUrl
-    authorization_url: AnyHttpUrl
     algorithms: List[str] = ["RS256"]
-    admin_users: List[str]
+    # optional additional checks:
+    scope: Optional[str] = None
+    admin_users: Optional[List[str]] = None  # 'sub' whitelist
 
 
-class AccessTokenVerifierSettings(BaseModel):
-    issuer: str
-    resource_server_id: str
-    algorithms: List[str] = ["RS256"]
-    admin_users: List[str]
-    scope_validation_enabled: bool = True
-    prefix: str = "bearer"
+class OAuth2SPAClientSettings(BaseModel):
+    client_id: str
+    token_url: AnyHttpUrl
+    authorization_url: AnyHttpUrl
 
 
-class OAuth2AccessTokenVerifier:
+class TokenVerifier:
     """A class for verifying OAuth2 Access Tokens from AWS Cognito
 
     The verification steps followed are documented here:
 
     https://docs.aws.amazon.com/cognito/latest/developerguide/amazon- ⏎
     cognito-user-pools-using-tokens-verifying-a-jwt.html
     """
 
     # allow 2 minutes leeway for verifying token expiry:
     LEEWAY = 120
 
-    def __init__(
-        self,
-        scope: str,
-        issuer: str,
-        resource_server_id: str,
-        algorithms: List[str],
-        admin_users: List[str],
-        verify_scope_enabled: bool = True,
-    ):
-        self.scope = scope
-        self.verify_scope_enabled = verify_scope_enabled
-        self.issuer = issuer
-        self.algorithms = algorithms
-        self.resource_server_id = resource_server_id
-        self.admin_users = admin_users
-        self.jwk_client = PyJWKClient(f"{issuer}/.well-known/jwks.json")
+    def __init__(self, settings: TokenVerifierSettings):
+        self.settings = settings
+        self.jwk_client = PyJWKClient(f"{settings.issuer}/.well-known/jwks.json")
+
+    def __call__(self, authorization: Optional[str]) -> Claims:
+        # Step 0: retrieve the token from the Authorization header
+        # See https://tools.ietf.org/html/rfc6750#section-2.1,
+        # Bearer is case-sensitive and there is exactly 1 separator after.
+        if authorization is None:
+            raise Unauthorized()
+        token = authorization[7:] if authorization.startswith("Bearer") else None
+        if token is None:
+            raise Unauthorized()
 
-    def __call__(self, token: str) -> Dict:
         # Step 1: Confirm the structure of the JWT. This check is part of get_kid since
         # jwt.get_unverified_header will raise a JWTError if the structure is wrong.
         try:
             key = self.get_key(token)  # JSON Web Key
         except PyJWTError:
             # logger.info("Token is invalid: %s", e)
             raise Unauthorized()
         # Step 2: Validate the JWT signature and standard claims
         try:
             claims = jwt.decode(
                 token,
                 key.key,
-                algorithms=self.algorithms,
-                issuer=self.issuer,
+                algorithms=self.settings.algorithms,
+                issuer=self.settings.issuer,
                 leeway=self.LEEWAY,
                 options={
                     "require": ["exp", "iss", "sub", "scope", "token_use"],
                 },
             )
         except PyJWTError:
             # logger.info("Token is invalid: %s", e)
             raise Unauthorized()
         # Step 3: Verify additional claims. At this point, we have passed
         # verification, so unverified claims may be used safely.
+        scope = self.parse_scope(claims)
+        tenant = self.parse_tenant(claims)
         self.verify_token_use(claims)
-        self.verify_scope(claims)
-        # Step 4: Authorization: we currently work with a hardcoded
-        # list of users ('sub' claims)
-        self.authorize(claims)
-        return claims
+        self.verify_scope(scope)
+        # Step 4: Authorization: verify 'sub' claim against 'admin_users'
+        self.verify_sub(claims)
+        return Claims(scope=scope, tenant=tenant)
 
     def get_key(self, token) -> jwt.PyJWK:
         """Return the JSON Web KEY (JWK) corresponding to kid."""
         return self.jwk_client.get_signing_key_from_jwt(token)
 
-    def verify_token_use(self, claims):
+    def verify_token_use(self, claims: Dict) -> None:
         """Check the token_use claim."""
         if claims["token_use"] != "access":
             # logger.info("Token has invalid token_use claim: %s", claims["token_use"])
             raise Unauthorized()
 
-    def verify_scope(self, claims):
-        """Check scope claim.
-
-        Cognito includes the resource server id inside the scope, like this:
-
-           raster.lizard.net/*.readwrite
-        """
-        if not self.verify_scope_enabled:
+    def verify_scope(self, claims_scope: FrozenSet[str]) -> None:
+        """Parse scopes and optionally check scope claim."""
+        if self.settings.scope is None:
             return
-        if f"{self.resource_server_id}{self.scope}" not in claims["scope"].split(" "):
+        if self.settings.scope not in claims_scope:
             # logger.info("Token has invalid scope claim: %s", claims["scope"])
             raise Unauthorized()
 
-    def authorize(self, claims):
+    def verify_sub(self, claims: Dict) -> None:
         """The subject (sub) claim should be in a hard-coded whitelist."""
-        if claims.get("sub") not in self.admin_users:
+        if self.settings.admin_users is None:
+            return
+        if claims.get("sub") not in self.settings.admin_users:
             # logger.info("User with sub %s is not authorized", claims.get("sub"))
             raise PermissionDenied()
+
+    def parse_scope(self, claims: Dict) -> FrozenSet[str]:
+        return frozenset(claims["scope"].split(" "))
+
+    def parse_tenant(self, claims: Dict) -> Optional[Tenant]:
+        if claims.get("tenant"):
+            tenant = Tenant(id=claims["tenant"], name=claims.get("tenant_name", ""))
+        else:
+            tenant = None
+        return tenant
```

### Comparing `clean-python-0.2.0b3/clean_python/sql/sql_gateway.py` & `clean-python-0.2.1/clean_python/sql/sql_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/sql/sql_provider.py` & `clean-python-0.2.1/clean_python/sql/sql_provider.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/sql/testing.py` & `clean-python-0.2.1/clean_python/sql/testing.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python/testing/profilers.py` & `clean-python-0.2.1/clean_python/testing/profilers.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/clean_python.egg-info/PKG-INFO` & `clean-python-0.2.1/clean_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-python
-Version: 0.2.0b3
+Version: 0.2.1
 Summary: Clean architecture in Python
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: homepage, https://github.com/nens/clean-python
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `clean-python-0.2.0b3/clean_python.egg-info/SOURCES.txt` & `clean-python-0.2.1/clean_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 clean_python/fastapi/fastapi_access_logger.py
 clean_python/fastapi/request_query.py
 clean_python/fastapi/resource.py
 clean_python/fastapi/service.py
 clean_python/fluentbit/__init__.py
 clean_python/fluentbit/fluentbit_gateway.py
 clean_python/oauth2/__init__.py
+clean_python/oauth2/claims.py
 clean_python/oauth2/oauth2.py
 clean_python/sql/__init__.py
 clean_python/sql/sql_gateway.py
 clean_python/sql/sql_provider.py
 clean_python/sql/testing.py
 clean_python/testing/__init__.py
 clean_python/testing/attr_dict.py
@@ -62,15 +63,14 @@
 tests/test_celery_rmq_broker.py
 tests/test_dramatiq_task_logger.py
 tests/test_exceptions.py
 tests/test_fastapi_access_logger.py
 tests/test_gateway.py
 tests/test_internal_gateway.py
 tests/test_manage.py
-tests/test_oauth2.py
 tests/test_repository.py
 tests/test_request_query.py
 tests/test_resource.py
 tests/test_root_entity.py
 tests/test_service.py
 tests/test_sql_gateway.py
 tests/test_value_object.py
```

### Comparing `clean-python-0.2.0b3/pyproject.toml` & `clean-python-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-asyncio",
     "debugpy",
+    "httpx",
 ]
 dramatiq = ["dramatiq"]
 fastapi = ["fastapi"]
 auth = ["pyjwt[crypto]==2.6.0"]
 celery = ["pika"]
 fluentbit = ["fluent-logger"]
 sql = ["sqlalchemy==2.*", "asyncpg"]
```

### Comparing `clean-python-0.2.0b3/tests/test_async_actor.py` & `clean-python-0.2.1/tests/test_async_actor.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_celery_rmq_broker.py` & `clean-python-0.2.1/tests/test_celery_rmq_broker.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_dramatiq_task_logger.py` & `clean-python-0.2.1/tests/test_dramatiq_task_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_exceptions.py` & `clean-python-0.2.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_fastapi_access_logger.py` & `clean-python-0.2.1/tests/test_fastapi_access_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_gateway.py` & `clean-python-0.2.1/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_internal_gateway.py` & `clean-python-0.2.1/tests/test_internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_manage.py` & `clean-python-0.2.1/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_repository.py` & `clean-python-0.2.1/tests/test_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,78 +58,80 @@
 async def test_all(filter_m, user_repository, page_options):
     filter_m.return_value = Page(total=0, items=[])
     assert await user_repository.all(page_options) is filter_m.return_value
 
     filter_m.assert_awaited_once_with([], params=page_options)
 
 
-async def test_add(user_repository):
-    actual: User = await user_repository.add(User.create(name="d"))
+async def test_add(user_repository: UserRepository):
+    actual = await user_repository.add(User.create(name="d"))
     assert actual.name == "d"
     assert user_repository.gateway.data[4] == actual.model_dump()
 
 
-async def test_add_json(user_repository):
-    actual: User = await user_repository.add({"name": "d"})
+async def test_add_json(user_repository: UserRepository):
+    actual = await user_repository.add({"name": "d"})
     assert actual.name == "d"
     assert user_repository.gateway.data[4] == actual.model_dump()
 
 
-async def test_add_json_validates(user_repository):
+async def test_add_json_validates(user_repository: UserRepository):
     with pytest.raises(BadRequest):
         await user_repository.add({"id": "d"})
 
 
-async def test_update(user_repository):
-    actual: User = await user_repository.update(id=2, values={"name": "d"})
+async def test_update(user_repository: UserRepository):
+    actual = await user_repository.update(id=2, values={"name": "d"})
     assert actual.name == "d"
     assert user_repository.gateway.data[2] == actual.model_dump()
 
 
-async def test_update_does_not_exist(user_repository):
+async def test_update_does_not_exist(user_repository: UserRepository):
     with pytest.raises(DoesNotExist):
         await user_repository.update(id=4, values={"name": "d"})
 
 
-async def test_update_validates(user_repository):
+async def test_update_validates(user_repository: UserRepository):
     with pytest.raises(BadRequest):
         await user_repository.update(id=2, values={"id": 6})
 
 
-async def test_remove(user_repository):
+async def test_remove(user_repository: UserRepository):
     assert await user_repository.remove(2)
     assert 2 not in user_repository.gateway.data
 
 
-async def test_remove_does_not_exist(user_repository):
+async def test_remove_does_not_exist(user_repository: UserRepository):
     assert not await user_repository.remove(4)
 
 
-async def test_upsert_updates(user_repository):
-    actual: User = await user_repository.upsert(User.create(id=2, name="d"))
+async def test_upsert_updates(user_repository: UserRepository):
+    actual = await user_repository.upsert(User.create(id=2, name="d"))
     assert actual.name == "d"
     assert user_repository.gateway.data[2] == actual.model_dump()
 
 
-async def test_upsert_adds(user_repository):
-    actual: User = await user_repository.upsert(User.create(id=4, name="d"))
+async def test_upsert_adds(user_repository: UserRepository):
+    actual = await user_repository.upsert(User.create(id=4, name="d"))
     assert actual.name == "d"
     assert user_repository.gateway.data[4] == actual.model_dump()
 
 
 @mock.patch.object(InMemoryGateway, "count")
-async def test_filter(count_m, user_repository, users):
-    actual: Page = await user_repository.filter([Filter(field="name", values=["b"])])
+async def test_filter(count_m, user_repository: UserRepository, users):
+    actual = await user_repository.filter([Filter(field="name", values=["b"])])
     assert actual == Page(total=1, items=[users[1]], limit=None, offest=None)
     assert not count_m.called
 
 
 @mock.patch.object(InMemoryGateway, "count")
-async def test_filter_with_pagination(count_m, user_repository, users, page_options):
-    actual: Page = await user_repository.filter(
+async def test_filter_with_pagination(
+    count_m, user_repository: UserRepository, users, page_options
+):
+    actual = await user_repository.filter(
         [Filter(field="name", values=["b"])], page_options
     )
     assert actual == Page(
         total=1, items=[users[1]], limit=page_options.limit, offset=page_options.offset
     )
     assert not count_m.called
 
@@ -139,29 +141,29 @@
     [
         PageOptions(limit=3, offset=0, order_by="id"),
         PageOptions(limit=10, offset=1, order_by="id"),
     ],
 )
 @mock.patch.object(InMemoryGateway, "count")
 async def test_filter_with_pagination_calls_count(
-    count_m, user_repository, users, page_options
+    count_m, user_repository: UserRepository, users, page_options
 ):
     count_m.return_value = 123
-    actual: Page = await user_repository.filter([], page_options)
+    actual = await user_repository.filter([], page_options)
     assert actual == Page(
         total=count_m.return_value,
         items=users[page_options.offset :],
         limit=page_options.limit,
         offset=page_options.offset,
     )
     assert count_m.called
 
 
 @mock.patch.object(Repository, "filter")
-async def test_by(filter_m, user_repository, page_options):
+async def test_by(filter_m, user_repository: UserRepository, page_options):
     filter_m.return_value = Page(total=0, items=[])
     assert await user_repository.by("name", "b", page_options) is filter_m.return_value
 
     filter_m.assert_awaited_once_with(
         [Filter(field="name", values=["b"])], params=page_options
     )
```

### Comparing `clean-python-0.2.0b3/tests/test_request_query.py` & `clean-python-0.2.1/tests/test_request_query.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_resource.py` & `clean-python-0.2.1/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_root_entity.py` & `clean-python-0.2.1/tests/test_root_entity.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_service.py` & `clean-python-0.2.1/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_sql_gateway.py` & `clean-python-0.2.1/tests/test_sql_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b3/tests/test_value_object.py` & `clean-python-0.2.1/tests/test_value_object.py`

 * *Files identical despite different names*

