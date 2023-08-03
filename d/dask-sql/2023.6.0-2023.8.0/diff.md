# Comparing `tmp/dask_sql-2023.6.0.tar.gz` & `tmp/dask_sql-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask_sql-2023.6.0.tar", last modified: Thu Jun  8 16:19:57 2023, max compression
+gzip compressed data, was "dask_sql-2023.8.0.tar", last modified: Thu Aug  3 18:52:10 2023, max compression
```

## Comparing `dask_sql-2023.6.0.tar` & `dask_sql-2023.8.0.tar`

### file list

```diff
@@ -1,183 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.155178 dask_sql-2023.6.0/dask_planner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.155178 dask_sql-2023.6.0/dask_planner/.cargo/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.cargo/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.classpath
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.155178 dask_sql-2023.6.0/dask_planner/.settings/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.settings/org.eclipse.core.resources.prefs
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.settings/org.eclipse.jdt.apt.core.prefs
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.settings/org.eclipse.jdt.core.prefs
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.settings/org.eclipse.m2e.core.prefs
--rw-r--r--   0 runner    (1001) docker     (123)   101603 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.155178 dask_sql-2023.6.0/dask_planner/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/dialect.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36601 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/expression.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    54871 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/parser.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.155178 dask_sql-2023.6.0/dask_planner/src/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/column.rs
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/exceptions.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/function.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.159178 dask_sql-2023.6.0/dask_planner/src/sql/logical/
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/aggregate.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/alter_schema.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/alter_table.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/analyze_table.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/create_catalog_schema.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/create_experiment.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/create_memory_table.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/create_model.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/create_table.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/describe_model.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_model.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_schema.rs
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_table.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/empty_relation.rs
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/export_model.rs
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/filter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/join.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/limit.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/predict_model.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/projection.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/repartition_by.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/show_columns.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/show_models.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/show_schemas.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/show_tables.rs
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/sort.rs
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/subquery_alias.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/table_scan.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/use_schema.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/window.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17170 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.159178 dask_sql-2023.6.0/dask_planner/src/sql/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/optimizer/join_reorder.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/optimizer.rs
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/parser_utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/schema.rs
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/statement.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/table.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.159178 dask_sql-2023.6.0/dask_planner/src/sql/types/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/types/rel_data_type.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/types/rel_data_type_field.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/types.rs
--rw-r--r--   0 runner    (1001) docker     (123)    32505 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql.rs
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/update-dependencies.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/dask_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/dask_sql/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    36798 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/datacontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.163178 dask_sql-2023.6.0/dask_sql/input_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/hive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/intake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/pandaslike.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.163178 dask_sql-2023.6.0/dask_sql/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/integrations/fugue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/integrations/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.163178 dask_sql-2023.6.0/dask_sql/physical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.163178 dask_sql-2023.6.0/dask_sql/physical/rel/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.167178 dask_sql-2023.6.0/dask_sql/physical/rel/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/alter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/analyze_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_catalog_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_memory_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/describe_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/distributeby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/export_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/predict_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/use_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    28036 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.167178 dask_sql-2023.6.0/dask_sql/physical/rel/logical/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21656 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/cross_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/subquery_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/table_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/union.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/values.py
--rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.167178 dask_sql-2023.6.0/dask_sql/physical/rex/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.167178 dask_sql-2023.6.0/dask_sql/physical/rex/core/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    36009 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/input_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/literal.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/subquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/dask_sql/physical/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/ml_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/dask_sql/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/server/presto_jdbc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/server/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/sql-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/sql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.163178 dask_sql-2023.6.0/dask_sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83601 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.574488 dask_sql-2023.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-08-03 18:52:10.574488 dask_sql-2023.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.538488 dask_sql-2023.8.0/dask_planner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.538488 dask_sql-2023.8.0/dask_planner/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/.cargo/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/.classpath
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.538488 dask_sql-2023.8.0/dask_planner/.settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/.settings/org.eclipse.core.resources.prefs
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/.settings/org.eclipse.jdt.apt.core.prefs
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/.settings/org.eclipse.jdt.core.prefs
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/.settings/org.eclipse.m2e.core.prefs
+-rw-r--r--   0 runner    (1001) docker     (123)   101573 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.542488 dask_sql-2023.8.0/dask_planner/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/dialect.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36601 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/expression.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    54871 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/parser.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.542488 dask_sql-2023.8.0/dask_planner/src/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/column.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/exceptions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/function.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.554488 dask_sql-2023.8.0/dask_planner/src/sql/logical/
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/aggregate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/alter_schema.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/alter_table.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/analyze_table.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/create_catalog_schema.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/create_experiment.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/create_memory_table.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/create_model.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/create_table.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/describe_model.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/drop_model.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/drop_schema.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/drop_table.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/empty_relation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/export_model.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/filter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/join.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/limit.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/predict_model.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/projection.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/repartition_by.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/show_columns.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/show_models.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/show_schemas.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/show_tables.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/sort.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/subquery_alias.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/table_scan.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/use_schema.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical/window.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17170 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/logical.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.554488 dask_sql-2023.8.0/dask_planner/src/sql/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)    44085 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/optimizer/dynamic_partition_pruning.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/optimizer/join_reorder.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/optimizer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/parser_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/schema.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/statement.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/table.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.554488 dask_sql-2023.8.0/dask_planner/src/sql/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/types/rel_data_type.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/types/rel_data_type_field.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql/types.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    34826 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/src/sql.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_planner/update-dependencies.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.574488 dask_sql-2023.8.0/dask_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-03 18:52:10.574488 dask_sql-2023.8.0/dask_sql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37110 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/datacontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.562488 dask_sql-2023.8.0/dask_sql/input_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/input_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/input_utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/input_utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/input_utils/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/input_utils/hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/input_utils/intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/input_utils/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/input_utils/pandaslike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/input_utils/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.562488 dask_sql-2023.8.0/dask_sql/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/integrations/fugue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/integrations/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.562488 dask_sql-2023.8.0/dask_sql/physical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.562488 dask_sql-2023.8.0/dask_sql/physical/rel/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.566488 dask_sql-2023.8.0/dask_sql/physical/rel/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/alter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/analyze_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/create_catalog_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/create_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/create_memory_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/describe_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/distributeby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/drop_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/drop_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/drop_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/export_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/predict_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/show_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/show_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/show_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/show_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/use_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28036 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/custom/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.570488 dask_sql-2023.8.0/dask_sql/physical/rel/logical/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21656 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/cross_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/subquery_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/table_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rel/logical/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.570488 dask_sql-2023.8.0/dask_sql/physical/rex/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rex/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.570488 dask_sql-2023.8.0/dask_sql/physical/rex/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rex/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rex/core/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36906 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rex/core/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rex/core/input_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rex/core/literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/rex/core/subquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.574488 dask_sql-2023.8.0/dask_sql/physical/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20259 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/utils/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/utils/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/utils/ml_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/physical/utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.574488 dask_sql-2023.8.0/dask_sql/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/server/presto_jdbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/server/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/sql-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/sql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/dask_sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 18:52:10.558488 dask_sql-2023.8.0/dask_sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-08-03 18:52:10.000000 dask_sql-2023.8.0/dask_sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-08-03 18:52:10.000000 dask_sql-2023.8.0/dask_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:52:10.000000 dask_sql-2023.8.0/dask_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-03 18:52:10.000000 dask_sql-2023.8.0/dask_sql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 18:52:10.000000 dask_sql-2023.8.0/dask_sql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-03 18:52:10.000000 dask_sql-2023.8.0/dask_sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 18:52:10.000000 dask_sql-2023.8.0/dask_sql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-03 18:52:10.574488 dask_sql-2023.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83601 2023-08-03 18:51:15.000000 dask_sql-2023.8.0/versioneer.py
```

### Comparing `dask_sql-2023.6.0/LICENSE.txt` & `dask_sql-2023.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/PKG-INFO` & `dask_sql-2023.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask_sql
-Version: 2023.6.0
+Version: 2023.8.0
 Summary: SQL query layer for Dask
 Home-page: https://github.com/dask-contrib/dask-sql/
 Maintainer: Nils Braun
 Maintainer-email: nilslennartbraun@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `dask_sql-2023.6.0/README.md` & `dask_sql-2023.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/.classpath` & `dask_sql-2023.8.0/dask_planner/.classpath`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/.gitignore` & `dask_sql-2023.8.0/dask_planner/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/Cargo.lock` & `dask_sql-2023.8.0/dask_planner/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -346,26 +346,26 @@
 name = "async-recursion"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "a564d521dd56509c4c47480d00b80ee55f7e385ae48db5744c67ad50c92d2ebf"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -690,15 +690,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
@@ -707,15 +707,15 @@
 name = "cxxbridge-macro"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
@@ -732,15 +732,15 @@
 version = "0.1.0"
 dependencies = [
  "async-trait",
  "datafusion-python",
  "env_logger",
  "log",
  "pyo3",
- "pyo3-build-config 0.19.0",
+ "pyo3-build-config 0.19.1",
  "pyo3-log",
 ]
 
 [[package]]
 name = "datafusion"
 version = "22.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -903,15 +903,15 @@
  "mimalloc",
  "object_store",
  "parking_lot",
  "pyo3",
  "pyo3-build-config 0.18.3",
  "rand",
  "regex-syntax 0.6.29",
- "syn 2.0.15",
+ "syn 2.0.23",
  "tokio",
  "url",
  "uuid",
 ]
 
 [[package]]
 name = "datafusion-row"
@@ -1167,15 +1167,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -2210,20 +2210,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "lz4"
 version = "1.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
 dependencies = [
@@ -2646,28 +2643,28 @@
 [[package]]
 name = "prettyplease"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ceca8aaf45b5c46ec7ed39fff75f57290368c1846d33d24a122ca81416ab058"
 dependencies = [
  "proc-macro2",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prodash"
 version = "23.1.2"
@@ -2751,17 +2748,17 @@
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
@@ -2771,17 +2768,17 @@
 dependencies = [
  "libc",
  "pyo3-build-config 0.18.3",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c94ff6535a6bae58d7d0b85e60d4c53f7f84d0d0aa35d6a28c3f3e70bfe51444"
+checksum = "f47b0777feb17f61eea78667d61103758b243a871edc09a7786500a50467b605"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
@@ -2821,17 +2818,17 @@
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -3128,15 +3125,15 @@
 name = "serde_derive"
 version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_derive_internals"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
@@ -3353,15 +3350,15 @@
  "prost-build",
  "prost-types",
  "schemars",
  "semver",
  "serde",
  "serde_json",
  "serde_yaml",
- "syn 2.0.15",
+ "syn 2.0.23",
  "typify",
  "walkdir",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.4.1"
@@ -3377,17 +3374,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3431,15 +3428,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "thrift"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
@@ -3535,15 +3532,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.23.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
@@ -3600,15 +3597,15 @@
 name = "tracing-attributes"
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
```

### Comparing `dask_sql-2023.6.0/dask_planner/Cargo.toml` & `dask_sql-2023.8.0/dask_planner/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 description = "Bindings for DataFusion used by Dask-SQL"
 readme = "README.md"
 license = "Apache-2.0"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
-async-trait = "0.1.68"
+async-trait = "0.1.71"
 datafusion-python = { git = "https://github.com/apache/arrow-datafusion-python.git", rev = "9493638" }
 env_logger = "0.10"
 log = "^0.4"
 pyo3 = { version = "0.18.3", features = ["extension-module", "abi3", "abi3-py38"] }
-pyo3-log = "0.8.2"
+pyo3-log = "0.8.3"
 
 [build-dependencies]
-pyo3-build-config = "0.19.0"
+pyo3-build-config = "0.19.1"
 
 [lib]
 crate-type = ["cdylib"]
```

### Comparing `dask_sql-2023.6.0/dask_planner/src/dialect.rs` & `dask_sql-2023.8.0/dask_planner/src/dialect.rs`

 * *Files 11% similar despite different names*

```diff
@@ -190,14 +190,43 @@
                         name: ObjectName(vec![Ident::new("dsql_totimestamp")]),
                         args,
                         over: None,
                         distinct: false,
                         special: false,
                     })))
                 }
+                Token::Word(w) if w.value.to_lowercase() == "extract" => {
+                    // EXTRACT(DATE FROM d)
+                    parser.next_token(); // skip extract
+                    parser.expect_token(&Token::LParen)?;
+                    if !parser.parse_keywords(&[Keyword::DATE, Keyword::FROM]) {
+                        // Parse EXTRACT(x FROM d) as normal
+                        parser.prev_token();
+                        parser.prev_token();
+                        return Ok(None);
+                    }
+                    let expr = parser.parse_expr()?;
+                    parser.expect_token(&Token::RParen)?;
+
+                    // convert to function args
+                    let args = vec![
+                        FunctionArg::Unnamed(FunctionArgExpr::Expr(Expr::Value(
+                            Value::SingleQuotedString("DATE".to_string()),
+                        ))),
+                        FunctionArg::Unnamed(FunctionArgExpr::Expr(expr)),
+                    ];
+
+                    Ok(Some(Expr::Function(Function {
+                        name: ObjectName(vec![Ident::new("extract_date")]),
+                        args,
+                        over: None,
+                        distinct: false,
+                        special: false,
+                    })))
+                }
                 _ => Ok(None),
             }
         }
         match parse_expr(parser) {
             Ok(Some(expr)) => Some(Ok(expr)),
             Ok(None) => None,
             Err(e) => Some(Err(e)),
```

### Comparing `dask_sql-2023.6.0/dask_planner/src/error.rs` & `dask_sql-2023.8.0/dask_planner/src/error.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/expression.rs` & `dask_sql-2023.8.0/dask_planner/src/expression.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/lib.rs` & `dask_sql-2023.8.0/dask_planner/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/parser.rs` & `dask_sql-2023.8.0/dask_planner/src/parser.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/column.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/column.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/exceptions.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/exceptions.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/function.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/function.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/aggregate.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/aggregate.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/alter_schema.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/alter_schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/alter_table.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/alter_table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/analyze_table.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/analyze_table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/create_catalog_schema.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/create_catalog_schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/create_experiment.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/create_experiment.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/create_memory_table.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/create_memory_table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/create_model.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/create_model.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/create_table.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/create_table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/describe_model.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/describe_model.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_model.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/drop_model.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_schema.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/drop_schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_table.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/drop_table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/empty_relation.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/empty_relation.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/explain.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/explain.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/export_model.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/export_model.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/filter.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/filter.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/join.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/join.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/limit.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/limit.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/predict_model.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/predict_model.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/projection.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/projection.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/repartition_by.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/repartition_by.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/show_columns.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/show_columns.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/show_models.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/show_models.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/show_schemas.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/show_schemas.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/show_tables.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/show_tables.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/sort.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/sort.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/subquery_alias.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/subquery_alias.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/table_scan.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/table_scan.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::sync::Arc;
+use std::{sync::Arc, vec};
 
 use datafusion_python::{
     datafusion_common::{DFSchema, ScalarValue},
     datafusion_expr::{logical_plan::TableScan, Expr, LogicalPlan},
 };
 use pyo3::prelude::*;
 
@@ -15,43 +15,45 @@
 #[pyclass(name = "TableScan", module = "dask_planner", subclass)]
 #[derive(Clone)]
 pub struct PyTableScan {
     pub(crate) table_scan: TableScan,
     input: Arc<LogicalPlan>,
 }
 
+type FilterTuple = (String, String, Option<Vec<PyObject>>);
 #[pyclass(name = "FilteredResult", module = "dask_planner", subclass)]
 #[derive(Debug, Clone)]
 pub struct PyFilteredResult {
     // Certain Expr(s) do not have supporting logic in pyarrow for IO filtering
     // at read time. Those Expr(s) cannot be ignored however. This field stores
     // those Expr(s) so that they can be used on the Python side to create
     // Dask operations that handle that filtering as an extra task in the graph.
     #[pyo3(get)]
     pub io_unfilterable_exprs: Vec<PyExpr>,
     // Expr(s) that can have their filtering logic performed in the pyarrow IO logic
     // are stored here in a DNF format that is expected by pyarrow.
     #[pyo3(get)]
-    pub filtered_exprs: Vec<(String, String, Vec<PyObject>)>,
+    pub filtered_exprs: Vec<(PyExpr, FilterTuple)>,
 }
 
 impl PyTableScan {
     /// Ensures that a valid Expr variant type is present
     fn _valid_expr_type(expr: &[Expr]) -> bool {
         expr.iter()
             .all(|f| matches!(f, Expr::Column(_) | Expr::Literal(_)))
     }
 
     /// Transform the singular Expr instance into its DNF form serialized in a Vec instance. Possibly recursively expanding
     /// it as well if needed.
     pub fn _expand_dnf_filter(
         filter: &Expr,
+        input: &Arc<LogicalPlan>,
         py: Python,
-    ) -> Result<Vec<(String, String, Vec<PyObject>)>, DaskPlannerError> {
-        let mut filter_tuple: Vec<(String, String, Vec<PyObject>)> = Vec::new();
+    ) -> Result<Vec<(PyExpr, FilterTuple)>, DaskPlannerError> {
+        let mut filter_tuple: Vec<(PyExpr, FilterTuple)> = Vec::new();
 
         match filter {
             Expr::InList {
                 expr,
                 list,
                 negated,
             } => {
@@ -96,52 +98,75 @@
                                 ))),
                             },
                             _ => Ok(f.canonical_name().into_py(py)),
                         })
                         .collect();
 
                     filter_tuple.push((
-                        ident.unwrap_or(expr.canonical_name()),
-                        op.to_string(),
-                        il?,
+                        PyExpr::from(filter.clone(), Some(vec![input.clone()])),
+                        (
+                            ident.unwrap_or(expr.canonical_name()),
+                            op.to_string(),
+                            Some(il?),
+                        ),
                     ));
                     Ok(filter_tuple)
                 } else {
                     let er = DaskPlannerError::InvalidIOFilter(format!(
                         "Invalid identifying column Expr instance `{}`. using in Dask instead",
                         filter
                     ));
-                    Err::<Vec<(String, String, Vec<PyObject>)>, DaskPlannerError>(er)
+                    Err::<Vec<(PyExpr, FilterTuple)>, DaskPlannerError>(er)
                 }
             }
+            Expr::IsNotNull(expr) => {
+                // Only handle simple Expr(s) for IsNotNull operations for now
+                let ident = match *expr.clone() {
+                    Expr::Column(col) => Ok(col.name),
+                    _ => Err(DaskPlannerError::InvalidIOFilter(format!(
+                        "Invalid IsNotNull Expr type `{}`. using in Dask instead",
+                        filter
+                    ))),
+                };
+
+                filter_tuple.push((
+                    PyExpr::from(filter.clone(), Some(vec![input.clone()])),
+                    (
+                        ident.unwrap_or(expr.canonical_name()),
+                        "is not".to_string(),
+                        None,
+                    ),
+                ));
+                Ok(filter_tuple)
+            }
             _ => {
                 let er = DaskPlannerError::InvalidIOFilter(format!(
                     "Unable to apply filter: `{}` to IO reader, using in Dask instead",
                     filter
                 ));
-                Err::<Vec<(String, String, Vec<PyObject>)>, DaskPlannerError>(er)
+                Err::<Vec<(PyExpr, FilterTuple)>, DaskPlannerError>(er)
             }
         }
     }
 
     /// Consume the `TableScan` filters (Expr(s)) and convert them into a PyArrow understandable
     /// DNF format that can be directly passed to PyArrow IO readers for Predicate Pushdown. Expr(s)
     /// that cannot be converted to correlating PyArrow IO calls will be returned as is and can be
     /// used in the Python logic to form Dask tasks for the graph to do computational filtering.
     pub fn _expand_dnf_filters(
         input: &Arc<LogicalPlan>,
         filters: &[Expr],
         py: Python,
     ) -> PyFilteredResult {
-        let mut filtered_exprs: Vec<(String, String, Vec<PyObject>)> = Vec::new();
+        let mut filtered_exprs: Vec<(PyExpr, FilterTuple)> = Vec::new();
         let mut unfiltered_exprs: Vec<PyExpr> = Vec::new();
 
         filters
             .iter()
-            .for_each(|f| match PyTableScan::_expand_dnf_filter(f, py) {
+            .for_each(|f| match PyTableScan::_expand_dnf_filter(f, input, py) {
                 Ok(mut expanded_dnf_filter) => filtered_exprs.append(&mut expanded_dnf_filter),
                 Err(_e) => {
                     unfiltered_exprs.push(PyExpr::from(f.clone(), Some(vec![input.clone()])))
                 }
             });
 
         PyFilteredResult {
```

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/use_schema.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/use_schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical/window.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical/window.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/logical.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/logical.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/optimizer/join_reorder.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/optimizer/join_reorder.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/optimizer.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/optimizer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,17 @@
         simplify_expressions::SimplifyExpressions,
         unwrap_cast_in_comparison::UnwrapCastInComparison,
         OptimizerContext,
     },
 };
 use log::{debug, trace};
 
+mod dynamic_partition_pruning;
+use dynamic_partition_pruning::DynamicPartitionPruning;
+
 mod join_reorder;
 use join_reorder::JoinReorder;
 
 /// Houses the optimization logic for Dask-SQL. This optimization controls the optimizations
 /// and their ordering in regards to their impact on the underlying `LogicalPlan` instance
 pub struct DaskSqlOptimizer {
     optimizer: Optimizer,
@@ -82,21 +85,40 @@
         ];
 
         Self {
             optimizer: Optimizer::with_rules(rules),
         }
     }
 
+    // Create a separate instance of this optimization rule, since we want to ensure that it only
+    // runs one time
+    pub fn dynamic_partition_pruner() -> Self {
+        let rule: Vec<Arc<dyn OptimizerRule + Sync + Send>> =
+            vec![Arc::new(DynamicPartitionPruning::new())];
+
+        Self {
+            optimizer: Optimizer::with_rules(rule),
+        }
+    }
+
     /// Iterates through the configured `OptimizerRule`(s) to transform the input `LogicalPlan`
     /// to its final optimized form
     pub(crate) fn optimize(&self, plan: LogicalPlan) -> Result<LogicalPlan, DataFusionError> {
         let config = OptimizerContext::new();
         self.optimizer.optimize(&plan, &config, Self::observe)
     }
 
+    /// Iterates once through the configured `OptimizerRule`(s) to transform the input `LogicalPlan`
+    /// to its final optimized form
+    pub(crate) fn optimize_once(&self, plan: LogicalPlan) -> Result<LogicalPlan, DataFusionError> {
+        let mut config = OptimizerContext::new();
+        config = OptimizerContext::with_max_passes(config, 1);
+        self.optimizer.optimize(&plan, &config, Self::observe)
+    }
+
     fn observe(optimized_plan: &LogicalPlan, optimization: &dyn OptimizerRule) {
         trace!(
             "== AFTER APPLYING RULE {} ==\n{}\n",
             optimization.name(),
             optimized_plan.display_indent()
         );
     }
```

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/parser_utils.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/parser_utils.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/schema.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/statement.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/statement.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/table.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/table.rs`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     /// Access optional statistics associated with this table source
     pub fn statistics(&self) -> Option<&DaskStatistics> {
         self.statistics.as_ref()
     }
 
     /// Access optional filepath associated with this table source
-    #[allow(dead_code)]
     pub fn filepath(&self) -> Option<&String> {
         self.filepath.as_ref()
     }
 }
 
 /// Implement TableSource, used in the logical query plan and in logical query optimizations
 #[async_trait]
```

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/types/rel_data_type.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/types/rel_data_type.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/types/rel_data_type_field.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/types/rel_data_type_field.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql/types.rs` & `dask_sql-2023.8.0/dask_planner/src/sql/types.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_planner/src/sql.rs` & `dask_sql-2023.8.0/dask_planner/src/sql.rs`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 #[pyclass(name = "DaskSQLContext", module = "dask_planner", subclass)]
 #[derive(Debug, Clone)]
 pub struct DaskSQLContext {
     current_catalog: String,
     current_schema: String,
     schemas: HashMap<String, schema::DaskSchema>,
     options: ConfigOptions,
+    dynamic_partition_pruning: bool,
 }
 
 impl ContextProvider for DaskSQLContext {
     fn get_table_provider(
         &self,
         name: TableReference,
     ) -> Result<Arc<dyn TableSource>, DataFusionError> {
@@ -239,26 +240,43 @@
                             DataType::Date64,
                         ]),
                         TypeSignature::Exact(vec![
                             DataType::Utf8,
                             DataType::Int64,
                             DataType::Timestamp(TimeUnit::Nanosecond, None),
                         ]),
+                        TypeSignature::Exact(vec![
+                            DataType::Utf8,
+                            DataType::Int64,
+                            DataType::Int64,
+                        ]),
                     ],
                     Volatility::Immutable,
                 );
                 let rtf: ReturnTypeFunction = Arc::new(|_| Ok(Arc::new(DataType::Date64)));
                 return Some(Arc::new(ScalarUDF::new(name, &sig, &rtf, &fun)));
             }
             "timestampdiff" => {
-                let sig = Signature::exact(
+                let sig = Signature::one_of(
                     vec![
-                        DataType::Utf8,
-                        DataType::Timestamp(TimeUnit::Nanosecond, None),
-                        DataType::Timestamp(TimeUnit::Nanosecond, None),
+                        TypeSignature::Exact(vec![
+                            DataType::Utf8,
+                            DataType::Timestamp(TimeUnit::Nanosecond, None),
+                            DataType::Timestamp(TimeUnit::Nanosecond, None),
+                        ]),
+                        TypeSignature::Exact(vec![
+                            DataType::Utf8,
+                            DataType::Date64,
+                            DataType::Date64,
+                        ]),
+                        TypeSignature::Exact(vec![
+                            DataType::Utf8,
+                            DataType::Int64,
+                            DataType::Int64,
+                        ]),
                     ],
                     Volatility::Immutable,
                 );
                 let rtf: ReturnTypeFunction = Arc::new(|_| Ok(Arc::new(DataType::Int64)));
                 return Some(Arc::new(ScalarUDF::new(name, &sig, &rtf, &fun)));
             }
             "dsql_totimestamp" => {
@@ -305,14 +323,28 @@
                         TypeSignature::Exact(vec![DataType::Int64, DataType::Int64]),
                     ],
                     Volatility::Immutable,
                 );
                 let rtf: ReturnTypeFunction = Arc::new(|_| Ok(Arc::new(DataType::Int64)));
                 return Some(Arc::new(ScalarUDF::new(name, &sig, &rtf, &fun)));
             }
+            "extract_date" => {
+                let sig = Signature::one_of(
+                    vec![
+                        TypeSignature::Exact(vec![DataType::Utf8, DataType::Date64]),
+                        TypeSignature::Exact(vec![
+                            DataType::Utf8,
+                            DataType::Timestamp(TimeUnit::Nanosecond, None),
+                        ]),
+                    ],
+                    Volatility::Immutable,
+                );
+                let rtf: ReturnTypeFunction = Arc::new(|_| Ok(Arc::new(DataType::Date64)));
+                return Some(Arc::new(ScalarUDF::new(name, &sig, &rtf, &fun)));
+            }
             _ => (),
         }
 
         // Loop through all of the user defined functions
         for schema in self.schemas.values() {
             for (fun_name, func_mutex) in &schema.functions {
                 if fun_name.eq(name) {
@@ -453,17 +485,23 @@
     #[new]
     pub fn new(default_catalog_name: &str, default_schema_name: &str) -> Self {
         Self {
             current_catalog: default_catalog_name.to_owned(),
             current_schema: default_schema_name.to_owned(),
             schemas: HashMap::new(),
             options: ConfigOptions::new(),
+            dynamic_partition_pruning: false,
         }
     }
 
+    pub fn apply_dynamic_partition_pruning(&mut self, config: bool) -> PyResult<()> {
+        self.dynamic_partition_pruning = config;
+        Ok(())
+    }
+
     /// Change the current schema
     pub fn use_schema(&mut self, schema_name: &str) -> PyResult<()> {
         if self.schemas.contains_key(schema_name) {
             self.current_schema = schema_name.to_owned();
             Ok(())
         } else {
             Err(py_runtime_err(format!(
@@ -542,21 +580,34 @@
             Ok(valid) => {
                 match valid {
                     VisitRecursion::Stop => {
                         // This LogicalPlan does not support Optimization. Return original
                         warn!("This LogicalPlan does not support Optimization. Returning original");
                         Ok(existing_plan)
                     }
-                    _ => optimizer::DaskSqlOptimizer::new()
-                        .optimize(existing_plan.original_plan)
-                        .map(|k| PyLogicalPlan {
-                            original_plan: k,
-                            current_node: None,
-                        })
-                        .map_err(py_optimization_exp),
+                    _ => {
+                        let optimized_plan = optimizer::DaskSqlOptimizer::new()
+                            .optimize(existing_plan.original_plan)
+                            .map(|k| PyLogicalPlan {
+                                original_plan: k,
+                                current_node: None,
+                            })
+                            .map_err(py_optimization_exp);
+                        if self.dynamic_partition_pruning {
+                            optimizer::DaskSqlOptimizer::dynamic_partition_pruner()
+                                .optimize_once(optimized_plan.unwrap().original_plan)
+                                .map(|k| PyLogicalPlan {
+                                    original_plan: k,
+                                    current_node: None,
+                                })
+                                .map_err(py_optimization_exp)
+                        } else {
+                            optimized_plan
+                        }
+                    }
                 }
             }
             Err(e) => Err(py_optimization_exp(e)),
         }
     }
 }
```

### Comparing `dask_sql-2023.6.0/dask_sql/cmd.py` & `dask_sql-2023.8.0/dask_sql/cmd.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/context.py` & `dask_sql-2023.8.0/dask_sql/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,18 @@
         # A started SQL server (useful for jupyter notebooks)
         self.sql_server = None
 
         # Create the `DaskSQLContext` Rust context
         self.context = DaskSQLContext(self.catalog_name, self.schema_name)
         self.context.register_schema(self.schema_name, DaskSchema(self.schema_name))
 
+        self.context.apply_dynamic_partition_pruning(
+            dask_config.get("sql.dynamic_partition_pruning")
+        )
+
         # # Register any default plugins, if nothing was registered before.
         RelConverter.add_plugin_class(logical.DaskAggregatePlugin, replace=False)
         RelConverter.add_plugin_class(logical.DaskCrossJoinPlugin, replace=False)
         RelConverter.add_plugin_class(logical.DaskEmptyRelationPlugin, replace=False)
         RelConverter.add_plugin_class(logical.DaskFilterPlugin, replace=False)
         RelConverter.add_plugin_class(logical.DaskJoinPlugin, replace=False)
         RelConverter.add_plugin_class(logical.DaskLimitPlugin, replace=False)
@@ -791,14 +795,17 @@
 
         return schema_list
 
     def _get_ral(self, sql):
         """Helper function to turn the sql query into a relational algebra and resulting column names"""
 
         logger.debug(f"Entering _get_ral('{sql}')")
+        self.context.apply_dynamic_partition_pruning(
+            dask_config.get("sql.dynamic_partition_pruning")
+        )
 
         # get the schema of what we currently have registered
         schemas = self._prepare_schemas()
         for schema in schemas:
             self.context.register_schema(schema.name, schema)
         try:
             sqlTree = self.context.parse_sql(sql)
@@ -834,34 +841,37 @@
         logger.debug(f"Extracted relational algebra:\n {rel_string}")
 
         return rel, rel_string
 
     def _compute_table_from_rel(self, rel: "LogicalPlan", return_futures: bool = True):
         dc = RelConverter.convert(rel, context=self)
 
-        # Optimization might remove some alias projects. Make sure to keep them here.
-        select_names = [field for field in rel.getRowType().getFieldList()]
-
         if rel.get_current_node_type() == "Explain":
             return dc
         if dc is None:
             return
 
+        # Optimization might remove some alias projects. Make sure to keep them here.
+        select_names = [field for field in rel.getRowType().getFieldList()]
+
         if select_names:
+            cc = dc.column_container
+
+            select_names = select_names[: len(cc.columns)]
+
             # Use FQ name if not unique and simple name if it is unique. If a join contains the same column
             # names the output col is prepended with the fully qualified column name
             field_counts = Counter([field.getName() for field in select_names])
             select_names = [
                 field.getQualifiedName()
                 if field_counts[field.getName()] > 1
                 else field.getName()
                 for field in select_names
             ]
 
-            cc = dc.column_container
             cc = cc.rename(
                 {
                     df_col: select_name
                     for df_col, select_name in zip(cc.columns, select_names)
                 }
             )
             dc = DataContainer(dc.df, cc)
```

### Comparing `dask_sql-2023.6.0/dask_sql/datacontainer.py` & `dask_sql-2023.8.0/dask_sql/datacontainer.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/input_utils/convert.py` & `dask_sql-2023.8.0/dask_sql/input_utils/convert.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/input_utils/dask.py` & `dask_sql-2023.8.0/dask_sql/input_utils/dask.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/input_utils/hive.py` & `dask_sql-2023.8.0/dask_sql/input_utils/hive.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/input_utils/intake.py` & `dask_sql-2023.8.0/dask_sql/input_utils/intake.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/input_utils/location.py` & `dask_sql-2023.8.0/dask_sql/input_utils/location.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/input_utils/pandaslike.py` & `dask_sql-2023.8.0/dask_sql/input_utils/pandaslike.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/input_utils/sqlalchemy.py` & `dask_sql-2023.8.0/dask_sql/input_utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/integrations/fugue.py` & `dask_sql-2023.8.0/dask_sql/integrations/fugue.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/integrations/ipython.py` & `dask_sql-2023.8.0/dask_sql/integrations/ipython.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/mappings.py` & `dask_sql-2023.8.0/dask_sql/mappings.py`

 * *Files 5% similar despite different names*

```diff
@@ -327,32 +327,42 @@
         df[column_name] = casted_column
 
     return df
 
 
 def cast_column_to_type(col: dd.Series, expected_type: str):
     """Cast the given column to the expected type"""
+    pdt = pd.api.types
+
+    is_dt_ns = pdt.is_datetime64_ns_dtype
+    is_dt_tz = lambda t: is_dt_ns(t) and pdt.is_datetime64tz_dtype(t)
+    is_dt_ntz = lambda t: is_dt_ns(t) and not pdt.is_datetime64tz_dtype(t)
+
     current_type = col.dtype
 
     if similar_type(current_type, expected_type):
         logger.debug("...not converting.")
         return None
 
-    if pd.api.types.is_integer_dtype(expected_type):
+    if pdt.is_integer_dtype(expected_type):
         if pd.api.types.is_float_dtype(current_type):
             logger.debug("...truncating...")
             # Currently "trunc" can not be applied to NA (the pandas missing value type),
             # because NA is a different type. It works with np.NaN though.
             # For our use case, that does not matter, as the conversion to integer later
             # will convert both NA and np.NaN to NA.
             col = da.trunc(col.fillna(value=np.NaN))
-        elif pd.api.types.is_timedelta64_dtype(current_type):
+        elif pdt.is_timedelta64_dtype(current_type):
             logger.debug(f"Explicitly casting from {current_type} to np.int64")
             return col.astype(np.int64)
 
+    if is_dt_tz(current_type) and is_dt_ntz(expected_type):
+        # casting from timezone-aware to timezone-naive datatypes with astype is deprecated in pandas 2
+        return col.dt.tz_localize(None)
+
     logger.debug(f"Need to cast from {current_type} to {expected_type}")
     return col.astype(expected_type)
 
 
 def is_decimal(dtype):
     """
     Check if dtype is a decimal type
```

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/base.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, List, Optional
 
 import dask.dataframe as dd
 
 from dask_sql.datacontainer import ColumnContainer, DataContainer
 from dask_sql.mappings import cast_column_type, sql_to_python_type
 
 if TYPE_CHECKING:
@@ -26,23 +26,25 @@
 
     def convert(self, rel: "LogicalPlan", context: "dask_sql.Context") -> dd.DataFrame:
         """Base method to implement"""
         raise NotImplementedError
 
     @staticmethod
     def fix_column_to_row_type(
-        cc: ColumnContainer, row_type: "RelDataType"
+        cc: ColumnContainer, row_type: "RelDataType", join_type: Optional[str] = None
     ) -> ColumnContainer:
         """
         Make sure that the given column container
         has the column names specified by the row type.
         We assume that the column order is already correct
         and will just "blindly" rename the columns.
         """
         field_names = [str(x) for x in row_type.getFieldNames()]
+        if join_type in ("leftsemi", "leftanti"):
+            field_names = field_names[: len(cc.columns)]
 
         logger.debug(f"Renaming {cc.columns} to {field_names}")
         cc = cc.rename_handle_duplicates(
             from_columns=cc.columns, to_columns=field_names
         )
 
         # TODO: We can also check for the types here and do any conversions if needed
@@ -80,31 +82,36 @@
 
         # Late import to remove cycling dependency
         from dask_sql.physical.rel.convert import RelConverter
 
         return [RelConverter.convert(input_rel, context) for input_rel in input_rels]
 
     @staticmethod
-    def fix_dtype_to_row_type(dc: DataContainer, row_type: "RelDataType"):
+    def fix_dtype_to_row_type(
+        dc: DataContainer, row_type: "RelDataType", join_type: Optional[str] = None
+    ):
         """
         Fix the dtype of the given data container (or: the df within it)
         to the data type given as argument.
         To prevent unneeded conversions, do only convert if really needed,
         e.g. if the two types are "similar" enough, do not convert.
         Similarity involves the same general type (int, float, string etc)
         but not necessary the size (int64 and int32 are compatible)
         or the nullability.
         TODO: we should check the nullability of the SQL type
         """
         df = dc.df
         cc = dc.column_container
 
+        field_list = row_type.getFieldList()
+        if join_type in ("leftsemi", "leftanti"):
+            field_list = field_list[: len(cc.columns)]
+
         field_types = {
-            str(field.getQualifiedName()): field.getType()
-            for field in row_type.getFieldList()
+            str(field.getQualifiedName()): field.getType() for field in field_list
         }
 
         for field_name, field_type in field_types.items():
             sql_type = field_type.getSqlType()
             sql_type_args = tuple()
 
             if str(sql_type) == "SqlTypeName.DECIMAL":
```

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/convert.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/convert.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/__init__.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/alter.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/alter.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/analyze_table.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/analyze_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,32 +43,28 @@
             columns = dc.column_container.columns
 
         # Define some useful shortcuts
         mapping = dc.column_container.get_backend_by_frontend_name
         df = dc.df
 
         # Calculate statistics
-        statistics = dd.from_pandas(
-            pd.DataFrame({col: [] for col in columns}), npartitions=1
-        )
-        statistics = statistics.append(df[[mapping(col) for col in columns]].describe())
-
-        # Add additional information
-        statistics = statistics.append(
-            pd.Series(
-                {
-                    col: str(python_to_sql_type(df[mapping(col)].dtype)).lower()
-                    for col in columns
-                },
-                name="data_type",
-            )
-        )
-        statistics = statistics.append(
-            pd.Series(
-                {col: col for col in columns},
-                name="col_name",
-            )
+        statistics = dd.concat(
+            [
+                df[[mapping(col) for col in columns]].describe(),
+                pd.DataFrame(
+                    {
+                        mapping(col): str(
+                            python_to_sql_type(df[mapping(col)].dtype)
+                        ).lower()
+                        for col in columns
+                    },
+                    index=["data_type"],
+                ),
+                pd.DataFrame(
+                    {mapping(col): col for col in columns}, index=["col_name"]
+                ),
+            ]
         )
 
         cc = ColumnContainer(statistics.columns)
         dc = DataContainer(statistics, cc)
         return dc
```

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_catalog_schema.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/create_catalog_schema.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_experiment.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/create_experiment.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_memory_table.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/create_memory_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_model.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/create_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_table.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/create_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/describe_model.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/describe_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/distributeby.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/distributeby.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_model.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/drop_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_schema.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/drop_schema.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_table.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/drop_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/export_model.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/export_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/metrics.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/metrics.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/predict_model.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/predict_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_columns.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/show_columns.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_models.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/show_models.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_schemas.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/show_schemas.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_tables.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/show_tables.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/use_schema.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/use_schema.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/custom/wrappers.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/custom/wrappers.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/__init__.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/aggregate.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/aggregate.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/cross_join.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/cross_join.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/empty.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/empty.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/filter.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, List, Union
 
 import dask.config as dask_config
 import dask.dataframe as dd
 import numpy as np
 
 from dask_sql.datacontainer import DataContainer
 from dask_sql.physical.rel.base import BaseRelPlugin
@@ -13,15 +13,19 @@
 if TYPE_CHECKING:
     import dask_sql
     from dask_planner.rust import LogicalPlan
 
 logger = logging.getLogger(__name__)
 
 
-def filter_or_scalar(df: dd.DataFrame, filter_condition: Union[np.bool_, dd.Series]):
+def filter_or_scalar(
+    df: dd.DataFrame,
+    filter_condition: Union[np.bool_, dd.Series],
+    add_filters: List = None,
+):
     """
     Some (complex) SQL queries can lead to a strange condition which is always true or false.
     We do not need to filter in this case.
     See https://github.com/dask-contrib/dask-sql/issues/87.
     """
     if np.isscalar(filter_condition):
         if not filter_condition:  # pragma: no cover
@@ -31,15 +35,15 @@
         else:
             return df
 
     # In SQL, a NULL in a boolean is False on filtering
     filter_condition = filter_condition.fillna(False)
     out = df[filter_condition]
     if dask_config.get("sql.predicate_pushdown"):
-        return attempt_predicate_pushdown(out)
+        return attempt_predicate_pushdown(out, add_filters=add_filters)
     else:
         return out
 
 
 class DaskFilterPlugin(BaseRelPlugin):
     """
     DaskFilter is used on WHERE clauses.
```

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/join.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/join.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from dask.highlevelgraph import HighLevelGraph
 
 from dask_sql._compat import BROADCAST_JOIN_SUPPORT_WORKING
 from dask_sql.datacontainer import ColumnContainer, DataContainer
 from dask_sql.physical.rel.base import BaseRelPlugin
 from dask_sql.physical.rel.logical.filter import filter_or_scalar
 from dask_sql.physical.rex import RexConverter
+from dask_sql.utils import is_cudf_type
 
 if TYPE_CHECKING:
     import dask_sql
     from dask_planner.rust import Expression, LogicalPlan
 
 logger = logging.getLogger(__name__)
 
@@ -41,15 +42,16 @@
     class_name = "Join"
 
     JOIN_TYPE_MAPPING = {
         "INNER": "inner",
         "LEFT": "left",
         "RIGHT": "right",
         "FULL": "outer",
-        "LEFTSEMI": "inner",  # TODO: Need research here! This is likely not a true inner join
+        "LEFTSEMI": "leftsemi",
+        "LEFTANTI": "leftanti",
     }
 
     def convert(self, rel: "LogicalPlan", context: "dask_sql.Context") -> DataContainer:
         # Joining is a bit more complicated, so lets do it in steps:
 
         join = rel.join()
 
@@ -70,14 +72,18 @@
         dc_rhs_renamed = DataContainer(dc_rhs.df, cc_rhs_renamed)
 
         df_lhs_renamed = dc_lhs_renamed.assign()
         df_rhs_renamed = dc_rhs_renamed.assign()
 
         join_type = join.getJoinType()
         join_type = self.JOIN_TYPE_MAPPING[str(join_type)]
+        # TODO: update with correct implementation of leftsemi for CPU
+        # https://github.com/dask-contrib/dask-sql/issues/1190
+        if join_type == "leftsemi" and not is_cudf_type(df_lhs_renamed):
+            join_type = "inner"
 
         # 3. The join condition can have two forms, that we can understand
         # (a) a = b
         # (b) X AND Y AND a = b AND Z ... (can also be multiple a = b)
         # The first case is very simple and we do not need any additional filter
         # In the second case we do a merge on all the a = b,
         # and then apply a filter using the other expressions.
@@ -166,30 +172,35 @@
             warnings.warn(
                 "Need to do a cross-join, which is typically very resource heavy",
                 ResourceWarning,
             )
 
         # 6. So the next step is to make sure
         # we have the correct column order (and to remove the temporary join columns)
-        correct_column_order = list(df_lhs_renamed.columns) + list(
-            df_rhs_renamed.columns
-        )
+        if join_type in ("leftsemi", "leftanti"):
+            correct_column_order = list(df_lhs_renamed.columns)
+        else:
+            correct_column_order = list(df_lhs_renamed.columns) + list(
+                df_rhs_renamed.columns
+            )
         cc = ColumnContainer(df.columns).limit_to(correct_column_order)
 
         # and to rename them like the rel specifies
         row_type = rel.getRowType()
         field_specifications = [str(f) for f in row_type.getFieldNames()]
+        if join_type in ("leftsemi", "leftanti"):
+            field_specifications = field_specifications[: len(cc.columns)]
 
         cc = cc.rename(
             {
                 from_col: to_col
                 for from_col, to_col in zip(cc.columns, field_specifications)
             }
         )
-        cc = self.fix_column_to_row_type(cc, row_type)
+        cc = self.fix_column_to_row_type(cc, row_type, join_type)
         dc = DataContainer(df, cc)
 
         # 7. Last but not least we apply any filters by and-chaining together the filters
         if filter_condition:
             # This line is a bit of code duplication with RexCallPlugin - but I guess it is worth to keep it separate
             filter_condition = reduce(
                 operator.and_,
@@ -198,15 +209,15 @@
                     for rex in filter_condition
                 ],
             )
             logger.debug(f"Additionally applying filter {filter_condition}")
             df = filter_or_scalar(df, filter_condition)
             dc = DataContainer(df, cc)
 
-        dc = self.fix_dtype_to_row_type(dc, rel.getRowType())
+        dc = self.fix_dtype_to_row_type(dc, rel.getRowType(), join_type)
         # # Rename underlying DataFrame column names back to their original values before returning
         # df = dc.assign()
         # dc = DataContainer(df, ColumnContainer(cc.columns))
         return dc
 
     def _join_on_columns(
         self,
@@ -223,15 +234,15 @@
         # SQL, so we get rid of them here
         if join_type in ["inner", "right"]:
             df_lhs_filter = reduce(
                 operator.and_,
                 [~df_lhs_renamed.iloc[:, index].isna() for index in lhs_on],
             )
             df_lhs_renamed = df_lhs_renamed[df_lhs_filter]
-        if join_type in ["inner", "left"]:
+        if join_type in ["inner", "left", "leftanti", "leftsemi"]:
             df_rhs_filter = reduce(
                 operator.and_,
                 [~df_rhs_renamed.iloc[:, index].isna() for index in rhs_on],
             )
             df_rhs_renamed = df_rhs_renamed[df_rhs_filter]
 
         lhs_columns_to_add = {
@@ -252,20 +263,32 @@
             isinstance(broadcast, float) or broadcast
         ):
             warnings.warn(
                 "Broadcast Joins may not work as expected with dask<2023.1.1"
                 "For more information refer to https://github.com/dask/dask/issues/9851"
                 " and https://github.com/dask/dask/issues/9870"
             )
-        df = df_lhs_with_tmp.merge(
-            df_rhs_with_tmp,
-            on=added_columns,
-            how=join_type,
-            broadcast=broadcast,
-        ).drop(columns=added_columns)
+        if join_type == "leftanti" and not is_cudf_type(df_lhs_with_tmp):
+            df = df_lhs_with_tmp.merge(
+                df_rhs_with_tmp,
+                on=added_columns,
+                how="left",
+                broadcast=broadcast,
+                indicator=True,
+            ).drop(columns=added_columns)
+            df = df[df["_merge"] == "left_only"].drop(
+                columns=["_merge"] + list(df_rhs_with_tmp.columns), errors="ignore"
+            )
+        else:
+            df = df_lhs_with_tmp.merge(
+                df_rhs_with_tmp,
+                on=added_columns,
+                how=join_type,
+                broadcast=broadcast,
+            ).drop(columns=added_columns)
 
         return df
 
     def _split_join_condition(
         self, join_condition: "Expression"
     ) -> Tuple[List[str], List[str], List["Expression"]]:
         if str(join_condition.getRexType()) in ["RexType.Literal", "RexType.Reference"]:
```

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/limit.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/limit.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/project.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/project.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/sample.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/sample.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/sort.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/sort.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/subquery_alias.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/subquery_alias.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/table_scan.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/table_scan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 import operator
 from functools import reduce
 from typing import TYPE_CHECKING
 
+from dask.utils_test import hlg_layer
+
 from dask_sql.datacontainer import DataContainer
 from dask_sql.physical.rel.base import BaseRelPlugin
 from dask_sql.physical.rel.logical.filter import filter_or_scalar
 from dask_sql.physical.rex import RexConverter
 
 if TYPE_CHECKING:
     import dask_sql
@@ -73,20 +75,42 @@
             ]
         cc = cc.limit_to(field_specifications)
         return DataContainer(df, cc)
 
     def _apply_filters(self, table_scan, rel, dc, context):
         df = dc.df
         cc = dc.column_container
-        filters = table_scan.getFilters()
-        # All partial filters here are applied in conjunction (&)
-        if filters:
+        all_filters = table_scan.getFilters()
+        conjunctive_dnf_filters = table_scan.getDNFFilters().filtered_exprs
+        non_dnf_filters = table_scan.getDNFFilters().io_unfilterable_exprs
+
+        if conjunctive_dnf_filters:
+            # Extract the PyExprs from the conjunctive DNF filters
+            filter_exprs = [f[0] for f in conjunctive_dnf_filters]
+            if non_dnf_filters:
+                filter_exprs.extend(non_dnf_filters)
+
+            df_condition = reduce(
+                operator.and_,
+                [
+                    RexConverter.convert(rel, rex, dc, context=context)
+                    for rex in filter_exprs
+                ],
+            )
+            df = filter_or_scalar(
+                df, df_condition, add_filters=[f[1] for f in conjunctive_dnf_filters]
+            )
+        elif all_filters:
             df_condition = reduce(
                 operator.and_,
                 [
                     RexConverter.convert(rel, rex, dc, context=context)
-                    for rex in filters
+                    for rex in all_filters
                 ],
             )
             df = filter_or_scalar(df, df_condition)
+        try:
+            logger.debug(hlg_layer(df.dask, "read-parquet").creation_info)
+        except KeyError:
+            pass
 
         return DataContainer(df, cc)
```

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/union.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/union.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/values.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/values.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rel/logical/window.py` & `dask_sql-2023.8.0/dask_sql/physical/rel/logical/window.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rex/base.py` & `dask_sql-2023.8.0/dask_sql/physical/rex/base.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rex/convert.py` & `dask_sql-2023.8.0/dask_sql/physical/rex/convert.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rex/core/alias.py` & `dask_sql-2023.8.0/dask_sql/physical/rex/core/alias.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rex/core/call.py` & `dask_sql-2023.8.0/dask_sql/physical/rex/core/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pandas as pd
 from dask.base import tokenize
 from dask.dataframe.core import Series
 from dask.highlevelgraph import HighLevelGraph
 from dask.utils import random_state_data
 
 from dask_planner.rust import SqlTypeName
+from dask_sql._compat import DASK_CUDF_TODATETIME_SUPPORT, PANDAS_GT_200
 from dask_sql.datacontainer import DataContainer
 from dask_sql.mappings import (
     cast_column_to_type,
     sql_to_python_type,
     sql_to_python_value,
 )
 from dask_sql.physical.rex import RexConverter
@@ -246,14 +247,17 @@
         sql_type = SqlTypeName.fromString(output_type)
         sql_type_args = ()
 
         # decimal datatypes require precision and scale
         if output_type == "DECIMAL":
             sql_type_args = rex.getPrecisionScale()
 
+        if output_type == "TIMESTAMP" and pd.api.types.is_integer_dtype(operand):
+            operand = operand * 10**9
+
         if not is_frame(operand):  # pragma: no cover
             return sql_to_python_value(sql_type, operand)
 
         python_type = sql_to_python_type(sql_type, *sql_type_args)
 
         return_column = cast_column_to_type(operand, python_type)
 
@@ -608,25 +612,16 @@
 
     def to_timestamp(self, df, format):
         default_format = "%Y-%m-%d %H:%M:%S"
         # Remove double and single quotes from string
         format = format.replace('"', "")
         format = format.replace("'", "")
 
-        # TODO: format timestamps for GPU tests
-        if is_cudf_type(df):
-            if format != default_format:
-                raise RuntimeError("Non-default timestamp formats not supported on GPU")
-            if df.dtype == "object":
-                return df
-            else:
-                nanoseconds_to_seconds = 10**9
-                return df * nanoseconds_to_seconds
         # String cases
-        elif type(df) == str:
+        if type(df) == str:
             return np.datetime64(datetime.strptime(df, format))
         elif df.dtype == "object":
             return dd.to_datetime(df, format=format)
         # Integer cases
         elif np.isscalar(df):
             if format != default_format:
                 raise RuntimeError("Integer input does not accept a format argument")
@@ -651,15 +646,19 @@
         super().__init__(self.timestampadd)
 
     def timestampadd(self, unit, interval, df: SeriesOrScalar):
         unit = unit.upper()
         interval = int(interval)
         if interval < 0:
             raise RuntimeError(f"Negative time interval {interval} is not supported.")
-        df = df.astype("datetime64[ns]")
+        df = (
+            df.astype("datetime64[s]")
+            if pd.api.types.is_integer_dtype(df)
+            else df.astype("datetime64[ns]")
+        )
 
         if is_cudf_type(df):
             from cudf import DateOffset
         else:
             from pandas.tseries.offsets import DateOffset
 
         if unit in {"YEAR", "YEARS"}:
@@ -695,19 +694,31 @@
     which also specifies a sql interval return type for the operation.
     """
 
     def __init__(self):
         super().__init__(self.datetime_sub)
 
     def datetime_sub(self, unit, df1, df2):
+        if pd.api.types.is_integer_dtype(df1):
+            df1 = df1 * 10**9
+        if pd.api.types.is_integer_dtype(df2):
+            df2 = df2 * 10**9
+        if "datetime64[s]" == str(getattr(df1, "dtype", "")):
+            df1 = df1.astype("datetime64[ns]")
+        if "datetime64[s]" == str(getattr(df2, "dtype", "")):
+            df2 = df2.astype("datetime64[ns]")
+
         subtraction_op = ReduceOperation(
             operation=operator.sub, unary_operation=lambda x: -x
         )
         result = subtraction_op(df2, df1)
 
+        if is_cudf_type(df1):
+            result = result.astype("int")
+
         if unit in {"NANOSECOND", "NANOSECONDS"}:
             return result
         elif unit in {"MICROSECOND", "MICROSECONDS"}:
             return result // 1_000
         elif unit in {"SECOND", "SECONDS"}:
             return result // 1_000_000_000
         elif unit in {"MINUTE", "MINUTES"}:
@@ -922,17 +933,27 @@
         elif what in {"MONTH", "MONTHS"}:
             return df.month
         elif what in {"QUARTER", "QUARTERS"}:
             return df.quarter
         elif what in {"SECOND", "SECONDS"}:
             return df.second
         elif what in {"WEEK", "WEEKS"}:
-            return df.week
+            return df.isocalendar().week if PANDAS_GT_200 else df.week
         elif what in {"YEAR", "YEARS"}:
             return df.year
+        elif what == "DATE":
+            if isinstance(df, pd.Timestamp):
+                return df.date()
+            else:
+                if is_cudf_type(df) and not DASK_CUDF_TODATETIME_SUPPORT:
+                    raise RuntimeError(
+                        "Dask-cuDF to_datetime support requires Dask version >= 2023.5.1"
+                    )
+                else:
+                    return dd.to_datetime(df.strftime("%Y-%m-%d"))
         else:
             raise NotImplementedError(f"Extraction of {what} is not (yet) implemented.")
 
 
 class BetweenOperation(Operation):
     """
     Function for finding rows between two scalar values
@@ -1066,14 +1087,15 @@
         "overlay": OverlayOperation(),
         "substr": SubStringOperation(),
         "substring": SubStringOperation(),
         "initcap": TensorScalarOperation(lambda x: x.str.title(), lambda x: x.title()),
         "coalesce": CoalesceOperation(),
         "replace": ReplaceOperation(),
         # date/time operations
+        "extract_date": ExtractOperation(),
         "localtime": Operation(lambda *args: pd.Timestamp.now()),
         "localtimestamp": Operation(lambda *args: pd.Timestamp.now()),
         "current_time": Operation(lambda *args: pd.Timestamp.now()),
         "current_date": Operation(lambda *args: pd.Timestamp.now()),
         "current_timestamp": Operation(lambda *args: pd.Timestamp.now()),
         "last_day": TensorScalarOperation(
             lambda x: x + pd.tseries.offsets.MonthEnd(1),
```

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rex/core/input_ref.py` & `dask_sql-2023.8.0/dask_sql/physical/rex/core/input_ref.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rex/core/literal.py` & `dask_sql-2023.8.0/dask_sql/physical/rex/core/literal.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/rex/core/subquery.py` & `dask_sql-2023.8.0/dask_sql/physical/rex/core/subquery.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/utils/filter.py` & `dask_sql-2023.8.0/dask_sql/physical/utils/filter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import itertools
 import logging
 import operator
 
 import dask.dataframe as dd
 import numpy as np
 from dask.blockwise import Blockwise
@@ -10,28 +12,52 @@
 from dask.utils import M, apply, is_arraylike
 
 from dask_sql._compat import PQ_IS_SUPPORT, PQ_NOT_IN_SUPPORT
 
 logger = logging.getLogger(__name__)
 
 
-def attempt_predicate_pushdown(ddf: dd.DataFrame) -> dd.DataFrame:
+def attempt_predicate_pushdown(
+    ddf: dd.DataFrame,
+    preserve_filters: bool = True,
+    extract_filters: bool = True,
+    add_filters: list | tuple | DNF | None = None,
+) -> dd.DataFrame:
     """Use graph information to update IO-level filters
 
     The original `ddf` will be returned if/when the
     predicate-pushdown optimization fails.
 
     This is a special optimization that must be called
     eagerly on a DataFrame collection when filters are
     applied. The "eager" requirement for this optimization
     is due to the fact that `npartitions` and `divisions`
     may change when this optimization is applied (invalidating
     npartition/divisions-specific logic in following Layers).
+
+    Parameters
+    ----------
+    ddf
+        Dask-DataFrame target for predicate pushdown.
+    preserve_filters
+        Whether to preserve pre-existing filters in the case that either
+        `add_filters` is specified, or `extract_filters` is `True` and
+        filters are successfully extracted from `ddf`. Default is `True`.
+    extract_filters
+        Whether to extract filters from the task graph of `ddf`. Default
+        is `True`.
+    add_filters
+        Custom filters to manually add to the IO layer of `ddf`.
     """
 
+    if not (extract_filters or add_filters):
+        # Not extracting filters from the graph or
+        # manually adding user-defined filters. Return
+        return ddf
+
     # Check that we have a supported `ddf` object
     if not isinstance(ddf, dd.DataFrame):
         raise ValueError(
             f"Predicate pushdown optimization skipped. Type {type(ddf)} "
             f"does not support predicate pushdown."
         )
     elif not isinstance(ddf.dask, HighLevelGraph):
@@ -46,66 +72,73 @@
     io_layer = []
     for k, v in ddf.dask.layers.items():
         if isinstance(v, DataFrameIOLayer):
             io_layer.append(k)
             creation_info = (
                 (v.creation_info or {}) if hasattr(v, "creation_info") else {}
             )
-            if (
-                "filters" not in creation_info.get("kwargs", {})
-                or creation_info["kwargs"]["filters"] is not None
-            ):
-                # No filters support, or filters is already set
+            if "filters" not in creation_info.get("kwargs", {}):
+                # No filters support
                 return ddf
     if len(io_layer) != 1:
         # Not a single IO layer
         return ddf
     io_layer = io_layer.pop()
 
-    # Bail if any filters are already present in ddf
+    # Get pre-existing filters
     existing_filters = (
         ddf.dask.layers[io_layer].creation_info.get("kwargs", {}).get("filters")
     )
-    if existing_filters:
-        return ddf
 
     # Start by converting the HLG to a `RegenerableGraph`.
     # Succeeding here means that all layers in the graph
     # are regenerable.
     try:
         dsk = RegenerableGraph.from_hlg(ddf.dask)
     except (ValueError, TypeError):
         logger.warning(
             "Predicate pushdown optimization skipped. One or more "
             "layers in the HighLevelGraph was not 'regenerable'."
         )
         return ddf
 
-    # Extract a DNF-formatted filter expression
     name = ddf._name
-    try:
-        filters = dsk.layers[name]._dnf_filter_expression(dsk)
-        if not isinstance(filters, frozenset):
-            # No filters encountered
-            return ddf
-        filters = filters.to_list_tuple()
-    except (ValueError, TypeError):
-        # DNF dispatching failed for 1+ layers
-        logger.warning(
-            "Predicate pushdown optimization skipped. One or more "
-            "layers has an unknown filter expression."
-        )
+    extracted_filters = DNF(None)
+    if extract_filters:
+        # Extract a DNF-formatted filter expression
+        try:
+            extracted_filters = dsk.layers[name]._dnf_filter_expression(dsk)
+        except (ValueError, TypeError):
+            # DNF dispatching failed for 1+ layers
+            logger.warning(
+                "Predicate pushdown optimization skipped. One or more "
+                "layers has an unknown filter expression."
+            )
+
+    # Combine filters
+    filters = DNF(None)
+    if preserve_filters:
+        filters = filters.combine(existing_filters)
+    if extract_filters:
+        filters = filters.combine(extracted_filters)
+    if add_filters:
+        filters = filters.combine(add_filters)
+    if not filters:
+        # No filters encountered
         return ddf
+    filters = filters.to_list_tuple()
 
     # Regenerate collection with filtered IO layer
     try:
+        _regen_cache = {}
         return dsk.layers[name]._regenerate_collection(
             dsk,
             # TODO: shouldn't need to specify index=False after dask#9661 is merged
             new_kwargs={io_layer: {"filters": filters, "index": False}},
+            _regen_cache=_regen_cache,
         )
     except ValueError as err:
         # Most-likely failed to apply filters in read_parquet.
         # We can just bail on predicate pushdown, but we also
         # raise a warning to encourage the user to file an issue.
         logger.warning(
             f"Predicate pushdown failed to apply filters: {filters}. "
@@ -113,60 +146,111 @@
             f"https://github.com/dask-contrib/dask-sql/issues/new/choose "
             f"and include the following error message: {err}"
         )
 
         return ddf
 
 
-class Or(frozenset):
-    """Helper class for 'OR' expressions"""
+class DNF:
+    """Manage filters in Disjunctive Normal Form (DNF)"""
 
-    def to_list_tuple(self):
-        # NDF "or" is List[List[Tuple]]
-        def _maybe_list(val):
-            if isinstance(val, tuple) and val and isinstance(val[0], (tuple, list)):
-                return list(val)
-            return [val]
-
-        return [
-            _maybe_list(val.to_list_tuple())
-            if hasattr(val, "to_list_tuple")
-            else _maybe_list(val)
-            for val in self
-        ]
-
-
-class And(frozenset):
-    """Helper class for 'AND' expressions"""
-
-    def to_list_tuple(self):
-        # NDF "and" is List[Tuple]
-        return tuple(
-            val.to_list_tuple() if hasattr(val, "to_list_tuple") else val
-            for val in self
-        )
+    class _Or(frozenset):
+        """Fozen set of disjunctions"""
 
+        def to_list_tuple(self) -> list:
+            # DNF "or" is List[List[Tuple]]
+            def _maybe_list(val):
+                if isinstance(val, tuple) and val and isinstance(val[0], (tuple, list)):
+                    return list(val)
+                return [val]
+
+            return [
+                _maybe_list(val.to_list_tuple())
+                if hasattr(val, "to_list_tuple")
+                else _maybe_list(val)
+                for val in self
+            ]
+
+    class _And(frozenset):
+        """Frozen set of conjunctions"""
+
+        def to_list_tuple(self) -> list:
+            # DNF "and" is List[Tuple]
+            return tuple(
+                val.to_list_tuple() if hasattr(val, "to_list_tuple") else val
+                for val in self
+            )
 
-def to_dnf(expr):
-    """Normalize a boolean filter expression to disjunctive normal form (DNF)"""
+    _filters: _And | _Or | None  # Underlying filter expression
 
-    # Credit: https://stackoverflow.com/a/58372345
-    if not isinstance(expr, (Or, And)):
-        if not isinstance(expr, tuple):
-            raise TypeError(f"expected tuple, got {expr}")
-        result = Or((And((expr,)),))
-    elif isinstance(expr, Or):
-        result = Or(se for e in expr for se in to_dnf(e))
-    elif isinstance(expr, And):
-        total = []
-        for c in itertools.product(*[to_dnf(e) for e in expr]):
-            conjunction = [se for e in c for se in e if isinstance(se, tuple)]
-            total.append(And(conjunction))
-        result = Or(total)
-    return result
+    def __init__(self, filters: DNF | _And | _Or | list | tuple | None) -> DNF:
+        if isinstance(filters, DNF):
+            self._filters = filters._filters
+        else:
+            self._filters = self.normalize(filters)
+
+    def to_list_tuple(self) -> list:
+        return self._filters.to_list_tuple()
+
+    def __bool__(self) -> bool:
+        return bool(self._filters)
+
+    @classmethod
+    def normalize(cls, filters: _And | _Or | list | tuple | None):
+        """Convert raw filters to the `_Or(_And)` DNF representation"""
+
+        def _valid_tuple(predicate: tuple):
+            col, op, val = predicate
+            if isinstance(col, tuple):
+                raise TypeError("filters must be List[Tuple] or List[List[Tuple]]")
+            if op in ("in", "not in"):
+                return (col, op, tuple(val))
+            else:
+                return predicate
+
+        def _valid_list(conjunction: list):
+            valid = []
+            for predicate in conjunction:
+                if not isinstance(predicate, tuple):
+                    raise TypeError(f"Predicate must be a tuple, got {predicate}")
+                valid.append(_valid_tuple(predicate))
+            return valid
+
+        if not filters:
+            result = None
+        elif isinstance(filters, list):
+            conjunctions = filters if isinstance(filters[0], list) else [filters]
+            result = cls._Or(
+                [cls._And(_valid_list(conjunction)) for conjunction in conjunctions]
+            )
+        elif isinstance(filters, tuple):
+            result = cls._Or((cls._And((_valid_tuple(filters),)),))
+        elif isinstance(filters, cls._Or):
+            result = cls._Or(se for e in filters for se in cls.normalize(e))
+        elif isinstance(filters, cls._And):
+            total = []
+            for c in itertools.product(*[cls.normalize(e) for e in filters]):
+                total.append(cls._And(se for e in c for se in e))
+            result = cls._Or(total)
+        else:
+            raise TypeError(f"{type(filters)} not a supported type for DNF")
+        return result
+
+    def combine(self, other: DNF | _And | _Or | list | tuple | None) -> DNF:
+        """Combine with another DNF object"""
+        if not isinstance(other, DNF):
+            other = DNF(other)
+        assert isinstance(other, DNF)
+        if self._filters is None:
+            result = other._filters
+        elif other._filters is None:
+            result = self._filters
+        else:
+            result = self._And([self._filters, other._filters])
+        return DNF(result)
 
 
 # Define all supported comparison functions
 # (and their mapping to a string expression)
 _comparison_symbols = {
     operator.eq: "==",
     operator.ne: "!=",
@@ -264,15 +348,16 @@
     ):
         """Regenerate a Dask collection for this layer using the
         provided inputs and key-word arguments
         """
 
         # Return regenerated layer if the work was
         # already done
-        _regen_cache = _regen_cache or {}
+        if _regen_cache is None:
+            _regen_cache = {}
         if self.layer.output in _regen_cache:
             return _regen_cache[self.layer.output]
 
         # Recursively generate necessary inputs to
         # this layer to generate the collection
         inputs = []
         for key, ind in self.layer.indices:
@@ -409,43 +494,43 @@
         "in": "not in",
         "not in": "in",
         "is": "is not",
         "is not": "is",
     }.get(symbol, symbol)
 
 
-def _blockwise_comparison_dnf(op, indices: list, dsk: RegenerableGraph):
+def _blockwise_comparison_dnf(op, indices: list, dsk: RegenerableGraph) -> DNF:
     # Return DNF expression pattern for a simple comparison
     left = _get_blockwise_input(0, indices, dsk)
     right = _get_blockwise_input(1, indices, dsk)
 
     if is_arraylike(left) and hasattr(left, "item") and left.size == 1:
         left = left.item()
         # Need inverse comparison in read_parquet
-        return to_dnf((right, _inv(_comparison_symbols[op]), left))
+        return DNF((right, _inv(_comparison_symbols[op]), left))
     if is_arraylike(right) and hasattr(right, "item") and right.size == 1:
         right = right.item()
-    return to_dnf((left, _comparison_symbols[op], right))
+    return DNF((left, _comparison_symbols[op], right))
 
 
-def _blockwise_logical_dnf(op, indices: list, dsk: RegenerableGraph):
+def _blockwise_logical_dnf(op, indices: list, dsk: RegenerableGraph) -> DNF:
     # Return DNF expression pattern for logical "and" or "or"
     left = _get_blockwise_input(0, indices, dsk)
     right = _get_blockwise_input(1, indices, dsk)
 
-    vals = []
+    filters = []
     for val in [left, right]:
-        if not isinstance(val, (tuple, Or, And)):
+        if not isinstance(val, (tuple, DNF)):
             raise TypeError(f"Invalid logical operand: {val}")
-        vals.append(to_dnf(val))
+        filters.append(DNF(val)._filters)
 
     if op == operator.or_:
-        return to_dnf(Or(vals))
+        return DNF(DNF._Or(filters))
     elif op == operator.and_:
-        return to_dnf(And(vals))
+        return DNF(DNF._And(filters))
     else:
         raise ValueError
 
 
 def _blockwise_getitem_dnf(op, indices: list, dsk: RegenerableGraph):
     # Return dnf of key (selected by getitem)
     key = _get_blockwise_input(1, indices, dsk)
@@ -453,38 +538,38 @@
 
 
 def _blockwise_pass_through_dnf(op, indices: list, dsk: RegenerableGraph):
     # Return dnf of input collection
     return _get_blockwise_input(0, indices, dsk)
 
 
-def _blockwise_isin_dnf(op, indices: list, dsk: RegenerableGraph):
+def _blockwise_isin_dnf(op, indices: list, dsk: RegenerableGraph) -> DNF:
     # Return DNF expression pattern for a simple "in" comparison
     left = _get_blockwise_input(0, indices, dsk)
     right = _get_blockwise_input(1, indices, dsk)
-    return to_dnf((left, "in", tuple(right)))
+    return DNF((left, "in", tuple(right)))
 
 
-def _blockwise_isna_dnf(op, indices: list, dsk: RegenerableGraph):
+def _blockwise_isna_dnf(op, indices: list, dsk: RegenerableGraph) -> DNF:
     # Return DNF expression pattern for `isna`
     if not PQ_IS_SUPPORT:
         raise ValueError("This version of dask does not support 'is' predicates.")
     left = _get_blockwise_input(0, indices, dsk)
-    return to_dnf((left, "is", None))
+    return DNF((left, "is", None))
 
 
-def _blockwise_inv_dnf(op, indices: list, dsk: RegenerableGraph):
+def _blockwise_inv_dnf(op, indices: list, dsk: RegenerableGraph) -> DNF:
     # Return DNF expression pattern for the inverse of a comparison
     expr = _get_blockwise_input(0, indices, dsk).to_list_tuple()
     new_expr = []
     count = 0
     for conjunction in expr:
         new_conjunction = []
         for col, op, val in conjunction:
             count += 1
             new_conjunction.append((col, _inv(op), val))
-        new_expr.append(And(new_conjunction))
+        new_expr.append(DNF._And(new_conjunction))
     if count > 1:
         # Havent taken the time to think through
         # general inversion yet.
         raise ValueError("inv(DNF) case not implemented.")
-    return to_dnf(Or(new_expr))
+    return DNF(DNF._Or(new_expr))
```

### Comparing `dask_sql-2023.6.0/dask_sql/physical/utils/groupby.py` & `dask_sql-2023.8.0/dask_sql/physical/utils/groupby.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/utils/ml_classes.py` & `dask_sql-2023.8.0/dask_sql/physical/utils/ml_classes.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/utils/sort.py` & `dask_sql-2023.8.0/dask_sql/physical/utils/sort.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/physical/utils/statistics.py` & `dask_sql-2023.8.0/dask_sql/physical/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/server/app.py` & `dask_sql-2023.8.0/dask_sql/server/app.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/server/presto_jdbc.py` & `dask_sql-2023.8.0/dask_sql/server/presto_jdbc.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 
     # TODO: add support for catalogs in presto interface
     # see https://github.com/dask-contrib/dask-sql/pull/351
     # if catalog and len(catalog.strip()) > 0:
     #     catalogs = pd.DataFrame().append(create_catalog_row(catalog), ignore_index=True)
     #     c.create_table("catalogs", catalogs, schema_name=system_schema)
 
-    schemas = pd.DataFrame().append(create_schema_row(), ignore_index=True)
+    schemas = pd.DataFrame(create_schema_row(), index=[0])
     c.create_table("schemas", schemas, schema_name=system_schema)
     schema_rows = []
 
-    tables = pd.DataFrame().append(create_table_row(), ignore_index=True)
+    tables = pd.DataFrame(create_table_row(), index=[0])
     c.create_table("tables", tables, schema_name=system_schema)
     table_rows = []
 
-    columns = pd.DataFrame().append(create_column_row(), ignore_index=True)
+    columns = pd.DataFrame(create_column_row(), index=[0])
     c.create_table("columns", columns, schema_name=system_schema)
     column_rows = []
 
     for schema_name, schema in c.schema.items():
         schema_rows.append(create_schema_row(catalog, schema_name))
         for table_name, dc in schema.tables.items():
             df = dc.df
```

### Comparing `dask_sql-2023.6.0/dask_sql/server/responses.py` & `dask_sql-2023.8.0/dask_sql/server/responses.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql/sql-schema.yaml` & `dask_sql-2023.8.0/dask_sql/sql-schema.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,19 @@
           Whether the first generated logical plan should be further optimized or used as is.
 
       predicate_pushdown:
         type: boolean
         description: |
           Whether to try pushing down filter predicates into IO (when possible).
 
+      dynamic_partition_pruning:
+        type: boolean
+        description: |
+          Whether to apply the dynamic partition pruning optimizer rule.
+
       sort:
         type: object
         properties:
 
           topk-nelem-limit:
             type: integer
             description: |
```

### Comparing `dask_sql-2023.6.0/dask_sql/utils.py` & `dask_sql-2023.8.0/dask_sql/utils.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/dask_sql.egg-info/PKG-INFO` & `dask_sql-2023.8.0/dask_sql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-sql
-Version: 2023.6.0
+Version: 2023.8.0
 Summary: SQL query layer for Dask
 Home-page: https://github.com/dask-contrib/dask-sql/
 Maintainer: Nils Braun
 Maintainer-email: nilslennartbraun@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `dask_sql-2023.6.0/dask_sql.egg-info/SOURCES.txt` & `dask_sql-2023.8.0/dask_sql.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 dask_planner/src/sql/logical/show_schemas.rs
 dask_planner/src/sql/logical/show_tables.rs
 dask_planner/src/sql/logical/sort.rs
 dask_planner/src/sql/logical/subquery_alias.rs
 dask_planner/src/sql/logical/table_scan.rs
 dask_planner/src/sql/logical/use_schema.rs
 dask_planner/src/sql/logical/window.rs
+dask_planner/src/sql/optimizer/dynamic_partition_pruning.rs
 dask_planner/src/sql/optimizer/join_reorder.rs
 dask_planner/src/sql/types/rel_data_type.rs
 dask_planner/src/sql/types/rel_data_type_field.rs
 dask_sql/__init__.py
 dask_sql/_compat.py
 dask_sql/_version.py
 dask_sql/cmd.py
```

### Comparing `dask_sql-2023.6.0/setup.cfg` & `dask_sql-2023.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.6.0/setup.py` & `dask_sql-2023.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,19 +38,19 @@
             path="dask_planner/Cargo.toml",
             debug=debug_build,
         )
     ],
     python_requires=">=3.8",
     setup_requires=sphinx_requirements,
     install_requires=[
-        "dask[dataframe]>=2022.3.0,<=2023.5.1",
-        "distributed>=2022.3.0,<=2023.5.1",
+        "dask[dataframe]>=2022.3.0,<=2023.7.1",
+        "distributed>=2022.3.0,<=2023.7.1",
         "pandas>=1.4.0",
-        # FIXME: handling is needed for httpx-based fastapi>=0.87.0
-        "fastapi>=0.69.0,<0.87.0",
+        "fastapi>=0.92.0",
+        "httpx>=0.24.1",
         "uvicorn>=0.13.4",
         "tzlocal>=2.1",
         "prompt_toolkit>=3.0.8",
         "pygments>=2.7.1",
         "tabulate",
     ],
     extras_require={
```

### Comparing `dask_sql-2023.6.0/versioneer.py` & `dask_sql-2023.8.0/versioneer.py`

 * *Files identical despite different names*

