# Comparing `tmp/nsj_rest_lib-1.5.0.tar.gz` & `tmp/nsj_rest_lib-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-1.5.0.tar", last modified: Sat Jul 22 20:07:36 2023, max compression
+gzip compressed data, was "nsj_rest_lib-1.5.1.tar", last modified: Wed Aug  2 23:57:36 2023, max compression
```

## Comparing `nsj_rest_lib-1.5.0.tar` & `nsj_rest_lib-1.5.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.415616 nsj_rest_lib-1.5.0/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-07-22 20:07:36.415616 nsj_rest_lib-1.5.0/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-07-22 20:07:36.415616 nsj_rest_lib-1.5.0/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.403616 nsj_rest_lib-1.5.0/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.407616 nsj_rest_lib-1.5.0/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.411616 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       74 2023-07-22 20:03:52.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/constants.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3907 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4590 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4351 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/patch_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3931 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4341 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.411616 nsj_rest_lib-1.5.0/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    21249 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.411616 nsj_rest_lib-1.5.0/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4737 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.411616 nsj_rest_lib-1.5.0/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/descriptor/conjunto_type.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    13146 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.411616 nsj_rest_lib-1.5.0/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7760 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.411616 nsj_rest_lib-1.5.0/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.411616 nsj_rest_lib-1.5.0/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    24142 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      707 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.415616 nsj_rest_lib-1.5.0/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-22 20:07:36.407616 nsj_rest_lib-1.5.0/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-07-22 20:07:36.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1738 2023-07-22 20:07:36.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-22 20:07:36.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-07-22 20:07:36.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-07-22 20:07:36.000000 nsj_rest_lib-1.5.0/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.381750 nsj_rest_lib-1.5.1/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.381750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.381750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       74 2023-07-22 20:03:52.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/constants.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3907 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4590 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4351 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/patch_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3931 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4341 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    21249 2023-07-31 18:42:01.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1235 2023-08-02 23:56:53.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4737 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/conjunto_type.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    13146 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7760 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    24142 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      707 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.385750 nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-07-21 15:01:40.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-08-02 23:57:36.381750 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-08-02 23:57:36.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1738 2023-08-02 23:57:36.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-08-02 23:57:36.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-08-02 23:57:36.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-08-02 23:57:36.000000 nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-1.5.0/PKG-INFO` & `nsj_rest_lib-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_rest_lib
-Version: 1.5.0
+Version: 1.5.1
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.5.0/setup.cfg` & `nsj_rest_lib-1.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 1.5.0
+version = 1.5.1
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/list_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/patch_route.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/patch_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/dao/dao_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
             pagination_where = f"""
                 and (
                     false
                     or {' or '.join(list_page_where)}
                 )
             """
 
-        # Resulvendo o join de conjuntos (se houver)
+        # Resolvendo o join de conjuntos (se houver)
         with_conjunto = ""
         fields_conjunto = ""
         join_conjuntos = ""
         conjunto_map = {}
         if conjunto_type is not None:
             (
                 join_conjuntos,
```

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/db_pool_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 def create_pool(database_conn_url):
     # Creating database connection pool
     db_pool = sqlalchemy.create_engine(
         database_conn_url,
         pool_size=5,
         max_overflow=2,
         pool_timeout=30,
-        pool_recycle=1800
+        pool_recycle=1800,
     )
     return db_pool
 
 
-if DATABASE_DRIVER.upper() == 'SINGLE_STORE':
-    database_conn_url = f'mysql+pymysql://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}'
+if DATABASE_DRIVER.upper() in ["SINGLE_STORE", "MYSQL"]:
+    database_conn_url = f"mysql+pymysql://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}"
 else:
-    if ENV.upper() == 'GCP':
-        database_conn_url = f'postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@/{DATABASE_NAME}?unix_sock=/cloudsql/{CLOUD_SQL_CONN_NAME}/.s.PGSQL.{DATABASE_PORT}'
+    if ENV.upper() == "GCP":
+        database_conn_url = f"postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@/{DATABASE_NAME}?unix_sock=/cloudsql/{CLOUD_SQL_CONN_NAME}/.s.PGSQL.{DATABASE_PORT}"
     else:
-        database_conn_url = f'postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}'
+        database_conn_url = f"postgresql+pg8000://{DATABASE_USER}:{DATABASE_PASS}@{DATABASE_HOST}:{DATABASE_PORT}/{DATABASE_NAME}"
 
 db_pool = create_pool(database_conn_url)
```

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/dto/dto_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/service/service_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-rest-lib
-Version: 1.5.0
+Version: 1.5.1
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.5.0/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-1.5.1/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

