# Comparing `tmp/serra-0.7.1.tar.gz` & `tmp/serra-0.7.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serra-0.7.1.tar", last modified: Tue Aug  1 21:22:37 2023, max compression
+gzip compressed data, was "serra-0.7.11.tar", last modified: Thu Aug  3 20:32:08 2023, max compression
```

## Comparing `serra-0.7.1.tar` & `serra-0.7.11.tar`

### file list

```diff
@@ -1,107 +1,110 @@
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.706422 serra-0.7.1/
--rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-08-01 20:57:39.000000 serra-0.7.1/LICENSE.md
--rw-r--r--   0 alanwang   (501) staff       (20)      242 2023-08-01 21:22:37.706051 serra-0.7.1/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     4478 2023-08-01 20:57:39.000000 serra-0.7.1/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.694127 serra-0.7.1/serra/
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-01 20:57:39.000000 serra-0.7.1/serra/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2006 2023-08-01 20:57:39.000000 serra-0.7.1/serra/aws.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1872 2023-08-01 20:57:39.000000 serra-0.7.1/serra/cli.py
--rw-r--r--   0 alanwang   (501) staff       (20)      252 2023-08-01 20:57:39.000000 serra-0.7.1/serra/config.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1788 2023-08-01 20:57:39.000000 serra-0.7.1/serra/config_parser.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.691014 serra-0.7.1/serra/data/
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.695679 serra-0.7.1/serra/data/autocomplete/
--rw-r--r--   0 alanwang   (501) staff       (20)     1110 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/README.md
--rw-r--r--   0 alanwang   (501) staff       (20)     1636 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/gen_schemas.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.695809 serra-0.7.1/serra/data/autocomplete/inputs/
--rw-r--r--   0 alanwang   (501) staff       (20)     2249 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/inputs/specs.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.698058 serra-0.7.1/serra/data/autocomplete/output/
--rw-r--r--   0 alanwang   (501) staff       (20)      391 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/AddColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      276 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/AmazonS3Reader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      341 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/AmazonS3Writer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      267 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/CaseWhenTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      216 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/CastColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      206 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/DatabricksReader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      389 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/DatabricksWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/DropColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/GetCountTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      354 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/JoinTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      148 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/LocalReader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/LocalWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)      331 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/MapTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      408 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/PivotTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/RenameColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      210 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/SelectTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/SnowflakeWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)     7553 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/output/serra_yaml_schema.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.698540 serra-0.7.1/serra/data/autocomplete/templates/
--rw-r--r--   0 alanwang   (501) staff       (20)      326 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/templates/schema_template.json
--rw-r--r--   0 alanwang   (501) staff       (20)       95 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/autocomplete/templates/transformer_template.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.698911 serra-0.7.1/serra/data/workspace_example/
--rw-r--r--   0 alanwang   (501) staff       (20)      137 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.699464 serra-0.7.1/serra/data/workspace_example/examples/
--rw-r--r--   0 alanwang   (501) staff       (20)     1610 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/examples/ratings.csv
--rw-r--r--   0 alanwang   (501) staff       (20)     6706 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/examples/sales.csv
--rw-r--r--   0 alanwang   (501) staff       (20)     1124 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/examples/states_to_abbreviation.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.700328 serra-0.7.1/serra/data/workspace_example/jobs/
--rw-r--r--   0 alanwang   (501) staff       (20)      912 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/CloudDemo.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      945 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/Demo.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      418 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/LocalExample.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      220 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/ReadExample.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      456 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/ReadJoinWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      393 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/ReadMapWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      397 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/jobs/ReadPivotWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      323 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/profiles.yml
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.700591 serra-0.7.1/serra/data/workspace_example/sql/
--rw-r--r--   0 alanwang   (501) staff       (20)     2603 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/sql/easy_demo.sql
--rw-r--r--   0 alanwang   (501) staff       (20)     2909 2023-08-01 20:57:39.000000 serra-0.7.1/serra/data/workspace_example/sql/hard_demo.sql
--rw-r--r--   0 alanwang   (501) staff       (20)     2964 2023-08-01 20:57:39.000000 serra-0.7.1/serra/databricks.py
--rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-08-01 20:57:39.000000 serra-0.7.1/serra/exceptions.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1120 2023-08-01 20:57:39.000000 serra-0.7.1/serra/profile.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.701647 serra-0.7.1/serra/readers/
--rw-r--r--   0 alanwang   (501) staff       (20)      233 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1457 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/amazon_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/databricks_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      501 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/local_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/s3_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1380 2023-08-01 20:57:39.000000 serra-0.7.1/serra/readers/snowflaker_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2977 2023-08-01 20:57:39.000000 serra-0.7.1/serra/run.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.702033 serra-0.7.1/serra/runners/
--rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-08-01 20:57:39.000000 serra-0.7.1/serra/runners/ExecutionGraph.py
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-08-01 20:57:39.000000 serra-0.7.1/serra/runners/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3148 2023-08-01 20:57:39.000000 serra-0.7.1/serra/runners/graph_runner.py
--rw-r--r--   0 alanwang   (501) staff       (20)      443 2023-08-01 20:57:39.000000 serra-0.7.1/serra/tests.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.704734 serra-0.7.1/serra/transformers/
--rw-r--r--   0 alanwang   (501) staff       (20)      624 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/add_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/case_when_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/cast_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/drop_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      623 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/filter_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/get_count_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1288 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/join_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1947 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/map_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1255 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/pivot_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/rename_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1091 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/select_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-08-01 20:57:39.000000 serra-0.7.1/serra/transformers/transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1967 2023-08-01 20:57:39.000000 serra-0.7.1/serra/translate_client.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2293 2023-08-01 20:57:39.000000 serra-0.7.1/serra/utils.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.705824 serra-0.7.1/serra/writers/
--rw-r--r--   0 alanwang   (501) staff       (20)      232 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/amazon_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      678 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/databricks_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/local_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      569 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/s3_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3048 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/snowflake_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-08-01 20:57:39.000000 serra-0.7.1/serra/writers/writer.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-08-01 21:22:37.695289 serra-0.7.1/serra.egg-info/
--rw-r--r--   0 alanwang   (501) staff       (20)      242 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     3366 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/SOURCES.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/dependency_links.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/entry_points.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-08-01 20:58:40.000000 serra-0.7.1/serra.egg-info/not-zip-safe
--rw-r--r--   0 alanwang   (501) staff       (20)       83 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/requires.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-08-01 21:22:37.000000 serra-0.7.1/serra.egg-info/top_level.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-08-01 21:22:37.706525 serra-0.7.1/setup.cfg
--rw-r--r--   0 alanwang   (501) staff       (20)      920 2023-08-01 21:22:33.000000 serra-0.7.1/setup.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.737346 serra-0.7.11/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3860 2023-08-03 20:28:12.000000 serra-0.7.11/LICENSE.md
+-rw-r--r--   0 albertstanley   (501) staff       (20)      243 2023-08-03 20:32:08.737039 serra-0.7.11/PKG-INFO
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3917 2023-08-03 20:28:12.000000 serra-0.7.11/README.md
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.711951 serra-0.7.11/serra/
+-rw-r--r--   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:28:12.000000 serra-0.7.11/serra/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2006 2023-08-03 20:28:12.000000 serra-0.7.11/serra/aws.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1872 2023-08-03 20:28:12.000000 serra-0.7.11/serra/cli.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      252 2023-08-03 20:28:12.000000 serra-0.7.11/serra/config.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1788 2023-08-03 20:28:12.000000 serra-0.7.11/serra/config_parser.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.707844 serra-0.7.11/serra/data/
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.715115 serra-0.7.11/serra/data/autocomplete/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1110 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/README.md
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1636 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/gen_schemas.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.715410 serra-0.7.11/serra/data/autocomplete/inputs/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2249 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/inputs/specs.json
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.720404 serra-0.7.11/serra/data/autocomplete/output/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      391 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/AddColumnTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      276 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/AmazonS3Reader.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      341 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/AmazonS3Writer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      267 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/CaseWhenTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      216 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/CastColumnTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      206 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/DatabricksReader.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      389 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/DatabricksWriter.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      213 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/DropColumnTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      274 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/GetCountTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      354 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/JoinTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      148 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/LocalReader.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      213 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/LocalWriter.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      331 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/MapTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      408 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/PivotTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      274 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/RenameColumnTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      210 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/SelectTransformer.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)      452 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/SnowflakeWriter.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)     7553 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/output/serra_yaml_schema.json
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.720854 serra-0.7.11/serra/data/autocomplete/templates/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      326 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/templates/schema_template.json
+-rw-r--r--   0 albertstanley   (501) staff       (20)       95 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/autocomplete/templates/transformer_template.json
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.721326 serra-0.7.11/serra/data/workspace_example/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      137 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/README.md
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.721990 serra-0.7.11/serra/data/workspace_example/examples/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1610 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/examples/ratings.csv
+-rw-r--r--   0 albertstanley   (501) staff       (20)     6706 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/examples/sales.csv
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1124 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/examples/states_to_abbreviation.json
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.723521 serra-0.7.11/serra/data/workspace_example/jobs/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      912 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/CloudDemo.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      952 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/Demo.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      418 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/LocalExample.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      220 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/ReadExample.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      456 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/ReadJoinWrite.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      393 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/ReadMapWrite.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      397 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/jobs/ReadPivotWrite.yml
+-rw-r--r--   0 albertstanley   (501) staff       (20)      323 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/profiles.yml
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.723962 serra-0.7.11/serra/data/workspace_example/sql/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2603 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/sql/easy_demo.sql
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2909 2023-08-03 20:28:12.000000 serra-0.7.11/serra/data/workspace_example/sql/hard_demo.sql
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2964 2023-08-03 20:28:12.000000 serra-0.7.11/serra/databricks.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      106 2023-08-03 20:28:12.000000 serra-0.7.11/serra/exceptions.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1120 2023-08-03 20:28:12.000000 serra-0.7.11/serra/profile.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.725617 serra-0.7.11/serra/readers/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      233 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2182 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/amazon_reader.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1238 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/databricks_reader.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      962 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/local_reader.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      277 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/reader.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2063 2023-08-03 20:28:12.000000 serra-0.7.11/serra/readers/snowflaker_reader.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2984 2023-08-03 20:28:12.000000 serra-0.7.11/serra/run.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.726532 serra-0.7.11/serra/runners/
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2631 2023-08-03 20:28:12.000000 serra-0.7.11/serra/runners/ExecutionGraph.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:28:12.000000 serra-0.7.11/serra/runners/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3148 2023-08-03 20:28:12.000000 serra-0.7.11/serra/runners/graph_runner.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      443 2023-08-03 20:28:12.000000 serra-0.7.11/serra/tests.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.734121 serra-0.7.11/serra/transformers/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      624 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1512 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/add_column_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1225 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/aggregate_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      631 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/case_when_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1318 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/cast_columns_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1016 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/coalesce_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      875 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/drop_columns_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1002 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/filter_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1138 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/get_count_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      910 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/get_distinct_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1339 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/impute_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2175 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/join_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2867 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/map_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1145 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/order_by_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1986 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/pivot_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1009 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/rename_column_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1423 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/select_transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      310 2023-08-03 20:28:12.000000 serra-0.7.11/serra/transformers/transformer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3211 2023-08-03 20:28:12.000000 serra-0.7.11/serra/translate_client.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2293 2023-08-03 20:28:12.000000 serra-0.7.11/serra/utils.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.736496 serra-0.7.11/serra/writers/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      232 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/__init__.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     2143 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/amazon_writer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     1400 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/databricks_writer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      957 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/local_writer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3864 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/snowflake_writer.py
+-rw-r--r--   0 albertstanley   (501) staff       (20)      284 2023-08-03 20:28:12.000000 serra-0.7.11/serra/writers/writer.py
+drwxr-xr-x   0 albertstanley   (501) staff       (20)        0 2023-08-03 20:32:08.714361 serra-0.7.11/serra.egg-info/
+-rw-r--r--   0 albertstanley   (501) staff       (20)      243 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/PKG-INFO
+-rw-r--r--   0 albertstanley   (501) staff       (20)     3530 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/SOURCES.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)        1 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/dependency_links.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)       88 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/entry_points.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)        1 2023-08-03 20:28:34.000000 serra-0.7.11/serra.egg-info/not-zip-safe
+-rw-r--r--   0 albertstanley   (501) staff       (20)       83 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/requires.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)        6 2023-08-03 20:32:08.000000 serra-0.7.11/serra.egg-info/top_level.txt
+-rw-r--r--   0 albertstanley   (501) staff       (20)       38 2023-08-03 20:32:08.737473 serra-0.7.11/setup.cfg
+-rw-r--r--   0 albertstanley   (501) staff       (20)      922 2023-08-03 20:32:02.000000 serra-0.7.11/setup.py
```

### Comparing `serra-0.7.1/LICENSE.md` & `serra-0.7.11/LICENSE.md`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/README.md` & `serra-0.7.11/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Serra.
 
 ```bash
-pip install serra==0.6
+pip install serra
 ```
 
 # Setup
 
 Setup your virtual environment below.
 
 ```bash
@@ -53,16 +53,16 @@
 
 Other jobs available can be found in the **workspace_example/jobs** folder.
 
 # Connector Credentials
 Update your credentials for AWS, Databricks, and Snowflake in `workspace/profiles.yml`
 
 ```
-AWS Access Key ID: [YOUR ACCESS KEY]
-AWS Secret Access Key: [YOUR SECRET ACCESS KEY]
+AWS_ACCESS_KEY_ID: [YOUR ACCESS KEY]
+AWS_SECRET_ACCESS_KEY: [YOUR SECRET ACCESS KEY]
 
 AWS_CONFIG_BUCKET: ENTER_HERE # Bucket to use to place job config files (not needed for quickstart)
 
 DATABRICKS_HOST: ENTER_HERE
 DATABRICKS_TOKEN: ENTER_HERE
 DATABRICKS_CLUSTER_ID: ENTER_HERE
 
@@ -100,42 +100,14 @@
 
 ## Deploy to Databricks
 ```bash
 serra deploy {job_name}
 ```
 Run your job configuration files directly on Databricks. 
 
-
-# AWS S3 Local Setup
-
-### Step 1: Install AWS CLI
-```bash
-pip install awscli
-```
-
-### Step 2: Configure AWS Credentials
-```bash
-aws configure
-```
-* Fill out the credentials as so:
-```
-AWS Access Key ID: [YOUR ACCESS KEY]
-AWS Secret Access Key: [YOUR SECRET ACCESS KEY]
-Default region name: [YOUR DEFAULT S3 REGION]
-Default output format: [DEFAULT FORMAT]
-```
-
-### Step 3: Update workspace_examples/profiles.yml
-* Update your credentials like you did in Step 2:
-```
-AWS Access Key ID: [YOUR ACCESS KEY]
-AWS Secret Access Key: [YOUR SECRET ACCESS KEY]
-```
-
-
 # Databricks Development Guide
 
 ## If you make changes to the package (not just a new config)
 
 ### Step 1: Create wheel
 ```bash
 source env/bin/activate
@@ -189,8 +161,8 @@
 
 * All local spark sessions can now read from DB ie
 ```python
 from pyspark.sql.session import SparkSession
 
 spark = SparkSession.builder.getOrCreate()
 spark.sql("SELECT * FROM demo.sales_by_store")
-```
+```
```

### Comparing `serra-0.7.1/serra/aws.py` & `serra-0.7.11/serra/aws.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/cli.py` & `serra-0.7.11/serra/cli.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/config_parser.py` & `serra-0.7.11/serra/config_parser.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/data/autocomplete/README.md` & `serra-0.7.11/serra/data/autocomplete/README.md`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/data/autocomplete/gen_schemas.py` & `serra-0.7.11/serra/data/autocomplete/gen_schemas.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/data/autocomplete/inputs/specs.json` & `serra-0.7.11/serra/data/autocomplete/inputs/specs.json`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/data/autocomplete/output/serra_yaml_schema.json` & `serra-0.7.11/serra/data/autocomplete/output/serra_yaml_schema.json`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/data/workspace_example/examples/ratings.csv` & `serra-0.7.11/serra/data/workspace_example/examples/ratings.csv`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/data/workspace_example/examples/sales.csv` & `serra-0.7.11/serra/data/workspace_example/examples/sales.csv`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/data/workspace_example/examples/states_to_abbreviation.json` & `serra-0.7.11/serra/data/workspace_example/examples/states_to_abbreviation.json`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/data/workspace_example/jobs/CloudDemo.yml` & `serra-0.7.11/serra/data/workspace_example/jobs/CloudDemo.yml`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/data/workspace_example/jobs/Demo.yml` & `serra-0.7.11/serra/data/workspace_example/jobs/Demo.yml`

 * *Files 15% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 
 filter_states:
   FilterTransformer:
     input_block: map_state_names
     column: 'region_abbr'
     condition: ['AK', 'AL', 'CA', 'TX', 'CO', 'DE', 'FL']
 
-cast_ratings:
+cast_customers:
   CastColumnTransformer:
     input_block: filter_states
     cast_columns:
-      rating: ['rating', 'double']
+      rating: ['customers', 'double']
 
 pivot:
  PivotTransformer:
-   input_block: cast_ratings
+   input_block: cast_customers
    row_level: 'restaurant'
    column_level: "region_abbr"
    aggregate_type: "sum"
    sum_col: "customers"
 
 local_write:
   LocalWriter:
```

### Comparing `serra-0.7.1/serra/data/workspace_example/sql/easy_demo.sql` & `serra-0.7.11/serra/data/workspace_example/sql/easy_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/data/workspace_example/sql/hard_demo.sql` & `serra-0.7.11/serra/data/workspace_example/sql/hard_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/databricks.py` & `serra-0.7.11/serra/databricks.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/profile.py` & `serra-0.7.11/serra/profile.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/readers/amazon_reader.py` & `serra-0.7.11/serra/readers/amazon_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import boto3
 import pandas as pd
 
 from serra.utils import get_or_create_spark_session
 from serra.profile import get_serra_profile
 
 class AmazonS3Reader():
+    """
+    A class to read data from Amazon S3 and return a Spark DataFrame.
+
+    :param config: A dictionary containing the configuration for the reader.
+                   It should have the following keys:
+                   - 'bucket_name': The name of the S3 bucket containing the file.
+                   - 'file_path': The path to the file within the S3 bucket.
+                   - 'file_type': The type of file to be read (e.g., 'csv', 'parquet').
+    """
+
     def __init__(self, config):
         self.config = config
         self.serra_profile = get_serra_profile()
     
     @property
     def bucket_name(self):
         return self.config.get("bucket_name")
@@ -22,14 +32,20 @@
         return self.config.get("file_type")
     
     @property
     def dependencies(self):
         return []
     
     def read(self):
+        """
+        Read data from Amazon S3 and return a Spark DataFrame.
+
+        :return: A Spark DataFrame containing the data read from the S3 bucket.
+        :raises: Any exceptions that may occur during file reading or DataFrame creation.
+        """
         session = boto3.Session(
             aws_access_key_id=self.serra_profile.aws_access_key_id,
             aws_secret_access_key=self.serra_profile.aws_secret_access_key
         )
 
         # Create an S3 client using the session
         s3_client = session.client('s3')
```

### Comparing `serra-0.7.1/serra/run.py` & `serra-0.7.11/serra/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,31 +34,30 @@
         user_configs_folder = get_path_to_user_configs_folder()
         config_path = f"{user_configs_folder}/{job_name}.yml"
         cf = ConfigParser.from_local_config(config_path)
         run_job_with_graph(cf)
     except SerraRunException as e:
         logger.error(e)
 
-# translates your given sql file, gives you the config output, and saves the config in a new yml file
-
-# Use the paths as needed
-
-
 def translate_job(sql_path, is_run):
+    """
+    translates your given sql file, gives you the config output, and saves the config in a new yml file
+    """
+
+    # Get serra token from ~/.serra/credentials.json if it exists
     logger.info(f"Starting translation process for {sql_path}...")
     yaml_path = os.path.splitext(sql_path)[0]
 
     # Translate job by getting root dir, sql folder, sql path, get response, package path is just serra/
     sql_folder_path = './sql'
 
     sql_path = f"{sql_folder_path}/{sql_path}"
 
     translated_yaml = get_translated_yaml(sql_path)
     if not translated_yaml:
-        logger.error("Unable to translate file")
         return
 
     # Save in new yaml file (config folder with same name as sql path)
     user_configs_folder = get_path_to_user_configs_folder()
     yaml_path = f"{user_configs_folder}/{yaml_path}.yml"
     logger.info(f"Translation complete. Yaml file can be found at {os.path.abspath(yaml_path)}")
     save_as_yaml(translated_yaml, yaml_path)
```

### Comparing `serra-0.7.1/serra/runners/ExecutionGraph.py` & `serra-0.7.11/serra/runners/ExecutionGraph.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/runners/graph_runner.py` & `serra-0.7.11/serra/runners/graph_runner.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/transformers/__init__.py` & `serra-0.7.11/serra/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/transformers/add_column_transformer.py` & `serra-0.7.11/serra/transformers/filter_transformer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from pyspark.sql import functions as F
 
 from serra.transformers.transformer import Transformer
-from serra.exceptions import SerraRunException
 
-class AddColumnTransformer(Transformer):
+class FilterTransformer(Transformer):
     """
-    Test transformer to add a column to dataframe
-    :param config: Holds column value
+    A transformer to filter the DataFrame based on a specified condition.
+
+    :param config: A dictionary containing the configuration for the transformer.
+                   It should have the following keys:
+                   - 'condition': A list of values to filter the DataFrame by.
+                   - 'column': The name of the column to apply the filter on.
     """
 
     def __init__(self, config):
         self.config = config
-        self.name = config.get("name")
-        self.value = config.get("value")
-        self.column_type = config.get("column_type")
-        
+        self.condition = config.get("condition")
+        self.column = config.get("column")
+
     def transform(self, df):
         """
-        Add column with col_value to dataframe
-        :return; Dataframe w/ new column containing col_value
+        Filter the DataFrame based on the specified condition.
+
+        :param df: The input DataFrame to be transformed.
+        :return: A new DataFrame with rows filtered based on the specified condition.
         """
-        if self.name in df.columns:
-            raise SerraRunException(f"Column '{self.name}' already exists in the DataFrame. Choose a different name.")
-        
-        return df.withColumn(
-            self.name, F.lit(self.value).cast(self.column_type)  
-        )
+
+        return df.filter(df[self.column].isin(self.condition))
```

### Comparing `serra-0.7.1/serra/transformers/case_when_transformer.py` & `serra-0.7.11/serra/transformers/case_when_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/transformers/map_transformer.py` & `serra-0.7.11/serra/transformers/map_transformer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 from pyspark.sql import functions as F
 import json
 from serra.transformers.transformer import Transformer
 from serra.exceptions import SerraRunException
 
 class MapTransformer(Transformer):
     """
-    Test transformer to add a column to dataframe
-    :param config: Holds column value
+    A transformer to map values in a DataFrame column to new values based on a given mapping dictionary.
+
+    :param config: A dictionary containing the configuration for the transformer.
+                   It should have the following keys:
+                   - 'name': The name of the new column to be added after mapping.
+                   - 'map_dict': A dictionary containing the mapping of old values to new values.
+                                 If 'map_dict' is not provided, 'map_dict_path' should be specified.
+                   - 'map_dict_path': The path to a JSON file containing the mapping dictionary.
+                   - 'col_key': The name of the DataFrame column to be used as the key for mapping.
     """
 
     def __init__(self, config):
         self.config = config
         self.name = config.get("name")
         self.map_dict = config.get("map_dict")
         self.map_dict_path = config.get("map_dict_path")
         self.col_key = config.get('col_key')
 
     def transform(self, df):
         """
-        Add column with col_value to dataframe
-        :return; Dataframe w/ new column containing col_value
+        Map values in the DataFrame column to new values based on the specified mapping.
+
+        :param df: The input DataFrame to be transformed.
+        :return: A new DataFrame with the new column containing the mapped values.
+        :raises: SerraRunException if any required config parameter is missing or if column specified
+                 as 'col_key' does not exist in the DataFrame.
         """
         if not self.name or not self.col_key:
             raise SerraRunException("Both 'name' and 'col_key' must be provided in the config.")
         
         if not self.map_dict and not self.map_dict_path:
             raise SerraRunException("Either 'map_dict' or 'map_dict_path' must be provided in the config.")
```

### Comparing `serra-0.7.1/serra/transformers/select_transformer.py` & `serra-0.7.11/serra/transformers/select_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,33 @@
 from pyspark.sql import functions as F
 
 from serra.transformers.transformer import Transformer
 from serra.exceptions import SerraRunException
 
 class SelectTransformer(Transformer):
     """
-    Transformer to perform a SELECT operation on a DataFrame.
-    :param config: Holds the list of columns to select from the DataFrame.
+    A transformer to perform a SELECT operation on a DataFrame.
+
+    :param config: A dictionary containing the configuration for the transformer.
+                   It should have the following key:
+                   - 'columns': A list of column names to select from the DataFrame.
     """
 
     def __init__(self, config):
         self.config = config
         self.columns = config.get("columns", [])
 
     def transform(self, df: DataFrame) -> DataFrame:
         """
         Perform the SELECT operation on the DataFrame.
-        :param df: Input DataFrame.
-        :return: Transformed DataFrame with only the selected columns.
+
+        :param df: The input DataFrame to be transformed.
+        :return: A new DataFrame containing only the selected columns.
+        :raises: SerraRunException if no columns are specified in the configuration
+                 or if none of the specified columns exist in the DataFrame.
         """
         if not self.columns:
             raise SerraRunException("No columns specified in the configuration.")
 
         selected_columns = [F.col(col) for col in self.columns if col in df.columns]
 
         if not selected_columns:
```

### Comparing `serra-0.7.1/serra/utils.py` & `serra-0.7.11/serra/utils.py`

 * *Files identical despite different names*

### Comparing `serra-0.7.1/serra/writers/snowflake_writer.py` & `serra-0.7.11/serra/writers/snowflake_writer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 import snowflake.connector
 from loguru import logger
 
 from serra.profile import get_serra_profile
 from serra.exceptions import SerraRunException
 
 class SnowflakeWriter():
+    """
+    A writer to write data from a Spark DataFrame to a Snowflake table.
+
+    :param config: A dictionary containing the configuration for the writer.
+                   It should have the following keys:
+                   - 'type': The type of operation to perform. Possible values are 'create' or 'insert'.
+                   - 'warehouse': The Snowflake warehouse to use for the connection.
+                   - 'database': The name of the Snowflake database to write to.
+                   - 'schema': The name of the Snowflake schema to write to.
+                   - 'table': The name of the Snowflake table to write to.
+    """
+
     def __init__(self, config):
         self.config = config
         self.type = self.config.get('type')
         self.snowflake_account = get_serra_profile().snowflake_account
     
     @property
     def user(self):
@@ -23,14 +35,19 @@
         return self.snowflake_account.get("ACCOUNT")
     
     @property
     def dependencies(self):
         return [self.config.get('input_block')]
     
     def write(self, spark_df):
+        """
+        Write data from a Spark DataFrame to a Snowflake table.
+
+        :param spark_df: The Spark DataFrame to be written to the Snowflake table.
+        """
         pandas_df = spark_df.toPandas()
 
         conn = snowflake.connector.connect(
             user=self.user,
             password=self.password,
             account=self.account,
             warehouse=self.config.get('warehouse'),
```

### Comparing `serra-0.7.1/serra.egg-info/SOURCES.txt` & `serra-0.7.11/serra.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -58,32 +58,35 @@
 serra/data/workspace_example/sql/easy_demo.sql
 serra/data/workspace_example/sql/hard_demo.sql
 serra/readers/__init__.py
 serra/readers/amazon_reader.py
 serra/readers/databricks_reader.py
 serra/readers/local_reader.py
 serra/readers/reader.py
-serra/readers/s3_reader.py
 serra/readers/snowflaker_reader.py
 serra/runners/ExecutionGraph.py
 serra/runners/__init__.py
 serra/runners/graph_runner.py
 serra/transformers/__init__.py
 serra/transformers/add_column_transformer.py
+serra/transformers/aggregate_transformer.py
 serra/transformers/case_when_transformer.py
 serra/transformers/cast_columns_transformer.py
+serra/transformers/coalesce_transformer.py
 serra/transformers/drop_columns_transformer.py
 serra/transformers/filter_transformer.py
 serra/transformers/get_count_transformer.py
+serra/transformers/get_distinct_transformer.py
+serra/transformers/impute_transformer.py
 serra/transformers/join_transformer.py
 serra/transformers/map_transformer.py
+serra/transformers/order_by_transformer.py
 serra/transformers/pivot_transformer.py
 serra/transformers/rename_column_transformer.py
 serra/transformers/select_transformer.py
 serra/transformers/transformer.py
 serra/writers/__init__.py
 serra/writers/amazon_writer.py
 serra/writers/databricks_writer.py
 serra/writers/local_writer.py
-serra/writers/s3_writer.py
 serra/writers/snowflake_writer.py
 serra/writers/writer.py
```

### Comparing `serra-0.7.1/setup.py` & `serra-0.7.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import setup
 
 setup(name='serra',
-      version='0.7.1',
+      version='0.7.11',
       description='Simplified Data Pipelines',
       url='http://github.com',
       author='Serra Technologies',
       author_email='founders@serra.io',
       packages=setuptools.find_packages(),
       package_data={"serra": ["data/workspace_example/*",
                               "data/workspace_example/*/*",
@@ -24,8 +24,8 @@
       ],
       zip_safe=False,
       entry_points={
         'console_scripts': [
             'serra=serra.cli:main',
             'serra_databricks=serra.cli:serra_databricks'
         ]
-    })
+    })
```

