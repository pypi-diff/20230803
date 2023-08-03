# Comparing `tmp/cleanlab-studio-1.0.9.tar.gz` & `tmp/cleanlab-studio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.0.9.tar", last modified: Mon Jun 26 17:29:52 2023, max compression
+gzip compressed data, was "cleanlab-studio-1.1.0.tar", last modified: Thu Aug  3 00:01:10 2023, max compression
```

## Comparing `cleanlab-studio-1.0.9.tar` & `cleanlab-studio-1.1.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.569508 cleanlab-studio-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-06-26 17:29:52.569508 cleanlab-studio-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.561508 cleanlab-studio-1.0.9/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.561508 cleanlab-studio-1.0.9/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.561508 cleanlab-studio-1.0.9/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.561508 cleanlab-studio-1.0.9/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.565508 cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/schema_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/upload_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.565508 cleanlab-studio-1.0.9/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.565508 cleanlab-studio-1.0.9/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.565508 cleanlab-studio-1.0.9/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.565508 cleanlab-studio-1.0.9/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.565508 cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.565508 cleanlab-studio-1.0.9/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/studio/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/studio/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.561508 cleanlab-studio-1.0.9/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-06-26 17:29:52.000000 cleanlab-studio-1.0.9/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-26 17:29:52.000000 cleanlab-studio-1.0.9/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:29:52.000000 cleanlab-studio-1.0.9/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 17:29:52.000000 cleanlab-studio-1.0.9/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-26 17:29:52.000000 cleanlab-studio-1.0.9/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 17:29:52.000000 cleanlab-studio-1.0.9/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:29:52.569508 cleanlab-studio-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.565508 cleanlab-studio-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:52.569508 cleanlab-studio-1.0.9/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/tests/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/tests/datasets/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/tests/datasets/test_excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/tests/datasets/test_json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-26 17:29:35.000000 cleanlab-studio-1.0.9/tests/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.026109 cleanlab-studio-1.1.0/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.026109 cleanlab-studio-1.1.0/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.026109 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/schema_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.030110 cleanlab-studio-1.1.0/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/studio/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/studio/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/studio/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.026109 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 00:01:10.000000 cleanlab-studio-1.1.0/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 00:01:10.034110 cleanlab-studio-1.1.0/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/test_excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/test_json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-08-03 00:00:52.000000 cleanlab-studio-1.1.0/tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.0.9/LICENSE` & `cleanlab-studio-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/PKG-INFO` & `cleanlab-studio-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.9
+Version: 1.1.0
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
@@ -209,8 +209,19 @@
 
 The `datetime` type should be used for datetime strings, e.g. "2015-02-24 11:35:52 -0800", and Unix timestamps (which
 will be integers or floats). Datetime values must be parseable
 by [polars.from_epoch](https://pola-rs.github.io/polars/py-polars/html/reference/expressions/api/polars.from_epoch.html) for integer/floats or [polars.Expr.str.strptime](https://pola-rs.github.io/polars/py-polars/html/reference/expressions/api/polars.Expr.str.strptime.html) for strings.
 
 `version` indicates the version of the Cleanlab CLI package version used to generate the schema.
 
+## Other Resources
+
+- [Cleanlab Blog](https://cleanlab.ai/blog/) -- applications of Cleanlab Studio, case studies, feature announcements/explanations, ...
+- [Cleanlab Studio Audits](https://cleanlab.ai/blog/csa/) -- issues in famous datasets detected with Cleanlab Studio
+- [Slack Community](https://cleanlab.ai/slack/) -- ask questions, request features, discuss Data-Centric AI with others, ...
+- Need professional help? Reach out via email: team@cleanlab.ai
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/studio.png" width=80% height=80%>
+</p>
+
 [PyPI]: https://pypi.org/project/cleanlab-studio/
```

### Comparing `cleanlab-studio-1.0.9/README.md` & `cleanlab-studio-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -178,8 +178,19 @@
 
 The `datetime` type should be used for datetime strings, e.g. "2015-02-24 11:35:52 -0800", and Unix timestamps (which
 will be integers or floats). Datetime values must be parseable
 by [polars.from_epoch](https://pola-rs.github.io/polars/py-polars/html/reference/expressions/api/polars.from_epoch.html) for integer/floats or [polars.Expr.str.strptime](https://pola-rs.github.io/polars/py-polars/html/reference/expressions/api/polars.Expr.str.strptime.html) for strings.
 
 `version` indicates the version of the Cleanlab CLI package version used to generate the schema.
 
+## Other Resources
+
+- [Cleanlab Blog](https://cleanlab.ai/blog/) -- applications of Cleanlab Studio, case studies, feature announcements/explanations, ...
+- [Cleanlab Studio Audits](https://cleanlab.ai/blog/csa/) -- issues in famous datasets detected with Cleanlab Studio
+- [Slack Community](https://cleanlab.ai/slack/) -- ask questions, request features, discuss Data-Centric AI with others, ...
+- Need professional help? Reach out via email: team@cleanlab.ai
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/studio.png" width=80% height=80%>
+</p>
+
 [PyPI]: https://pypi.org/project/cleanlab-studio/
```

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/api_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,23 @@
 
 MAX_PARALLEL_UPLOADS = 32  # XXX choose this dynamically?
 INITIAL_BACKOFF = 0.25  # seconds
 MAX_RETRIES = 4
 
 
 def _construct_headers(
-    api_key: Optional[str], content_type: Optional[str] = "application/json"
+    api_key: Optional[str],
+    content_type: Optional[str] = "application/json",
 ) -> JSONDict:
     retval = dict()
     if api_key:
         retval["Authorization"] = f"bearer {api_key}"
     if content_type:
         retval["Content-Type"] = content_type
+    retval["Client-Type"] = "cli"
     return retval
 
 
 def handle_api_error(res: requests.Response, show_warning: bool = False) -> None:
     handle_api_error_from_json(res.json(), show_warning)
```

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/helpers.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/image_utils.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/image_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/schema_types.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/schema_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from cleanlab_studio.cli.decorators.auth_config import AuthConfig
 from cleanlab_studio.internal import api
 from cleanlab_studio.internal.dataset_source import FilepathDatasetSource
 from cleanlab_studio.internal.types import JSONDict
 
 
 @click.command(help="upload your dataset to Cleanlab Studio")
-@click.option(
-    "--filepath",
-    "-f",
+@click.argument(
+    "filepath",
     type=click.Path(),
-    help="Dataset filepath",
+    required=False,
+    default=None,
 )
 @click.option(
     "--schema_path",
     "-s",
     type=click.Path(),
     help="If uploading with a schema, specify the JSON schema filepath.",
 )
@@ -66,15 +66,15 @@
         proceed_upload = None
         if schema is None or schema.get("immutable", False):
             proceed_upload = True
         else:
             log(json.dumps(schema, indent=2))
             info(f"No schema was provided. We propose the above schema based on your dataset.")
 
-            proceed_upload = click.confirm("\nUse this schema?", default=None)
+            proceed_upload = click.confirm("\nUse this schema?", default=True)
             if not proceed_upload:
                 info(
                     "Proposed schema rejected. Please submit your own schema using --schema.\n",
                 )
 
             save_filepath = click_helpers.confirm_save_prompt_filepath(
                 save_message="Save the generated schema?",
```

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/upload_helpers.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/dataset/upload_types.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/dataset/upload_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.1.0/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/errors.py` & `cleanlab-studio-1.1.0/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-1.1.0/cleanlab_studio/internal/api/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,48 @@
+import io
 import os
 import time
-from typing import Any, Callable, List, Optional, Tuple, Dict
+from typing import Callable, cast, List, Optional, Tuple, Dict, Union, Any
 from cleanlab_studio.errors import APIError
 
 import requests
 from tqdm import tqdm
 import pandas as pd
+import numpy as np
+import numpy.typing as npt
+
+try:
+    import pyspark.sql
+
+    pyspark_exists = True
+except ImportError:
+    pyspark_exists = False
 
 from cleanlab_studio.internal.types import JSONDict
 from cleanlab_studio.version import __version__
 
+
 base_url = os.environ.get("CLEANLAB_API_BASE_URL", "https://api.cleanlab.ai/api")
 cli_base_url = f"{base_url}/cli/v0"
 upload_base_url = f"{base_url}/upload/v0"
 dataset_base_url = f"{base_url}/datasets"
 project_base_url = f"{base_url}/projects"
 cleanset_base_url = f"{base_url}/cleansets"
+model_base_url = f"{base_url}/v1/deployment"
 
 
 def _construct_headers(
     api_key: Optional[str], content_type: Optional[str] = "application/json"
 ) -> JSONDict:
     retval = dict()
     if api_key:
         retval["Authorization"] = f"bearer {api_key}"
     if content_type:
         retval["Content-Type"] = content_type
+    retval["Client-Type"] = "python-api"
     return retval
 
 
 def handle_api_error(res: requests.Response) -> None:
     handle_api_error_from_json(res.json())
 
 
@@ -149,33 +162,70 @@
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
     label_column: str = res.json()["label_column"]
     return label_column
 
 
-def download_cleanlab_columns(api_key: str, cleanset_id: str, all: bool = False) -> pd.DataFrame:
+def download_cleanlab_columns(
+    api_key: str,
+    cleanset_id: str,
+    all: bool = True,
+    to_spark: bool = False,
+) -> Any:
     """
     Download all rows from specified Cleanlab columns
 
     :param api_key:
     :param cleanset_id:
     :param all: whether to download all Cleanlab columns or just the clean_label column
-    :return: return (rows, id_column)
+    :return: return a dataframe, either pandas or spark. Type is Any because don't want to require spark installed
     """
     res = requests.get(
-        cli_base_url + f"/cleansets/{cleanset_id}/columns?all={all}",
+        cli_base_url + f"/cleansets/{cleanset_id}/columns",
+        params=dict(to_spark=to_spark, all=all),
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
-    cleanset_json: str = res.json()["cleanset_json"]
-    cleanset_df: pd.DataFrame = pd.read_json(cleanset_json, orient="table")
     id_col = get_id_column(api_key, cleanset_id)
-    cleanset_df.rename(columns={"id": id_col}, inplace=True)
-    return cleanset_df
+    cleanset_json: str = res.json()["cleanset_json"]
+    if to_spark:
+        if not pyspark_exists:
+            raise ImportError(
+                "pyspark is not installed. Please install pyspark to download cleanlab columns as a pyspark DataFrame."
+            )
+        from pyspark.sql import SparkSession
+
+        spark = SparkSession.builder.getOrCreate()
+        rdd = spark.sparkContext.parallelize([cleanset_json])
+        cleanset_pyspark: pyspark.sql.DataFrame = spark.read.json(rdd)
+        cleanset_pyspark = cleanset_pyspark.withColumnRenamed("id", id_col)
+        return cleanset_pyspark
+
+    cleanset_pd: pd.DataFrame = pd.read_json(cleanset_json, orient="table")
+    cleanset_pd.rename(columns={"id": id_col}, inplace=True)
+    return cleanset_pd
+
+
+def download_array(
+    api_key: str, cleanset_id: str, name: str
+) -> Union[npt.NDArray[np.float_], pd.DataFrame]:
+    res = requests.get(
+        cli_base_url + f"/cleansets/{cleanset_id}/{name}",
+        headers=_construct_headers(api_key),
+    )
+    handle_api_error(res)
+    res_json: JSONDict = res.json()
+    if res_json["success"]:
+        if res_json["array_type"] == "numpy":
+            np_data: npt.NDArray[np.float_] = np.array(res_json[name])
+            return np_data
+        pd_data: pd.DataFrame = pd.read_json(res_json[name], orient="records")
+        return pd_data
+    raise APIError(f"{name} for cleanset {cleanset_id} not found")
 
 
 def get_id_column(api_key: str, cleanset_id: str) -> str:
     res = requests.get(
         cli_base_url + f"/cleansets/{cleanset_id}/id_column",
         headers=_construct_headers(api_key),
     )
@@ -279,7 +329,45 @@
             if res["status"] == "error":
                 raise APIError(res["error_message"])
             pbar.update(float(res["progress"]) - pbar.n)
             time.sleep(0.5)
             res = request_function(progress_id)
         pbar.update(float(1) - pbar.n)
     return res
+
+
+def upload_predict_batch(api_key: str, model_id: str, batch: io.StringIO) -> str:
+    """Uploads prediction batch and returns query ID."""
+    url = f"{model_base_url}/{model_id}/upload"
+    res = requests.post(
+        url,
+        headers=_construct_headers(api_key),
+    )
+
+    handle_api_error(res)
+    presigned_url = res.json()["upload_url"]
+    query_id: str = res.json()["query_id"]
+
+    requests.post(presigned_url["url"], data=presigned_url["fields"], files={"file": batch})
+
+    return query_id
+
+
+def start_prediction(api_key: str, model_id: str, query_id: str) -> None:
+    """Starts prediction for query."""
+    res = requests.post(
+        f"{model_base_url}/{model_id}/predict/{query_id}",
+        headers=_construct_headers(api_key),
+    )
+
+    handle_api_error(res)
+
+
+def get_prediction_status(api_key: str, query_id: str) -> Dict[str, str]:
+    """Gets status of model prediction query. Returns status, and optionally the result url or error message."""
+    res = requests.get(
+        f"{model_base_url}/predict/{query_id}",
+        headers=_construct_headers(api_key),
+    )
+    handle_api_error(res)
+
+    return cast(Dict[str, str], res.json())
```

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 from typing import Any, Optional
 
 from .dataset_source import DatasetSource
 
 
 class FilepathDatasetSource(DatasetSource):
     def __init__(
-        self, *args: Any, filepath: pathlib.Path, dataset_name: Optional[str] = None, **kwargs: Any
+        self,
+        *args: Any,
+        filepath: pathlib.Path,
+        dataset_name: Optional[str] = None,
+        **kwargs: Any,
     ):
         super().__init__(*args, **kwargs)
         self.dataset_name = dataset_name if dataset_name is not None else filepath.name
         self.file_size = filepath.stat().st_size
-        maybe_file_type = mimetypes.guess_type(self.dataset_name)[0]
+        maybe_file_type = mimetypes.guess_type(filepath)[0]
         if maybe_file_type is None:
             raise ValueError(
                 f"Could not identify type of file at {filepath}. Make sure file name has valid extension"
             )
         self.file_type = maybe_file_type
         self._filepath = filepath
```

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-1.1.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/internal/settings.py` & `cleanlab-studio-1.1.0/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-1.1.0/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/internal/util.py` & `cleanlab-studio-1.1.0/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/studio/clean.py` & `cleanlab-studio-1.1.0/cleanlab_studio/studio/clean.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/studio/studio.py` & `cleanlab-studio-1.1.0/cleanlab_studio/studio/studio.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-from typing import Any, List, Literal, Optional
+"""
+Python API for Cleanlab Studio.
+"""
+from typing import Any, List, Literal, Optional, Union
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
-try:
-    import pyspark.sql
-
-    pyspark_exists = True
-except ImportError:
-    pyspark_exists = False
-
-from . import clean, upload
+from . import clean, upload, inference
 from cleanlab_studio.internal.api import api
-from cleanlab_studio.internal.util import init_dataset_source, check_none, check_not_none
+from cleanlab_studio.internal.util import (
+    init_dataset_source,
+    check_none,
+    check_not_none,
+)
 from cleanlab_studio.internal.settings import CleanlabSettings
 from cleanlab_studio.internal.types import FieldSchemaDict
 
+_pyspark_exists = api.pyspark_exists
+if _pyspark_exists:
+    import pyspark.sql
+
 
 class Studio:
+    """Used to interact with Cleanlab Studio."""
+
     _api_key: str
 
     def __init__(self, api_key: Optional[str]):
         if not api.is_valid_client_version():
             raise ValueError(
                 "CLI is out of date and must be updated. Run 'pip install --upgrade cleanlab-studio'."
             )
@@ -33,67 +39,108 @@
                     raise ValueError
             except (FileNotFoundError, KeyError, ValueError):
                 raise ValueError(
                     "No API key found; either specify API key or log in with 'cleanlab login' first"
                 )
         api.validate_api_key(api_key)
         self._api_key = api_key
+        self.experimental = self.Experimental(self)  # type: ignore
 
     def upload_dataset(
         self,
         dataset: Any,
         dataset_name: Optional[str] = None,
         *,
         schema_overrides: Optional[FieldSchemaDict] = None,
         modality: Optional[str] = None,
         id_column: Optional[str] = None,
     ) -> str:
+        """
+        Uploads a dataset to Cleanlab Studio.
+
+        Args:
+            dataset: Object representing the dataset to upload. Currently supported formats include a `str` path to your dataset, a pandas DataFrame, a pyspark DataFrame.
+            dataset_name: Name for your dataset in Cleanlab Studio (optional if uploading from filepath).
+            schema_overrides: Optional dictionary of overrides you would like to make to the schema of your dataset. If not provided, schema will be inferred.
+            modality: Optional parameter to override the modality of your dataset. If not provided, modality will be inferred.
+            id_column: Optional parameter to override the ID column of your dataset. If not provided, a monotonically increasing ID column will be generated.
+
+        Returns:
+            ID of uploaded dataset.
+        """
         ds = init_dataset_source(dataset, dataset_name)
         return upload.upload_dataset(
             self._api_key,
             ds,
             schema_overrides=schema_overrides,
             modality=modality,
             id_column=id_column,
         )
 
     def download_cleanlab_columns(
         self,
         cleanset_id: str,
         include_action: bool = False,
-    ) -> pd.DataFrame:
-        rows_df: pd.DataFrame = api.download_cleanlab_columns(self._api_key, cleanset_id, all=True)
+        to_spark: bool = False,
+    ) -> Any:
+        """
+        Downloads Cleanlab columns for a cleanset.
+
+        Args:
+            cleanset_id: ID of cleanset to download columns from. To obtain cleanset ID from project ID use, [get_latest_cleanset_id](#method-get_latest_cleanset_id).
+            include_action: Whether to include a column with any actions taken on the cleanset in the downloaded columns.
+
+        Returns:
+            A pandas or pyspark DataFrame. Type is `Any` to avoid requiring pyspark installation.
+        """
+        rows_df = api.download_cleanlab_columns(
+            self._api_key, cleanset_id, all=True, to_spark=to_spark
+        )
         if not include_action:
-            rows_df.drop("action", inplace=True, axis=1)
+            if to_spark:
+                rows_df = rows_df.drop("action")
+            else:
+                rows_df.drop("action", inplace=True, axis=1)
         return rows_df
 
-    def apply_corrections(self, cleanset_id: str, dataset: Any) -> Any:
+    def apply_corrections(self, cleanset_id: str, dataset: Any, keep_excluded: bool = False) -> Any:
+        """
+        Applies corrections from a Cleanlab Studio cleanset to your dataset. Corrections can be made by viewing your project in the Cleanlab Studio webapp (see [Cleanlab Studio web quickstart](/guide/quickstart/web#review-the-errors)).
+
+        Args:
+            cleanset_id: ID of cleanset to apply corrections from.
+            dataset: Dataset to apply corrections to. Supported formats include pandas DataFrame and pyspark DataFrame. Dataset should have the same number of rows as the dataset used to create the project. It should also contain a label column with the same name as the label column for the project.
+            keep_excluded: Whether to retain rows with an "exclude" action. By default these rows will be removed from the dataset.
+
+        Returns:
+            A copy of the dataset with corrections applied.
+        """
         project_id = api.get_project_of_cleanset(self._api_key, cleanset_id)
         label_column = api.get_label_column_of_project(self._api_key, project_id)
         id_col = api.get_id_column(self._api_key, cleanset_id)
-        cl_cols = self.download_cleanlab_columns(cleanset_id, include_action=True)
-        if pyspark_exists and isinstance(dataset, pyspark.sql.DataFrame):
+        if _pyspark_exists and isinstance(dataset, pyspark.sql.DataFrame):
             from pyspark.sql.functions import udf
 
-            spark = dataset.sparkSession
-            cl_cols_df = spark.createDataFrame(cl_cols)
-            corrected_ds = dataset.alias("corrected_ds")
-            if id_col not in corrected_ds.columns:
+            cl_cols = self.download_cleanlab_columns(
+                cleanset_id, include_action=True, to_spark=True
+            )
+            corrected_ds_spark = dataset.alias("corrected_ds")
+            if id_col not in corrected_ds_spark.columns:
                 from pyspark.sql.functions import (
                     row_number,
                     monotonically_increasing_id,
                 )
                 from pyspark.sql.window import Window
 
-                corrected_ds = corrected_ds.withColumn(
+                corrected_ds_spark = corrected_ds_spark.withColumn(
                     id_col,
                     row_number().over(Window.orderBy(monotonically_increasing_id())) - 1,
                 )
-            both = cl_cols_df.select([id_col, "action", "clean_label"]).join(
-                corrected_ds.select([id_col, label_column]),
+            both = cl_cols.select([id_col, "action", "clean_label"]).join(
+                corrected_ds_spark.select([id_col, label_column]),
                 on=id_col,
                 how="left",
             )
             final = both.withColumn(
                 "__cleanlab_final_label",
                 # XXX hacky, checks if label is none by hand
                 # instead, use original JSON, which uses null values where it's not specified
@@ -102,33 +149,37 @@
                     "clean_label",
                 ),
             )
             new_labels = final.select(
                 [id_col, "action", "__cleanlab_final_label"]
             ).withColumnRenamed("__cleanlab_final_label", label_column)
             return (
-                corrected_ds.drop(label_column)
+                corrected_ds_spark.drop(label_column)
                 .join(new_labels, on=id_col, how="right")
                 .where(new_labels["action"] != "exclude")
                 .drop("action")
             )
         elif isinstance(dataset, pd.DataFrame):
+            cl_cols = self.download_cleanlab_columns(cleanset_id, include_action=True)
             joined_ds: pd.DataFrame
             if id_col in dataset.columns:
                 joined_ds = dataset.join(cl_cols.set_index(id_col), on=id_col)
             else:
                 joined_ds = dataset.join(cl_cols.set_index(id_col).sort_values(by=id_col))
             joined_ds["__cleanlab_final_label"] = joined_ds["clean_label"].where(
                 np.asarray(list(map(check_not_none, joined_ds["clean_label"].to_numpy()))),
                 dataset[label_column].to_numpy(),
             )
 
-            corrected_ds = dataset.copy()
+            corrected_ds: pd.DataFrame = dataset.copy()
             corrected_ds[label_column] = joined_ds["__cleanlab_final_label"]
-            corrected_ds = corrected_ds.loc[joined_ds["action"] != "exclude"]
+            if not keep_excluded:
+                corrected_ds = corrected_ds.loc[(joined_ds["action"] != "exclude").fillna(True)]
+            else:
+                corrected_ds["action"] = joined_ds["action"]
             return corrected_ds
 
         else:
             raise ValueError(
                 f"Provided unsupported dataset of type: {type(dataset)}. We currently support applying corrections to pandas or pyspark dataframes"
             )
 
@@ -141,26 +192,28 @@
         task_type: Literal["multi-class", "multi-label"] = "multi-class",
         model_type: Literal["fast", "regular"] = "regular",
         label_column: Optional[str] = None,
         feature_columns: Optional[List[str]] = None,
         text_column: Optional[str] = None,
     ) -> str:
         """
-        Creates a Cleanlab Studio project
+        Creates a Cleanlab Studio project.
 
-        :param dataset_id: ID of dataset to create project for
-        :param project_name: name for resulting project
-        :param modality: modality of project (i.e. text, tabular, image)
-        :keyword task_type: type of classification to perform (i.e. multi-class, multi-label)
-        :keyword model_type: type of model to train (i.e. fast, regular)
-        :keyword label_column: name of column in dataset containing labels (if not supplied, we'll make our best guess)
-        :keyword feature_columns: list of columns to use as features when training tabular modality project (if not supplied and modality is "tabular" we'll use all valid feature columns)
-        :keyword text_column: name of column containing the text to train text modality project on (if not supplied and modality is "text" we'll make our best guess)
+        Args:
+            dataset_id: ID of dataset to create project for.
+            project_name: Name for resulting project.
+            modality: Modality of project (i.e. text, tabular, image).
+            task_type: Type of classification to perform (i.e. multi-class, multi-label).
+            model_type: Type of model to train (i.e. fast, regular).
+            label_column: Name of column in dataset containing labels (if not supplied, we'll make our best guess).
+            feature_columns: List of columns to use as features when training tabular modality project (if not supplied and modality is "tabular" we'll use all valid feature columns).
+            text_column: Name of column containing the text to train text modality project on (if not supplied and modality is "text" we'll make our best guess).
 
-        :return: ID of project
+        Returns:
+            ID of created project.
         """
         dataset_details = api.get_dataset_details(self._api_key, dataset_id)
 
         if label_column is not None:
             if label_column not in dataset_details["label_columns"]:
                 raise ValueError(
                     f"Invalid label column: {label_column}. Label column must have categorical feature type"
@@ -200,21 +253,76 @@
             label_column=label_column,
             feature_columns=feature_columns if feature_columns is not None else [],
             text_column=text_column,
         )
 
     def poll_cleanset_status(self, cleanset_id: str, timeout: Optional[int] = None) -> bool:
         """
-        Polls for cleanset status. Blocks until cleanset is ready, there is a cleanset error, or `timeout` is exceeded
+        Repeatedly polls for cleanset status while the cleanset is being generated. Blocks until cleanset is ready, there is a cleanset error, or `timeout` is exceeded.
+
+        Args:
+            cleanset_id: ID of cleanset to check status of.
+            timeout: Optional timeout after which to stop polling for progress. If not provided, will block until cleanset is ready.
 
-        :return: True if cleanset is ready, False otherwise
+        Returns:
+            After cleanset is done being generated, returns `True` if cleanset is ready to use, `False` otherwise.
         """
         return clean.poll_cleanset_status(self._api_key, cleanset_id, timeout)
 
     def get_latest_cleanset_id(self, project_id: str) -> str:
-        """Gets latest cleanset ID for a project"""
+        """
+        Gets latest cleanset ID for a project.
+
+        Args:
+            project_id: ID of project.
+
+        Returns:
+            ID of latest associated cleanset.
+        """
         return api.get_latest_cleanset_id(self._api_key, project_id)
 
     def delete_project(self, project_id: str) -> None:
-        """Deletes project with given ID"""
+        """
+        Deletes a project from Cleanlab Studio.
+
+        Args:
+            project_id: ID of project to delete.
+        """
         api.delete_project(self._api_key, project_id)
         print(f"Successfully deleted project: {project_id}")
+
+    def get_model(self, model_id: str) -> inference.Model:
+        """
+        Gets a model deployed by Cleanlab Studio.
+
+        Args:
+            model_id: ID of model to get. This ID should be fetched in the deployments page of the app UI.
+
+        Returns:
+            Model object with methods to run predictions on new input data
+        """
+        return inference.Model(self._api_key, model_id)
+
+    class Experimental:
+        def __init__(self, outer):  # type: ignore
+            self._outer = outer
+
+        def download_pred_probs(
+            self,
+            cleanset_id: str,
+        ) -> Union[npt.NDArray[np.float_], pd.DataFrame]:
+            """
+            Downloads predicted probabilities for a cleanset
+            Old pred_probs were saved as numpy arrays, which is still compatible
+            Newer pred_probs are saved as pd.DataFrames
+            """
+            return api.download_array(self._outer._api_key, cleanset_id, "pred_probs")
+
+        def download_embeddings(
+            self,
+            cleanset_id: str,
+        ) -> Union[npt.NDArray[np.float_], pd.DataFrame]:
+            """
+            Downloads embeddings for a cleanset
+            The downloaded array will always be a numpy array, the above is just for typing purposes
+            """
+            return api.download_array(self._outer._api_key, cleanset_id, "embeddings")
```

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio/studio/upload.py` & `cleanlab-studio-1.1.0/cleanlab_studio/studio/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-1.1.0/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.9
+Version: 1.1.0
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://cleanlab-studio.readthedocs.io/en/latest/index.html
@@ -209,8 +209,19 @@
 
 The `datetime` type should be used for datetime strings, e.g. "2015-02-24 11:35:52 -0800", and Unix timestamps (which
 will be integers or floats). Datetime values must be parseable
 by [polars.from_epoch](https://pola-rs.github.io/polars/py-polars/html/reference/expressions/api/polars.from_epoch.html) for integer/floats or [polars.Expr.str.strptime](https://pola-rs.github.io/polars/py-polars/html/reference/expressions/api/polars.Expr.str.strptime.html) for strings.
 
 `version` indicates the version of the Cleanlab CLI package version used to generate the schema.
 
+## Other Resources
+
+- [Cleanlab Blog](https://cleanlab.ai/blog/) -- applications of Cleanlab Studio, case studies, feature announcements/explanations, ...
+- [Cleanlab Studio Audits](https://cleanlab.ai/blog/csa/) -- issues in famous datasets detected with Cleanlab Studio
+- [Slack Community](https://cleanlab.ai/slack/) -- ask questions, request features, discuss Data-Centric AI with others, ...
+- Need professional help? Reach out via email: team@cleanlab.ai
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/studio.png" width=80% height=80%>
+</p>
+
 [PyPI]: https://pypi.org/project/cleanlab-studio/
```

### Comparing `cleanlab-studio-1.0.9/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.1.0/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
 cleanlab_studio/internal/dataset_source/dataset_source.py
 cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
 cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
 cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
 cleanlab_studio/studio/__init__.py
 cleanlab_studio/studio/clean.py
+cleanlab_studio/studio/inference.py
 cleanlab_studio/studio/studio.py
 cleanlab_studio/studio/upload.py
 tests/__init__.py
 tests/datasets/__init__.py
 tests/datasets/constants.py
 tests/datasets/test_csv_dataset.py
 tests/datasets/test_excel_dataset.py
```

### Comparing `cleanlab-studio-1.0.9/setup.py` & `cleanlab-studio-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,26 +42,27 @@
     ],
     keywords="cleanlab",
     packages=find_packages(exclude=[]),
     py_modules=["main"],
     python_requires=">=3.8",
     install_requires=[
         "aiohttp>=3.8.1",
-        "Click>=8.1.0",
+        "Click>=8.1.0,<=8.1.3",
         "colorama>=0.4.4",
-        "pandas>=1.0.0",
+        "pandas==2.*",
         "pyexcel>=0.7.0",
         "pyexcel-xls>=0.7.0",
         "pyexcel-xlsx>=0.6.0",
         "requests>=2.27.1",
         "tqdm>=4.64.0",
         "ijson>=3.1.4",
         "jsonstreams>=0.6.0",
         "semver>=2.13.0,<3.0.0",
         "Pillow>=9.2.0",
+        "typing_extensions==4.2.0",
         "openpyxl==3.0.10",
         "validators>=0.20.0",
     ],
     extras_require={
         "docs": [
             "sphinx==6.2.1",
             "sphinx_toolbox==3.4.0",
```

### Comparing `cleanlab-studio-1.0.9/tests/datasets/test_csv_dataset.py` & `cleanlab-studio-1.1.0/tests/datasets/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/tests/datasets/test_excel_dataset.py` & `cleanlab-studio-1.1.0/tests/datasets/test_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/tests/datasets/test_json_dataset.py` & `cleanlab-studio-1.1.0/tests/datasets/test_json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.9/tests/datasets/utils.py` & `cleanlab-studio-1.1.0/tests/datasets/utils.py`

 * *Files identical despite different names*

