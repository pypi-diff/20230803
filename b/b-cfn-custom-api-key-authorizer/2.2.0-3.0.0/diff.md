# Comparing `tmp/b_cfn_custom_api_key_authorizer-2.2.0.tar.gz` & `tmp/b_cfn_custom_api_key_authorizer-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b_cfn_custom_api_key_authorizer-2.2.0.tar", last modified: Mon Aug 22 09:41:33 2022, max compression
+gzip compressed data, was "b_cfn_custom_api_key_authorizer-3.0.0.tar", last modified: Thu Aug  3 13:57:58 2023, max compression
```

## Comparing `b_cfn_custom_api_key_authorizer-2.2.0.tar` & `b_cfn_custom_api_key_authorizer-3.0.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12407 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7908 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.758689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/api_keys_database.py
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/authorization_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     4865 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/custom_authorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.758689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.758689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/authorizer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/authorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/authorizer/function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.758689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/index.py
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/policy_document.py
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/base_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.758689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/deleter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/deleter/function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.758689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/deleter/source/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/deleter/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/deleter/source/index.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.758689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/exists/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/exists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      820 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/exists/function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/exists/source/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/exists/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/exists/source/index.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/generator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/generator/function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/generator/source/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/generator/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/generator/source/index.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/validator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/validator/function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/validator/source/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/validator/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/validator/source/index.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.758689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12407 2022-08-22 09:41:33.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3813 2022-08-22 09:41:33.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 09:41:33.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-08-22 09:41:33.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-08-22 09:41:33.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/authorizer_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/source/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/source/python/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/source/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/source/python/api_keys_verification.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/source/python/api_secret_hash.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/source/python/auth_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.758689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/fixtures/api_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/api_key_secret_auth_endpoint_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/authorized_api_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/basic_auth_endpoint_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2400 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/main_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4256 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_authorizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_deleter.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_exists.py
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/util/lambda_invoke.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 09:41:33.762689 b_cfn_custom_api_key_authorizer-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-08-22 09:32:58.000000 b_cfn_custom_api_key_authorizer-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.345995 b_cfn_custom_api_key_authorizer-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-08-03 13:57:58.345995 b_cfn_custom_api_key_authorizer-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.337995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/api_keys_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/authorization_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/custom_authorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.337995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/authorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/authorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/authorizer/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/policy_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/base_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/deleter/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/deleter/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/deleter/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/deleter/source/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/exists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/exists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/exists/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/exists/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/exists/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/exists/source/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/generator/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/generator/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/generator/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/generator/source/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/validator/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/validator/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/validator/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/validator/source/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.337995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-08-03 13:57:58.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-03 13:57:58.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 13:57:58.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-03 13:57:58.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 13:57:58.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/authorizer_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/source/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/source/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/source/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/source/python/api_keys_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/source/python/api_secret_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/source/python/auth_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.337995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.341995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/fixtures/api_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.345995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/api_key_secret_auth_endpoint_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/authorized_api_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/basic_auth_endpoint_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/main_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.345995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_authorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:57:58.345995 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/util/lambda_invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 13:57:58.345995 b_cfn_custom_api_key_authorizer-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-03 13:52:29.000000 b_cfn_custom_api_key_authorizer-3.0.0/setup.py
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/HISTORY.md` & `b_cfn_custom_api_key_authorizer-3.0.0/HISTORY.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Release history
 
+### 3.0.0
+
+* Upgrade CDK support from v1 to v2.
+* Upgrade GitHub pipelines checkout version from v2 to v3.
+* Set GitHub pipelines node version 18.
+* Set GitHub pipelines python version 3.10.
+
+### 2.3.0
+
+* Update of `authorizer` function. Removing of sensitive information form lambda event implemented. 
+
 ### 2.2.0
 
 * Remove unnecessary dependencies.
 
 ### 2.1.1
 
 * Add more integration tests.
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/LICENSE` & `b_cfn_custom_api_key_authorizer-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/PKG-INFO` & `b_cfn_custom_api_key_authorizer-3.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,343 +1,354 @@
 Metadata-Version: 2.1
 Name: b_cfn_custom_api_key_authorizer
-Version: 2.2.0
+Version: 3.0.0
 Summary: Enables ApiKey functionality (like in ApiGateway V1) for ApiGateway V2.
 Home-page: https://github.com/biomapas/B.CfnCustomApiKeyAuthorizer.git
 License: Apache License 2.0
-Description: # B.CfnCustomApiKeyAuthorizer
-        
-        ![Pipeline](https://github.com/Biomapas/B.CfnCustomApiKeyAuthorizer/workflows/Pipeline/badge.svg?branch=master)
-        
-        An AWS CDK resource that enables protection of your public APIs by 
-        using Api Keys (ApiKey and Secret).
-        
-        ### Description
-        
-        This custom authorizer enables Api Key functionality 
-        (something similar to ApiGateway V1 version: https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-setup-api-key-with-console.html)
-        
-        APIs created via ApiGateway V2 do not have Api Key authorization functionality out-of-the-box. 
-        If you want to protect your V2 API by generating a secret key and giving only for the 
-        intended clients - this library is just for you. This library allows you to protect you
-        ApiGatewayV2-based endpoints with a combination of ApiKey and ApiSecret. Refer to usages & examples 
-        to understand how to use this library. 
-        
-        The authorizer library exposes these lambda functions that can be called directly:
-        - `authorizer` - _ApiKeysAuthorizerFunction_ - used by a custom (this) authorizer that is attached to your API.
-        - `deleter` - _ApiKeysDeleterFunction_ - allows revoking access to your API i.e. deletes api keys.
-        - `exists` - _ApiKeysExistsFunction_ - allows you to check whether a given API key exists in the database.
-        - `generator` - _ApiKeysGeneratorFunction_ - generates api key and api secret pair and saves in an internal database.
-        - `validator` - _ApiKeysValidatorFunction_ - validates given api key and api secret against the ones in the database.
-        
-        ### Remarks
-        
-        [Biomapas](https://www.biomapas.com/) aims to modernise life-science industry by sharing its IT knowledge with other
-        companies and the community. This is an open source library intended to be used by anyone. Improvements and pull
-        requests are welcome.
-        
-        ### Related technology
-        
-        - Python3
-        - AWS CDK
-        - AWS CloudFormation
-        - AWS API Gateway
-        - AWS API Gateway Authorizer
-        - AWS Lambda
-        
-        ### Assumptions
-        
-        This project assumes you are an expert in infrastructure-as-code via AWS CloudFormation and AWS CDK. You must clearly
-        understand how AWS API Gateway endpoints are protected with Authorizers / Custom Authorizers and how it is managed via
-        CloudFormation or CDK.
-        
-        - Excellent knowledge in IaaC (Infrastructure as a Code) principles.
-        - Excellent knowledge in API Gateway, Authorizers.
-        - Good experience in AWS CDK and AWS CloudFormation.
-        - Good Python skills and basics of OOP.
-        
-        ### Useful sources
-        
-        - AWS CDK:<br>https://docs.aws.amazon.com/cdk/api/latest/docs/aws-construct-library.html
-        - AWS CloudFormation:<br>https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html
-        - API Gateway with
-          CloudFormation:<br>https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigatewayv2-api.html
-        - AWS Custom
-          Authorizers:<br>https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-use-lambda-authorizer.html
-        
-        ### Install
-        
-        Before installing this library, ensure you have these tools setup:
-        
-        - Python / Pip
-        - AWS CDK
-        
-        To install this project from source run:
-        
-        ```
-        pip install .
-        ```
-        
-        Or you can install it from a PyPi repository:
-        
-        ```
-        pip install b-cfn-custom-api-key-authorizer
-        ```
-        
-        ### Usage & Examples
-        
-        Firstly, create an api and stage:
-        
-        ```python
-        from aws_cdk.aws_apigatewayv2 import CfnApi, CfnStage
-        
-        api = CfnApi(...)
-        api_stage = CfnStage(...)
-        ```
-        
-        Create api key custom authorizer:
-        
-        ```python
-        from b_cfn_custom_api_key_authorizer.custom_authorizer import ApiKeyCustomAuthorizer
-        from b_cfn_custom_api_key_authorizer.authorization_type import AuthorizationType
-        
-        authorizer = ApiKeyCustomAuthorizer(
-            scope=Stack(...),
-            resource_name_prefix='MyCool',
-            api=api,
-            # If you specify this, your API will look for "ApiKey" and "ApiSecret" headers in your request.
-            # authorization_type=AuthorizationType.API_KEY_AND_SECRET_HEADERS
-            # If you specify this, your API will treat your request with basic auth in mind ("Authorization" header).
-            # authorization_type=AuthorizationType.AUTHORIZATION_HEADER
-        )
-        ```
-        
-        Use that authorizer to protect your routes (endpoints):
-        
-        ```python
-        from aws_cdk.aws_apigatewayv2 import CfnRoute
-        
-        route = CfnRoute(
-            scope=Stack(...),
-            id='DummyRoute',
-            api_id=api.ref,
-            route_key='GET /dummy/endpoint',
-            authorization_type='CUSTOM',
-            target=f'integrations/{integration.ref}',
-            authorizer_id=authorizer.ref
-        )
-        ```
-        
-        Once your infrastructure is deployed, try calling your api endpoint. You will get "Unauthorized" error.
-        
-        ```python
-        import urllib3
-        
-        response = urllib3.PoolManager().request(
-            method='GET',
-            url='https://your-api-url/dummy/endpoint',
-            headers={},
-        )
-        
-        >>> response.status
-        >>> 401
-        ```
-        
-        Create `ApiKey` and `ApiSecret` by invoking a dedicated api keys generator lambda function:
-        
-        ```python
-        # Your supplied prefix for the infrastrucutre.
-        resource_name_prefix = 'MyCool'
-        # Created generator lambda function name.
-        function_name = 'ApiKeysGeneratorFunction'
-        # Full function name is a combination of both.
-        function_name = resource_name_prefix + function_name
-        
-        response = boto3.client('lambda').invoke(
-            FunctionName=function_name,
-            InvocationType='RequestResponse',
-        )
-        
-        response = json.loads(response['Payload'].read())
-        api_key = response['ApiKey']
-        api_secret = response['ApiSecret']
-        ```
-        
-        Now try calling the same api with api keys:
-        
-        ```python
-        import urllib3
-        
-        response = urllib3.PoolManager().request(
-            method='GET',
-            url='https://your-api-url/dummy/endpoint',
-            headers={
-                'ApiKey': api_key,
-                'ApiSecret': api_secret
-            },
-        )
-        
-        >>> response.status
-        >>> 200
-        ```
-        
-        #### Exposed lambda functions
-        
-        The authorizer exposes these lambda functions that can be called directly:
-        - `authorizer` - ApiKeysAuthorizerFunction
-          
-        ```python
-        response = boto3.client('lambda').invoke(
-            FunctionName=prefix + 'ApiKeysAuthorizerFunction',
-            InvocationType='RequestResponse',
-            Payload=json.dumps({
-                'ApiKey': '123',
-                'ApiSecret': '123'
-            }).encode()
-        )
-        
-        response = json.loads(response['Payload'].read())
-        
-        # This will contain a dictionary of IAM based 
-        # permission either to "allow" or "deny" the request.
-        print(response)
-        ```
-        
-        - `deleter` - ApiKeysDeleterFunction
-          
-        ```python
-        # This does not produce a response.
-        boto3.client('lambda').invoke(
-            FunctionName=prefix + 'ApiKeysDeleterFunction',
-            InvocationType='RequestResponse',
-            Payload=json.dumps({
-                'ApiKey': '123',
-            }).encode()
-        )
-        ```
-        
-        - `exists` - ApiKeysExistsFunction
-          
-        ```python
-        response = boto3.client('lambda').invoke(
-            FunctionName=prefix + 'ApiKeysExistsFunction',
-            InvocationType='RequestResponse',
-            Payload=json.dumps({
-                'ApiKey': '123',
-            }).encode()
-        )
-        
-        response = json.loads(response['Payload'].read())
-        
-        # Check whether your ApiKey/Secret exists in the database.
-        assert response['Exists'] is True
-        ```
-        
-        - `generator` - ApiKeysGeneratorFunction
-          
-        ```python
-        response = boto3.client('lambda').invoke(
-            FunctionName=prefix + 'ApiKeysGeneratorFunction',
-            InvocationType='RequestResponse',
-        )
-        
-        response = json.loads(response['Payload'].read())
-        
-        api_key = response['ApiKey']
-        api_secret = response['ApiSecret']
-        ```
-        
-        - `validator` - ApiKeysValidatorFunction
-        
-        ```python
-        response = boto3.client('lambda').invoke(
-            FunctionName=prefix + 'ApiKeysValidatorFunction',
-            InvocationType='RequestResponse',
-            Payload=json.dumps({
-                'ApiKey': '123',
-                'ApiSecret': '123',
-            }).encode()
-        )
-        
-        response = json.loads(response['Payload'].read())
-        
-        # Check whether your ApiKey/Secret is valid.
-        assert response['Valid'] is True
-        ```
-        
-        ### Testing
-        
-        This package has integration tests based on **pytest**. To run tests simply run:
-        
-        ```
-        
-        pytest b_cfn_custom_api_key_authorizer_test/integration/tests
-        
-        ```
-        
-        ### Contribution
-        
-        Found a bug? Want to add or suggest a new feature? Contributions of any kind are gladly welcome. You may contact us
-        directly, create a pull-request or an issue in github platform. Lets modernize the world together.
-        
-        
-        # Release history
-        
-        ### 2.2.0
-        
-        * Remove unnecessary dependencies.
-        
-        ### 2.1.1
-        
-        * Add more integration tests.
-        * Update README documentation.
-        
-        ### 2.1.0
-        
-        * Add ability to specify what type of authentication strategy to use.
-          Support for both `ApiKey` / `ApiSecret` and `Authorization` headers.
-        
-        ### 2.0.1
-        
-        * Dollar sign excluded from API secret.
-        
-        ### 2.0.0
-        
-        * Restructured project.
-        * All lambda functions are under `functions` directory.
-        * Add `deleter` function to revoke api keys.
-        * Add `exists` function to check whether given api key exists.
-        * Add `validator` function to validate api key and api secret.
-        * Increase the length of api key (15) and api secret (30).
-        * Move authentication checking logic to a lambda layer.
-        * Add more lambda-level logging.
-        * Add more integrations tests (total 11 as of now).
-        * **Very important security improvement** - api secrets are now hashed, to avoid
-          leaks if the database is pawned. This is a standard password-level storage security.
-        * Greatly improve documentation.
-        
-        ### 1.1.0
-        
-        * Create a dedicated lambda function to generate
-          api keys. You should not interact with the database directly.
-        
-        ### 1.0.0
-        
-        * Prod-ready version.
-        * Added documentation.
-        * Added more tests.
-        * Some code improvements.
-        
-        ### 0.1.0
-        
-        * Initial testing done. Authorizer works.
-        * Need more tests and edge case handling before promoting to 1.0.0.
-        
-        ### 0.0.1
-        
-        * Initial build.
-        
 Keywords: AWS Cognito api_key Authorizer
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# B.CfnCustomApiKeyAuthorizer
+
+![Pipeline](https://github.com/Biomapas/B.CfnCustomApiKeyAuthorizer/workflows/Pipeline/badge.svg?branch=master)
+
+An AWS CDK resource that enables protection of your public APIs by 
+using Api Keys (ApiKey and Secret).
+
+### Description
+
+This custom authorizer enables Api Key functionality 
+(something similar to ApiGateway V1 version: https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-setup-api-key-with-console.html)
+
+APIs created via ApiGateway V2 do not have Api Key authorization functionality out-of-the-box. 
+If you want to protect your V2 API by generating a secret key and giving only for the 
+intended clients - this library is just for you. This library allows you to protect you
+ApiGatewayV2-based endpoints with a combination of ApiKey and ApiSecret. Refer to usages & examples 
+to understand how to use this library. 
+
+The authorizer library exposes these lambda functions that can be called directly:
+- `authorizer` - _ApiKeysAuthorizerFunction_ - used by a custom (this) authorizer that is attached to your API.
+- `deleter` - _ApiKeysDeleterFunction_ - allows revoking access to your API i.e. deletes api keys.
+- `exists` - _ApiKeysExistsFunction_ - allows you to check whether a given API key exists in the database.
+- `generator` - _ApiKeysGeneratorFunction_ - generates api key and api secret pair and saves in an internal database.
+- `validator` - _ApiKeysValidatorFunction_ - validates given api key and api secret against the ones in the database.
+
+### Remarks
+
+[Biomapas](https://www.biomapas.com/) aims to modernise life-science industry by sharing its IT knowledge with other
+companies and the community. This is an open source library intended to be used by anyone. Improvements and pull
+requests are welcome.
+
+### Related technology
+
+- Python3
+- AWS CDK
+- AWS CloudFormation
+- AWS API Gateway
+- AWS API Gateway Authorizer
+- AWS Lambda
+
+### Assumptions
+
+This project assumes you are an expert in infrastructure-as-code via AWS CloudFormation and AWS CDK. You must clearly
+understand how AWS API Gateway endpoints are protected with Authorizers / Custom Authorizers and how it is managed via
+CloudFormation or CDK.
+
+- Excellent knowledge in IaaC (Infrastructure as a Code) principles.
+- Excellent knowledge in API Gateway, Authorizers.
+- Good experience in AWS CDK and AWS CloudFormation.
+- Good Python skills and basics of OOP.
+
+### Useful sources
+
+- AWS CDK:<br>https://docs.aws.amazon.com/cdk/api/latest/docs/aws-construct-library.html
+- AWS CloudFormation:<br>https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html
+- API Gateway with
+  CloudFormation:<br>https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigatewayv2-api.html
+- AWS Custom
+  Authorizers:<br>https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-use-lambda-authorizer.html
+
+### Install
+
+Before installing this library, ensure you have these tools setup:
+
+- Python / Pip
+- AWS CDK
+
+To install this project from source run:
+
+```
+pip install .
+```
+
+Or you can install it from a PyPi repository:
+
+```
+pip install b-cfn-custom-api-key-authorizer
+```
+
+### Usage & Examples
+
+Firstly, create an api and stage:
+
+```python
+from aws_cdk.aws_apigatewayv2 import CfnApi, CfnStage
+
+api = CfnApi(...)
+api_stage = CfnStage(...)
+```
+
+Create api key custom authorizer:
+
+```python
+from b_cfn_custom_api_key_authorizer.custom_authorizer import ApiKeyCustomAuthorizer
+from b_cfn_custom_api_key_authorizer.authorization_type import AuthorizationType
+
+authorizer = ApiKeyCustomAuthorizer(
+    scope=Stack(...),
+    resource_name_prefix='MyCool',
+    api=api,
+    # If you specify this, your API will look for "ApiKey" and "ApiSecret" headers in your request.
+    # authorization_type=AuthorizationType.API_KEY_AND_SECRET_HEADERS
+    # If you specify this, your API will treat your request with basic auth in mind ("Authorization" header).
+    # authorization_type=AuthorizationType.AUTHORIZATION_HEADER
+)
+```
+
+Use that authorizer to protect your routes (endpoints):
+
+```python
+from aws_cdk.aws_apigatewayv2 import CfnRoute
+
+route = CfnRoute(
+    scope=Stack(...),
+    id='DummyRoute',
+    api_id=api.ref,
+    route_key='GET /dummy/endpoint',
+    authorization_type='CUSTOM',
+    target=f'integrations/{integration.ref}',
+    authorizer_id=authorizer.ref
+)
+```
+
+Once your infrastructure is deployed, try calling your api endpoint. You will get "Unauthorized" error.
+
+```python
+import urllib3
+
+response = urllib3.PoolManager().request(
+    method='GET',
+    url='https://your-api-url/dummy/endpoint',
+    headers={},
+)
+
+>>> response.status
+>>> 401
+```
+
+Create `ApiKey` and `ApiSecret` by invoking a dedicated api keys generator lambda function:
+
+```python
+# Your supplied prefix for the infrastrucutre.
+resource_name_prefix = 'MyCool'
+# Created generator lambda function name.
+function_name = 'ApiKeysGeneratorFunction'
+# Full function name is a combination of both.
+function_name = resource_name_prefix + function_name
+
+response = boto3.client('lambda').invoke(
+    FunctionName=function_name,
+    InvocationType='RequestResponse',
+)
+
+response = json.loads(response['Payload'].read())
+api_key = response['ApiKey']
+api_secret = response['ApiSecret']
+```
+
+Now try calling the same api with api keys:
+
+```python
+import urllib3
+
+response = urllib3.PoolManager().request(
+    method='GET',
+    url='https://your-api-url/dummy/endpoint',
+    headers={
+        'ApiKey': api_key,
+        'ApiSecret': api_secret
+    },
+)
+
+>>> response.status
+>>> 200
+```
+
+#### Exposed lambda functions
+
+The authorizer exposes these lambda functions that can be called directly:
+- `authorizer` - ApiKeysAuthorizerFunction
+  
+```python
+response = boto3.client('lambda').invoke(
+    FunctionName=prefix + 'ApiKeysAuthorizerFunction',
+    InvocationType='RequestResponse',
+    Payload=json.dumps({
+        'ApiKey': '123',
+        'ApiSecret': '123'
+    }).encode()
+)
+
+response = json.loads(response['Payload'].read())
+
+# This will contain a dictionary of IAM based 
+# permission either to "allow" or "deny" the request.
+print(response)
+```
+
+- `deleter` - ApiKeysDeleterFunction
+  
+```python
+# This does not produce a response.
+boto3.client('lambda').invoke(
+    FunctionName=prefix + 'ApiKeysDeleterFunction',
+    InvocationType='RequestResponse',
+    Payload=json.dumps({
+        'ApiKey': '123',
+    }).encode()
+)
+```
+
+- `exists` - ApiKeysExistsFunction
+  
+```python
+response = boto3.client('lambda').invoke(
+    FunctionName=prefix + 'ApiKeysExistsFunction',
+    InvocationType='RequestResponse',
+    Payload=json.dumps({
+        'ApiKey': '123',
+    }).encode()
+)
+
+response = json.loads(response['Payload'].read())
+
+# Check whether your ApiKey/Secret exists in the database.
+assert response['Exists'] is True
+```
+
+- `generator` - ApiKeysGeneratorFunction
+  
+```python
+response = boto3.client('lambda').invoke(
+    FunctionName=prefix + 'ApiKeysGeneratorFunction',
+    InvocationType='RequestResponse',
+)
+
+response = json.loads(response['Payload'].read())
+
+api_key = response['ApiKey']
+api_secret = response['ApiSecret']
+```
+
+- `validator` - ApiKeysValidatorFunction
+
+```python
+response = boto3.client('lambda').invoke(
+    FunctionName=prefix + 'ApiKeysValidatorFunction',
+    InvocationType='RequestResponse',
+    Payload=json.dumps({
+        'ApiKey': '123',
+        'ApiSecret': '123',
+    }).encode()
+)
+
+response = json.loads(response['Payload'].read())
+
+# Check whether your ApiKey/Secret is valid.
+assert response['Valid'] is True
+```
+
+### Testing
+
+This package has integration tests based on **pytest**. To run tests simply run:
+
+```
+
+pytest b_cfn_custom_api_key_authorizer_test/integration/tests
+
+```
+
+### Contribution
+
+Found a bug? Want to add or suggest a new feature? Contributions of any kind are gladly welcome. You may contact us
+directly, create a pull-request or an issue in github platform. Lets modernize the world together.
+
+
+# Release history
+
+### 3.0.0
+
+* Upgrade CDK support from v1 to v2.
+* Upgrade GitHub pipelines checkout version from v2 to v3.
+* Set GitHub pipelines node version 18.
+* Set GitHub pipelines python version 3.10.
+
+### 2.3.0
+
+* Update of `authorizer` function. Removing of sensitive information form lambda event implemented. 
+
+### 2.2.0
+
+* Remove unnecessary dependencies.
+
+### 2.1.1
+
+* Add more integration tests.
+* Update README documentation.
+
+### 2.1.0
+
+* Add ability to specify what type of authentication strategy to use.
+  Support for both `ApiKey` / `ApiSecret` and `Authorization` headers.
+
+### 2.0.1
+
+* Dollar sign excluded from API secret.
+
+### 2.0.0
+
+* Restructured project.
+* All lambda functions are under `functions` directory.
+* Add `deleter` function to revoke api keys.
+* Add `exists` function to check whether given api key exists.
+* Add `validator` function to validate api key and api secret.
+* Increase the length of api key (15) and api secret (30).
+* Move authentication checking logic to a lambda layer.
+* Add more lambda-level logging.
+* Add more integrations tests (total 11 as of now).
+* **Very important security improvement** - api secrets are now hashed, to avoid
+  leaks if the database is pawned. This is a standard password-level storage security.
+* Greatly improve documentation.
+
+### 1.1.0
+
+* Create a dedicated lambda function to generate
+  api keys. You should not interact with the database directly.
+
+### 1.0.0
+
+* Prod-ready version.
+* Added documentation.
+* Added more tests.
+* Some code improvements.
+
+### 0.1.0
+
+* Initial testing done. Authorizer works.
+* Need more tests and edge case handling before promoting to 1.0.0.
+
+### 0.0.1
+
+* Initial build.
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/README.md` & `b_cfn_custom_api_key_authorizer-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/api_keys_database.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/api_keys_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 
+from aws_cdk import Stack, RemovalPolicy
 from aws_cdk.aws_dynamodb import Attribute, Table, BillingMode, AttributeType, TableEncryption
-from aws_cdk.core import Stack, RemovalPolicy
 
 
 class ApiKeysDatabase(Table, ABC):
     def __init__(self, scope: Stack, table_name: str) -> None:
         self.__scope = scope
         self.__table_name = table_name
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/authorization_type.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/authorization_type.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/custom_authorizer.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/custom_authorizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
+from aws_cdk import Stack
 from aws_cdk.aws_apigatewayv2 import CfnAuthorizer, CfnApi
 from aws_cdk.aws_dynamodb import Table
-from aws_cdk.core import Stack
 
 from b_cfn_custom_api_key_authorizer.api_keys_database import ApiKeysDatabase
 from b_cfn_custom_api_key_authorizer.authorization_type import AuthorizationType
 from b_cfn_custom_api_key_authorizer.functions.authorizer.function import AuthorizerFunction
 from b_cfn_custom_api_key_authorizer.functions.deleter.function import DeleterFunction
 from b_cfn_custom_api_key_authorizer.functions.exists.function import ExistsFunction
 from b_cfn_custom_api_key_authorizer.functions.generator.function import GeneratorFunction
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/authorizer/function.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/authorizer/function.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from aws_cdk import Stack
 from aws_cdk.aws_apigatewayv2 import CfnApi
 from aws_cdk.aws_lambda import Code, CfnPermission
-from aws_cdk.core import Stack
 
 from b_cfn_custom_api_key_authorizer.api_keys_database import ApiKeysDatabase
 from b_cfn_custom_api_key_authorizer.functions.base_function import BaseFunction
 from b_cfn_custom_api_key_authorizer_layer.authorizer_layer import AuthorizerLayer
 
 
 class AuthorizerFunction(BaseFunction):
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/index.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 root_logger.setLevel(logging.INFO)
 for handler in root_logger.handlers:
     handler.setLevel(logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 def handler(event, context):
-    logger.info(f'Received event:\n{json.dumps(event)}.')
-
     document = PolicyDocument(
         region=os.environ['AWS_REGION'],
         account_id=os.environ['AWS_ACCOUNT'],
         api_id=os.environ['AWS_API_ID'],
         api_key=None
     )
 
     try:
         # Extract api key and secret from lambda event in various strategies.
         api_key, api_secret = __extract_api_key_secret_from_event(event)
 
+        logger.info(f'Received event:\n{json.dumps(event)}.')
+
         # Since ApiKey was extracted, set it in the policy document:
         document.api_key = api_key
 
         # Verify the authorization token.
         logger.info(f'Attempting to verify api credentials (api key: {document.api_key})...')
         ApiKeysVerification(api_key, api_secret).verify()
         logger.info(f'Authentication succeeded for api key: {document.api_key}.')
@@ -46,25 +46,28 @@
         # Log the error.
         logger.info(f'Authentication failed for api key: {document.api_key}. Message: {repr(ex)}.')
         # Authorization has failed. Return "Deny".
         return document.create_policy_statement(allow=False)
 
 
 def __extract_api_key_secret_from_event(event: Dict[str, Any]) -> Tuple[Optional[str], Optional[str]]:
+    # Remove Identity Source from the event as it contains sensitive information.
+    event.pop('identitySource', None)
+
     # Firstly, try to extract from ApiKey & ApiSecret headers.
     # (identity_source=['$request.header.ApiKey', '$request.header.ApiSecret']).
-    api_key: Optional[str] = event.get('headers', {}).get('apikey')
-    api_secret: Optional[str] = event.get('headers', {}).get('apisecret')
+    api_key: Optional[str] = event.get('headers', {}).pop('apikey', None)
+    api_secret: Optional[str] = event.get('headers', {}).pop('apisecret', None)
 
     if api_key and api_secret:
         return api_key, api_secret
 
     # Secondly, try to extract from basic auth (which is way more standard).
     # (identity_source=['$request.header.Authorization']).
-    basic_auth: Optional[str] = event.get('headers', {}).get('authorization')
+    basic_auth: Optional[str] = event.get('headers', {}).pop('authorization', None)
     if basic_auth:
         basic_auth = basic_auth.replace('Basic ', '')
 
         try:
             basic_auth = base64.b64decode(basic_auth.encode()).decode()
         except binascii.Error:
             raise AuthException('Invalid base64 string.')
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/policy_document.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/authorizer/source/policy_document.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/base_function.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/base_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import abstractmethod, ABC
 
+from aws_cdk import Duration, Stack
 from aws_cdk.aws_iam import PolicyStatement
 from aws_cdk.aws_lambda import Function, Code, Runtime
 from aws_cdk.aws_logs import RetentionDays
-from aws_cdk.core import Duration, Stack
 
 from b_cfn_custom_api_key_authorizer.api_keys_database import ApiKeysDatabase
 from b_cfn_custom_api_key_authorizer_layer.authorizer_layer import AuthorizerLayer
 
 
 class BaseFunction(ABC, Function):
     def __init__(
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/deleter/function.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/validator/function.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from aws_cdk import Stack
 from aws_cdk.aws_lambda import Code
-from aws_cdk.core import Stack
 
 from b_cfn_custom_api_key_authorizer.api_keys_database import ApiKeysDatabase
 from b_cfn_custom_api_key_authorizer.functions.base_function import BaseFunction
 from b_cfn_custom_api_key_authorizer_layer.authorizer_layer import AuthorizerLayer
 
 
-class DeleterFunction(BaseFunction):
+class ValidatorFunction(BaseFunction):
     def __init__(
             self,
             scope: Stack,
             name: str,
             api_keys_database: ApiKeysDatabase,
             authorizer_layer: AuthorizerLayer
     ) -> None:
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/deleter/source/index.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/deleter/source/index.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/exists/function.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/generator/function.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from aws_cdk import Stack
 from aws_cdk.aws_lambda import Code
-from aws_cdk.core import Stack
 
 from b_cfn_custom_api_key_authorizer.api_keys_database import ApiKeysDatabase
 from b_cfn_custom_api_key_authorizer.functions.base_function import BaseFunction
 from b_cfn_custom_api_key_authorizer_layer.authorizer_layer import AuthorizerLayer
 
 
-class ExistsFunction(BaseFunction):
+class GeneratorFunction(BaseFunction):
     def __init__(
             self,
             scope: Stack,
             name: str,
             api_keys_database: ApiKeysDatabase,
             authorizer_layer: AuthorizerLayer
     ) -> None:
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/exists/source/index.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/exists/source/index.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/generator/function.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/deleter/function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from aws_cdk import Stack
 from aws_cdk.aws_lambda import Code
-from aws_cdk.core import Stack
 
 from b_cfn_custom_api_key_authorizer.api_keys_database import ApiKeysDatabase
 from b_cfn_custom_api_key_authorizer.functions.base_function import BaseFunction
 from b_cfn_custom_api_key_authorizer_layer.authorizer_layer import AuthorizerLayer
 
 
-class GeneratorFunction(BaseFunction):
+class DeleterFunction(BaseFunction):
     def __init__(
             self,
             scope: Stack,
             name: str,
             api_keys_database: ApiKeysDatabase,
             authorizer_layer: AuthorizerLayer
     ) -> None:
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/generator/source/index.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/generator/source/index.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/validator/function.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/exists/function.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from aws_cdk import Stack
 from aws_cdk.aws_lambda import Code
-from aws_cdk.core import Stack
 
 from b_cfn_custom_api_key_authorizer.api_keys_database import ApiKeysDatabase
 from b_cfn_custom_api_key_authorizer.functions.base_function import BaseFunction
 from b_cfn_custom_api_key_authorizer_layer.authorizer_layer import AuthorizerLayer
 
 
-class ValidatorFunction(BaseFunction):
+class ExistsFunction(BaseFunction):
     def __init__(
             self,
             scope: Stack,
             name: str,
             api_keys_database: ApiKeysDatabase,
             authorizer_layer: AuthorizerLayer
     ) -> None:
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer/functions/validator/source/index.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer/functions/validator/source/index.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer.egg-info/SOURCES.txt` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/authorizer_layer.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/authorizer_layer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, List
 
+from aws_cdk import Stack
 from aws_cdk.aws_lambda import Runtime, LayerVersion, AssetCode
-from aws_cdk.core import Stack
 
 
 class AuthorizerLayer(LayerVersion):
     def __init__(self, scope: Stack) -> None:
         """
         Constructor.
 
@@ -22,9 +22,11 @@
     def get_source_path() -> str:
         from . import layer_root
         return f'{layer_root}/source'
 
     @staticmethod
     def runtimes() -> Optional[List[Runtime]]:
         return [
-            Runtime.PYTHON_3_8
+            Runtime.PYTHON_3_8,
+            Runtime.PYTHON_3_9,
+            Runtime.PYTHON_3_10,
         ]
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_layer/source/python/api_keys_verification.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_layer/source/python/api_keys_verification.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/conftest.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 GLOBAL_PREFIX = os.environ.get('GLOBAL_PREFIX')
 DO_NOT_CREATE_INFRASTRUCTURE = int(os.environ.get('DO_NOT_CREATE_INFRASTRUCTURE', 0))
 DO_NOT_DESTROY_INFRASTRUCTURE = int(os.environ.get('DO_NOT_DESTROY_INFRASTRUCTURE', 0))
 
 CDK_PATH = f'{os.path.dirname(os.path.abspath(__file__))}'
 MANAGER = TestingManager(Credentials(), CdkToolConfig(CDK_PATH, destroy_before_preparing=False))
-if GLOBAL_PREFIX: MANAGER.set_global_prefix(f'B{GLOBAL_PREFIX[:10]}')
+if GLOBAL_PREFIX: MANAGER.set_global_prefix(GLOBAL_PREFIX[:10])
 
 # Import all fixtures.
 # noinspection PyUnresolvedReferences
 from .fixtures import *
 
 
 def pytest_sessionstart(session):
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/fixtures/api_keys.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/fixtures/api_keys.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/api_key_secret_auth_endpoint_stack.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/api_key_secret_auth_endpoint_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from aws_cdk import Stack, Duration
 from aws_cdk.aws_apigatewayv2 import CfnRoute, CfnApi
 from aws_cdk.aws_lambda import Function, Code, Runtime, CfnPermission
-from aws_cdk.core import Stack, Duration
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 from b_cfn_lambda_integration.lambda_integration import LambdaIntegration
 
 from b_cfn_custom_api_key_authorizer.authorization_type import AuthorizationType
 from b_cfn_custom_api_key_authorizer.custom_authorizer import ApiKeyCustomAuthorizer
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/authorized_api_stack.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/authorized_api_stack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from aws_cdk import Stack
 from aws_cdk.aws_apigatewayv2 import CfnApi, CfnStage
-from aws_cdk.core import Construct, Stack
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
+from constructs import Construct
 
 
 class AuthorizedApiStack(Stack):
     def __init__(self, scope: Construct) -> None:
         prefix = TestingStack.global_prefix()
 
         super().__init__(
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/basic_auth_endpoint_stack.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/basic_auth_endpoint_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from aws_cdk import Stack, Duration
 from aws_cdk.aws_apigatewayv2 import CfnRoute, CfnApi
 from aws_cdk.aws_dynamodb import Table
 from aws_cdk.aws_lambda import Function, Code, Runtime, CfnPermission
-from aws_cdk.core import Stack, Duration
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 from b_cfn_lambda_integration.lambda_integration import LambdaIntegration
 
 from b_cfn_custom_api_key_authorizer.authorization_type import AuthorizationType
 from b_cfn_custom_api_key_authorizer.custom_authorizer import ApiKeyCustomAuthorizer
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/main_stack.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/infrastructure/main_stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from aws_cdk.core import Construct
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
+from constructs import Construct
 
 from b_cfn_custom_api_key_authorizer_test.integration.infrastructure.api_key_secret_auth_endpoint_stack import ApiKeySecretAuthEndpointStack
 from b_cfn_custom_api_key_authorizer_test.integration.infrastructure.authorized_api_stack import AuthorizedApiStack
 from b_cfn_custom_api_key_authorizer_test.integration.infrastructure.basic_auth_endpoint_stack import BasicAuthEndpointStack
 
 
 class MainStack(TestingStack):
```

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_authorizer.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_authorizer.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_deleter.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_deleter.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_exists.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_exists.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_generator.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_validator.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `b_cfn_custom_api_key_authorizer-2.2.0/b_cfn_custom_api_key_authorizer_test/integration/util/lambda_invoke.py` & `b_cfn_custom_api_key_authorizer-3.0.0/b_cfn_custom_api_key_authorizer_test/integration/util/lambda_invoke.py`

 * *Files identical despite different names*

