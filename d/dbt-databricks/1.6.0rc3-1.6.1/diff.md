# Comparing `tmp/dbt-databricks-1.6.0rc3.tar.gz` & `tmp/dbt-databricks-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.6.0rc3.tar", last modified: Thu Jul 27 19:21:05 2023, max compression
+gzip compressed data, was "dbt-databricks-1.6.1.tar", last modified: Wed Aug  2 20:49:03 2023, max compression
```

## Comparing `dbt-databricks-1.6.0rc3.tar` & `dbt-databricks-1.6.1.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.368743 dbt-databricks-1.6.0rc3/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       46 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/MANIFEST.in
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     5379 2023-07-27 19:21:05.368539 dbt-databricks-1.6.0rc3/PKG-INFO
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     4624 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/README.md
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.352894 dbt-databricks-1.6.0rc3/dbt/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.352716 dbt-databricks-1.6.0rc3/dbt/adapters/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.359133 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      626 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       26 2023-07-27 19:20:54.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2708 2023-05-10 18:27:27.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/auth.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      586 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/column.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    35924 2023-07-19 22:57:01.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/connections.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    21196 2023-07-27 19:15:21.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/impl.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    17743 2023-07-19 17:29:22.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     3564 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/relation.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2117 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.353007 dbt-databricks-1.6.0rc3/dbt/include/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.360233 dbt-databricks-1.6.0rc3/dbt/include/databricks/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       52 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/__init__.py
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       77 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.361666 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)    18808 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/adapters.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      592 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/catalog.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2409 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/copy_into.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.362839 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.363594 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     4331 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     3910 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2066 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/validate.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.364584 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/materialized_view/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      318 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/materialized_view/create_materialized_view_as.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1682 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      279 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/materialized_view/refresh_materialized_view.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.365110 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/seeds/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2451 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2476 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/seeds/seeds.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     5397 2023-05-08 06:46:27.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/snapshot.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.365691 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/streaming_table/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      636 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1698 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1616 2023-05-08 06:46:27.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1316 2023-07-19 18:00:12.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/view.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      648 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/statement.sql
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.366401 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/utils/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      318 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      338 2023-04-27 19:55:38.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 raymond.cypher   (502) staff       (20)      535 2023-05-10 18:27:27.000000 dbt-databricks-1.6.0rc3/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 raymond.cypher   (502) staff       (20)        0 2023-07-27 19:21:05.368235 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     5379 2023-07-27 19:21:05.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     1959 2023-07-27 19:21:05.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)        1 2023-07-27 19:21:05.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)        1 2023-06-15 16:25:03.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       91 2023-07-27 19:21:05.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)        4 2023-07-27 19:21:05.000000 dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 raymond.cypher   (502) staff       (20)       38 2023-07-27 19:21:05.368800 dbt-databricks-1.6.0rc3/setup.cfg
--rw-r--r--   0 raymond.cypher   (502) staff       (20)     2502 2023-07-19 22:21:58.000000 dbt-databricks-1.6.0rc3/setup.py
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.478017 dbt-databricks-1.6.1/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       46 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/MANIFEST.in
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     5376 2023-08-02 20:49:03.477527 dbt-databricks-1.6.1/PKG-INFO
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     4624 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/README.md
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.456039 dbt-databricks-1.6.1/dbt/
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.455787 dbt-databricks-1.6.1/dbt/adapters/
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.462118 dbt-databricks-1.6.1/dbt/adapters/databricks/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      626 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       23 2023-08-02 20:48:37.000000 dbt-databricks-1.6.1/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2708 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/adapters/databricks/auth.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      586 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/adapters/databricks/column.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)    35924 2023-08-02 20:21:56.000000 dbt-databricks-1.6.1/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)    21196 2023-08-02 20:48:37.000000 dbt-databricks-1.6.1/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)    17743 2023-07-25 17:48:29.000000 dbt-databricks-1.6.1/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     3564 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/dbt/adapters/databricks/relation.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2117 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.456230 dbt-databricks-1.6.1/dbt/include/
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.463250 dbt-databricks-1.6.1/dbt/include/databricks/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       52 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/__init__.py
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       77 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.465127 dbt-databricks-1.6.1/dbt/include/databricks/macros/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)    18820 2023-08-02 20:21:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/adapters.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      592 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/catalog.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2409 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/copy_into.sql
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.466768 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2802 2023-08-02 20:21:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/clone.sql
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.467754 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     4331 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     3910 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2066 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/incremental/validate.sql
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.469177 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/materialized_view/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      318 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/materialized_view/create_materialized_view_as.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     1682 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      279 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/materialized_view/refresh_materialized_view.sql
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.469882 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/seeds/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2451 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2476 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/seeds/seeds.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     5397 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/snapshot.sql
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.471330 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/streaming_table/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      636 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     1698 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     1616 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     1316 2023-08-01 21:22:03.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/view.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2992 2023-08-02 20:21:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/python.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      648 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/statement.sql
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.472971 dbt-databricks-1.6.1/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      318 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      338 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)      535 2023-06-14 20:34:56.000000 dbt-databricks-1.6.1/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 jesse.whitehouse   (502) staff       (20)        0 2023-08-02 20:49:03.476893 dbt-databricks-1.6.1/dbt_databricks.egg-info/
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     5376 2023-08-02 20:49:03.000000 dbt-databricks-1.6.1/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2057 2023-08-02 20:49:03.000000 dbt-databricks-1.6.1/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)        1 2023-08-02 20:49:03.000000 dbt-databricks-1.6.1/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)        1 2023-07-07 19:50:48.000000 dbt-databricks-1.6.1/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       88 2023-08-02 20:49:03.000000 dbt-databricks-1.6.1/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)        4 2023-08-02 20:49:03.000000 dbt-databricks-1.6.1/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)       38 2023-08-02 20:49:03.478082 dbt-databricks-1.6.1/setup.cfg
+-rw-r--r--   0 jesse.whitehouse   (502) staff       (20)     2499 2023-08-02 20:21:56.000000 dbt-databricks-1.6.1/setup.py
```

### Comparing `dbt-databricks-1.6.0rc3/PKG-INFO` & `dbt-databricks-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.6.0rc3
+Version: 1.6.1
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.6.0rc3/README.md` & `dbt-databricks-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/__init__.py` & `dbt-databricks-1.6.1/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/auth.py` & `dbt-databricks-1.6.1/dbt/adapters/databricks/auth.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/column.py` & `dbt-databricks-1.6.1/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/connections.py` & `dbt-databricks-1.6.1/dbt/adapters/databricks/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/impl.py` & `dbt-databricks-1.6.1/dbt/adapters/databricks/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/python_submissions.py` & `dbt-databricks-1.6.1/dbt/adapters/databricks/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/relation.py` & `dbt-databricks-1.6.1/dbt/adapters/databricks/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/adapters/databricks/utils.py` & `dbt-databricks-1.6.1/dbt/adapters/databricks/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/adapters.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/adapters.sql`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     {#--
     N.B. Python models _can_ write to temp views HOWEVER they use a different session
     and have already expired by the time they need to be used (I.E. in merges for incremental models)
 
     TODO: Deep dive into spark sessions to see if we can reuse a single session for an entire
     dbt invocation.
      --#}
-    {{ py_write_table(compiled_code=compiled_code, target_relation=relation) }}
+    {{ databricks__py_write_table(compiled_code=compiled_code, target_relation=relation) }}
   {%- endif -%}
 {%- endmacro -%}
 
 {% macro databricks__create_view_as(relation, sql) -%}
   create or replace view {{ relation }}
   {{ comment_clause() }}
   {%- set contract_config = config.get('contract') -%}
```

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/catalog.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/copy_into.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/strategies.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/incremental/validate.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/seeds/helpers.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/seeds/seeds.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/seeds/seeds.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/streaming_table/create_or_refresh_streaming_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/streaming_table/streaming_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/materializations/view.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/macros/statement.sql` & `dbt-databricks-1.6.1/dbt/include/databricks/macros/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt/include/databricks/profile_template.yml` & `dbt-databricks-1.6.1/dbt/include/databricks/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-1.6.1/dbt_databricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.6.0rc3
+Version: 1.6.1
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.6.0rc3/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-1.6.1/dbt_databricks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 dbt/adapters/databricks/utils.py
 dbt/include/databricks/__init__.py
 dbt/include/databricks/dbt_project.yml
 dbt/include/databricks/profile_template.yml
 dbt/include/databricks/macros/adapters.sql
 dbt/include/databricks/macros/catalog.sql
 dbt/include/databricks/macros/copy_into.sql
+dbt/include/databricks/macros/python.sql
 dbt/include/databricks/macros/statement.sql
+dbt/include/databricks/macros/materializations/clone.sql
 dbt/include/databricks/macros/materializations/snapshot.sql
 dbt/include/databricks/macros/materializations/table.sql
 dbt/include/databricks/macros/materializations/view.sql
 dbt/include/databricks/macros/materializations/incremental/incremental.sql
 dbt/include/databricks/macros/materializations/incremental/strategies.sql
 dbt/include/databricks/macros/materializations/incremental/validate.sql
 dbt/include/databricks/macros/materializations/materialized_view/create_materialized_view_as.sql
```

### Comparing `dbt-databricks-1.6.0rc3/setup.py` & `dbt-databricks-1.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     long_description_content_type="text/markdown",
     author="Databricks",
     author_email="feedback@databricks.com",
     url="https://github.com/databricks/dbt-databricks",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-spark==1.6.0rc1",
+        "dbt-spark==1.6.0",
         "databricks-sql-connector~=2.7.0",
         "databricks-sdk>=0.1.7",
         "keyring>=23.13.0",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

