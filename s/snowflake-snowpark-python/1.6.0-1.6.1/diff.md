# Comparing `tmp/snowflake-snowpark-python-1.6.0.tar.gz` & `tmp/snowflake-snowpark-python-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-snowpark-python-1.6.0.tar", last modified: Mon Jul 31 21:45:31 2023, max compression
+gzip compressed data, was "snowflake-snowpark-python-1.6.1.tar", last modified: Thu Aug  3 01:29:15 2023, max compression
```

## Comparing `snowflake-snowpark-python-1.6.0.tar` & `snowflake-snowpark-python-1.6.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:45:31.172767 snowflake-snowpark-python-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-07-31 21:45:19.000000 snowflake-snowpark-python-1.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-31 21:45:19.000000 snowflake-snowpark-python-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 21:45:19.000000 snowflake-snowpark-python-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    40004 2023-07-31 21:45:31.172767 snowflake-snowpark-python-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-31 21:45:19.000000 snowflake-snowpark-python-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:45:31.172767 snowflake-snowpark-python-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:45:31.164767 snowflake-snowpark-python-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:45:31.164767 snowflake-snowpark-python-1.6.0/src/snowflake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:45:31.168767 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:45:31.168767 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:45:31.172767 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38812 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    36373 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/binary_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/grouping_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    43127 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/select_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)    41482 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/sort_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/table_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/unary_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/window_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    26737 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/code_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    22116 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/packaging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/server_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/type_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40565 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/udf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27196 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/async_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/context.py
--rw-r--r--   0 runner    (1001) docker     (123)   155080 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/dataframe_na_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31616 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/dataframe_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/dataframe_stat_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/dataframe_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/file_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/files.py
--rw-r--r--   0 runner    (1001) docker     (123)   291315 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/query_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/relational_grouped_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/row.py
--rw-r--r--   0 runner    (1001) docker     (123)   113249 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/stored_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)    29974 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/table_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/udaf.py
--rw-r--r--   0 runner    (1001) docker     (123)    46552 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/udf.py
--rw-r--r--   0 runner    (1001) docker     (123)    39832 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/udtf.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-07-31 21:45:20.000000 snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:45:31.172767 snowflake-snowpark-python-1.6.0/src/snowflake_snowpark_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40004 2023-07-31 21:45:31.000000 snowflake-snowpark-python-1.6.0/src/snowflake_snowpark_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-31 21:45:31.000000 snowflake-snowpark-python-1.6.0/src/snowflake_snowpark_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:45:31.000000 snowflake-snowpark-python-1.6.0/src/snowflake_snowpark_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 21:45:31.000000 snowflake-snowpark-python-1.6.0/src/snowflake_snowpark_python.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:45:30.000000 snowflake-snowpark-python-1.6.0/src/snowflake_snowpark_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 21:45:31.000000 snowflake-snowpark-python-1.6.0/src/snowflake_snowpark_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 21:45:31.000000 snowflake-snowpark-python-1.6.0/src/snowflake_snowpark_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:29:15.217811 snowflake-snowpark-python-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    40004 2023-08-03 01:29:15.217811 snowflake-snowpark-python-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 01:29:15.217811 snowflake-snowpark-python-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:29:15.205811 snowflake-snowpark-python-1.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:29:15.205811 snowflake-snowpark-python-1.6.1/src/snowflake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:29:15.213811 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:29:15.213811 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:29:15.217811 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38812 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36373 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/binary_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/grouping_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43127 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/select_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41482 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/sort_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/table_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/unary_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/window_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26737 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22116 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/packaging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25879 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/server_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40611 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/udf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27196 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/async_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34396 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155080 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/dataframe_na_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31616 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/dataframe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/dataframe_stat_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/dataframe_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/file_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291315 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/query_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/relational_grouped_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113249 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/stored_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29974 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/table_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/udaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46552 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/udf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39832 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/udtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-08-03 01:29:03.000000 snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 01:29:15.217811 snowflake-snowpark-python-1.6.1/src/snowflake_snowpark_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40004 2023-08-03 01:29:15.000000 snowflake-snowpark-python-1.6.1/src/snowflake_snowpark_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-03 01:29:15.000000 snowflake-snowpark-python-1.6.1/src/snowflake_snowpark_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:29:15.000000 snowflake-snowpark-python-1.6.1/src/snowflake_snowpark_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 01:29:15.000000 snowflake-snowpark-python-1.6.1/src/snowflake_snowpark_python.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 01:29:15.000000 snowflake-snowpark-python-1.6.1/src/snowflake_snowpark_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-03 01:29:15.000000 snowflake-snowpark-python-1.6.1/src/snowflake_snowpark_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 01:29:15.000000 snowflake-snowpark-python-1.6.1/src/snowflake_snowpark_python.egg-info/top_level.txt
```

### Comparing `snowflake-snowpark-python-1.6.0/CHANGELOG.md` & `snowflake-snowpark-python-1.6.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Release History
 
-## 1.6.0 (2023-07-28)
+## 1.6.1 (2023-08-02)
 
 ### New Features
 
 - Added support for these new functions in `snowflake.snowpark.functions`:
   - `array_sort`
   - `sort_array`
   - `array_min`
```

### Comparing `snowflake-snowpark-python-1.6.0/LICENSE.txt` & `snowflake-snowpark-python-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/PKG-INFO` & `snowflake-snowpark-python-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-snowpark-python
-Version: 1.6.0
+Version: 1.6.1
 Summary: Snowflake Snowpark for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/developer-guide/snowpark/python/index.html
 Project-URL: Source, https://github.com/snowflakedb/snowpark-python
@@ -132,15 +132,15 @@
 [snowflake lab sample code]: https://github.com/Snowflake-Labs/snowpark-python-demos
 [samples]: https://github.com/snowflakedb/snowpark-python/blob/main/README.md#samples
 [contributing]: https://github.com/snowflakedb/snowpark-python/blob/main/CONTRIBUTING.md
 
 
 # Release History
 
-## 1.6.0 (2023-07-28)
+## 1.6.1 (2023-08-02)
 
 ### New Features
 
 - Added support for these new functions in `snowflake.snowpark.functions`:
   - `array_sort`
   - `sort_array`
   - `array_min`
```

### Comparing `snowflake-snowpark-python-1.6.0/README.md` & `snowflake-snowpark-python-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/setup.py` & `snowflake-snowpark-python-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/__init__.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/analyzer.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/binary_expression.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/binary_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/expression.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/grouping_set.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/grouping_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/schema_utils.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/schema_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/select_statement.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/select_statement.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/sort_expression.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/sort_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/table_function.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/table_function.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/unary_expression.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/unary_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/analyzer/window_expression.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/analyzer/window_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/code_generation.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/code_generation.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/error_message.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/error_message.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/packaging_utils.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/server_connection.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/server_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/telemetry.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/type_utils.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/type_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/udf_utils.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/udf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,32 +161,28 @@
                 ]
             )
         else:  # both type hints and return type are specified
             return None
     elif return_type_hint is None:
         return None
     else:
-        # Vectorized UDTF
-        if not installed_pandas:
-            raise RuntimeError(
-                "No pandas detected in local environment, please install pandas to use vectorized UDTF"
-            )
-        elif typing.get_origin(return_type_hint) == PandasDataFrame:
-            return PandasDataFrameType(
-                col_types=[
-                    python_type_to_snow_type(x)[0]
-                    for x in typing.get_args(return_type_hint)
-                ],
-                col_names=output_schema,
-            )
-        elif return_type_hint is pandas.DataFrame:
-            return PandasDataFrameType(
-                []
-            )  # placeholder, indicating the return type is pandas DataFrame
-        elif return_type_hint is NoneType:
+        if installed_pandas:  # Vectorized UDTF
+            if typing.get_origin(return_type_hint) == PandasDataFrame:
+                return PandasDataFrameType(
+                    col_types=[
+                        python_type_to_snow_type(x)[0]
+                        for x in typing.get_args(return_type_hint)
+                    ],
+                    col_names=output_schema,
+                )
+            elif return_type_hint is pandas.DataFrame:
+                return PandasDataFrameType(
+                    []
+                )  # placeholder, indicating the return type is pandas DataFrame
+        if return_type_hint is NoneType:
             return None
         else:
             raise ValueError(
                 f"The return type hint for a UDTF handler must be a collection type or None or a PandasDataFrame. {return_type_hint} is used."
             )
 
 
@@ -407,15 +403,15 @@
               then just use the types inferred from type hints.
     """
 
     (
         return_type_from_type_hints,
         input_types_from_type_hints,
     ) = get_types_from_type_hints(func, object_type, output_schema)
-    if return_type and return_type_from_type_hints:
+    if installed_pandas and return_type and return_type_from_type_hints:
         if isinstance(return_type_from_type_hints, PandasSeriesType):
             res_return_type = (
                 return_type.element_type
                 if isinstance(return_type, PandasSeriesType)
                 else return_type
             )
             res_input_types = (
@@ -445,15 +441,16 @@
                 [x.datatype for x in return_type], [x.name for x in return_type]
             )
 
     res_return_type = return_type or return_type_from_type_hints
     res_input_types = input_types or input_types_from_type_hints
 
     if not res_return_type or (
-        isinstance(res_return_type, PandasSeriesType)
+        installed_pandas
+        and isinstance(res_return_type, PandasSeriesType)
         and not res_return_type.element_type
     ):
         raise TypeError("The return type must be specified")
 
     # We only want to have this check when only type hints are provided
     if (
         not return_type
@@ -470,14 +467,17 @@
         if num_args != len(input_types_from_type_hints):
             raise TypeError(
                 f'{"" if object_type == TempObjectType.FUNCTION else f"Excluding session argument in stored procedure, "}'
                 f"the number of arguments ({num_args}) is different from "
                 f"the number of argument type hints ({len(input_types_from_type_hints)})"
             )
 
+    if not installed_pandas:
+        return False, False, res_return_type, res_input_types
+
     if isinstance(res_return_type, PandasSeriesType):
         if len(res_input_types) == 0:
             return True, False, res_return_type.element_type, []
         elif len(res_input_types) == 1 and isinstance(
             res_input_types[0], PandasDataFrameType
         ):
             return (
@@ -961,15 +961,15 @@
         if not session._runtime_version_from_requirement
         else session._runtime_version_from_requirement
     )
     if replace and if_not_exists:
         raise ValueError("options replace and if_not_exists are incompatible")
     if isinstance(return_type, StructType):
         return_sql = f'RETURNS TABLE ({",".join(f"{field.name} {convert_sp_to_sf_type(field.datatype)}" for field in return_type.fields)})'
-    elif isinstance(return_type, PandasDataFrameType):
+    elif installed_pandas and isinstance(return_type, PandasDataFrameType):
         return_sql = f'RETURNS TABLE ({",".join(f"{name} {convert_sp_to_sf_type(datatype)}" for name, datatype in zip(return_type.col_names, return_type.col_types))})'
     else:
         return_sql = f"RETURNS {convert_sp_to_sf_type(return_type)}"
     input_sql_types = [convert_sp_to_sf_type(arg.datatype) for arg in input_args]
     sql_func_args = ",".join(
         [f"{a.name} {t}" for a, t in zip(input_args, input_sql_types)]
     )
```

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/_internal/utils.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/async_job.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/async_job.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/column.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/column.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/context.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/context.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/dataframe.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/dataframe.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/dataframe_na_functions.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/dataframe_na_functions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/dataframe_reader.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/dataframe_reader.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/dataframe_stat_functions.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/dataframe_stat_functions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/dataframe_writer.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/dataframe_writer.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/exceptions.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/file_operation.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/file_operation.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/files.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/files.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/functions.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/functions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/query_history.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/query_history.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/relational_grouped_dataframe.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/relational_grouped_dataframe.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/row.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/row.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/session.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/session.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/stored_procedure.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/stored_procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/table.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/table.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/table_function.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/table_function.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/types.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/types.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/udaf.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/udaf.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/udf.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/udf.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/udtf.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/udtf.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake/snowpark/window.py` & `snowflake-snowpark-python-1.6.1/src/snowflake/snowpark/window.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake_snowpark_python.egg-info/PKG-INFO` & `snowflake-snowpark-python-1.6.1/src/snowflake_snowpark_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-snowpark-python
-Version: 1.6.0
+Version: 1.6.1
 Summary: Snowflake Snowpark for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/developer-guide/snowpark/python/index.html
 Project-URL: Source, https://github.com/snowflakedb/snowpark-python
@@ -132,15 +132,15 @@
 [snowflake lab sample code]: https://github.com/Snowflake-Labs/snowpark-python-demos
 [samples]: https://github.com/snowflakedb/snowpark-python/blob/main/README.md#samples
 [contributing]: https://github.com/snowflakedb/snowpark-python/blob/main/CONTRIBUTING.md
 
 
 # Release History
 
-## 1.6.0 (2023-07-28)
+## 1.6.1 (2023-08-02)
 
 ### New Features
 
 - Added support for these new functions in `snowflake.snowpark.functions`:
   - `array_sort`
   - `sort_array`
   - `array_min`
```

### Comparing `snowflake-snowpark-python-1.6.0/src/snowflake_snowpark_python.egg-info/SOURCES.txt` & `snowflake-snowpark-python-1.6.1/src/snowflake_snowpark_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

