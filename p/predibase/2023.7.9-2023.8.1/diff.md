# Comparing `tmp/predibase-2023.7.9.tar.gz` & `tmp/predibase-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-2023.7.9.tar", last modified: Wed Jul 19 04:40:19 2023, max compression
+gzip compressed data, was "predibase-2023.8.1.tar", last modified: Thu Aug  3 01:12:09 2023, max compression
```

## Comparing `predibase-2023.7.9.tar` & `predibase-2023.8.1.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.931286 predibase-2023.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-19 04:39:16.000000 predibase-2023.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 04:40:19.931286 predibase-2023.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-19 04:39:16.000000 predibase-2023.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.927286 predibase-2023.7.9/predibase/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.927286 predibase-2023.7.9/predibase/cli_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/cli_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/connection_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/dataset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/deployment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/engine_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/llm_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/model_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/permission_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.927286 predibase-2023.7.9/predibase/pql/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/pql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/pql/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/pql/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/pql/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/query_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.931286 predibase-2023.7.9/predibase/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/connection_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/connection_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)    39312 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/resource_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/triton_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.927286 predibase-2023.7.9/predibase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-19 04:40:19.000000 predibase-2023.7.9/predibase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.931286 predibase-2023.7.9/predibase_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:40:19.931286 predibase-2023.7.9/predibase_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:39:16.000000 predibase-2023.7.9/predibase_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 04:40:19.000000 predibase-2023.7.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-19 04:39:16.000000 predibase-2023.7.9/requirements_predictor.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 04:40:19.931286 predibase-2023.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-19 04:39:16.000000 predibase-2023.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.871128 predibase-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-03 01:11:12.000000 predibase-2023.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 01:12:09.871128 predibase-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-03 01:11:12.000000 predibase-2023.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.855128 predibase-2023.8.1/predibase/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.863128 predibase-2023.8.1/predibase/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/cli_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/connection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/dataset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/deployment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/engine_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/llm_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/model_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/permission_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.863128 predibase-2023.8.1/predibase/pql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/pql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/pql/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/pql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/pql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/query_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.871128 predibase-2023.8.1/predibase/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/connection_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/connection_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/resource_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/triton_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.859128 predibase-2023.8.1/predibase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-03 01:12:09.000000 predibase-2023.8.1/predibase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.871128 predibase-2023.8.1/predibase_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:12:09.871128 predibase-2023.8.1/predibase_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:11:12.000000 predibase-2023.8.1/predibase_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-03 01:12:09.000000 predibase-2023.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-03 01:11:12.000000 predibase-2023.8.1/requirements_predictor.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 01:12:09.871128 predibase-2023.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-03 01:11:12.000000 predibase-2023.8.1/setup.py
```

### Comparing `predibase-2023.7.9/predibase/cli_commands/delete.py` & `predibase-2023.8.1/predibase/cli_commands/delete.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/cli_commands/deploy.py` & `predibase-2023.8.1/predibase/cli_commands/deploy.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,26 +34,32 @@
         DEFAULT_TEMPLATE,
         "--engine-template",
         "-e",
         prompt="Engine name",
         prompt_required=False,
         help="Optional engine template to provision for hosting the model",
     ),
-    # auto_suspend_secs: Optional[int] = 3600,  # TODO: add ability to auto suspend
+    auto_suspend_secs: Optional[int] = 3600,
 ):
     # raise ValueError if name is not lower case alphanumeric characters or '-'
     if re.match(r"^[a-z0-9-]+$", deployment_name) is None:
         raise ValueError("name must be lower case alphanumeric characters or '-'")
 
     client = get_client()
 
     get_console().print("Deploying an LLM with the following parameters:")
     get_console().print("\tdeployment_name:", deployment_name)
     get_console().print("\tmodel_name:", model_name)
     get_console().print("\tengine_template:", engine_template)
+    get_console().print("\tauto_suspend_secs:", auto_suspend_secs)
 
-    client.deploy_llm(deployment_name, model_name, engine_template=engine_template)
+    client.deploy_llm(
+        deployment_name,
+        model_name,
+        engine_template=engine_template,
+        scale_down_period=auto_suspend_secs,
+    )
     get_console().print("Deploy request sent.")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `predibase-2023.7.9/predibase/cli_commands/prompt.py` & `predibase-2023.8.1/predibase/cli_commands/prompt.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/cli_commands/settings.py` & `predibase-2023.8.1/predibase/cli_commands/settings.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/cli_commands/utils.py` & `predibase-2023.8.1/predibase/cli_commands/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any, Dict, Optional
 
 import yaml
 from rich.console import Console
 
 from predibase import PredibaseClient
 from predibase.pql.api import Session
+from predibase.resource.dataset import Dataset
 from predibase.resource.engine import Engine
 from predibase.resource.model import ModelRepo
 
 
 @dataclass
 class Defaults:
     repo: Optional[str] = None
@@ -29,28 +30,45 @@
     return PredibaseClient(session=defaults.session)
 
 
 def sanitize_engine_name(name: str) -> str:
     return name.replace("/", "-")
 
 
+def get_or_create_repo(repo_name: Optional[str] = None) -> ModelRepo:
+    repo_name = repo_name or defaults.repo
+    if repo_name is None:
+        raise ValueError("Repo name is required")
+    return get_client().create_model_repo(name=repo_name, exists_ok=True)
+
+
 def get_repo(repo_name: Optional[str] = None) -> ModelRepo:
     repo_name = repo_name or defaults.repo
     if repo_name is None:
         raise ValueError("Repo name is required")
     return get_client().get_model_repo(name=repo_name)
 
 
 def get_engine(engine_name: Optional[str] = None) -> Engine:
     engine_name = engine_name or defaults.engine
     if engine_name is None:
         raise ValueError("Engine name is required")
     return get_client().get_engine(name=engine_name)
 
 
+def get_dataset(dataset_name: Optional[str] = None) -> Dataset:
+    if dataset_name is None:
+        raise ValueError("Dataset name is required")
+
+    conn_name = None
+    if "/" in dataset_name:
+        conn_name, dataset_name = dataset_name.split("/")
+    return get_client().get_dataset(dataset_name=dataset_name, connection_name=conn_name)
+
+
 def set_defaults_from_settings(settings: Dict[str, Any]):
     global defaults
     defaults = Defaults(
         repo=settings.get("repo"),
         engine=settings.get("engine"),
         session=Session(token=settings.get("token"), url=settings.get("endpoint")),
     )
```

### Comparing `predibase-2023.7.9/predibase/client.py` & `predibase-2023.8.1/predibase/client.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/connection.py` & `predibase-2023.8.1/predibase/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/connection_mixin.py` & `predibase-2023.8.1/predibase/connection_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/dataset_mixin.py` & `predibase-2023.8.1/predibase/dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/deployment_mixin.py` & `predibase-2023.8.1/predibase/deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/engine_mixin.py` & `predibase-2023.8.1/predibase/engine_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/llm_mixin.py` & `predibase-2023.8.1/predibase/llm_mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 from typing import Dict, List, Optional, Union
 
 import pandas as pd
 
 from predibase.pql.api import Session
 from predibase.resource.connection import Connection
 from predibase.resource.dataset import Dataset
-from predibase.resource.llm import GeneratedResponse
+from predibase.util import sanitize_prompt
 
 
 class LlmMixin:
     session: Session
 
     def prompt(
         self,
         templates: Union[str, List[str]],
         model_name: Union[str, List[str]],
         index_name: Optional[Union[str, Dataset]] = None,
         dataset_name: Optional[Union[str, Dataset]] = None,
         limit: Optional[int] = None,
         options: Optional[Dict[str, float]] = None,
-        return_df: bool = False,
-    ) -> Union[List[GeneratedResponse], pd.DataFrame]:
+    ) -> pd.DataFrame:
         options_str = ", ".join(f"{k}={v}" for k, v in options.items()) if options else ""
         options_clause = f"WITH OPTIONS ({options_str}) " if options_str else ""
 
         models = [model_name] if isinstance(model_name, str) else model_name
         models_str = ", ".join(f'"{m}"' for m in models)
         model_clause = f"USING {models_str} " if models_str else ""
 
@@ -35,34 +34,41 @@
         dataset = self.get_dataset(dataset_name) if isinstance(dataset_name, str) else dataset_name
         limit_clause = f" LIMIT {limit}" if limit else ""
         given_clause = (
             f'GIVEN select * from "{dataset.connection.name}"."{dataset.name}"{limit_clause}' if dataset else ""
         )
 
         templates = [templates] if isinstance(templates, str) else templates
-        templates_str = ", ".join(f"'{t}'" for t in templates)
+        templates_str = ", ".join(f"'{sanitize_prompt(t)}'" for t in templates)
         query_str = f"PROMPT {templates_str} {options_clause}{model_clause}{index_clause}{given_clause};"
 
         conn_id = None
         if isinstance(dataset, Dataset):
             conn_id = dataset.connection_id
         elif isinstance(index, Dataset):
             conn_id = index.connection_id
         else:
             conn_id = self.list_connections()[0].id
 
         return self.session.execute(query_str, connection_id=conn_id)
 
-    def deploy_llm(self, deployment_name: str, model_name: str, engine_template: Optional[str] = None):
+    def deploy_llm(
+        self,
+        deployment_name: str,
+        model_name: str,
+        engine_template: Optional[str] = None,
+        scale_down_period=3600,
+    ):
         self.session.post_json(
             "/llms",
             json={
                 "name": deployment_name,
                 "modelName": model_name,
                 "engineTemplate": engine_template,
+                "scaleDownPeriod": scale_down_period,
             },
         )
 
     def delete_llm(self, deployment_name: str):
         self.session.delete_json(f"/llms/{deployment_name}")
 
     @abstractmethod
```

### Comparing `predibase-2023.7.9/predibase/model_mixin.py` & `predibase-2023.8.1/predibase/model_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/permission_mixin.py` & `predibase-2023.8.1/predibase/permission_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/pql/__init__.py` & `predibase-2023.8.1/predibase/pql/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/pql/adapter.py` & `predibase-2023.8.1/predibase/pql/adapter.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/pql/api.py` & `predibase-2023.8.1/predibase/pql/api.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/pql/utils.py` & `predibase-2023.8.1/predibase/pql/utils.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/predictor.py` & `predibase-2023.8.1/predibase/predictor.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/query_mixin.py` & `predibase-2023.8.1/predibase/query_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/config.py` & `predibase-2023.8.1/predibase/resource/config.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/connection.py` & `predibase-2023.8.1/predibase/resource/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/connection_object.py` & `predibase-2023.8.1/predibase/resource/connection_object.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/connection_properties.py` & `predibase-2023.8.1/predibase/resource/connection_properties.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/dataset.py` & `predibase-2023.8.1/predibase/resource/dataset.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/dataset_info.py` & `predibase-2023.8.1/predibase/resource/dataset_info.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/deployment.py` & `predibase-2023.8.1/predibase/resource/deployment.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/engine.py` & `predibase-2023.8.1/predibase/resource/engine.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/llm.py` & `predibase-2023.8.1/predibase/resource/llm.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/model.py` & `predibase-2023.8.1/predibase/resource/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -773,27 +773,31 @@
     def _wait_until_ready(self):
         """Utility function to wait until a model is fully ready, including evaluation and visualization steps.
         Certain operations may otherwise fail in a racy way.
 
         :param model: the Model to wait for.
         :return: None
         """
-        self.session.get_json_until(
-            f"/models/version/{self._id}",
-            lambda resp: resp["modelVersion"]["status"] == "ready"
-            or resp["modelVersion"]["status"] == "deploying"
-            or resp["modelVersion"]["status"] == "deployed"
-            or resp["modelVersion"]["status"] == "undeploying",
-            lambda resp: (
-                f"Failed to wait for ready model: status {resp['modelVersion']['status'].upper()} and error "
-                f"{resp['modelVersion']['errorText']}"
-            )
-            if resp["modelVersion"]["status"] in {"failed", "canceled"}
-            else None,
+        wait_until_model_ready(self._id, self.session)
+
+
+def wait_until_model_ready(model_id: int, session: Session) -> Dict[str, Any]:
+    return session.get_json_until(
+        f"/models/version/{model_id}",
+        lambda resp: resp["modelVersion"]["status"] == "ready"
+        or resp["modelVersion"]["status"] == "deploying"
+        or resp["modelVersion"]["status"] == "deployed"
+        or resp["modelVersion"]["status"] == "undeploying",
+        lambda resp: (
+            f"Failed to train model with status {resp['modelVersion']['status'].upper()} and error "
+            f"{resp['modelVersion']['errorText']}"
         )
+        if resp["modelVersion"]["status"] in {"failed", "canceled"}
+        else None,
+    )
 
 
 class ModelFuture:
     def __init__(self, version_id: int, session: Session):
         self.version_id = version_id
         self.session = session
 
@@ -810,21 +814,15 @@
         self.session.post_json(f"/models/version/{self.version_id}/cancel", {})
 
     def is_finished(self) -> bool:
         resp = self.session.get_json(f"/models/version/{self.version_id}")
         return resp["modelVersion"]["status"] in {"ready", "failed", "canceled"}
 
     def _wait_for_ready(self) -> Dict[str, Any]:
-        return self.session.get_json_until(
-            f"/models/version/{self.version_id}",
-            lambda resp: resp["modelVersion"]["completed"] is not None,
-            lambda resp: f"Failed to train model with status {resp['modelVersion']['status'].upper()}"
-            if resp["modelVersion"]["status"] in {"failed", "canceled"}
-            else None,
-        )
+        return wait_until_model_ready(self.version_id, self.session)
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
 class ModelDraft:
     session: Session
     dataset: Dataset
```

### Comparing `predibase-2023.7.9/predibase/resource/query.py` & `predibase-2023.8.1/predibase/resource/query.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource/user.py` & `predibase-2023.8.1/predibase/resource/user.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/resource_util.py` & `predibase-2023.8.1/predibase/resource_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/triton_util.py` & `predibase-2023.8.1/predibase/triton_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase/util.py` & `predibase-2023.8.1/predibase/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,18 @@
         url = session.url
         if "api." in url:
             url = url.replace("api.", "").replace("/v1", "")
         root_url = url
     return f"{root_url}/{endpoint}"
 
 
+def sanitize_prompt(prompt: str) -> str:
+    return prompt.replace("'", "''")
+
+
 class JSONFloat(float):
     def __repr__(self):
         return format(Decimal(self), "f")
 
 
 class ConfigEncoder:
     def decimalize(self, val):
```

### Comparing `predibase-2023.7.9/predibase.egg-info/SOURCES.txt` & `predibase-2023.8.1/predibase.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,18 @@
 predibase.egg-info/SOURCES.txt
 predibase.egg-info/dependency_links.txt
 predibase.egg-info/entry_points.txt
 predibase.egg-info/not-zip-safe
 predibase.egg-info/requires.txt
 predibase.egg-info/top_level.txt
 predibase/cli_commands/__init__.py
+predibase/cli_commands/create.py
 predibase/cli_commands/delete.py
 predibase/cli_commands/deploy.py
+predibase/cli_commands/list.py
 predibase/cli_commands/prompt.py
 predibase/cli_commands/settings.py
 predibase/cli_commands/utils.py
 predibase/pql/__init__.py
 predibase/pql/adapter.py
 predibase/pql/api.py
 predibase/pql/utils.py
```

### Comparing `predibase-2023.7.9/predibase_notebook/__init__.py` & `predibase-2023.8.1/predibase_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/predibase_notebook/env.py` & `predibase-2023.8.1/predibase_notebook/env.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.7.9/setup.py` & `predibase-2023.8.1/setup.py`

 * *Files identical despite different names*

