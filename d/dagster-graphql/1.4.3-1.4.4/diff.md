# Comparing `tmp/dagster-graphql-1.4.3.tar.gz` & `tmp/dagster-graphql-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.4.3.tar", last modified: Mon Jul 31 22:58:53 2023, max compression
+gzip compressed data, was "dagster-graphql-1.4.4.tar", last modified: Thu Aug  3 21:50:50 2023, max compression
```

## Comparing `dagster-graphql-1.4.3.tar` & `dagster-graphql-1.4.4.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.977937 dagster-graphql-1.4.3/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-31 22:58:53.977937 dagster-graphql-1.4.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.957937 dagster-graphql-1.4.3/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.957937 dagster-graphql-1.4.3/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17966 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.961937 dagster-graphql-1.4.3/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18592 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.965937 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11422 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9850 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3725 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4591 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4396 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7244 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25530 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     2369 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12589 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2436 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    14972 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)     9554 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    21120 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8042 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.969937 dagster-graphql-1.4.3/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2877 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40455 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     8754 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)      838 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16867 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4823 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18061 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16361 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    10983 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6708 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28430 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.973937 dagster-graphql-1.4.3/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20983 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    17622 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.973937 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11058 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    40083 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8353 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.977937 dagster-graphql-1.4.3/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    26779 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    37803 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5088 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.977937 dagster-graphql-1.4.3/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8306 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29569 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.977937 dagster-graphql-1.4.3/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6751 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:53.957937 dagster-graphql-1.4.3/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4286 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-31 22:58:53.000000 dagster-graphql-1.4.3/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-07-31 22:58:53.993937 dagster-graphql-1.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1509 2023-07-31 22:58:19.000000 dagster-graphql-1.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.191340 dagster-graphql-1.4.4/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-03 21:50:50.191340 dagster-graphql-1.4.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.167339 dagster-graphql-1.4.4/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.167339 dagster-graphql-1.4.4/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17966 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.175339 dagster-graphql-1.4.4/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18592 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.175339 dagster-graphql-1.4.4/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11422 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4591 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7244 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25530 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12589 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    14972 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    21120 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8042 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.183339 dagster-graphql-1.4.4/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2877 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40455 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     8754 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)      838 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16867 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18061 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16361 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6937 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28430 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.183339 dagster-graphql-1.4.4/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20983 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    17622 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.187340 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11058 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    40083 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8353 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.191340 dagster-graphql-1.4.4/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    26779 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    37803 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.191340 dagster-graphql-1.4.4/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8306 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29569 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.191340 dagster-graphql-1.4.4/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6751 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 21:50:50.167339 dagster-graphql-1.4.4/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-08-03 21:50:50.000000 dagster-graphql-1.4.4/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-08-03 21:50:50.000000 dagster-graphql-1.4.4/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 21:50:50.000000 dagster-graphql-1.4.4/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-08-03 21:50:50.000000 dagster-graphql-1.4.4/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-08-03 21:50:50.000000 dagster-graphql-1.4.4/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-03 21:50:50.000000 dagster-graphql-1.4.4/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-08-03 21:50:50.195340 dagster-graphql-1.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-08-03 21:49:40.000000 dagster-graphql-1.4.4/setup.py
```

### Comparing `dagster-graphql-1.4.3/LICENSE` & `dagster-graphql-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/PKG-INFO` & `dagster-graphql-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.4.3
+Version: 1.4.4
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.4.3/dagster_graphql/__init__.py` & `dagster-graphql-1.4.4/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/cli.py` & `dagster-graphql-1.4.4/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/client/client.py` & `dagster-graphql-1.4.4/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.4.4/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/client/query.py` & `dagster-graphql-1.4.4/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/client/utils.py` & `dagster-graphql-1.4.4/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/events.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/external.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.4.4/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/errors.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/execution.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/external.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/instance.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
     runLauncher = graphene.Field(GrapheneRunLauncher)
     runQueuingSupported = graphene.NonNull(graphene.Boolean)
     executablePath = graphene.NonNull(graphene.String)
     daemonHealth = graphene.NonNull(GrapheneDaemonHealth)
     hasInfo = graphene.NonNull(graphene.Boolean)
     hasCapturedLogManager = graphene.NonNull(graphene.Boolean)
     autoMaterializePaused = graphene.NonNull(graphene.Boolean)
+    supportsConcurrencyLimits = graphene.NonNull(graphene.Boolean)
     concurrencyLimits = non_null_list(GrapheneConcurrencyKeyInfo)
 
     class Meta:
         name = "Instance"
 
     def __init__(self, instance):
         super().__init__()
@@ -163,13 +164,16 @@
 
     def resolve_hasCapturedLogManager(self, _graphene_info: ResolveInfo):
         return isinstance(self._instance.compute_log_manager, CapturedLogManager)
 
     def resolve_autoMaterializePaused(self, _graphene_info: ResolveInfo):
         return get_auto_materialize_paused(self._instance)
 
+    def resolve_supportsConcurrencyLimits(self, _graphene_info: ResolveInfo):
+        return self._instance.event_log_storage.supports_global_concurrency_limits
+
     def resolve_concurrencyLimits(self, _graphene_info: ResolveInfo):
         res = []
         for key in self._instance.event_log_storage.get_concurrency_keys():
             key_info = self._instance.event_log_storage.get_concurrency_info(key)
             res.append(GrapheneConcurrencyKeyInfo(key_info))
         return res
```

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/resources.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/roots/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/runs.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/solids.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/table.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/tags.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/schema/util.py` & `dagster-graphql-1.4.4/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql/test/utils.py` & `dagster-graphql-1.4.4/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.4.4/dagster_graphql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.4.3
+Version: 1.4.4
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.4.3/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.4.4/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.4.3/setup.py` & `dagster-graphql-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.4.3",
+        "dagster==1.4.4",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
         "urllib3<2.0.0",  # https://github.com/psf/requests/issues/6432
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
```

