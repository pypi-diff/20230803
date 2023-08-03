# Comparing `tmp/clean-python-0.2.0b2.tar.gz` & `tmp/clean-python-0.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-python-0.2.0b2.tar", last modified: Wed Aug  2 11:46:47 2023, max compression
+gzip compressed data, was "clean-python-0.2.0b3.tar", last modified: Wed Aug  2 11:59:52 2023, max compression
```

## Comparing `clean-python-0.2.0b2.tar` & `clean-python-0.2.0b3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.069037 clean-python-0.2.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-08-02 11:46:47.069037 clean-python-0.2.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.061037 clean-python-0.2.0b2/clean_python/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.061037 clean-python-0.2.0b2/clean_python/base/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.061037 clean-python-0.2.0b2/clean_python/base/application/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/application/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.061037 clean-python-0.2.0b2/clean_python/base/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/domain_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/root_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/domain/value_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/base/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/infrastructure/in_memory_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/infrastructure/internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/infrastructure/tmpdir_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/base/presentation/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/presentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/base/presentation/link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/celery/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/celery/celery_rmq_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/dramatiq/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/dramatiq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/dramatiq/async_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/dramatiq/dramatiq_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/dramatiq/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/error_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/fastapi_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fastapi/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/fluentbit/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fluentbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/fluentbit/fluentbit_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/oauth2/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/oauth2/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/sql/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/sql/sql_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/sql/sql_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/sql/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.065037 clean-python-0.2.0b2/clean_python/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/testing/attr_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/testing/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/clean_python/testing/profilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.061037 clean-python-0.2.0b2/clean_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-08-02 11:46:47.000000 clean-python-0.2.0b2/clean_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-02 11:46:47.000000 clean-python-0.2.0b2/clean_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:46:47.000000 clean-python-0.2.0b2/clean_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:46:46.000000 clean-python-0.2.0b2/clean_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-02 11:46:47.000000 clean-python-0.2.0b2/clean_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 11:46:47.000000 clean-python-0.2.0b2/clean_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 11:46:47.069037 clean-python-0.2.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:46:47.069037 clean-python-0.2.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_async_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_celery_rmq_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_dramatiq_task_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_fastapi_access_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_internal_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_root_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_sql_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-02 11:46:37.000000 clean-python-0.2.0b2/tests/test_value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.634187 clean-python-0.2.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-08-02 11:59:52.634187 clean-python-0.2.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/base/application/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/application/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/base/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/domain_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/root_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/domain/value_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/base/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/infrastructure/in_memory_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/infrastructure/internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/infrastructure/tmpdir_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python/base/presentation/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/presentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/base/presentation/link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/celery/celery_rmq_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/dramatiq/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/dramatiq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/dramatiq/async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/dramatiq/dramatiq_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/dramatiq/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/error_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/fastapi_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fastapi/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/fluentbit/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fluentbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/fluentbit/fluentbit_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/oauth2/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/sql/sql_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/sql/sql_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/sql/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.630187 clean-python-0.2.0b3/clean_python/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/testing/attr_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/testing/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/clean_python/testing/profilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.626186 clean-python-0.2.0b3/clean_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 11:59:52.000000 clean-python-0.2.0b3/clean_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-02 11:59:52.634187 clean-python-0.2.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:59:52.634187 clean-python-0.2.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_celery_rmq_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_dramatiq_task_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_fastapi_access_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_internal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_root_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_sql_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-02 11:59:43.000000 clean-python-0.2.0b3/tests/test_value_object.py
```

### Comparing `clean-python-0.2.0b2/CHANGES.md` & `clean-python-0.2.0b3/CHANGES.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Changelog of clean-python
 
 
+0.2.0b3 (2023-08-02)
+--------------------
+
+- Bugfix: remove bearer prefix from api-key
+
+
 0.2.0b2 (2023-08-02)
 --------------------
 
 - ApiKey authentication now uses `Authorization` header and `bearer` prefix by default.
 
 
 0.1.2 (2023-07-31)
```

### Comparing `clean-python-0.2.0b2/LICENSE` & `clean-python-0.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/PKG-INFO` & `clean-python-0.2.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-python
-Version: 0.2.0b2
+Version: 0.2.0b3
 Summary: Clean architecture in Python
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: homepage, https://github.com/nens/clean-python
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `clean-python-0.2.0b2/README.md` & `clean-python-0.2.0b3/README.md`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/base/application/manage.py` & `clean-python-0.2.0b3/clean_python/base/application/manage.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/base/domain/domain_event.py` & `clean-python-0.2.0b3/clean_python/base/domain/domain_event.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/base/domain/exceptions.py` & `clean-python-0.2.0b3/clean_python/base/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/base/domain/gateway.py` & `clean-python-0.2.0b3/clean_python/base/domain/gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/base/domain/repository.py` & `clean-python-0.2.0b3/clean_python/base/domain/repository.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/base/domain/root_entity.py` & `clean-python-0.2.0b3/clean_python/base/domain/root_entity.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/base/domain/value_object.py` & `clean-python-0.2.0b3/clean_python/base/domain/value_object.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/base/infrastructure/in_memory_gateway.py` & `clean-python-0.2.0b3/clean_python/base/infrastructure/in_memory_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/base/infrastructure/internal_gateway.py` & `clean-python-0.2.0b3/clean_python/base/infrastructure/internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/celery/celery_rmq_broker.py` & `clean-python-0.2.0b3/clean_python/celery/celery_rmq_broker.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/dramatiq/async_actor.py` & `clean-python-0.2.0b3/clean_python/dramatiq/async_actor.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/dramatiq/dramatiq_task_logger.py` & `clean-python-0.2.0b3/clean_python/dramatiq/dramatiq_task_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/dramatiq/testing.py` & `clean-python-0.2.0b3/clean_python/dramatiq/testing.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/fastapi/context.py` & `clean-python-0.2.0b3/clean_python/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/fastapi/error_responses.py` & `clean-python-0.2.0b3/clean_python/fastapi/error_responses.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/fastapi/fastapi_access_logger.py` & `clean-python-0.2.0b3/clean_python/fastapi/fastapi_access_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/fastapi/request_query.py` & `clean-python-0.2.0b3/clean_python/fastapi/request_query.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/fastapi/resource.py` & `clean-python-0.2.0b3/clean_python/fastapi/resource.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/fastapi/service.py` & `clean-python-0.2.0b3/clean_python/fastapi/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     async def __call__(
         self, request: Request, api_key_header: str = Security(api_key_header)
     ) -> None:
         if not api_key_header.lower().startswith(self.prefix.lower()):
             raise HTTPException(status_code=HTTP_401_UNAUTHORIZED)
 
         # skip bearer part
-        api_key_header = api_key_header[len(self.prefix) + 1, :]
+        api_key_header = api_key_header[len(self.prefix) + 1 :]
         try:
             claims = await self.verifier(api_key_header)
             request.scope["user"] = claims
         except Unauthorized:
             raise HTTPException(status_code=HTTP_401_UNAUTHORIZED)
         except PermissionDenied:
             raise HTTPException(status_code=HTTP_403_FORBIDDEN)
```

### Comparing `clean-python-0.2.0b2/clean_python/oauth2/oauth2.py` & `clean-python-0.2.0b3/clean_python/oauth2/oauth2.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/sql/sql_gateway.py` & `clean-python-0.2.0b3/clean_python/sql/sql_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/sql/sql_provider.py` & `clean-python-0.2.0b3/clean_python/sql/sql_provider.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/sql/testing.py` & `clean-python-0.2.0b3/clean_python/sql/testing.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/testing/debugger.py` & `clean-python-0.2.0b3/clean_python/testing/debugger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python/testing/profilers.py` & `clean-python-0.2.0b3/clean_python/testing/profilers.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/clean_python.egg-info/PKG-INFO` & `clean-python-0.2.0b3/clean_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-python
-Version: 0.2.0b2
+Version: 0.2.0b3
 Summary: Clean architecture in Python
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: homepage, https://github.com/nens/clean-python
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `clean-python-0.2.0b2/clean_python.egg-info/SOURCES.txt` & `clean-python-0.2.0b3/clean_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/pyproject.toml` & `clean-python-0.2.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_async_actor.py` & `clean-python-0.2.0b3/tests/test_async_actor.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_celery_rmq_broker.py` & `clean-python-0.2.0b3/tests/test_celery_rmq_broker.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_dramatiq_task_logger.py` & `clean-python-0.2.0b3/tests/test_dramatiq_task_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_exceptions.py` & `clean-python-0.2.0b3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_fastapi_access_logger.py` & `clean-python-0.2.0b3/tests/test_fastapi_access_logger.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_gateway.py` & `clean-python-0.2.0b3/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_internal_gateway.py` & `clean-python-0.2.0b3/tests/test_internal_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_manage.py` & `clean-python-0.2.0b3/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_oauth2.py` & `clean-python-0.2.0b3/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_repository.py` & `clean-python-0.2.0b3/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_request_query.py` & `clean-python-0.2.0b3/tests/test_request_query.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_resource.py` & `clean-python-0.2.0b3/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_root_entity.py` & `clean-python-0.2.0b3/tests/test_root_entity.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_service.py` & `clean-python-0.2.0b3/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_sql_gateway.py` & `clean-python-0.2.0b3/tests/test_sql_gateway.py`

 * *Files identical despite different names*

### Comparing `clean-python-0.2.0b2/tests/test_value_object.py` & `clean-python-0.2.0b3/tests/test_value_object.py`

 * *Files identical despite different names*

