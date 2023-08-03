# Comparing `tmp/unify-cli-3.5.1.tar.gz` & `tmp/unify-cli-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unify-cli-3.5.1.tar", last modified: Wed Jul 12 19:28:41 2023, max compression
+gzip compressed data, was "dist/unify-cli-3.5.2.tar", last modified: Thu Aug  3 17:05:15 2023, max compression
```

## Comparing `unify-cli-3.5.1.tar` & `unify-cli-3.5.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2023-07-12 19:28:17.000000 unify-cli-3.5.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11718 2023-07-12 19:28:41.000000 unify-cli-3.5.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11321 2023-07-12 19:28:17.000000 unify-cli-3.5.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-12 19:28:41.000000 unify-cli-3.5.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3562 2023-07-12 19:28:17.000000 unify-cli-3.5.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/access/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/access/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2677 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/access/commands.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2293 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/ah.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/cluster/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/cluster/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/cluster/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/common/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/common/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/dataset/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/dataset/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4854 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/dataset/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/datastream/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/datastream/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4429 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/datastream/commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   485294 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/datastream/tags.csv
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/graph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/graph/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/graph/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/hierarchy/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/hierarchy/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2474 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/hierarchy/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/org/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/org/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4929 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/org/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/permissions/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/permissions/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2750 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/permissions/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/permissions/rules/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/permissions/rules/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4854 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/permissions/rules/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/permissions/selectors/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/permissions/selectors/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2209 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/permissions/selectors/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/pipeline/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1677 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/pipeline/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/template/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/template/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1281 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/template/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/user/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/user/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8891 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/user/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/utils/util_methods.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/source/workflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/workflow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9700 2023-07-12 19:28:17.000000 unify-cli-3.5.1/source/workflow/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2289 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/data_test.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1408 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/properties.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2040 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_asset_access.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3585 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_cluster_command.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4264 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_datasets_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2520 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_graph_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_help.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      209 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_org_command.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_pipeline_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1931 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_templates_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4946 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_user_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4061 2023-07-12 19:28:17.000000 unify-cli-3.5.1/tests/test_workflow_commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 19:28:41.000000 unify-cli-3.5.1/unify_cli.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11718 2023-07-12 19:28:41.000000 unify-cli-3.5.1/unify_cli.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1585 2023-07-12 19:28:41.000000 unify-cli-3.5.1/unify_cli.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-12 19:28:41.000000 unify-cli-3.5.1/unify_cli.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-07-12 19:28:41.000000 unify-cli-3.5.1/unify_cli.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-07-12 19:28:41.000000 unify-cli-3.5.1/unify_cli.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-12 19:28:41.000000 unify-cli-3.5.1/unify_cli.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2023-08-03 17:04:50.000000 unify-cli-3.5.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11718 2023-08-03 17:05:15.000000 unify-cli-3.5.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11321 2023-08-03 17:04:50.000000 unify-cli-3.5.2/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-03 17:05:15.000000 unify-cli-3.5.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3562 2023-08-03 17:04:50.000000 unify-cli-3.5.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/access/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/access/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2677 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/access/commands.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2293 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/ah.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/cluster/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/cluster/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/cluster/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/common/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/common/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/dataset/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/dataset/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4854 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/dataset/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/datastream/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/datastream/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4429 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/datastream/commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   485294 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/datastream/tags.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/graph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/graph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/graph/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/hierarchy/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/hierarchy/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2474 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/hierarchy/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/org/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/org/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4929 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/org/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/permissions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/permissions/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2750 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/permissions/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/permissions/rules/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/permissions/rules/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4854 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/permissions/rules/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/permissions/selectors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/permissions/selectors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2209 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/permissions/selectors/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/pipeline/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1677 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/pipeline/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/template/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/template/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1281 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/template/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/user/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/user/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8891 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/user/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/utils/util_methods.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/source/workflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/workflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9700 2023-08-03 17:04:50.000000 unify-cli-3.5.2/source/workflow/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2289 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/data_test.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1408 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/properties.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2040 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_asset_access.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3585 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_cluster_command.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4264 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_datasets_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2520 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_graph_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_help.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      209 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_org_command.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_pipeline_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1931 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_templates_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4946 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_user_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4061 2023-08-03 17:04:50.000000 unify-cli-3.5.2/tests/test_workflow_commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 17:05:15.000000 unify-cli-3.5.2/unify_cli.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11718 2023-08-03 17:05:14.000000 unify-cli-3.5.2/unify_cli.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1585 2023-08-03 17:05:15.000000 unify-cli-3.5.2/unify_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 17:05:14.000000 unify-cli-3.5.2/unify_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-08-03 17:05:14.000000 unify-cli-3.5.2/unify_cli.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-08-03 17:05:14.000000 unify-cli-3.5.2/unify_cli.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-08-03 17:05:14.000000 unify-cli-3.5.2/unify_cli.egg-info/top_level.txt
```

### Comparing `unify-cli-3.5.1/LICENSE` & `unify-cli-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/PKG-INFO` & `unify-cli-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-cli
-Version: 3.5.1
+Version: 3.5.2
 Summary: Element Unify command line tool
 Home-page: https://github.com/ElementAnalytics/element-unify-cli
 Author: Element Analytics
 Author-email: platform@ean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3
```

### Comparing `unify-cli-3.5.1/README.md` & `unify-cli-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/setup.py` & `unify-cli-3.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/access/commands.py` & `unify-cli-3.5.2/source/access/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/ah.py` & `unify-cli-3.5.2/source/ah.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/cluster/commands.py` & `unify-cli-3.5.2/source/cluster/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/common/commands.py` & `unify-cli-3.5.2/source/common/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/dataset/commands.py` & `unify-cli-3.5.2/source/dataset/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/datastream/commands.py` & `unify-cli-3.5.2/source/datastream/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/datastream/tags.csv` & `unify-cli-3.5.2/source/datastream/tags.csv`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/graph/commands.py` & `unify-cli-3.5.2/source/graph/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/hierarchy/commands.py` & `unify-cli-3.5.2/source/hierarchy/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/org/commands.py` & `unify-cli-3.5.2/source/org/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/permissions/commands.py` & `unify-cli-3.5.2/source/permissions/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/permissions/rules/commands.py` & `unify-cli-3.5.2/source/permissions/rules/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/permissions/selectors/commands.py` & `unify-cli-3.5.2/source/permissions/selectors/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/pipeline/commands.py` & `unify-cli-3.5.2/source/pipeline/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/template/commands.py` & `unify-cli-3.5.2/source/template/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/user/commands.py` & `unify-cli-3.5.2/source/user/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/utils/util_methods.py` & `unify-cli-3.5.2/source/utils/util_methods.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/source/workflow/commands.py` & `unify-cli-3.5.2/source/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/__init__.py` & `unify-cli-3.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/properties.py` & `unify-cli-3.5.2/tests/properties.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/test_asset_access.py` & `unify-cli-3.5.2/tests/test_asset_access.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/test_cluster_command.py` & `unify-cli-3.5.2/tests/test_cluster_command.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/test_datasets_commands.py` & `unify-cli-3.5.2/tests/test_datasets_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/test_graph_commands.py` & `unify-cli-3.5.2/tests/test_graph_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/test_help.py` & `unify-cli-3.5.2/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/test_org_command.py` & `unify-cli-3.5.2/tests/test_org_command.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/test_pipeline_commands.py` & `unify-cli-3.5.2/tests/test_pipeline_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/test_templates_commands.py` & `unify-cli-3.5.2/tests/test_templates_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/test_user_commands.py` & `unify-cli-3.5.2/tests/test_user_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/tests/test_workflow_commands.py` & `unify-cli-3.5.2/tests/test_workflow_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.5.1/unify_cli.egg-info/PKG-INFO` & `unify-cli-3.5.2/unify_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-cli
-Version: 3.5.1
+Version: 3.5.2
 Summary: Element Unify command line tool
 Home-page: https://github.com/ElementAnalytics/element-unify-cli
 Author: Element Analytics
 Author-email: platform@ean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3
```

### Comparing `unify-cli-3.5.1/unify_cli.egg-info/SOURCES.txt` & `unify-cli-3.5.2/unify_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

