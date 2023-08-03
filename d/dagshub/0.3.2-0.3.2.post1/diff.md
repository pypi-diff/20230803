# Comparing `tmp/dagshub-0.3.2.tar.gz` & `tmp/dagshub-0.3.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagshub-0.3.2.tar", last modified: Tue Aug  1 15:11:17 2023, max compression
+gzip compressed data, was "dagshub-0.3.2.post1.tar", last modified: Thu Aug  3 07:46:05 2023, max compression
```

## Comparing `dagshub-0.3.2.tar` & `dagshub-0.3.2.post1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.338408 dagshub-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-01 15:11:06.000000 dagshub-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 15:11:06.000000 dagshub-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-08-01 15:11:17.334408 dagshub-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-08-01 15:11:06.000000 dagshub-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.322408 dagshub-0.3.2/dagshub/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.326408 dagshub-0.3.2/dagshub/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/auth/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/auth/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.326408 dagshub-0.3.2/dagshub/common/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.326408 dagshub-0.3.2/dagshub/common/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/api/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/api/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/rich_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.326408 dagshub-0.3.2/dagshub/data_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.326408 dagshub-0.3.2/dagshub/data_engine/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/annotation/voxel_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.330408 dagshub-0.3.2/dagshub/data_engine/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/client/data_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/client/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/client/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.330408 dagshub-0.3.2/dagshub/data_engine/client/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/client/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/client/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/client/loaders/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/client/loaders/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.330408 dagshub-0.3.2/dagshub/data_engine/client/query_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/client/query_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/datasources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.330408 dagshub-0.3.2/dagshub/data_engine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/model/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    28457 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/model/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/model/datasource_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/model/query_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.330408 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.322408 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.330408 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.330408 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.330408 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
--rw-r--r--   0 runner    (1001) docker     (123)   182256 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.334408 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/routes/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.334408 dagshub-0.3.2/dagshub/fastai/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/fastai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/fastai/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.334408 dagshub-0.3.2/dagshub/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/keras/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.334408 dagshub-0.3.2/dagshub/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/pytorch_lightning/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/pytorch_lightning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.334408 dagshub-0.3.2/dagshub/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/streaming/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/streaming/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    40226 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/streaming/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/streaming/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.334408 dagshub-0.3.2/dagshub/upload/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/upload/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26699 2023-08-01 15:11:06.000000 dagshub-0.3.2/dagshub/upload/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.326408 dagshub-0.3.2/dagshub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-08-01 15:11:17.000000 dagshub-0.3.2/dagshub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-08-01 15:11:17.000000 dagshub-0.3.2/dagshub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:11:17.000000 dagshub-0.3.2/dagshub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 15:11:17.000000 dagshub-0.3.2/dagshub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 15:11:17.000000 dagshub-0.3.2/dagshub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 15:11:17.000000 dagshub-0.3.2/dagshub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:11:17.338408 dagshub-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-01 15:11:06.000000 dagshub-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:11:17.334408 dagshub-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-01 15:11:06.000000 dagshub-0.3.2/tests/test_dagshub_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-01 15:11:06.000000 dagshub-0.3.2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-01 15:11:06.000000 dagshub-0.3.2/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.740729 dagshub-0.3.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-08-03 07:46:05.740729 dagshub-0.3.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.732729 dagshub-0.3.2.post1/dagshub/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.732729 dagshub-0.3.2.post1/dagshub/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/auth/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/auth/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.732729 dagshub-0.3.2.post1/dagshub/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.732729 dagshub-0.3.2.post1/dagshub/common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/api/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/rich_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.732729 dagshub-0.3.2.post1/dagshub/data_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.736729 dagshub-0.3.2.post1/dagshub/data_engine/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/annotation/voxel_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.736729 dagshub-0.3.2.post1/dagshub/data_engine/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/client/data_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/client/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/client/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.736729 dagshub-0.3.2.post1/dagshub/data_engine/client/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/client/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/client/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/client/loaders/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/client/loaders/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.736729 dagshub-0.3.2.post1/dagshub/data_engine/client/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/client/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/datasources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.736729 dagshub-0.3.2.post1/dagshub/data_engine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/model/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28457 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/model/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/model/datasource_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/model/query_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.736729 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.728729 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.736729 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.736729 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.736729 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   182256 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.740729 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/routes/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.740729 dagshub-0.3.2.post1/dagshub/fastai/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/fastai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/fastai/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.740729 dagshub-0.3.2.post1/dagshub/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/keras/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.740729 dagshub-0.3.2.post1/dagshub/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/pytorch_lightning/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/pytorch_lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.740729 dagshub-0.3.2.post1/dagshub/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/streaming/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/streaming/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40226 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/streaming/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/streaming/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.740729 dagshub-0.3.2.post1/dagshub/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/upload/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27582 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/dagshub/upload/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.732729 dagshub-0.3.2.post1/dagshub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-08-03 07:46:05.000000 dagshub-0.3.2.post1/dagshub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-08-03 07:46:05.000000 dagshub-0.3.2.post1/dagshub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 07:46:05.000000 dagshub-0.3.2.post1/dagshub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-03 07:46:05.000000 dagshub-0.3.2.post1/dagshub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-03 07:46:05.000000 dagshub-0.3.2.post1/dagshub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 07:46:05.000000 dagshub-0.3.2.post1/dagshub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 07:46:05.740729 dagshub-0.3.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 07:46:05.740729 dagshub-0.3.2.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/tests/test_dagshub_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-03 07:45:48.000000 dagshub-0.3.2.post1/tests/test_misc.py
```

### Comparing `dagshub-0.3.2/LICENSE` & `dagshub-0.3.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/PKG-INFO` & `dagshub-0.3.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.2
+Version: 0.3.2.post1
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.2 Summary: DagsHub client
-libraries Home-page: https://github.com/DagsHub/client Author: DagsHub Author-
-email: contact@dagshub.com Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.2.post1 Summary: DagsHub
+client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
+Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
+3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
 
 [![Tests](https://github.com/dagshub/client/actions/workflows/python-
 package.yml/badge.svg?branch=master)](https://github.com/DAGsHub/client/
 actions/workflows/python-package.yml) [![pip](https://img.shields.io/pypi/v/
```

### Comparing `dagshub-0.3.2/README.md` & `dagshub-0.3.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/auth/oauth.py` & `dagshub-0.3.2.post1/dagshub/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/auth/token_auth.py` & `dagshub-0.3.2.post1/dagshub/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/auth/tokens.py` & `dagshub-0.3.2.post1/dagshub/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/common/analytics.py` & `dagshub-0.3.2.post1/dagshub/common/analytics.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/common/api/repo.py` & `dagshub-0.3.2.post1/dagshub/common/api/repo.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/common/api/responses.py` & `dagshub-0.3.2.post1/dagshub/common/api/responses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/common/cli.py` & `dagshub-0.3.2.post1/dagshub/common/cli.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/common/config.py` & `dagshub-0.3.2.post1/dagshub/common/config.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/common/download.py` & `dagshub-0.3.2.post1/dagshub/common/download.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/common/helpers.py` & `dagshub-0.3.2.post1/dagshub/common/helpers.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/common/init.py` & `dagshub-0.3.2.post1/dagshub/common/init.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/common/logging_util.py` & `dagshub-0.3.2.post1/dagshub/common/logging_util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/common/util.py` & `dagshub-0.3.2.post1/dagshub/common/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/annotation/voxel_conversion.py` & `dagshub-0.3.2.post1/dagshub/data_engine/annotation/voxel_conversion.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/client/data_client.py` & `dagshub-0.3.2.post1/dagshub/data_engine/client/data_client.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/client/gql_mutations.py` & `dagshub-0.3.2.post1/dagshub/data_engine/client/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/client/gql_queries.py` & `dagshub-0.3.2.post1/dagshub/data_engine/client/gql_queries.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/client/loaders/base.py` & `dagshub-0.3.2.post1/dagshub/data_engine/client/loaders/base.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/client/loaders/tf.py` & `dagshub-0.3.2.post1/dagshub/data_engine/client/loaders/tf.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/client/loaders/torch.py` & `dagshub-0.3.2.post1/dagshub/data_engine/client/loaders/torch.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/client/models.py` & `dagshub-0.3.2.post1/dagshub/data_engine/client/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/client/query_builder/__init__.py` & `dagshub-0.3.2.post1/dagshub/data_engine/client/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/datasets.py` & `dagshub-0.3.2.post1/dagshub/data_engine/datasets.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/datasources.py` & `dagshub-0.3.2.post1/dagshub/data_engine/datasources.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/model/datapoint.py` & `dagshub-0.3.2.post1/dagshub/data_engine/model/datapoint.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/model/datasource.py` & `dagshub-0.3.2.post1/dagshub/data_engine/model/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/model/datasource_state.py` & `dagshub-0.3.2.post1/dagshub/data_engine/model/datasource_state.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/model/errors.py` & `dagshub-0.3.2.post1/dagshub/data_engine/model/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/model/query.py` & `dagshub-0.3.2.post1/dagshub/data_engine/model/query.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/model/query_result.py` & `dagshub-0.3.2.post1/dagshub/data_engine/model/query_result.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/app.py` & `dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/app.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/models.py` & `dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg` & `dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js` & `dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/routes/annotation.py` & `dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/routes/annotation.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/routes/datasource.py` & `dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/routes/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/routes/util.py` & `dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/routes/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/routes/voxel.py` & `dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/routes/voxel.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/server.py` & `dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/server.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/data_engine/voxel_plugin_server/utils.py` & `dagshub-0.3.2.post1/dagshub/data_engine/voxel_plugin_server/utils.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/fastai/logger.py` & `dagshub-0.3.2.post1/dagshub/fastai/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/keras/logger.py` & `dagshub-0.3.2.post1/dagshub/keras/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/logger.py` & `dagshub-0.3.2.post1/dagshub/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/notebook.py` & `dagshub-0.3.2.post1/dagshub/notebook.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/pytorch_lightning/logger.py` & `dagshub-0.3.2.post1/dagshub/pytorch_lightning/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/streaming/dataclasses.py` & `dagshub-0.3.2.post1/dagshub/streaming/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/streaming/filesystem.py` & `dagshub-0.3.2.post1/dagshub/streaming/filesystem.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/streaming/mount.py` & `dagshub-0.3.2.post1/dagshub/streaming/mount.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/upload/errors.py` & `dagshub-0.3.2.post1/dagshub/upload/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/dagshub/upload/wrapper.py` & `dagshub-0.3.2.post1/dagshub/upload/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import httpx
 import rich.progress
 import rich.status
 
 import dagshub.auth
 from dagshub.auth.token_auth import HTTPBearerAuth
 from dagshub.common import config, rich_console
-from dagshub.common.api.repo import RepoAPI
+from dagshub.common.api.repo import RepoAPI, BranchNotFoundError
 from dagshub.common.helpers import log_message
 from dagshub.upload.errors import determine_upload_api_error
 
 # todo: handle api urls in common package
 CONTENT_UPLOAD_URL = "api/v1/repos/{owner}/{reponame}/content/{branch}/{path}"
 FILES_UI_URL = "{owner}/{reponame}/src/{branch}/{path}"
 DEFAULT_COMMIT_MESSAGE = "Upload files using DagsHub client"
@@ -208,15 +208,16 @@
         self.branch = branch
 
         self._api = RepoAPI(f"{owner}/{name}", host=self.host, auth=self.auth)
 
         # For mirror uploading: store the last revision for which we uploaded
         # When the last revision changes, that means the sync has been complete and we can upload a new batch
         self._last_upload_revision: Optional[str] = None
-        self._last_upload_had_changes: bool = False
+        self._last_upload_had_changes = False
+        self._uploading_to_new_branch = False
 
         self.current_progress: Optional[rich.progress.Progress] = None
 
         if self.branch is None:
             logger.debug("Branch wasn't provided. Fetching default branch...")
             self.branch = self._api.default_branch
         logger.debug(f"Set branch: {self.branch}")
@@ -299,15 +300,26 @@
                     "new_branch_name": new_branch,
                 }
             )
         elif self._api.is_mirror:
             # If not uploading to a new branch, and we're in a mirror - wait for the sync to complete
             self._poll_mirror_up_to_date()
 
-        self._last_upload_revision = self._api.last_commit_sha(self.branch)
+        # Unset the new branch upload flag if it was set
+        # (do that only after mirror poll so commit 2 on a new branch pushes correctly)
+        if self._uploading_to_new_branch:
+            self._uploading_to_new_branch = False
+
+        try:
+            self._last_upload_revision = self._api.last_commit_sha(self.branch)
+        # New branch does not have a commit yet, so "last_upload_revision" will be None initially
+        # NOTE: checking for new_branch is not enough, because it doesn't take into account
+        # uploading to completely blank repos
+        except BranchNotFoundError:
+            self._uploading_to_new_branch = True
 
         if force:
             data["last_commit"] = self._last_upload_revision
 
         log_message(f'Uploading files ({len(files)}) to "{self._api.full_name}"...', logger)
         res = s.put(
             self.get_request_url(directory_path),
@@ -368,15 +380,16 @@
         When the revision changes, that means the sync has been completed and we can upload a new batch
         """
         if not self._api.is_mirror:
             return
 
         # Initial state - assume we can upload
         # Also can upload if last upload didn't have any changes
-        if self._last_upload_revision is None or not self._last_upload_had_changes:
+        if not self._uploading_to_new_branch and (
+            self._last_upload_revision is None or not self._last_upload_had_changes):
             return
 
         poll_interval = 1.0  # seconds
         poll_timeout = 600.0
         start_time = time.time()
 
         if self.current_progress is not None:
@@ -388,15 +401,20 @@
             status = rich.status.Status("Waiting for the mirror to sync", console=rich_console)
             status.start()
 
             def finish():
                 status.stop()
 
         while time.time() - start_time < poll_timeout:
-            new_revision = self._api.last_commit_sha(self.branch)
+            try:
+                new_revision = self._api.last_commit_sha(self.branch)
+            except BranchNotFoundError:
+                # New branch that didn't get back to DagsHub yet
+                time.sleep(poll_interval)
+                continue
             if new_revision == self._last_upload_revision:
                 time.sleep(poll_interval)
             else:
                 finish()
                 return
 
         finish()
```

### Comparing `dagshub-0.3.2/dagshub.egg-info/PKG-INFO` & `dagshub-0.3.2.post1/dagshub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.2
+Version: 0.3.2.post1
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.2 Summary: DagsHub client
-libraries Home-page: https://github.com/DagsHub/client Author: DagsHub Author-
-email: contact@dagshub.com Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.2.post1 Summary: DagsHub
+client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
+Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
+3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
 
 [![Tests](https://github.com/dagshub/client/actions/workflows/python-
 package.yml/badge.svg?branch=master)](https://github.com/DAGsHub/client/
 actions/workflows/python-package.yml) [![pip](https://img.shields.io/pypi/v/
```

### Comparing `dagshub-0.3.2/dagshub.egg-info/SOURCES.txt` & `dagshub-0.3.2.post1/dagshub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/setup.py` & `dagshub-0.3.2.post1/setup.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/tests/test_dagshub_logger.py` & `dagshub-0.3.2.post1/tests/test_dagshub_logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.2/tests/test_misc.py` & `dagshub-0.3.2.post1/tests/test_misc.py`

 * *Files identical despite different names*

