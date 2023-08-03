# Comparing `tmp/dagster-1.4.2.tar.gz` & `tmp/dagster-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.4.2.tar", last modified: Fri Jul 21 22:28:31 2023, max compression
+gzip compressed data, was "dagster-1.4.3.tar", last modified: Mon Jul 31 22:58:40 2023, max compression
```

## Comparing `dagster-1.4.2.tar` & `dagster-1.4.3.tar`

### file list

```diff
@@ -1,634 +1,636 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.371489 dagster-1.4.2/
--rw-r--r--   0 root         (0) root         (0)      549 2023-07-21 22:28:09.000000 dagster-1.4.2/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-07-21 22:28:09.000000 dagster-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-21 22:28:09.000000 dagster-1.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8744 2023-07-21 22:28:31.371489 dagster-1.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7171 2023-07-21 22:28:09.000000 dagster-1.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.231487 dagster-1.4.2/dagster/
--rw-r--r--   0 root         (0) root         (0)    25856 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.235487 dagster-1.4.2/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2882 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.235487 dagster-1.4.2/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51577 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.239487 dagster-1.4.2/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26302 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8271 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     7730 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     6088 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     4618 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    29907 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     6218 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5129 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19958 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15707 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.239487 dagster-1.4.2/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28391 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.243487 dagster-1.4.2/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15971 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    19601 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15605 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    16980 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.243487 dagster-1.4.2/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)    73675 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)     7448 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/pythonic_config/utils.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17162 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.247487 dagster-1.4.2/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13645 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.247487 dagster-1.4.2/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     4257 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.263487 dagster-1.4.2/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7632 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33355 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10944 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3604 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    37132 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    50413 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    20868 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7255 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    64803 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    24376 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/auto_materialize_condition.py
--rw-r--r--   0 root         (0) root         (0)     5317 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16093 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45671 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4287 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    13908 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    21526 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    20464 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.267487 dagster-1.4.2/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48782 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10673 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17845 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14396 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8665 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12195 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     7648 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    21443 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    40472 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    32058 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21168 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)    11045 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10700 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/freshness_based_auto_materialize.py
--rw-r--r--   0 root         (0) root         (0)     8241 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16201 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    46922 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3481 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    21170 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    53187 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    20308 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7183 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8851 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.267487 dagster-1.4.2/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    33115 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    56485 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    20891 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11927 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8041 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    22760 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    19256 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7509 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    18908 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    43384 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    44961 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8934 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27227 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.267487 dagster-1.4.2/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    18860 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    17543 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    17864 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    17618 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7796 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    22861 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15838 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    39126 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    38361 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5137 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10837 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    48845 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    15772 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    14173 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    78808 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15622 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7988 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3982 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    26509 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6391 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.267487 dagster-1.4.2/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    66637 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8156 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.275488 dagster-1.4.2/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38315 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    38679 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    14701 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6295 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.275488 dagster-1.4.2/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22931 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    16053 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9622 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    27620 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    31611 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    34894 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    45125 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18501 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5097 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5897 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8544 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14451 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.279488 dagster-1.4.2/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25266 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7270 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12550 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16658 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27342 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    11129 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    37483 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     4352 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    57998 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15920 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19280 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2100 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1651 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10329 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4228 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.279488 dagster-1.4.2/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15592 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.279488 dagster-1.4.2/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15576 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.279488 dagster-1.4.2/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.283488 dagster-1.4.2/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2807 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33518 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    32236 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    71828 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    12517 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19063 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3610 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.283488 dagster-1.4.2/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   112340 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12956 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24084 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.283488 dagster-1.4.2/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3758 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6808 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17249 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3691 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.287488 dagster-1.4.2/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11030 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.287488 dagster-1.4.2/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    22355 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.287488 dagster-1.4.2/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.287488 dagster-1.4.2/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18247 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.287488 dagster-1.4.2/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2842 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12099 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16654 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4495 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14452 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     3693 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.299488 dagster-1.4.2/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.299488 dagster-1.4.2/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.319488 dagster-1.4.2/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7204 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.319488 dagster-1.4.2/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8745 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16245 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9557 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    24416 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11640 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.319488 dagster-1.4.2/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17062 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3762 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7273 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7911 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     6502 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   104937 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.319488 dagster-1.4.2/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.319488 dagster-1.4.2/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1064 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7538 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10970 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13540 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8896 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10880 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    29582 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17301 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4355 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.323488 dagster-1.4.2/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23483 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.323488 dagster-1.4.2/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15474 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2425 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8697 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46286 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.323488 dagster-1.4.2/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.323488 dagster-1.4.2/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1064 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6830 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.327488 dagster-1.4.2/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6620 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     3710 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    23005 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.327488 dagster-1.4.2/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.327488 dagster-1.4.2/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7210 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4875 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3268 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1186 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    18046 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.327488 dagster-1.4.2/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13981 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    14855 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    28851 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    20093 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.339489 dagster-1.4.2/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7298 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    36380 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     4402 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.343489 dagster-1.4.2/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    28580 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4719 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4099 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.343489 dagster-1.4.2/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1971 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)     7880 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.343489 dagster-1.4.2/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.347489 dagster-1.4.2/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4423 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18390 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10611 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.347489 dagster-1.4.2/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    10031 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.347489 dagster-1.4.2/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16326 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    40350 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6647 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.347489 dagster-1.4.2/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.347489 dagster-1.4.2/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.227487 dagster-1.4.2/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.347489 dagster-1.4.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.351489 dagster-1.4.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.351489 dagster-1.4.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.351489 dagster-1.4.2/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.351489 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.351489 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.351489 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      279 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.355489 dagster-1.4.2/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.355489 dagster-1.4.2/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29251 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39700 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18451 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4204 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    21967 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.355489 dagster-1.4.2/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5551 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    12415 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    52785 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26559 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.355489 dagster-1.4.2/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      222 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.355489 dagster-1.4.2/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.359489 dagster-1.4.2/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37218 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.359489 dagster-1.4.2/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7557 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    37610 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.359489 dagster-1.4.2/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.359489 dagster-1.4.2/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.367489 dagster-1.4.2/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23346 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8782 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    27785 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     3813 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9412 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    12571 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3289 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.371489 dagster-1.4.2/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    12640 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    29928 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.371489 dagster-1.4.2/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4993 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 22:28:09.000000 dagster-1.4.2/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 22:28:31.235487 dagster-1.4.2/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8744 2023-07-21 22:28:31.000000 dagster-1.4.2/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25449 2023-07-21 22:28:31.000000 dagster-1.4.2/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 22:28:31.000000 dagster-1.4.2/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-21 22:28:31.000000 dagster-1.4.2/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1246 2023-07-21 22:28:31.000000 dagster-1.4.2/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-21 22:28:31.000000 dagster-1.4.2/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-07-21 22:28:31.371489 dagster-1.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6282 2023-07-21 22:28:10.000000 dagster-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.309835 dagster-1.4.3/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-07-31 22:58:19.000000 dagster-1.4.3/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-07-31 22:58:19.000000 dagster-1.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-31 22:58:19.000000 dagster-1.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8744 2023-07-31 22:58:40.309835 dagster-1.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7171 2023-07-31 22:58:19.000000 dagster-1.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.225835 dagster-1.4.3/dagster/
+-rw-r--r--   0 root         (0) root         (0)    25872 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.225835 dagster-1.4.3/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.225835 dagster-1.4.3/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51577 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.229835 dagster-1.4.3/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26302 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8271 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     6088 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     4618 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    29907 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     6218 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5129 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19958 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15707 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.229835 dagster-1.4.3/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28391 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.229835 dagster-1.4.3/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15971 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    19601 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15605 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    16980 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.233835 dagster-1.4.3/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)    73675 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)     7448 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/pythonic_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17162 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.233835 dagster-1.4.3/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13645 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.233835 dagster-1.4.3/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.245835 dagster-1.4.3/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7632 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10834 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/asset_daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    34222 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10944 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    37072 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     6115 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    29642 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    20868 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7255 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    66658 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    24376 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     7763 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/auto_materialize_condition.py
+-rw-r--r--   0 root         (0) root         (0)     5317 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3148 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/backfill_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16664 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45671 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    13908 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    21526 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    20468 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.249835 dagster-1.4.3/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50681 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10673 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17845 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14396 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8618 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12195 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     7648 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    22197 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    40472 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    32274 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21203 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11408 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10738 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/freshness_based_auto_materialize.py
+-rw-r--r--   0 root         (0) root         (0)     8241 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16158 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    46922 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3481 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    21170 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    53187 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    21547 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7188 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8855 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.249835 dagster-1.4.3/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    33211 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    56340 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20891 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8041 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    22760 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19256 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    18908 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    43384 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    45405 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8934 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27209 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.249835 dagster-1.4.3/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    19612 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    17585 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    18148 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    17618 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7796 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    22861 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15838 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    39126 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    38361 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5137 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10837 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    48845 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    16016 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    14173 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    78808 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15622 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7988 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    26477 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.249835 dagster-1.4.3/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    66637 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8156 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.253835 dagster-1.4.3/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38357 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    38606 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    14701 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6295 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.257835 dagster-1.4.3/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22931 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    16053 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9622 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    27620 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    31611 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    34894 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    45125 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18501 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14451 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6766 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.257835 dagster-1.4.3/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25266 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7270 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12550 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16658 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27342 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    11129 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    37483 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    57998 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19280 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10329 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4228 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.261835 dagster-1.4.3/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15602 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.261835 dagster-1.4.3/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15614 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.261835 dagster-1.4.3/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.261835 dagster-1.4.3/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33518 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    32236 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    73222 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    12481 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19063 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.261835 dagster-1.4.3/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   112455 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12956 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24084 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.265835 dagster-1.4.3/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3758 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6808 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17223 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.265835 dagster-1.4.3/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11030 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.265835 dagster-1.4.3/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    22355 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.265835 dagster-1.4.3/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.265835 dagster-1.4.3/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18247 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.265835 dagster-1.4.3/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12099 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16654 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14452 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.273835 dagster-1.4.3/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.273835 dagster-1.4.3/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.285835 dagster-1.4.3/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7524 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.285835 dagster-1.4.3/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8725 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16245 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    24416 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11640 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.285835 dagster-1.4.3/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17066 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7273 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7911 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     6502 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   104969 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.285835 dagster-1.4.3/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.285835 dagster-1.4.3/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7538 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10970 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13540 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8896 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10880 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    29582 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17301 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.285835 dagster-1.4.3/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23483 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.285835 dagster-1.4.3/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15474 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8697 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46286 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.285835 dagster-1.4.3/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.285835 dagster-1.4.3/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6830 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.289835 dagster-1.4.3/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6620 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    23005 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.289835 dagster-1.4.3/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.289835 dagster-1.4.3/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7210 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    18396 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.289835 dagster-1.4.3/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13981 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    14855 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    29628 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    20093 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.289835 dagster-1.4.3/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7262 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    36380 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.289835 dagster-1.4.3/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    28580 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4719 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.293835 dagster-1.4.3/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     7860 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.293835 dagster-1.4.3/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9161 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.293835 dagster-1.4.3/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4423 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18390 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10611 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.293835 dagster-1.4.3/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    10031 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.293835 dagster-1.4.3/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16326 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    40602 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6647 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.293835 dagster-1.4.3/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.293835 dagster-1.4.3/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.221835 dagster-1.4.3/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.293835 dagster-1.4.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.293835 dagster-1.4.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.293835 dagster-1.4.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.297835 dagster-1.4.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.297835 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.297835 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.297835 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      279 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.297835 dagster-1.4.3/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.297835 dagster-1.4.3/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29251 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39700 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18451 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    21967 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.297835 dagster-1.4.3/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5551 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    12417 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    52842 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26559 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.297835 dagster-1.4.3/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.297835 dagster-1.4.3/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.301835 dagster-1.4.3/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37218 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.301835 dagster-1.4.3/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7531 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    37610 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.301835 dagster-1.4.3/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.301835 dagster-1.4.3/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.305835 dagster-1.4.3/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23346 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8782 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    35693 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     3813 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9412 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    12571 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.309835 dagster-1.4.3/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    12640 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    29928 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.309835 dagster-1.4.3/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4993 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-31 22:58:19.000000 dagster-1.4.3/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 22:58:40.225835 dagster-1.4.3/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8744 2023-07-31 22:58:40.000000 dagster-1.4.3/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25543 2023-07-31 22:58:40.000000 dagster-1.4.3/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 22:58:40.000000 dagster-1.4.3/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-31 22:58:40.000000 dagster-1.4.3/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-07-31 22:58:40.000000 dagster-1.4.3/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 22:58:40.000000 dagster-1.4.3/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-31 22:58:40.313835 dagster-1.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6343 2023-07-31 22:58:19.000000 dagster-1.4.3/setup.py
```

### Comparing `dagster-1.4.2/COPYING` & `dagster-1.4.3/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/LICENSE` & `dagster-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/PKG-INFO` & `dagster-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.4.2
+Version: 1.4.3
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.4.2/README.md` & `dagster-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/__init__.py` & `dagster-1.4.3/dagster/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,15 +563,15 @@
 # in `_DEPRECATED` is required  for us to generate the deprecation warning.
 
 if TYPE_CHECKING:
     ##### EXAMPLE
     # from dagster.some.module import (
     #     Foo as Foo,
     # )
-    pass
+    pass  # noqa: TCH005
 
 
 _DEPRECATED: Final[Mapping[str, TypingTuple[str, str, str]]] = {
     ##### EXAMPLE
     # "Foo": (
     #     "dagster.some.module",
     #     "1.1.0",  # breaking version
```

### Comparing `dagster-1.4.2/dagster/_annotations.py` & `dagster-1.4.3/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_api/get_server_id.py` & `dagster-1.4.3/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_api/list_repositories.py` & `dagster-1.4.3/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_api/notebook_data.py` & `dagster-1.4.3/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_api/snapshot_execution_plan.py` & `dagster-1.4.3/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_api/snapshot_job.py` & `dagster-1.4.3/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_api/snapshot_partition.py` & `dagster-1.4.3/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_api/snapshot_repository.py` & `dagster-1.4.3/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_api/snapshot_schedule.py` & `dagster-1.4.3/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_api/snapshot_sensor.py` & `dagster-1.4.3/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_check/README.md` & `dagster-1.4.3/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_check/__init__.py` & `dagster-1.4.3/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/__init__.py` & `dagster-1.4.3/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/api.py` & `dagster-1.4.3/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/asset.py` & `dagster-1.4.3/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/code_server.py` & `dagster-1.4.3/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/config_scaffolder.py` & `dagster-1.4.3/dagster/_cli/config_scaffolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,9 +53,11 @@
         return defaults[config_type.given_name]  # type: ignore
     elif config_type.kind == ConfigTypeKind.ARRAY:
         return []
     elif config_type.kind == ConfigTypeKind.MAP:
         return {}
     elif config_type.kind == ConfigTypeKind.ENUM:
         return "|".join(sorted(map(lambda v: v.config_value, config_type.enum_values)))  # type: ignore
+    elif config_type.kind == ConfigTypeKind.NONEABLE:
+        return None
     else:
         check.failed(f"Do not know how to scaffold {config_type.given_name}")
```

### Comparing `dagster-1.4.2/dagster/_cli/debug.py` & `dagster-1.4.3/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/dev.py` & `dagster-1.4.3/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/instance.py` & `dagster-1.4.3/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/job.py` & `dagster-1.4.3/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/load_handle.py` & `dagster-1.4.3/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/project.py` & `dagster-1.4.3/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/run.py` & `dagster-1.4.3/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/schedule.py` & `dagster-1.4.3/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/sensor.py` & `dagster-1.4.3/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/utils.py` & `dagster-1.4.3/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_cli/workspace/cli_target.py` & `dagster-1.4.3/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/__init__.py` & `dagster-1.4.3/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/config_schema.py` & `dagster-1.4.3/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/config_type.py` & `dagster-1.4.3/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/errors.py` & `dagster-1.4.3/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/evaluate_value_result.py` & `dagster-1.4.3/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/field.py` & `dagster-1.4.3/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/field_utils.py` & `dagster-1.4.3/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/post_process.py` & `dagster-1.4.3/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/primitive_mapping.py` & `dagster-1.4.3/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/pythonic_config/__init__.py` & `dagster-1.4.3/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.4.3/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.4.3/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/pythonic_config/utils.py` & `dagster-1.4.3/dagster/_config/pythonic_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/snap.py` & `dagster-1.4.3/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/source.py` & `dagster-1.4.3/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/stack.py` & `dagster-1.4.3/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/traversal_context.py` & `dagster-1.4.3/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/type_printer.py` & `dagster-1.4.3/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_config/validate.py` & `dagster-1.4.3/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/assets.py` & `dagster-1.4.3/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/code_pointer.py` & `dagster-1.4.3/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/container_context/config.py` & `dagster-1.4.3/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/debug.py` & `dagster-1.4.3/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/decorator_utils.py` & `dagster-1.4.3/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/__init__.py` & `dagster-1.4.3/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/asset_graph.py` & `dagster-1.4.3/dagster/_core/definitions/asset_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.errors import DagsterInvalidInvocationError, DagsterInvariantViolationError
 from dagster._core.instance import DynamicPartitionsStore
 from dagster._core.selector.subset_selector import DependencyGraph, generate_asset_dep_graph
 from dagster._utils.cached_method import cached_method
 
 from .assets import AssetsDefinition
+from .backfill_policy import BackfillPolicy
 from .events import AssetKey, AssetKeyPartitionKey
 from .freshness_policy import FreshnessPolicy
 from .partition import PartitionsDefinition, PartitionsSubset
 from .partition_mapping import PartitionMapping, UpstreamPartitionsResult, infer_partition_mapping
 from .source_asset import SourceAsset
 from .time_window_partitions import (
     TimeWindowPartitionsDefinition,
@@ -64,26 +65,28 @@
         asset_dep_graph: DependencyGraph[AssetKey],
         source_asset_keys: AbstractSet[AssetKey],
         partitions_defs_by_key: Mapping[AssetKey, Optional[PartitionsDefinition]],
         partition_mappings_by_key: Mapping[AssetKey, Optional[Mapping[AssetKey, PartitionMapping]]],
         group_names_by_key: Mapping[AssetKey, Optional[str]],
         freshness_policies_by_key: Mapping[AssetKey, Optional[FreshnessPolicy]],
         auto_materialize_policies_by_key: Mapping[AssetKey, Optional[AutoMaterializePolicy]],
+        backfill_policies_by_key: Mapping[AssetKey, Optional[BackfillPolicy]],
         required_multi_asset_sets_by_key: Optional[Mapping[AssetKey, AbstractSet[AssetKey]]],
         code_versions_by_key: Mapping[AssetKey, Optional[str]],
         is_observable_by_key: Mapping[AssetKey, bool],
         auto_observe_interval_minutes_by_key: Mapping[AssetKey, Optional[float]],
     ):
         self._asset_dep_graph = asset_dep_graph
         self._source_asset_keys = source_asset_keys
         self._partitions_defs_by_key = partitions_defs_by_key
         self._partition_mappings_by_key = partition_mappings_by_key
         self._group_names_by_key = group_names_by_key
         self._freshness_policies_by_key = freshness_policies_by_key
         self._auto_materialize_policies_by_key = auto_materialize_policies_by_key
+        self._backfill_policies_by_key = backfill_policies_by_key
         self._required_multi_asset_sets_by_key = required_multi_asset_sets_by_key
         self._code_versions_by_key = code_versions_by_key
         self._is_observable_by_key = is_observable_by_key
         self._auto_observe_interval_minutes_by_key = auto_observe_interval_minutes_by_key
         # source assets keys can sometimes appear in the upstream dict
         self._materializable_asset_keys = (
             self._asset_dep_graph["upstream"].keys() - self.source_asset_keys
@@ -114,14 +117,18 @@
 
     @property
     def auto_materialize_policies_by_key(
         self,
     ) -> Mapping[AssetKey, Optional[AutoMaterializePolicy]]:
         return self._auto_materialize_policies_by_key
 
+    @property
+    def backfill_policies_by_key(self) -> Mapping[AssetKey, Optional[BackfillPolicy]]:
+        return self._backfill_policies_by_key
+
     def get_auto_observe_interval_minutes(self, asset_key: AssetKey) -> Optional[float]:
         return self._auto_observe_interval_minutes_by_key.get(asset_key)
 
     @staticmethod
     def from_assets(
         all_assets: Iterable[Union[AssetsDefinition, SourceAsset]]
     ) -> "InternalAssetGraph":
@@ -130,14 +137,15 @@
         partitions_defs_by_key: Dict[AssetKey, Optional[PartitionsDefinition]] = {}
         partition_mappings_by_key: Dict[
             AssetKey, Optional[Mapping[AssetKey, PartitionMapping]]
         ] = {}
         group_names_by_key: Dict[AssetKey, Optional[str]] = {}
         freshness_policies_by_key: Dict[AssetKey, Optional[FreshnessPolicy]] = {}
         auto_materialize_policies_by_key: Dict[AssetKey, Optional[AutoMaterializePolicy]] = {}
+        backfill_policies_by_key: Dict[AssetKey, Optional[BackfillPolicy]] = {}
         required_multi_asset_sets_by_key: Dict[AssetKey, AbstractSet[AssetKey]] = {}
         code_versions_by_key: Dict[AssetKey, Optional[str]] = {}
         is_observable_by_key: Dict[AssetKey, bool] = {}
         auto_observe_interval_minutes_by_key: Dict[AssetKey, Optional[float]] = {}
 
         for asset in all_assets:
             if isinstance(asset, SourceAsset):
@@ -153,27 +161,29 @@
                 partition_mappings_by_key.update(
                     {key: asset.partition_mappings for key in asset.keys}
                 )
                 partitions_defs_by_key.update({key: asset.partitions_def for key in asset.keys})
                 group_names_by_key.update(asset.group_names_by_key)
                 freshness_policies_by_key.update(asset.freshness_policies_by_key)
                 auto_materialize_policies_by_key.update(asset.auto_materialize_policies_by_key)
+                backfill_policies_by_key.update({key: asset.backfill_policy for key in asset.keys})
                 if len(asset.keys) > 1 and not asset.can_subset:
                     for key in asset.keys:
                         required_multi_asset_sets_by_key[key] = asset.keys
                 code_versions_by_key.update(asset.code_versions_by_key)
 
         return InternalAssetGraph(
             asset_dep_graph=generate_asset_dep_graph(assets_defs, source_assets),
             source_asset_keys={source_asset.key for source_asset in source_assets},
             partitions_defs_by_key=partitions_defs_by_key,
             partition_mappings_by_key=partition_mappings_by_key,
             group_names_by_key=group_names_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
             auto_materialize_policies_by_key=auto_materialize_policies_by_key,
+            backfill_policies_by_key=backfill_policies_by_key,
             required_multi_asset_sets_by_key=required_multi_asset_sets_by_key,
             assets=assets_defs,
             source_assets=source_assets,
             code_versions_by_key=code_versions_by_key,
             is_observable_by_key=is_observable_by_key,
             auto_observe_interval_minutes_by_key=auto_observe_interval_minutes_by_key,
         )
@@ -459,14 +469,17 @@
         return [
             {key for key in level} for level in toposort.toposort(self._asset_dep_graph["upstream"])
         ]
 
     def get_auto_materialize_policy(self, asset_key: AssetKey) -> Optional[AutoMaterializePolicy]:
         return self.auto_materialize_policies_by_key.get(asset_key)
 
+    def get_backfill_policy(self, asset_key: AssetKey) -> Optional[BackfillPolicy]:
+        return self.backfill_policies_by_key.get(asset_key)
+
     @cached_method
     def get_downstream_freshness_policies(
         self, *, asset_key: AssetKey
     ) -> AbstractSet[FreshnessPolicy]:
         downstream_policies = set().union(
             *(
                 self.get_downstream_freshness_policies(asset_key=child_key)
@@ -625,14 +638,15 @@
         asset_dep_graph: DependencyGraph[AssetKey],
         source_asset_keys: AbstractSet[AssetKey],
         partitions_defs_by_key: Mapping[AssetKey, Optional[PartitionsDefinition]],
         partition_mappings_by_key: Mapping[AssetKey, Optional[Mapping[AssetKey, PartitionMapping]]],
         group_names_by_key: Mapping[AssetKey, Optional[str]],
         freshness_policies_by_key: Mapping[AssetKey, Optional[FreshnessPolicy]],
         auto_materialize_policies_by_key: Mapping[AssetKey, Optional[AutoMaterializePolicy]],
+        backfill_policies_by_key: Mapping[AssetKey, Optional[BackfillPolicy]],
         required_multi_asset_sets_by_key: Optional[Mapping[AssetKey, AbstractSet[AssetKey]]],
         assets: Sequence[AssetsDefinition],
         source_assets: Sequence[SourceAsset],
         code_versions_by_key: Mapping[AssetKey, Optional[str]],
         is_observable_by_key: Mapping[AssetKey, bool],
         auto_observe_interval_minutes_by_key: Mapping[AssetKey, Optional[float]],
     ):
@@ -640,14 +654,15 @@
             asset_dep_graph=asset_dep_graph,
             source_asset_keys=source_asset_keys,
             partitions_defs_by_key=partitions_defs_by_key,
             partition_mappings_by_key=partition_mappings_by_key,
             group_names_by_key=group_names_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
             auto_materialize_policies_by_key=auto_materialize_policies_by_key,
+            backfill_policies_by_key=backfill_policies_by_key,
             required_multi_asset_sets_by_key=required_multi_asset_sets_by_key,
             code_versions_by_key=code_versions_by_key,
             is_observable_by_key=is_observable_by_key,
             auto_observe_interval_minutes_by_key=auto_observe_interval_minutes_by_key,
         )
         self._assets = assets
         self._source_assets = source_assets
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.4.3/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/asset_in.py` & `dagster-1.4.3/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/asset_layer.py` & `dagster-1.4.3/dagster/_core/definitions/asset_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,16 +808,14 @@
 def _subset_assets_defs(
     assets: Iterable["AssetsDefinition"],
     selected_asset_keys: AbstractSet[AssetKey],
 ) -> Tuple[Sequence["AssetsDefinition"], Sequence["AssetsDefinition"],]:
     """Given a list of asset key selection queries, generate a set of AssetsDefinition objects
     representing the included/excluded definitions.
     """
-    from dagster._core.definitions import AssetsDefinition
-
     included_assets: Set[AssetsDefinition] = set()
     excluded_assets: Set[AssetsDefinition] = set()
 
     for asset in set(assets):
         # intersection
         selected_subset = selected_asset_keys & asset.keys
         # all assets in this def are selected
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/asset_out.py` & `dagster-1.4.3/dagster/_core/definitions/asset_out.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Mapping, NamedTuple, Optional, Sequence, Type, Union
 
 import dagster._check as check
 from dagster._annotations import PublicAttr
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
+from dagster._core.definitions.backfill_policy import BackfillPolicy
 from dagster._core.definitions.events import (
     AssetKey,
     CoercibleToAssetKey,
     CoercibleToAssetKeyPrefix,
 )
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.input import NoValueSentinel
@@ -27,14 +28,15 @@
             ("description", PublicAttr[Optional[str]]),
             ("is_required", PublicAttr[bool]),
             ("dagster_type", PublicAttr[Union[DagsterType, Type[NoValueSentinel]]]),
             ("group_name", PublicAttr[Optional[str]]),
             ("code_version", PublicAttr[Optional[str]]),
             ("freshness_policy", PublicAttr[Optional[FreshnessPolicy]]),
             ("auto_materialize_policy", PublicAttr[Optional[AutoMaterializePolicy]]),
+            ("backfill_policy", PublicAttr[Optional[BackfillPolicy]]),
         ],
     )
 ):
     """Defines one of the assets produced by a :py:func:`@multi_asset <multi_asset>`.
 
     Attributes:
         key_prefix (Optional[Union[str, Sequence[str]]]): If provided, the asset's key is the
@@ -57,14 +59,15 @@
         group_name (Optional[str]): A string name used to organize multiple assets into groups. If
             not provided, the name "default" is used.
         code_version (Optional[str]): The version of the code that generates this asset.
         freshness_policy (Optional[FreshnessPolicy]): A policy which indicates how up to date this
             asset is intended to be.
         auto_materialize_policy (Optional[AutoMaterializePolicy]): AutoMaterializePolicy to apply to
             the specified asset.
+        backfill_policy (Optional[BackfillPolicy]): BackfillPolicy to apply to the specified asset.
     """
 
     def __new__(
         cls,
         key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
         key: Optional[CoercibleToAssetKey] = None,
         dagster_type: Union[Type, DagsterType] = NoValueSentinel,
@@ -72,14 +75,15 @@
         is_required: bool = True,
         io_manager_key: Optional[str] = None,
         metadata: Optional[MetadataUserInput] = None,
         group_name: Optional[str] = None,
         code_version: Optional[str] = None,
         freshness_policy: Optional[FreshnessPolicy] = None,
         auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
     ):
         if isinstance(key_prefix, str):
             key_prefix = [key_prefix]
 
         return super(AssetOut, cls).__new__(
             cls,
             key=AssetKey.from_coercible(key) if key is not None else None,
@@ -97,14 +101,17 @@
             code_version=check.opt_str_param(code_version, "code_version"),
             freshness_policy=check.opt_inst_param(
                 freshness_policy, "freshness_policy", FreshnessPolicy
             ),
             auto_materialize_policy=check.opt_inst_param(
                 auto_materialize_policy, "auto_materialize_policy", AutoMaterializePolicy
             ),
+            backfill_policy=check.opt_inst_param(
+                backfill_policy, "backfill_policy", BackfillPolicy
+            ),
         )
 
     def to_out(self) -> Out:
         return Out(
             dagster_type=self.dagster_type,
             description=self.description,
             metadata=self.metadata,
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.4.3/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import datetime
 import itertools
-import json
 from collections import defaultdict
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
-    Callable,
     Dict,
     FrozenSet,
     Iterable,
     Mapping,
-    NamedTuple,
     Optional,
     Sequence,
     Set,
     Tuple,
     cast,
 )
 
@@ -22,134 +19,47 @@
 
 import dagster._check as check
 from dagster._annotations import experimental
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.data_time import CachingDataTimeResolver
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.time_window_partitions import (
-    TimeWindowPartitionsDefinition,
     get_time_partitions_def,
 )
-from dagster._serdes.serdes import whitelist_for_serdes
 from dagster._utils.backcompat import deprecation_warning
 
+from .asset_daemon_cursor import AssetDaemonCursor
 from .asset_graph import AssetGraph
 from .asset_selection import AssetSelection
 from .auto_materialize_condition import (
+    AutoMaterializeAssetEvaluation,
     AutoMaterializeCondition,
     AutoMaterializeDecisionType,
     MaxMaterializationsExceededAutoMaterializeCondition,
     MissingAutoMaterializeCondition,
     ParentMaterializedAutoMaterializeCondition,
     ParentOutdatedAutoMaterializeCondition,
 )
 from .decorators.sensor_decorator import sensor
 from .freshness_based_auto_materialize import (
     determine_asset_partitions_to_auto_materialize_for_freshness,
 )
 from .partition import (
     PartitionsDefinition,
-    PartitionsSubset,
     ScheduleType,
-    SerializedPartitionsSubset,
 )
 from .run_request import RunRequest
 from .sensor_definition import DefaultSensorStatus, SensorDefinition
 from .utils import check_valid_name
 
 if TYPE_CHECKING:
     from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
 
 
-@whitelist_for_serdes
-class AutoMaterializeAssetEvaluation(NamedTuple):
-    """Represents the results of the auto-materialize logic for a single asset.
-
-    Properties:
-        asset_key (AssetKey): The asset key that was evaluated.
-        partition_subsets_by_condition: The conditions that impact if the asset should be materialized, skipped, or
-            discarded. If the asset is partitioned, this will be a list of tuples, where the first
-            element is the condition and the second element is the serialized subset of partitions that the
-            condition applies to. If it's not partitioned, the second element will be None.
-    """
-
-    asset_key: AssetKey
-    partition_subsets_by_condition: Sequence[
-        Tuple[AutoMaterializeCondition, Optional[SerializedPartitionsSubset]]
-    ]
-    num_requested: int
-    num_skipped: int
-    num_discarded: int
-    run_ids: Set[str] = set()
-
-    @staticmethod
-    def from_conditions(
-        asset_graph: AssetGraph,
-        asset_key: AssetKey,
-        conditions_by_asset_partition: Mapping[
-            AssetKeyPartitionKey, AbstractSet[AutoMaterializeCondition]
-        ],
-        dynamic_partitions_store: "DynamicPartitionsStore",
-    ) -> "AutoMaterializeAssetEvaluation":
-        num_requested = 0
-        num_skipped = 0
-        num_discarded = 0
-
-        for conditions in conditions_by_asset_partition.values():
-            decision_type = _decision_type_for_conditions(conditions)
-            if decision_type == AutoMaterializeDecisionType.MATERIALIZE:
-                num_requested += 1
-            elif decision_type == AutoMaterializeDecisionType.SKIP:
-                num_skipped += 1
-            elif decision_type == AutoMaterializeDecisionType.DISCARD:
-                num_discarded += 1
-
-        partitions_def = asset_graph.get_partitions_def(asset_key)
-        if partitions_def is None:
-            return AutoMaterializeAssetEvaluation(
-                asset_key=asset_key,
-                partition_subsets_by_condition=[
-                    (condition, None)
-                    for condition in set().union(*conditions_by_asset_partition.values())
-                ],
-                num_requested=num_requested,
-                num_skipped=num_skipped,
-                num_discarded=num_discarded,
-            )
-        else:
-            partition_keys_by_condition = defaultdict(set)
-
-            for asset_partition, conditions in conditions_by_asset_partition.items():
-                for condition in conditions:
-                    partition_keys_by_condition[condition].add(
-                        check.not_none(asset_partition.partition_key)
-                    )
-
-            return AutoMaterializeAssetEvaluation(
-                asset_key=asset_key,
-                partition_subsets_by_condition=[
-                    (
-                        condition,
-                        SerializedPartitionsSubset.from_subset(
-                            subset=partitions_def.empty_subset().with_partition_keys(
-                                partition_keys
-                            ),
-                            partitions_def=partitions_def,
-                            dynamic_partitions_store=dynamic_partitions_store,
-                        ),
-                    )
-                    for condition, partition_keys in partition_keys_by_condition.items()
-                ],
-                num_requested=num_requested,
-                num_skipped=num_skipped,
-                num_discarded=num_discarded,
-            )
-
-
 def get_implicit_auto_materialize_policy(
     asset_graph: AssetGraph, asset_key: AssetKey
 ) -> Optional[AutoMaterializePolicy]:
     """For backcompat with pre-auto materialize policy graphs, assume a default scope of 1 day."""
     auto_materialize_policy = asset_graph.get_auto_materialize_policy(asset_key)
     if auto_materialize_policy is None:
         time_partitions_def = get_time_partitions_def(asset_graph.get_partitions_def(asset_key))
@@ -166,392 +76,17 @@
             ),
             for_freshness=True,
             max_materializations_per_minute=max_materializations_per_minute,
         )
     return auto_materialize_policy
 
 
-class AssetReconciliationCursor(NamedTuple):
-    """State that's saved between reconciliation evaluations.
-
-    Attributes:
-        latest_storage_id:
-            The latest observed storage ID across all assets. Useful for finding out what has
-            happened since the last tick.
-        handled_root_asset_keys:
-            Every entry is a non-partitioned asset with no parents that has been requested by this
-            sensor, discarded by this sensor, or has been materialized (even if not by this sensor).
-        handled_root_partitions_by_asset_key:
-            Every key is a partitioned root asset. Every value is the set of that asset's partitions
-            that have been requested by this sensor, discarded by this sensor,
-            or have been materialized (even if not by this sensor).
-        last_observe_request_timestamp_by_asset_key:
-            Every key is an observable source asset that has been auto-observed. The value is the
-            timestamp of the tick that requested the observation.
-    """
-
-    latest_storage_id: Optional[int]
-    handled_root_asset_keys: AbstractSet[AssetKey]
-    handled_root_partitions_by_asset_key: Mapping[AssetKey, PartitionsSubset]
-    evaluation_id: int
-    last_observe_request_timestamp_by_asset_key: Mapping[AssetKey, float]
-
-    def was_previously_handled(self, asset_key: AssetKey) -> bool:
-        return asset_key in self.handled_root_asset_keys
-
-    def get_unhandled_partitions(
-        self,
-        asset_key: AssetKey,
-        asset_graph,
-        dynamic_partitions_store: "DynamicPartitionsStore",
-        current_time: datetime.datetime,
-    ) -> Iterable[str]:
-        partitions_def = asset_graph.get_partitions_def(asset_key)
-
-        handled_subset = self.handled_root_partitions_by_asset_key.get(
-            asset_key, partitions_def.empty_subset()
-        )
-
-        return handled_subset.get_partition_keys_not_in_subset(
-            current_time=current_time,
-            dynamic_partitions_store=dynamic_partitions_store,
-        )
-
-    def with_updates(
-        self,
-        latest_storage_id: Optional[int],
-        conditions_by_asset_partition: Mapping[
-            AssetKeyPartitionKey, AbstractSet[AutoMaterializeCondition]
-        ],
-        newly_materialized_root_asset_keys: AbstractSet[AssetKey],
-        newly_materialized_root_partitions_by_asset_key: Mapping[AssetKey, AbstractSet[str]],
-        evaluation_id: int,
-        asset_graph: AssetGraph,
-        newly_observe_requested_asset_keys: Sequence[AssetKey],
-        observe_request_timestamp: float,
-    ) -> "AssetReconciliationCursor":
-        """Returns a cursor that represents this cursor plus the updates that have happened within the
-        tick.
-        """
-        handled_root_partitions_by_asset_key: Dict[AssetKey, Set[str]] = defaultdict(set)
-        handled_non_partitioned_root_assets: Set[AssetKey] = set()
-
-        for asset_partition, conditions in conditions_by_asset_partition.items():
-            if (
-                # only consider root assets
-                not asset_graph.has_non_source_parents(asset_partition.asset_key)
-                # which were discarded or materialized
-                and (
-                    _decision_type_for_conditions(conditions)
-                    in (
-                        AutoMaterializeDecisionType.DISCARD,
-                        AutoMaterializeDecisionType.MATERIALIZE,
-                    )
-                )
-            ):
-                if asset_partition.partition_key:
-                    handled_root_partitions_by_asset_key[asset_partition.asset_key].add(
-                        asset_partition.partition_key
-                    )
-                else:
-                    handled_non_partitioned_root_assets.add(asset_partition.asset_key)
-
-        result_handled_root_partitions_by_asset_key = {**self.handled_root_partitions_by_asset_key}
-        for asset_key in set(newly_materialized_root_partitions_by_asset_key.keys()) | set(
-            handled_root_partitions_by_asset_key.keys()
-        ):
-            prior_materialized_partitions = self.handled_root_partitions_by_asset_key.get(asset_key)
-            if prior_materialized_partitions is None:
-                prior_materialized_partitions = cast(
-                    PartitionsDefinition, asset_graph.get_partitions_def(asset_key)
-                ).empty_subset()
-
-            result_handled_root_partitions_by_asset_key[
-                asset_key
-            ] = prior_materialized_partitions.with_partition_keys(
-                itertools.chain(
-                    newly_materialized_root_partitions_by_asset_key[asset_key],
-                    handled_root_partitions_by_asset_key[asset_key],
-                )
-            )
-
-        result_handled_root_asset_keys = (
-            self.handled_root_asset_keys
-            | newly_materialized_root_asset_keys
-            | handled_non_partitioned_root_assets
-        )
-
-        result_last_observe_request_timestamp_by_asset_key = {
-            **self.last_observe_request_timestamp_by_asset_key
-        }
-        for asset_key in newly_observe_requested_asset_keys:
-            result_last_observe_request_timestamp_by_asset_key[
-                asset_key
-            ] = observe_request_timestamp
-
-        if latest_storage_id and self.latest_storage_id:
-            check.invariant(
-                latest_storage_id >= self.latest_storage_id,
-                "Latest storage ID should be >= previous latest storage ID",
-            )
-
-        return AssetReconciliationCursor(
-            latest_storage_id=latest_storage_id or self.latest_storage_id,
-            handled_root_asset_keys=result_handled_root_asset_keys,
-            handled_root_partitions_by_asset_key=result_handled_root_partitions_by_asset_key,
-            evaluation_id=evaluation_id,
-            last_observe_request_timestamp_by_asset_key=result_last_observe_request_timestamp_by_asset_key,
-        )
-
-    @classmethod
-    def empty(cls) -> "AssetReconciliationCursor":
-        return AssetReconciliationCursor(
-            latest_storage_id=None,
-            handled_root_partitions_by_asset_key={},
-            handled_root_asset_keys=set(),
-            evaluation_id=0,
-            last_observe_request_timestamp_by_asset_key={},
-        )
-
-    @classmethod
-    def from_serialized(cls, cursor: str, asset_graph: AssetGraph) -> "AssetReconciliationCursor":
-        data = json.loads(cursor)
-
-        if isinstance(data, list):  # backcompat
-            check.invariant(len(data) in [3, 4], "Invalid serialized cursor")
-            (
-                latest_storage_id,
-                serialized_handled_root_asset_keys,
-                serialized_handled_root_partitions_by_asset_key,
-            ) = data[:3]
-
-            evaluation_id = data[3] if len(data) == 4 else 0
-            serialized_last_observe_request_timestamp_by_asset_key = {}
-        else:
-            latest_storage_id = data["latest_storage_id"]
-            serialized_handled_root_asset_keys = data["handled_root_asset_keys"]
-            serialized_handled_root_partitions_by_asset_key = data[
-                "handled_root_partitions_by_asset_key"
-            ]
-            evaluation_id = data["evaluation_id"]
-            serialized_last_observe_request_timestamp_by_asset_key = data.get(
-                "last_observe_request_timestamp_by_asset_key", {}
-            )
-
-        handled_root_partitions_by_asset_key = {}
-        for (
-            key_str,
-            serialized_subset,
-        ) in serialized_handled_root_partitions_by_asset_key.items():
-            key = AssetKey.from_user_string(key_str)
-            if key not in asset_graph.materializable_asset_keys:
-                continue
-
-            partitions_def = asset_graph.get_partitions_def(key)
-            if partitions_def is None:
-                continue
-
-            try:
-                # in the case that the partitions def has changed, we may not be able to deserialize
-                # the corresponding subset. in this case, we just use an empty subset
-                handled_root_partitions_by_asset_key[key] = partitions_def.deserialize_subset(
-                    serialized_subset
-                )
-            except:
-                handled_root_partitions_by_asset_key[key] = partitions_def.empty_subset()
-        return cls(
-            latest_storage_id=latest_storage_id,
-            handled_root_asset_keys={
-                AssetKey.from_user_string(key_str) for key_str in serialized_handled_root_asset_keys
-            },
-            handled_root_partitions_by_asset_key=handled_root_partitions_by_asset_key,
-            evaluation_id=evaluation_id,
-            last_observe_request_timestamp_by_asset_key={
-                AssetKey.from_user_string(key_str): timestamp
-                for key_str, timestamp in serialized_last_observe_request_timestamp_by_asset_key.items()
-            },
-        )
-
-    @classmethod
-    def get_evaluation_id_from_serialized(cls, cursor: str) -> Optional[int]:
-        data = json.loads(cursor)
-        if isinstance(data, list):  # backcompat
-            check.invariant(len(data) in [3, 4], "Invalid serialized cursor")
-            return data[3] if len(data) == 4 else None
-        else:
-            return data["evaluation_id"]
-
-    def serialize(self) -> str:
-        serializable_handled_root_partitions_by_asset_key = {
-            key.to_user_string(): subset.serialize()
-            for key, subset in self.handled_root_partitions_by_asset_key.items()
-        }
-        serialized = json.dumps(
-            {
-                "latest_storage_id": self.latest_storage_id,
-                "handled_root_asset_keys": [
-                    key.to_user_string() for key in self.handled_root_asset_keys
-                ],
-                "handled_root_partitions_by_asset_key": serializable_handled_root_partitions_by_asset_key,
-                "evaluation_id": self.evaluation_id,
-                "last_observe_request_timestamp_by_asset_key": {
-                    key.to_user_string(): timestamp
-                    for key, timestamp in self.last_observe_request_timestamp_by_asset_key.items()
-                },
-            }
-        )
-        return serialized
-
-
-def find_parent_materialized_asset_partitions(
-    instance_queryer: "CachingInstanceQueryer",
-    latest_storage_id: Optional[int],
-    target_asset_keys: AbstractSet[AssetKey],
-    target_asset_keys_and_parents: AbstractSet[AssetKey],
-    asset_graph: AssetGraph,
-    can_reconcile_fn: Callable[[AssetKeyPartitionKey], bool] = lambda _: True,
-    map_old_time_partitions: bool = True,
-) -> Tuple[AbstractSet[AssetKeyPartitionKey], Optional[int]]:
-    """Finds asset partitions in the given selection whose parents have been materialized since
-    latest_storage_id.
-
-    Returns:
-        - A set of asset partitions.
-        - The latest observed storage_id across all relevant assets. Can be used to avoid scanning
-            the same events the next time this function is called.
-    """
-    result_asset_partitions: Set[AssetKeyPartitionKey] = set()
-    result_latest_storage_id = latest_storage_id
-
-    for asset_key in target_asset_keys_and_parents:
-        if asset_graph.is_source(asset_key) and not asset_graph.is_observable(asset_key):
-            continue
-
-        # the set of asset partitions which have been updated since the latest storage id
-        new_asset_partitions = instance_queryer.get_asset_partitions_updated_after_cursor(
-            asset_key=asset_key,
-            asset_partitions=None,
-            after_cursor=latest_storage_id,
-        )
-        if not new_asset_partitions:
-            continue
-
-        partitions_def = asset_graph.get_partitions_def(asset_key)
-        if partitions_def is None:
-            latest_record = check.not_none(
-                instance_queryer.get_latest_materialization_or_observation_record(
-                    AssetKeyPartitionKey(asset_key)
-                )
-            )
-            for child in asset_graph.get_children_partitions(
-                dynamic_partitions_store=instance_queryer,
-                current_time=instance_queryer.evaluation_time,
-                asset_key=asset_key,
-            ):
-                child_partitions_def = asset_graph.get_partitions_def(child.asset_key)
-                if (
-                    child.asset_key in target_asset_keys
-                    # when mapping from unpartitioned assets to time partitioned assets, we ignore
-                    # historical time partitions
-                    and (
-                        map_old_time_partitions
-                        or not isinstance(child_partitions_def, TimeWindowPartitionsDefinition)
-                        or child.partition_key
-                        == child_partitions_def.get_last_partition_key(
-                            current_time=instance_queryer.evaluation_time
-                        )
-                    )
-                    and not instance_queryer.is_asset_planned_for_run(latest_record.run_id, child)
-                ):
-                    result_asset_partitions.add(child)
-        else:
-            partitions_subset = partitions_def.empty_subset().with_partition_keys(
-                [
-                    asset_partition.partition_key
-                    for asset_partition in new_asset_partitions
-                    if asset_partition.partition_key is not None
-                    and partitions_def.has_partition_key(
-                        asset_partition.partition_key,
-                        dynamic_partitions_store=instance_queryer,
-                        current_time=instance_queryer.evaluation_time,
-                    )
-                ]
-            )
-            for child in asset_graph.get_children(asset_key):
-                child_partitions_def = asset_graph.get_partitions_def(child)
-                if child not in target_asset_keys:
-                    continue
-                elif not child_partitions_def:
-                    result_asset_partitions.add(AssetKeyPartitionKey(child, None))
-                else:
-                    # we are mapping from the partitions of the parent asset to the partitions of
-                    # the child asset
-                    partition_mapping = asset_graph.get_partition_mapping(child, asset_key)
-                    child_partitions_subset = (
-                        partition_mapping.get_downstream_partitions_for_partitions(
-                            partitions_subset,
-                            downstream_partitions_def=child_partitions_def,
-                            dynamic_partitions_store=instance_queryer,
-                            current_time=instance_queryer.evaluation_time,
-                        )
-                    )
-                    for child_partition in child_partitions_subset.get_partition_keys():
-                        # we need to see if the child is planned for the same run, but this is
-                        # expensive, so we try to avoid doing so in as many situations as possible
-                        child_asset_partition = AssetKeyPartitionKey(child, child_partition)
-                        if not can_reconcile_fn(child_asset_partition):
-                            continue
-                        elif (
-                            # if child has a different partitions def than the parent, then it must
-                            # have been executed in a different run, so it's a valid candidate
-                            child_partitions_def != partitions_def
-                            # if child partition key is not the same as any newly materialized
-                            # parent key, then it could not have been executed in the same run as
-                            # its parent
-                            or child_partition not in partitions_subset
-                            # if child partition is not failed or in progress, then even if it was
-                            # executed in the same run, we can filter it out later with an is_reconciled
-                            # check (cheaper than the below logic)
-                            or child_partition
-                            not in instance_queryer.get_failed_or_in_progress_subset(
-                                asset_key=child
-                            )
-                        ):
-                            result_asset_partitions.add(child_asset_partition)
-                        else:
-                            # manually query to see if this asset partition was intended to be
-                            # executed in the same run as its parent
-                            latest_partition_record = check.not_none(
-                                instance_queryer.get_latest_materialization_or_observation_record(
-                                    AssetKeyPartitionKey(asset_key, child_partition),
-                                    after_cursor=latest_storage_id,
-                                )
-                            )
-                            if not instance_queryer.is_asset_planned_for_run(
-                                latest_partition_record.run_id, child
-                            ):
-                                result_asset_partitions.add(child_asset_partition)
-
-        asset_latest_storage_id = (
-            instance_queryer.get_latest_materialization_or_observation_storage_id(
-                AssetKeyPartitionKey(asset_key)
-            )
-        )
-        if (
-            result_latest_storage_id is None
-            or (asset_latest_storage_id or 0) > result_latest_storage_id
-        ):
-            result_latest_storage_id = asset_latest_storage_id
-
-    return (result_asset_partitions, result_latest_storage_id)
-
-
 def find_never_handled_root_asset_partitions(
     instance_queryer: "CachingInstanceQueryer",
-    cursor: AssetReconciliationCursor,
+    cursor: AssetDaemonCursor,
     target_asset_keys: AbstractSet[AssetKey],
     asset_graph: AssetGraph,
 ) -> Tuple[
     Iterable[AssetKeyPartitionKey], AbstractSet[AssetKey], Mapping[AssetKey, AbstractSet[str]]
 ]:
     """Finds asset partitions that have never been materialized or requested and that have no
     parents.
@@ -595,42 +130,27 @@
     return (
         never_handled,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
     )
 
 
-def _decision_type_for_conditions(
-    conditions: Optional[AbstractSet[AutoMaterializeCondition]],
-) -> Optional[AutoMaterializeDecisionType]:
-    """Based on a set of conditions, determine the resulting decision."""
-    if not conditions:
-        return None
-    condition_decision_types = {condition.decision_type for condition in conditions}
-    # precedence of decisions
-    for decision_type in [
-        AutoMaterializeDecisionType.SKIP,
-        AutoMaterializeDecisionType.DISCARD,
-        AutoMaterializeDecisionType.MATERIALIZE,
-    ]:
-        if decision_type in condition_decision_types:
-            return decision_type
-    return None
-
-
 def _will_materialize_for_conditions(
     conditions: Optional[AbstractSet[AutoMaterializeCondition]],
 ) -> bool:
     """Based on a set of conditions, determine if the asset will be materialized."""
-    return _decision_type_for_conditions(conditions) == AutoMaterializeDecisionType.MATERIALIZE
+    return (
+        AutoMaterializeDecisionType.from_conditions(conditions)
+        == AutoMaterializeDecisionType.MATERIALIZE
+    )
 
 
 def determine_asset_partitions_to_auto_materialize(
     instance_queryer: "CachingInstanceQueryer",
-    cursor: AssetReconciliationCursor,
+    cursor: AssetDaemonCursor,
     target_asset_keys: AbstractSet[AssetKey],
     target_asset_keys_and_parents: AbstractSet[AssetKey],
     asset_graph: AssetGraph,
     current_time: datetime.datetime,
     conditions_by_asset_partition_for_freshness: Mapping[
         AssetKeyPartitionKey, Set[AutoMaterializeCondition]
     ],
@@ -682,20 +202,21 @@
                     candidate.asset_key,
                     candidate.partition_key,
                 ).required_but_nonexistent_parents_partitions
             )
             > 0
         )
 
-    stale_candidates, latest_storage_id = find_parent_materialized_asset_partitions(
-        instance_queryer=instance_queryer,
+    (
+        stale_candidates,
+        latest_storage_id,
+    ) = instance_queryer.asset_partitions_with_newly_updated_parents_and_new_latest_storage_id(
         latest_storage_id=cursor.latest_storage_id,
-        target_asset_keys=target_asset_keys,
-        target_asset_keys_and_parents=target_asset_keys_and_parents,
-        asset_graph=asset_graph,
+        target_asset_keys=frozenset(target_asset_keys),
+        target_asset_keys_and_parents=frozenset(target_asset_keys_and_parents),
         can_reconcile_fn=can_reconcile_candidate,
         map_old_time_partitions=False,
     )
 
     def get_waiting_on_asset_keys(candidate: AssetKeyPartitionKey) -> FrozenSet[AssetKey]:
         """Returns the set of ancestor asset keys that must be materialized before this asset can be
         materialized.
@@ -744,19 +265,44 @@
             auto_materialize_policy.on_missing
             and not instance_queryer.asset_partition_has_materialization_or_observation(
                 asset_partition=candidate
             )
         ):
             conditions.add(MissingAutoMaterializeCondition())
 
-        # if the parent has been updated
-        if auto_materialize_policy.on_new_parent_data and not instance_queryer.is_reconciled(
-            asset_partition=candidate
-        ):
-            conditions.add(ParentMaterializedAutoMaterializeCondition())
+        # if parent data has been updated or will update
+        elif auto_materialize_policy.on_new_parent_data:
+            if not asset_graph.is_source(candidate.asset_key):
+                parent_asset_partitions = asset_graph.get_parents_partitions(
+                    dynamic_partitions_store=instance_queryer,
+                    current_time=evaluation_time,
+                    asset_key=candidate.asset_key,
+                    partition_key=candidate.partition_key,
+                ).parent_partitions
+
+                (
+                    updated_parent_asset_partitions,
+                    _,
+                ) = instance_queryer.get_updated_and_missing_parent_asset_partitions(
+                    candidate, parent_asset_partitions
+                )
+                updated_parents = {parent.asset_key for parent in updated_parent_asset_partitions}
+
+                will_update_parents = set()
+                for parent in parent_asset_partitions:
+                    if _will_materialize_for_conditions(conditions_by_asset_partition.get(parent)):
+                        will_update_parents.add(parent.asset_key)
+
+                if updated_parents or will_update_parents:
+                    conditions.add(
+                        ParentMaterializedAutoMaterializeCondition(
+                            updated_asset_keys=frozenset(updated_parents),
+                            will_update_asset_keys=frozenset(will_update_parents),
+                        )
+                    )
 
         # if the parents will not be resolved this tick
         waiting_on_asset_keys = get_waiting_on_asset_keys(candidate)
         if waiting_on_asset_keys:
             conditions.add(
                 ParentOutdatedAutoMaterializeCondition(waiting_on_asset_keys=waiting_on_asset_keys)
             )
@@ -811,23 +357,19 @@
     )
 
 
 def reconcile(
     asset_graph: AssetGraph,
     target_asset_keys: AbstractSet[AssetKey],
     instance: "DagsterInstance",
-    cursor: AssetReconciliationCursor,
+    cursor: AssetDaemonCursor,
     materialize_run_tags: Optional[Mapping[str, str]],
     observe_run_tags: Optional[Mapping[str, str]],
     auto_observe: bool,
-) -> Tuple[
-    Sequence[RunRequest],
-    AssetReconciliationCursor,
-    Sequence[AutoMaterializeAssetEvaluation],
-]:
+) -> Tuple[Sequence[RunRequest], AssetDaemonCursor, Sequence[AutoMaterializeAssetEvaluation],]:
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
 
     current_time = pendulum.now("UTC")
 
     instance_queryer = CachingInstanceQueryer(
         instance=instance, asset_graph=asset_graph, evaluation_time=current_time
     )
@@ -1110,17 +652,17 @@
         minimum_interval_seconds=minimum_interval_seconds,
         description=description,
         default_status=default_status,
     )
     def _sensor(context):
         asset_graph = context.repository_def.asset_graph
         cursor = (
-            AssetReconciliationCursor.from_serialized(context.cursor, asset_graph)
+            AssetDaemonCursor.from_serialized(context.cursor, asset_graph)
             if context.cursor
-            else AssetReconciliationCursor.empty()
+            else AssetDaemonCursor.empty()
         )
 
         # if there is a auto materialize policy set in the selection, filter down to that. Otherwise, use the
         # whole selection
         target_asset_keys = asset_selection.resolve(asset_graph)
         for target_key in target_asset_keys:
             check.invariant(
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/asset_selection.py` & `dagster-1.4.3/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.4.3/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/assets.py` & `dagster-1.4.3/dagster/_core/definitions/assets.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 )
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.decorator_utils import get_function_params
 from dagster._core.definitions.asset_layer import get_dep_node_handles_of_graph_backed_asset
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
+from dagster._core.definitions.backfill_policy import BackfillPolicy, BackfillPolicyType
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.metadata import ArbitraryMetadataMapping
 from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
 from dagster._core.definitions.op_selection import get_graph_subset
 from dagster._core.definitions.partition_mapping import MultiPartitionMapping
 from dagster._core.definitions.time_window_partition_mapping import TimeWindowPartitionMapping
 from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
@@ -79,14 +80,15 @@
     _resource_defs: Mapping[str, ResourceDefinition]
     _group_names_by_key: Mapping[AssetKey, str]
     _selected_asset_keys: AbstractSet[AssetKey]
     _can_subset: bool
     _metadata_by_key: Mapping[AssetKey, ArbitraryMetadataMapping]
     _freshness_policies_by_key: Mapping[AssetKey, FreshnessPolicy]
     _auto_materialize_policies_by_key: Mapping[AssetKey, AutoMaterializePolicy]
+    _backfill_policy: Optional[BackfillPolicy]
     _code_versions_by_key: Mapping[AssetKey, Optional[str]]
     _descriptions_by_key: Mapping[AssetKey, str]
 
     def __init__(
         self,
         *,
         keys_by_input_name: Mapping[str, AssetKey],
@@ -98,14 +100,15 @@
         selected_asset_keys: Optional[AbstractSet[AssetKey]] = None,
         can_subset: bool = False,
         resource_defs: Optional[Mapping[str, object]] = None,
         group_names_by_key: Optional[Mapping[AssetKey, str]] = None,
         metadata_by_key: Optional[Mapping[AssetKey, ArbitraryMetadataMapping]] = None,
         freshness_policies_by_key: Optional[Mapping[AssetKey, FreshnessPolicy]] = None,
         auto_materialize_policies_by_key: Optional[Mapping[AssetKey, AutoMaterializePolicy]] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
         descriptions_by_key: Optional[Mapping[AssetKey, str]] = None,
         # if adding new fields, make sure to handle them in the with_attributes, from_graph, and
         # get_attributes_dict methods
     ):
         from dagster._core.execution.build_resources import wrap_resources_for_execution
 
         from .graph_definition import GraphDefinition
@@ -228,14 +231,28 @@
         self._auto_materialize_policies_by_key = check.opt_mapping_param(
             auto_materialize_policies_by_key,
             "auto_materialize_policies_by_key",
             key_type=AssetKey,
             value_type=AutoMaterializePolicy,
         )
 
+        self._backfill_policy = check.opt_inst_param(
+            backfill_policy, "backfill_policy", BackfillPolicy
+        )
+
+        if self._partitions_def is None:
+            # check if backfill policy is BackfillPolicyType.SINGLE_RUN if asset is not partitioned
+            check.param_invariant(
+                backfill_policy.policy_type is BackfillPolicyType.SINGLE_RUN
+                if backfill_policy
+                else True,
+                "backfill_policy",
+                "Non partitioned asset can only have single run backfill policy",
+            )
+
         _validate_self_deps(
             input_keys=self._keys_by_input_name.values(),
             output_keys=self._selected_asset_keys,
             partition_mappings=self._partition_mappings,
             partitions_def=self._partitions_def,
         )
 
@@ -251,14 +268,15 @@
         selected_asset_keys: Optional[AbstractSet[AssetKey]],
         can_subset: bool,
         resource_defs: Optional[Mapping[str, object]],
         group_names_by_key: Optional[Mapping[AssetKey, str]],
         metadata_by_key: Optional[Mapping[AssetKey, ArbitraryMetadataMapping]],
         freshness_policies_by_key: Optional[Mapping[AssetKey, FreshnessPolicy]],
         auto_materialize_policies_by_key: Optional[Mapping[AssetKey, AutoMaterializePolicy]],
+        backfill_policy: Optional[BackfillPolicy],
         descriptions_by_key: Optional[Mapping[AssetKey, str]],
     ) -> "AssetsDefinition":
         return AssetsDefinition(
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name=keys_by_output_name,
             node_def=node_def,
             partitions_def=partitions_def,
@@ -267,14 +285,15 @@
             selected_asset_keys=selected_asset_keys,
             can_subset=can_subset,
             resource_defs=resource_defs,
             group_names_by_key=group_names_by_key,
             metadata_by_key=metadata_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
             auto_materialize_policies_by_key=auto_materialize_policies_by_key,
+            backfill_policy=backfill_policy,
             descriptions_by_key=descriptions_by_key,
         )
 
     def __call__(self, *args: object, **kwargs: object) -> object:
         from dagster._core.definitions.decorators.op_decorator import DecoratedOpFunction
         from dagster._core.execution.context.compute import OpExecutionContext
 
@@ -319,14 +338,15 @@
         group_names_by_output_name: Optional[Mapping[str, Optional[str]]] = None,
         descriptions_by_output_name: Optional[Mapping[str, str]] = None,
         metadata_by_output_name: Optional[Mapping[str, Optional[ArbitraryMetadataMapping]]] = None,
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
         auto_materialize_policies_by_output_name: Optional[
             Mapping[str, Optional[AutoMaterializePolicy]]
         ] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
         can_subset: bool = False,
     ) -> "AssetsDefinition":
         """Constructs an AssetsDefinition from a GraphDefinition.
 
         Args:
             graph_def (GraphDefinition): The GraphDefinition that is an asset.
             keys_by_input_name (Optional[Mapping[str, AssetKey]]): A mapping of the input
@@ -371,14 +391,15 @@
                 FreshnessPolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the FreshnessPolicies to be attached
                 to the associated asset.
             auto_materialize_policies_by_output_name (Optional[Mapping[str, Optional[AutoMaterializePolicy]]]): Defines an
                 AutoMaterializePolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the AutoMaterializePolicies to be attached
                 to the associated asset.
+            backfill_policy (Optional[BackfillPolicy]): Defines this asset's BackfillPolicy
         """
         if resource_defs is not None:
             experimental_arg_warning("resource_defs", "AssetsDefinition.from_graph")
         return AssetsDefinition._from_node(
             node_def=graph_def,
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name=keys_by_output_name,
@@ -389,14 +410,15 @@
             resource_defs=resource_defs,
             group_name=group_name,
             group_names_by_output_name=group_names_by_output_name,
             descriptions_by_output_name=descriptions_by_output_name,
             metadata_by_output_name=metadata_by_output_name,
             freshness_policies_by_output_name=freshness_policies_by_output_name,
             auto_materialize_policies_by_output_name=auto_materialize_policies_by_output_name,
+            backfill_policy=backfill_policy,
             can_subset=can_subset,
         )
 
     @public
     @staticmethod
     def from_op(
         op_def: OpDefinition,
@@ -411,14 +433,15 @@
         group_names_by_output_name: Optional[Mapping[str, Optional[str]]] = None,
         descriptions_by_output_name: Optional[Mapping[str, str]] = None,
         metadata_by_output_name: Optional[Mapping[str, Optional[ArbitraryMetadataMapping]]] = None,
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
         auto_materialize_policies_by_output_name: Optional[
             Mapping[str, Optional[AutoMaterializePolicy]]
         ] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
         can_subset: bool = False,
     ) -> "AssetsDefinition":
         """Constructs an AssetsDefinition from an OpDefinition.
 
         Args:
             op_def (OpDefinition): The OpDefinition that is an asset.
             keys_by_input_name (Optional[Mapping[str, AssetKey]]): A mapping of the input
@@ -459,14 +482,15 @@
                 FreshnessPolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the FreshnessPolicies to be attached
                 to the associated asset.
             auto_materialize_policies_by_output_name (Optional[Mapping[str, Optional[AutoMaterializePolicy]]]): Defines an
                 AutoMaterializePolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the AutoMaterializePolicies to be attached
                 to the associated asset.
+            backfill_policy (Optional[BackfillPolicy]): Defines this asset's BackfillPolicy
         """
         return AssetsDefinition._from_node(
             node_def=op_def,
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name=keys_by_output_name,
             key_prefix=key_prefix,
             internal_asset_deps=internal_asset_deps,
@@ -474,14 +498,15 @@
             partition_mappings=partition_mappings,
             group_name=group_name,
             group_names_by_output_name=group_names_by_output_name,
             descriptions_by_output_name=descriptions_by_output_name,
             metadata_by_output_name=metadata_by_output_name,
             freshness_policies_by_output_name=freshness_policies_by_output_name,
             auto_materialize_policies_by_output_name=auto_materialize_policies_by_output_name,
+            backfill_policy=backfill_policy,
             can_subset=can_subset,
         )
 
     @staticmethod
     def _from_node(
         node_def: Union[OpDefinition, "GraphDefinition"],
         *,
@@ -496,14 +521,15 @@
         group_names_by_output_name: Optional[Mapping[str, Optional[str]]] = None,
         descriptions_by_output_name: Optional[Mapping[str, str]] = None,
         metadata_by_output_name: Optional[Mapping[str, Optional[ArbitraryMetadataMapping]]] = None,
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
         auto_materialize_policies_by_output_name: Optional[
             Mapping[str, Optional[AutoMaterializePolicy]]
         ] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
         can_subset: bool = False,
     ) -> "AssetsDefinition":
         node_def = check.inst_param(node_def, "node_def", NodeDefinition)
         keys_by_input_name = _infer_keys_by_input_names(
             node_def,
             check.opt_mapping_param(
                 keys_by_input_name, "keys_by_input_name", key_type=str, value_type=AssetKey
@@ -598,14 +624,17 @@
             auto_materialize_policies_by_key={
                 keys_by_output_name_with_prefix[output_name]: auto_materialize_policy
                 for output_name, auto_materialize_policy in auto_materialize_policies_by_output_name.items()
                 if auto_materialize_policy is not None
             }
             if auto_materialize_policies_by_output_name
             else None,
+            backfill_policy=check.opt_inst_param(
+                backfill_policy, "backfill_policy", BackfillPolicy
+            ),
             descriptions_by_key={
                 keys_by_output_name_with_prefix[output_name]: description
                 for output_name, description in descriptions_by_output_name.items()
                 if description is not None
             }
             if descriptions_by_output_name
             else None,
@@ -743,14 +772,18 @@
     def freshness_policies_by_key(self) -> Mapping[AssetKey, FreshnessPolicy]:
         return self._freshness_policies_by_key
 
     @property
     def auto_materialize_policies_by_key(self) -> Mapping[AssetKey, AutoMaterializePolicy]:
         return self._auto_materialize_policies_by_key
 
+    @property
+    def backfill_policy(self) -> Optional[BackfillPolicy]:
+        return self._backfill_policy
+
     @public
     @property
     def partitions_def(self) -> Optional[PartitionsDefinition]:
         """Optional[PartitionsDefinition]: The PartitionsDefinition for this AssetsDefinition (if any).
         """
         return self._partitions_def
 
@@ -811,14 +844,15 @@
         metadata_by_key: Optional[Mapping[AssetKey, ArbitraryMetadataMapping]] = None,
         freshness_policy: Optional[
             Union[FreshnessPolicy, Mapping[AssetKey, FreshnessPolicy]]
         ] = None,
         auto_materialize_policy: Optional[
             Union[AutoMaterializePolicy, Mapping[AssetKey, AutoMaterializePolicy]]
         ] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
     ) -> "AssetsDefinition":
         output_asset_key_replacements = check.opt_mapping_param(
             output_asset_key_replacements,
             "output_asset_key_replacements",
             key_type=AssetKey,
             value_type=AssetKey,
         )
@@ -834,14 +868,16 @@
         descriptions_by_key = check.opt_mapping_param(
             descriptions_by_key, "descriptions_by_key", key_type=AssetKey, value_type=str
         )
         metadata_by_key = check.opt_mapping_param(
             metadata_by_key, "metadata_by_key", key_type=AssetKey, value_type=dict
         )
 
+        backfill_policy = check.opt_inst_param(backfill_policy, "backfill_policy", BackfillPolicy)
+
         if group_names_by_key:
             group_name_conflicts = [
                 asset_key
                 for asset_key in group_names_by_key
                 if asset_key in self.group_names_by_key
                 and self.group_names_by_key[asset_key] != DEFAULT_GROUP_NAME
             ]
@@ -951,14 +987,15 @@
             group_names_by_key={
                 **replaced_group_names_by_key,
                 **group_names_by_key,
             },
             metadata_by_key=replaced_metadata_by_key,
             freshness_policies_by_key=replaced_freshness_policies_by_key,
             auto_materialize_policies_by_key=replaced_auto_materialize_policies_by_key,
+            backfill_policy=backfill_policy if backfill_policy else self.backfill_policy,
             descriptions_by_key=replaced_descriptions_by_key,
         )
 
         return self.__class__(**merge_dicts(self.get_attributes_dict(), replaced_attributes))
 
     def _subset_graph_backed_asset(
         self,
@@ -1194,14 +1231,15 @@
             selected_asset_keys=self._selected_asset_keys,
             can_subset=self._can_subset,
             resource_defs=self._resource_defs,
             group_names_by_key=self._group_names_by_key,
             metadata_by_key=self._metadata_by_key,
             freshness_policies_by_key=self._freshness_policies_by_key,
             auto_materialize_policies_by_key=self._auto_materialize_policies_by_key,
+            backfill_policy=self._backfill_policy,
             descriptions_by_key=self._descriptions_by_key,
         )
 
 
 def _infer_keys_by_input_names(
     node_def: Union["GraphDefinition", OpDefinition], keys_by_input_name: Mapping[str, AssetKey]
 ) -> Mapping[str, AssetKey]:
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/assets_job.py` & `dagster-1.4.3/dagster/_core/definitions/assets_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.4.3/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.4.3/dagster/_core/definitions/cacheable_assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import AbstractSet, Any, List, Mapping, NamedTuple, Optional, Sequence, Union
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._config.field_utils import compute_fields_hash
 from dagster._core.definitions.assets import AssetsDefinition
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
+from dagster._core.definitions.backfill_policy import BackfillPolicy
 from dagster._core.definitions.events import AssetKey, CoercibleToAssetKeyPrefix
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.metadata import MetadataUserInput
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.resource_requirement import ResourceAddable
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils import hash_collection
@@ -32,14 +33,15 @@
             ("can_subset", bool),
             ("extra_metadata", Optional[Mapping[Any, Any]]),
             ("freshness_policies_by_output_name", Optional[Mapping[str, FreshnessPolicy]]),
             (
                 "auto_materialize_policies_by_output_name",
                 Optional[Mapping[str, AutoMaterializePolicy]],
             ),
+            ("backfill_policy", Optional[BackfillPolicy]),
         ],
     )
 ):
     """Data representing cacheable metadata about assets, which can be used to generate
     AssetsDefinition objects in other processes.
     """
 
@@ -53,14 +55,15 @@
         key_prefix: Optional[Sequence[str]] = None,
         can_subset: bool = False,
         extra_metadata: Optional[Mapping[Any, Any]] = None,
         freshness_policies_by_output_name: Optional[Mapping[str, FreshnessPolicy]] = None,
         auto_materialize_policies_by_output_name: Optional[
             Mapping[str, AutoMaterializePolicy]
         ] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
     ):
         extra_metadata = check.opt_nullable_mapping_param(extra_metadata, "extra_metadata")
         try:
             # check that the value is JSON serializable
             seven.dumps(extra_metadata)
         except TypeError:
             check.failed("Value for `extra_metadata` is not JSON serializable.")
@@ -96,14 +99,17 @@
             ),
             auto_materialize_policies_by_output_name=check.opt_nullable_mapping_param(
                 auto_materialize_policies_by_output_name,
                 "auto_materialize_policies_by_output_name",
                 key_type=str,
                 value_type=AutoMaterializePolicy,
             ),
+            backfill_policy=check.opt_inst_param(
+                backfill_policy, "backfill_policy", BackfillPolicy
+            ),
         )
 
     # Allow this to be hashed for use in `lru_cache`. This is needed because:
     # - `ReconstructableJob` uses `lru_cache`
     # - `ReconstructableJob` has a `ReconstructableRepository` attribute
     # - `ReconstructableRepository` has a `RepositoryLoadData` attribute
     # - `RepositoryLoadData` has a `Mapping` attribute containing `AssetsDefinitionCacheableData`
@@ -170,24 +176,26 @@
         return PrefixOrGroupWrappedCacheableAssetsDefinition(self, prefix_for_all_assets=prefix)
 
     def with_attributes_for_all(
         self,
         group_name: Optional[str],
         freshness_policy: Optional[FreshnessPolicy],
         auto_materialize_policy: Optional[AutoMaterializePolicy],
+        backfill_policy: Optional[BackfillPolicy],
     ) -> "CacheableAssetsDefinition":
         """Utility method which allows setting attributes for all assets in this
         CacheableAssetsDefinition, since the keys may not be known at the time of
         construction.
         """
         return PrefixOrGroupWrappedCacheableAssetsDefinition(
             self,
             group_name_for_all_assets=group_name,
             freshness_policy=freshness_policy,
             auto_materialize_policy=auto_materialize_policy,
+            backfill_policy=backfill_policy,
         )
 
 
 class WrappedCacheableAssetsDefinition(CacheableAssetsDefinition):
     """Wraps an instance of CacheableAssetsDefinition, applying transformed_assets_def to the
     generated AssetsDefinition objects. This lets e.g. users define resources on
     the cacheable assets at repo creation time which are not actually bound until
@@ -243,22 +251,24 @@
         prefix_for_all_assets: Optional[List[str]] = None,
         freshness_policy: Optional[
             Union[FreshnessPolicy, Mapping[AssetKey, FreshnessPolicy]]
         ] = None,
         auto_materialize_policy: Optional[
             Union[AutoMaterializePolicy, Mapping[AssetKey, AutoMaterializePolicy]]
         ] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
     ):
         self._output_asset_key_replacements = output_asset_key_replacements or {}
         self._input_asset_key_replacements = input_asset_key_replacements or {}
         self._group_names_by_key = group_names_by_key or {}
         self._group_name_for_all_assets = group_name_for_all_assets
         self._prefix_for_all_assets = prefix_for_all_assets
         self._freshness_policy = freshness_policy
         self._auto_materialize_policy = auto_materialize_policy
+        self._backfill_policy = backfill_policy
 
         check.invariant(
             not (group_name_for_all_assets and group_names_by_key),
             "Cannot set both group_name_for_all_assets and group_names_by_key",
         )
         check.invariant(
             not (
@@ -345,14 +355,15 @@
         )
         return assets_def.with_attributes(
             output_asset_key_replacements=output_asset_key_replacements,
             input_asset_key_replacements=input_asset_key_replacements,
             group_names_by_key=group_names_by_key,
             freshness_policy=self._freshness_policy,
             auto_materialize_policy=self._auto_materialize_policy,
+            backfill_policy=self._backfill_policy,
         )
 
 
 class ResourceWrappedCacheableAssetsDefinition(WrappedCacheableAssetsDefinition):
     """Represents a CacheableAssetsDefinition that has been wrapped with resources."""
 
     def __init__(
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/composition.py` & `dagster-1.4.3/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/config.py` & `dagster-1.4.3/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/configurable.py` & `dagster-1.4.3/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/data_time.py` & `dagster-1.4.3/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/data_version.py` & `dagster-1.4.3/dagster/_core/definitions/data_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import functools
 from collections import OrderedDict
 from enum import Enum
 from hashlib import sha256
 from typing import (
     TYPE_CHECKING,
     Callable,
@@ -132,15 +130,15 @@
                 key_type=AssetKey,
                 value_type=DataVersion,
             ),
             is_user_provided=check.bool_param(is_user_provided, "is_user_provided"),
         )
 
     @staticmethod
-    def from_tags(tags: Mapping[str, str]) -> Optional[DataProvenance]:
+    def from_tags(tags: Mapping[str, str]) -> Optional["DataProvenance"]:
         from dagster._core.definitions.events import AssetKey
 
         code_version = tags.get(CODE_VERSION_TAG)
         if code_version is None:
             return None
         input_data_versions = {
             # Everything after the 2nd slash is the asset key
@@ -228,23 +226,23 @@
 
     hash_sig = sha256()
     hash_sig.update(bytearray("".join(all_inputs), "utf8"))
     return DataVersion(hash_sig.hexdigest())
 
 
 def extract_data_version_from_entry(
-    entry: EventLogEntry,
+    entry: "EventLogEntry",
 ) -> Optional[DataVersion]:
     tags = entry.tags or {}
     value = tags.get(DATA_VERSION_TAG) or tags.get(_OLD_DATA_VERSION_TAG)
     return None if value is None else DataVersion(value)
 
 
 def extract_data_provenance_from_entry(
-    entry: EventLogEntry,
+    entry: "EventLogEntry",
 ) -> Optional[DataProvenance]:
     tags = entry.tags or {}
     return DataProvenance.from_tags(tags)
 
 
 # ########################
 # ##### STALENESS OPERATIONS
@@ -266,18 +264,18 @@
     def __lt__(self, other: "StaleCauseCategory"):
         if self.__class__ is other.__class__:
             return self.value < other.value
         return NotImplemented
 
 
 class StaleCause(NamedTuple):
-    key: AssetKey
+    key: "AssetKey"
     category: StaleCauseCategory
     reason: str
-    dependency: Optional[AssetKey] = None
+    dependency: Optional["AssetKey"] = None
     children: Optional[Sequence["StaleCause"]] = None
 
 
 class CachingStaleStatusResolver:
     """Used to resolve data version information. Avoids redundant database
     calls that would otherwise occur. Intended for use within the scope of a
     single "request" (e.g. GQL request, RunRequest resolution).
@@ -300,50 +298,50 @@
         if isinstance(asset_graph, AssetGraph):
             self._asset_graph = asset_graph
             self._asset_graph_load_fn = None
         else:
             self._asset_graph = None
             self._asset_graph_load_fn = asset_graph
 
-    def get_status(self, key: AssetKey) -> StaleStatus:
+    def get_status(self, key: "AssetKey") -> StaleStatus:
         return self._get_status(key=key)
 
-    def get_stale_causes(self, key: AssetKey) -> Sequence[StaleCause]:
+    def get_stale_causes(self, key: "AssetKey") -> Sequence[StaleCause]:
         return self._get_stale_causes(key=key)
 
-    def get_stale_root_causes(self, key: AssetKey) -> Sequence[StaleCause]:
+    def get_stale_root_causes(self, key: "AssetKey") -> Sequence[StaleCause]:
         return self._get_stale_root_causes(key=key)
 
-    def get_current_data_version(self, key: AssetKey) -> DataVersion:
+    def get_current_data_version(self, key: "AssetKey") -> DataVersion:
         return self._get_current_data_version(key=key)
 
     @cached_method
-    def _get_status(self, key: AssetKey) -> StaleStatus:
+    def _get_status(self, key: "AssetKey") -> StaleStatus:
         current_version = self._get_current_data_version(key=key)
         if current_version == NULL_DATA_VERSION:
             return StaleStatus.MISSING
         elif self.asset_graph.is_source(key) or self._is_partitioned_or_downstream(key=key):
             return StaleStatus.FRESH
         else:
             causes = self._get_stale_causes(key=key)
             return StaleStatus.FRESH if len(causes) == 0 else StaleStatus.STALE
 
     @cached_method
-    def _get_stale_causes(self, key: AssetKey) -> Sequence[StaleCause]:
+    def _get_stale_causes(self, key: "AssetKey") -> Sequence[StaleCause]:
         current_version = self._get_current_data_version(key=key)
         if (
             current_version == NULL_DATA_VERSION
             or self.asset_graph.is_source(key)
             or self._is_partitioned_or_downstream(key=key)
         ):
             return []
         else:
             return list(self._get_stale_causes_materialized(key))
 
-    def _get_stale_causes_materialized(self, key: AssetKey) -> Iterator[StaleCause]:
+    def _get_stale_causes_materialized(self, key: "AssetKey") -> Iterator[StaleCause]:
         code_version = self.asset_graph.get_code_version(key)
         provenance = self._get_current_data_provenance(key=key)
         dependency_keys = self.asset_graph.get_parents(key)
 
         # only used if no provenance available
         materialization = check.not_none(self._get_latest_data_version_record(key=key))
         materialization_time = materialization.timestamp
@@ -425,15 +423,15 @@
                                 StaleCauseCategory.DATA,
                                 "has a new materialization",
                             )
                         ],
                     )
 
     @cached_method
-    def _get_stale_root_causes(self, key: AssetKey) -> Sequence[StaleCause]:
+    def _get_stale_root_causes(self, key: "AssetKey") -> Sequence[StaleCause]:
         causes = self._get_stale_causes(key=key)
         root_pairs = sorted([pair for cause in causes for pair in self._gather_leaves(cause)])
         # After sorting the pairs, we can drop the level and de-dup using an
         # ordered dict as an ordered set. This will give us unique root causes,
         # sorted by level.
         roots: Dict[StaleCause, None] = OrderedDict()
         for root_cause in [leaf_cause for _, leaf_cause in root_pairs]:
@@ -461,44 +459,44 @@
         from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
 
         if self._instance_queryer is None:
             self._instance_queryer = CachingInstanceQueryer(self._instance, self.asset_graph)
         return self._instance_queryer
 
     @cached_method
-    def _get_current_data_version(self, *, key: AssetKey) -> DataVersion:
+    def _get_current_data_version(self, *, key: "AssetKey") -> DataVersion:
         # Currently we can only use asset records, which are fetched in one shot, for non-source
         # assets. This is because the most recent AssetObservation is not stored on the AssetRecord.
         record = self._get_latest_data_version_record(key=key)
         if self.asset_graph.is_source(key) and record is None:
             return DEFAULT_DATA_VERSION
         elif record is None:
             return NULL_DATA_VERSION
         else:
             data_version = extract_data_version_from_entry(record.event_log_entry)
             return data_version or DEFAULT_DATA_VERSION
 
     @cached_method
-    def _is_current_data_version_user_provided(self, *, key: AssetKey) -> bool:
+    def _is_current_data_version_user_provided(self, *, key: "AssetKey") -> bool:
         if self.asset_graph.is_source(key):
             return True
         else:
             provenance = self._get_current_data_provenance(key=key)
             return provenance is not None and provenance.is_user_provided
 
     @cached_method
-    def _get_current_data_provenance(self, *, key: AssetKey) -> Optional[DataProvenance]:
+    def _get_current_data_provenance(self, *, key: "AssetKey") -> Optional[DataProvenance]:
         record = self._get_latest_data_version_record(key=key)
         if record is None:
             return None
         else:
             return extract_data_provenance_from_entry(record.event_log_entry)
 
     @cached_method
-    def _is_partitioned_or_downstream(self, *, key: AssetKey) -> bool:
+    def _is_partitioned_or_downstream(self, *, key: "AssetKey") -> bool:
         if self.asset_graph.get_partitions_def(key):
             return True
         elif self.asset_graph.is_source(key):
             return False
         else:
             return any(
                 self._is_partitioned_or_downstream(key=dep_key)
@@ -506,34 +504,34 @@
             )
 
     # Volatility means that an asset is assumed to be constantly changing. We assume that observable
     # source assets are non-volatile, since the primary purpose of the observation function is to
     # determine if a source asset has changed. We assume that regular assets are volatile if they
     # are at the root of the graph (have no dependencies) or are downstream of a volatile asset.
     @cached_method
-    def _is_volatile(self, *, key: AssetKey) -> bool:
+    def _is_volatile(self, *, key: "AssetKey") -> bool:
         if self.asset_graph.is_source(key):
             return self.asset_graph.is_observable(key)
         else:
             deps = self.asset_graph.get_parents(key)
             return len(deps) == 0 or any(self._is_volatile(key=dep_key) for dep_key in deps)
 
     @cached_method
     def _get_latest_data_version_event(
-        self, *, key: AssetKey
+        self, *, key: "AssetKey"
     ) -> Optional[Union["AssetMaterialization", "AssetObservation"]]:
         record = self._get_latest_data_version_record(key=key)
         if record:
             entry = record.event_log_entry
             return entry.asset_materialization or entry.asset_observation
         else:
             return None
 
     @cached_method
-    def _get_latest_data_version_record(self, key: AssetKey) -> Optional["EventLogRecord"]:
+    def _get_latest_data_version_record(self, key: "AssetKey") -> Optional["EventLogRecord"]:
         from dagster._core.definitions.events import AssetKeyPartitionKey
 
         # If an asset record is cached, all of its ancestors have already been cached.
         if not self.asset_graph.is_source(
             key
         ) and not self.instance_queryer.has_cached_asset_record(key):
             ancestors = self.asset_graph.get_ancestors(key, include_self=True)
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     deprecation_warning,
     experimental_arg_warning,
 )
 
 from ..asset_in import AssetIn
 from ..asset_out import AssetOut
 from ..assets import AssetsDefinition
+from ..backfill_policy import BackfillPolicy, BackfillPolicyType
 from ..decorators.graph_decorator import graph
 from ..decorators.op_decorator import _Op
 from ..events import AssetKey, CoercibleToAssetKey, CoercibleToAssetKeyPrefix
 from ..input import In
 from ..output import GraphOut, Out
 from ..partition import PartitionsDefinition
 from ..policy import RetryPolicy
@@ -73,14 +74,15 @@
     dagster_type: Optional[DagsterType] = ...,
     partitions_def: Optional[PartitionsDefinition] = ...,
     op_tags: Optional[Mapping[str, Any]] = ...,
     group_name: Optional[str] = ...,
     output_required: bool = ...,
     freshness_policy: Optional[FreshnessPolicy] = ...,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = ...,
+    backfill_policy: Optional[BackfillPolicy] = ...,
     retry_policy: Optional[RetryPolicy] = ...,
     code_version: Optional[str] = ...,
     key: Optional[CoercibleToAssetKey] = None,
     non_argument_deps: Optional[Union[Set[AssetKey], Set[str]]] = ...,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     ...
 
@@ -103,14 +105,15 @@
     dagster_type: Optional[DagsterType] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     op_tags: Optional[Mapping[str, Any]] = None,
     group_name: Optional[str] = None,
     output_required: bool = True,
     freshness_policy: Optional[FreshnessPolicy] = None,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+    backfill_policy: Optional[BackfillPolicy] = None,
     retry_policy: Optional[RetryPolicy] = None,
     code_version: Optional[str] = None,
     key: Optional[CoercibleToAssetKey] = None,
     non_argument_deps: Optional[Union[Set[AssetKey], Set[str]]] = None,
 ) -> Union[AssetsDefinition, Callable[[Callable[..., Any]], AssetsDefinition]]:
     """Create a definition for how to compute an asset.
 
@@ -169,14 +172,16 @@
         output_required (bool): Whether the decorated function will always materialize an asset.
             Defaults to True. If False, the function can return None, which will not be materialized to
             storage and will halt execution of downstream assets.
         freshness_policy (FreshnessPolicy): A constraint telling Dagster how often this asset is intended to be updated
             with respect to its root data.
         auto_materialize_policy (AutoMaterializePolicy): (Experimental) Configure Dagster to automatically materialize
             this asset according to its FreshnessPolicy and when upstream dependencies change.
+        backfill_policy (BackfillPolicy): (Experimental) Configure Dagster to backfill this asset according to its
+            BackfillPolicy.
         retry_policy (Optional[RetryPolicy]): The retry policy for the op that computes the asset.
         code_version (Optional[str]): (Experimental) Version of the code that generates this asset. In
             general, versions should be set only for code that deterministically produces the same
             output when given the same inputs.
         non_argument_deps (Optional[Union[Set[AssetKey], Set[str]]]): Deprecated, use deps instead.
             Set of asset keys that are upstream dependencies, but do not pass an input to the asset.
 
@@ -209,14 +214,15 @@
             dagster_type=dagster_type,
             partitions_def=partitions_def,
             op_tags=op_tags,
             group_name=group_name,
             output_required=output_required,
             freshness_policy=freshness_policy,
             auto_materialize_policy=auto_materialize_policy,
+            backfill_policy=backfill_policy,
             retry_policy=retry_policy,
             code_version=code_version,
             key=key,
         )
 
     if compute_fn is not None:
         return create_asset()(compute_fn)
@@ -234,14 +240,17 @@
 
         if io_manager_def is not None:
             experimental_arg_warning("io_manager_def", "asset")
 
         if auto_materialize_policy is not None:
             experimental_arg_warning("auto_materialize_policy", "asset")
 
+        if backfill_policy is not None:
+            experimental_arg_warning("backfill_policy", "asset")
+
         return create_asset()(fn)
 
     return inner
 
 
 class _Asset:
     def __init__(
@@ -261,14 +270,15 @@
         dagster_type: Optional[DagsterType] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         op_tags: Optional[Mapping[str, Any]] = None,
         group_name: Optional[str] = None,
         output_required: bool = True,
         freshness_policy: Optional[FreshnessPolicy] = None,
         auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
         retry_policy: Optional[RetryPolicy] = None,
         code_version: Optional[str] = None,
         key: Optional[CoercibleToAssetKey] = None,
     ):
         self.name = name
 
         if isinstance(key_prefix, str):
@@ -290,14 +300,15 @@
         self.op_tags = op_tags
         self.resource_defs = dict(check.opt_mapping_param(resource_defs, "resource_defs"))
         self.group_name = group_name
         self.output_required = output_required
         self.freshness_policy = freshness_policy
         self.retry_policy = retry_policy
         self.auto_materialize_policy = auto_materialize_policy
+        self.backfill_policy = backfill_policy
         self.code_version = code_version
 
         if (name or key_prefix) and key:
             raise DagsterInvalidDefinitionError(
                 "Cannot specify a name or key prefix for an asset when the key argument is"
                 " provided."
             )
@@ -383,14 +394,24 @@
                     **(self.op_tags or {}),
                 },
                 config_schema=self.config_schema,
                 retry_policy=self.retry_policy,
                 code_version=self.code_version,
             )(fn)
 
+            # check backfill policy is BackfillPolicyType.SINGLE_RUN for non-partitioned asset
+            if self.partitions_def is None:
+                check.param_invariant(
+                    self.backfill_policy.policy_type is BackfillPolicyType.SINGLE_RUN
+                    if self.backfill_policy
+                    else True,
+                    "backfill_policy",
+                    "Non partitioned asset can only have single run backfill policy",
+                )
+
         keys_by_input_name = {
             input_name: asset_key for asset_key, (input_name, _) in asset_ins.items()
         }
         partition_mappings = {
             keys_by_input_name[input_name]: asset_in.partition_mapping
             for input_name, asset_in in self.ins.items()
             if asset_in.partition_mapping is not None
@@ -406,14 +427,15 @@
             group_names_by_key={out_asset_key: self.group_name} if self.group_name else None,
             freshness_policies_by_key={out_asset_key: self.freshness_policy}
             if self.freshness_policy
             else None,
             auto_materialize_policies_by_key={out_asset_key: self.auto_materialize_policy}
             if self.auto_materialize_policy
             else None,
+            backfill_policy=self.backfill_policy,
             asset_deps=None,  # no asset deps in single-asset decorator
             selected_asset_keys=None,  # no subselection in decorator
             can_subset=False,
             metadata_by_key={out_asset_key: self.metadata} if self.metadata else None,
             descriptions_by_key=None,  # not supported for now
         )
 
@@ -426,14 +448,15 @@
     deps: Optional[Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]]] = None,
     description: Optional[str] = None,
     config_schema: Optional[UserConfigSchema] = None,
     required_resource_keys: Optional[Set[str]] = None,
     compute_kind: Optional[str] = None,
     internal_asset_deps: Optional[Mapping[str, Set[AssetKey]]] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
+    backfill_policy: Optional[BackfillPolicy] = None,
     op_tags: Optional[Mapping[str, Any]] = None,
     can_subset: bool = False,
     resource_defs: Optional[Mapping[str, object]] = None,
     group_name: Optional[str] = None,
     retry_policy: Optional[RetryPolicy] = None,
     code_version: Optional[str] = None,
     non_argument_deps: Optional[Union[Set[AssetKey], Set[str]]] = None,
@@ -465,14 +488,15 @@
         internal_asset_deps (Optional[Mapping[str, Set[AssetKey]]]): By default, it is assumed
             that all assets produced by a multi_asset depend on all assets that are consumed by that
             multi asset. If this default is not correct, you pass in a map of output names to a
             corrected set of AssetKeys that they depend on. Any AssetKeys in this list must be either
             used as input to the asset or produced within the op.
         partitions_def (Optional[PartitionsDefinition]): Defines the set of partition keys that
             compose the assets.
+        backfill_policy (Optional[BackfillPolicy]): The backfill policy for the op that computes the asset.
         op_tags (Optional[Dict[str, Any]]): A dictionary of tags for the op that computes the asset.
             Frameworks may expect and require certain metadata to be attached to a op. Values that
             are not strings will be json encoded and must meet the criteria that
             `json.loads(json.dumps(value)) == value`.
         can_subset (bool): If this asset's computation can emit a subset of the asset
             keys based on the context.selected_assets argument. Defaults to False.
         resource_defs (Optional[Mapping[str, object]]):
@@ -632,14 +656,15 @@
             if out.freshness_policy is not None
         }
         auto_materialize_policies_by_key = {
             keys_by_output_name[output_name]: out.auto_materialize_policy
             for output_name, out in outs.items()
             if out.auto_materialize_policy is not None
         }
+
         partition_mappings = {
             keys_by_input_name[input_name]: asset_in.partition_mapping
             for input_name, asset_in in (ins or {}).items()
             if asset_in.partition_mapping is not None
         }
         metadata_by_key = {
             keys_by_output_name[output_name]: out.metadata
@@ -655,14 +680,15 @@
             partitions_def=partitions_def,
             partition_mappings=partition_mappings if partition_mappings else None,
             can_subset=can_subset,
             resource_defs=resource_defs,
             group_names_by_key=group_names_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
             auto_materialize_policies_by_key=auto_materialize_policies_by_key,
+            backfill_policy=backfill_policy,
             selected_asset_keys=None,  # no subselection in decorator
             descriptions_by_key=None,  # not supported for now
             metadata_by_key=metadata_by_key,
         )
 
     return inner
 
@@ -752,14 +778,15 @@
     ins: Optional[Mapping[str, AssetIn]] = None,
     description: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     group_name: Optional[str] = None,
     metadata: Optional[MetadataUserInput] = ...,
     freshness_policy: Optional[FreshnessPolicy] = ...,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = ...,
+    backfill_policy: Optional[BackfillPolicy] = ...,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     ...
 
 
 def graph_asset(
     compose_fn: Optional[Callable] = None,
     *,
@@ -768,14 +795,15 @@
     ins: Optional[Mapping[str, AssetIn]] = None,
     description: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     group_name: Optional[str] = None,
     metadata: Optional[MetadataUserInput] = None,
     freshness_policy: Optional[FreshnessPolicy] = None,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+    backfill_policy: Optional[BackfillPolicy] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
 ) -> Union[AssetsDefinition, Callable[[Callable[..., Any]], AssetsDefinition]]:
     """Creates a software-defined asset that's computed using a graph of ops.
 
     This decorator is meant to decorate a function that composes a set of ops or graphs to define
     the dependencies between them.
 
@@ -795,14 +823,15 @@
             not provided, the name "default" is used.
         metadata (Optional[MetadataUserInput]): Dictionary of metadata to be associated with
             the asset.
         freshness_policy (Optional[FreshnessPolicy]): A constraint telling Dagster how often this asset is
             intended to be updated with respect to its root data.
         auto_materialize_policy (Optional[AutoMaterializePolicy]): The AutoMaterializePolicy to use
             for this asset.
+        backfill_policy (Optional[BackfillPolicy]): The BackfillPolicy to use for this asset.
 
     Examples:
         .. code-block:: python
 
             @op
             def fetch_files_from_slack(context) -> pd.DataFrame:
                 ...
@@ -825,14 +854,15 @@
             ins=ins,
             description=description,
             partitions_def=partitions_def,
             group_name=group_name,
             metadata=metadata,
             freshness_policy=freshness_policy,
             auto_materialize_policy=auto_materialize_policy,
+            backfill_policy=backfill_policy,
             resource_defs=resource_defs,
         )(fn)
 
     return inner
 
 
 class _GraphBackedAsset:
@@ -843,28 +873,30 @@
         ins: Optional[Mapping[str, AssetIn]] = None,
         description: Optional[str] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         group_name: Optional[str] = None,
         metadata: Optional[MetadataUserInput] = None,
         freshness_policy: Optional[FreshnessPolicy] = None,
         auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
     ):
         self.name = name
 
         if isinstance(key_prefix, str):
             key_prefix = [key_prefix]
         self.key_prefix = key_prefix
         self.ins = ins or {}
         self.description = description
         self.partitions_def = partitions_def
         self.group_name = group_name
         self.metadata = metadata
         self.freshness_policy = freshness_policy
         self.auto_materialize_policy = auto_materialize_policy
+        self.backfill_policy = backfill_policy
         self.resource_defs = resource_defs
 
     def __call__(self, fn: Callable) -> AssetsDefinition:
         asset_name = self.name or fn.__name__
         asset_ins = build_asset_ins(fn, self.ins or {}, set())
         out_asset_key = AssetKey(list(filter(None, [*(self.key_prefix or []), asset_name])))
 
@@ -890,25 +922,27 @@
             metadata_by_output_name={"result": self.metadata} if self.metadata else None,
             freshness_policies_by_output_name={"result": self.freshness_policy}
             if self.freshness_policy
             else None,
             auto_materialize_policies_by_output_name={"result": self.auto_materialize_policy}
             if self.auto_materialize_policy
             else None,
+            backfill_policy=self.backfill_policy,
             descriptions_by_output_name={"result": self.description} if self.description else None,
             resource_defs=self.resource_defs,
         )
 
 
 def graph_multi_asset(
     *,
     outs: Mapping[str, AssetOut],
     name: Optional[str] = None,
     ins: Optional[Mapping[str, AssetIn]] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
+    backfill_policy: Optional[BackfillPolicy] = None,
     group_name: Optional[str] = None,
     can_subset: bool = False,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     """Create a combined definition of multiple assets that are computed using the same graph of
     ops, and the same upstream assets.
 
@@ -918,14 +952,15 @@
     Args:
         name (Optional[str]): The name of the graph.
         outs: (Optional[Dict[str, AssetOut]]): The AssetOuts representing the produced assets.
         ins (Optional[Mapping[str, AssetIn]]): A dictionary that maps input names to information
             about the input.
         partitions_def (Optional[PartitionsDefinition]): Defines the set of partition keys that
             compose the assets.
+        backfill_policy (Optional[BackfillPolicy]): The backfill policy for the asset.
         group_name (Optional[str]): A string name used to organize multiple assets into groups. This
             group name will be applied to all assets produced by this multi_asset.
         can_subset (bool): Whether this asset's computation can emit a subset of the asset
             keys based on the context.selected_assets argument. Defaults to False.
     """
 
     def inner(fn: Callable) -> AssetsDefinition:
@@ -982,14 +1017,15 @@
             partitions_def=partitions_def,
             partition_mappings=partition_mappings if partition_mappings else None,
             group_name=group_name,
             can_subset=can_subset,
             metadata_by_output_name=metadata_by_output_name,
             freshness_policies_by_output_name=freshness_policies_by_output_name,
             auto_materialize_policies_by_output_name=auto_materialize_policies_by_output_name,
+            backfill_policy=backfill_policy,
             descriptions_by_output_name=descriptions_by_output_name,
             resource_defs=resource_defs,
         )
 
     return inner
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import copy
 from functools import update_wrapper
 from typing import (
-    TYPE_CHECKING,
     Callable,
     List,
     Mapping,
     Optional,
     Sequence,
     Set,
     Union,
@@ -34,17 +33,14 @@
     ScheduleEvaluationContext,
     has_at_least_one_parameter,
     validate_and_get_schedule_resource_dict,
 )
 from ..target import ExecutableDefinition
 from ..utils import validate_tags
 
-if TYPE_CHECKING:
-    pass
-
 
 def schedule(
     cron_schedule: Union[str, Sequence[str]],
     *,
     job_name: Optional[str] = None,
     name: Optional[str] = None,
     tags: Optional[Mapping[str, str]] = None,
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.4.3/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.4.3/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/definitions_class.py` & `dagster-1.4.3/dagster/_core/definitions/definitions_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import (
     TYPE_CHECKING,
     Any,
+    Dict,
     Iterable,
     List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Type,
@@ -172,15 +173,27 @@
         and (
             job.is_missing_required_resources() or _io_manager_needs_replacement(job, resource_defs)
         )
     ]
 
     # Create a mapping of job id to a version of the job with the resource defs bound
     unsatisfied_job_to_resource_bound_job = {
-        id(job): job.with_top_level_resources(resource_defs)
+        id(job): job.with_top_level_resources(
+            {
+                **resource_defs,
+                **job.resource_defs,
+                # special case for IO manager - the job-level IO manager does not take precedence
+                # if it is the default and a top-level IO manager is provided
+                **(
+                    {"io_manager": resource_defs["io_manager"]}
+                    if _io_manager_needs_replacement(job, resource_defs)
+                    else {}
+                ),
+            }
+        )
         for job in jobs
         if job in unsatisfied_jobs
     }
 
     # Update all jobs to use the resource bound version
     jobs_with_resources = [
         unsatisfied_job_to_resource_bound_job[id(job)] if job in unsatisfied_jobs else job
@@ -428,37 +441,41 @@
     def load_asset_value(
         self,
         asset_key: CoercibleToAssetKey,
         *,
         python_type: Optional[Type] = None,
         instance: Optional[DagsterInstance] = None,
         partition_key: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
     ) -> object:
         """Load the contents of an asset as a Python object.
 
         Invokes `load_input` on the :py:class:`IOManager` associated with the asset.
 
         If you want to load the values of multiple assets, it's more efficient to use
         :py:meth:`~dagster.Definitions.get_asset_value_loader`, which avoids spinning up
         resources separately for each asset.
 
         Args:
             asset_key (Union[AssetKey, Sequence[str], str]): The key of the asset to load.
             python_type (Optional[Type]): The python type to load the asset as. This is what will
                 be returned inside `load_input` by `context.dagster_type.typing_type`.
             partition_key (Optional[str]): The partition of the asset to load.
+            metadata (Optional[Dict[str, Any]]): Input metadata to pass to the :py:class:`IOManager`
+                (is equivalent to setting the metadata argument in `In` or `AssetIn`).
 
         Returns:
             The contents of an asset as a Python object.
         """
         return self.get_repository_def().load_asset_value(
             asset_key=asset_key,
             python_type=python_type,
             instance=instance,
             partition_key=partition_key,
+            metadata=metadata,
         )
 
     @public
     def get_asset_value_loader(
         self, instance: Optional[DagsterInstance] = None
     ) -> "AssetValueLoader":
         """Returns an object that can load the contents of assets as Python objects.
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/dependency.py` & `dagster-1.4.3/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/events.py` & `dagster-1.4.3/dagster/_core/definitions/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,24 +272,27 @@
     @property
     def metadata(self) -> MetadataMapping:
         return self._metadata
 
     @public
     @property
     def value(self) -> Any:
+        """Any: The value returned by the compute function."""
         return self._value
 
     @public
     @property
     def output_name(self) -> str:
+        """str: Name of the corresponding :py:class:`Out`."""
         return self._output_name
 
     @public
     @property
     def data_version(self) -> Optional[DataVersion]:
+        """Optional[DataVersion]: A data version that was manually set on the `Output`."""
         return self._data_version
 
     def __eq__(self, other: object) -> bool:
         return (
             isinstance(other, Output)
             and self.value == other.value
             and self.output_name == other.output_name
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/executor_definition.py` & `dagster-1.4.3/dagster/_core/definitions/executor_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING, Any, Callable, Dict, Mapping, Optional, Sequence, Union, overload
 
 from typing_extensions import Self, TypeAlias
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._builtins import Int
-from dagster._config import Field, Selector, UserConfigSchema
+from dagster._config import Field, Noneable, Selector, UserConfigSchema
 from dagster._core.definitions.configurable import (
     ConfiguredDefinitionConfigSchema,
     NamedConfigurableDefinition,
 )
 from dagster._core.definitions.job_base import IJob
 from dagster._core.definitions.reconstruct import ReconstructableJob
 from dagster._core.errors import DagsterUnmetExecutorRequirementsError
@@ -331,27 +331,27 @@
     start_method = None
     start_cfg: Dict[str, object] = {}
     start_selector = check.opt_dict_elem(config, "start_method")
     if start_selector:
         start_method, start_cfg = list(start_selector.items())[0]
 
     return MultiprocessExecutor(
-        max_concurrent=check.int_elem(config, "max_concurrent"),
+        max_concurrent=check.opt_int_elem(config, "max_concurrent"),
         tag_concurrency_limits=check.opt_list_elem(config, "tag_concurrency_limits"),
         retries=RetryMode.from_config(check.dict_elem(config, "retries")),  # type: ignore
         start_method=start_method,
         explicit_forkserver_preload=check.opt_list_elem(start_cfg, "preload_modules", of_type=str),
     )
 
 
 MULTI_PROC_CONFIG = Field(
     {
         "max_concurrent": Field(
-            Int,
-            default_value=0,
+            Noneable(Int),
+            default_value=None,
             description=(
                 "The number of processes that may run concurrently. "
                 "By default, this is set to be the return value of `multiprocessing.cpu_count()`."
             ),
         ),
         "tag_concurrency_limits": get_tag_concurrency_limits_config(),
         "start_method": Field(
@@ -414,15 +414,15 @@
 
         execution:
           config:
             multiprocess:
               max_concurrent: 4
 
     The ``max_concurrent`` arg is optional and tells the execution engine how many processes may run
-    concurrently. By default, or if you set ``max_concurrent`` to be 0, this is the return value of
+    concurrently. By default, or if you set ``max_concurrent`` to be None or 0, this is the return value of
     :py:func:`python:multiprocessing.cpu_count`.
 
     Execution priority can be configured using the ``dagster/priority`` tag via op metadata,
     where the higher the number the higher the priority. 0 is the default and both positive
     and negative numbers can be used.
     """
     return _core_multiprocess_executor_creation(init_context.executor_config)
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.4.3/dagster/_core/definitions/external_asset_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.host_representation.external import ExternalRepository
 from dagster._core.host_representation.handle import RepositoryHandle
 from dagster._core.selector.subset_selector import DependencyGraph
 from dagster._core.workspace.workspace import IWorkspace
 
 from .asset_graph import AssetGraph
+from .backfill_policy import BackfillPolicy
 from .events import AssetKey
 from .freshness_policy import FreshnessPolicy
 from .partition import PartitionsDefinition
 from .partition_mapping import PartitionMapping
 
 if TYPE_CHECKING:
     from dagster._core.host_representation.external_data import ExternalAssetNode
@@ -35,14 +36,15 @@
         asset_dep_graph: DependencyGraph[AssetKey],
         source_asset_keys: AbstractSet[AssetKey],
         partitions_defs_by_key: Mapping[AssetKey, Optional[PartitionsDefinition]],
         partition_mappings_by_key: Mapping[AssetKey, Optional[Mapping[AssetKey, PartitionMapping]]],
         group_names_by_key: Mapping[AssetKey, Optional[str]],
         freshness_policies_by_key: Mapping[AssetKey, Optional[FreshnessPolicy]],
         auto_materialize_policies_by_key: Mapping[AssetKey, Optional[AutoMaterializePolicy]],
+        backfill_policies_by_key: Mapping[AssetKey, Optional[BackfillPolicy]],
         required_multi_asset_sets_by_key: Optional[Mapping[AssetKey, AbstractSet[AssetKey]]],
         repo_handles_by_key: Mapping[AssetKey, RepositoryHandle],
         job_names_by_key: Mapping[AssetKey, Sequence[str]],
         code_versions_by_key: Mapping[AssetKey, Optional[str]],
         is_observable_by_key: Mapping[AssetKey, bool],
         auto_observe_interval_minutes_by_key: Mapping[AssetKey, Optional[float]],
     ):
@@ -50,14 +52,15 @@
             asset_dep_graph=asset_dep_graph,
             source_asset_keys=source_asset_keys,
             partitions_defs_by_key=partitions_defs_by_key,
             partition_mappings_by_key=partition_mappings_by_key,
             group_names_by_key=group_names_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
             auto_materialize_policies_by_key=auto_materialize_policies_by_key,
+            backfill_policies_by_key=backfill_policies_by_key,
             required_multi_asset_sets_by_key=required_multi_asset_sets_by_key,
             code_versions_by_key=code_versions_by_key,
             is_observable_by_key=is_observable_by_key,
             auto_observe_interval_minutes_by_key=auto_observe_interval_minutes_by_key,
         )
         self._repo_handles_by_key = repo_handles_by_key
         self._materialization_job_names_by_key = job_names_by_key
@@ -110,14 +113,15 @@
         partitions_defs_by_key: Dict[AssetKey, Optional[PartitionsDefinition]] = {}
         partition_mappings_by_key: Dict[AssetKey, Dict[AssetKey, PartitionMapping]] = defaultdict(
             defaultdict
         )
         group_names_by_key = {}
         freshness_policies_by_key = {}
         auto_materialize_policies_by_key = {}
+        backfill_policies_by_key = {}
         asset_keys_by_atomic_execution_unit_id: Dict[str, Set[AssetKey]] = defaultdict(set)
         repo_handles_by_key = {
             node.asset_key: repo_handle
             for repo_handle, node in repo_handle_external_asset_nodes
             if not node.is_source or node.is_observable
         }
         job_names_by_key = {
@@ -163,14 +167,15 @@
                 node.partitions_def_data.get_partitions_definition()
                 if node.partitions_def_data
                 else None
             )
             group_names_by_key[node.asset_key] = node.group_name
             freshness_policies_by_key[node.asset_key] = node.freshness_policy
             auto_materialize_policies_by_key[node.asset_key] = node.auto_materialize_policy
+            backfill_policies_by_key[node.asset_key] = node.backfill_policy
 
             if node.atomic_execution_unit_id is not None:
                 asset_keys_by_atomic_execution_unit_id[node.atomic_execution_unit_id].add(
                     node.asset_key
                 )
 
         downstream: Dict[AssetKey, Set[AssetKey]] = defaultdict(set)
@@ -188,14 +193,15 @@
             asset_dep_graph={"upstream": upstream, "downstream": downstream},
             source_asset_keys=source_asset_keys,
             partitions_defs_by_key=partitions_defs_by_key,
             partition_mappings_by_key=partition_mappings_by_key,
             group_names_by_key=group_names_by_key,
             freshness_policies_by_key=freshness_policies_by_key,
             auto_materialize_policies_by_key=auto_materialize_policies_by_key,
+            backfill_policies_by_key=backfill_policies_by_key,
             required_multi_asset_sets_by_key=required_multi_asset_sets_by_key,
             repo_handles_by_key=repo_handles_by_key,
             job_names_by_key=job_names_by_key,
             code_versions_by_key=code_versions_by_key,
             is_observable_by_key=is_observable_by_key,
             auto_observe_interval_minutes_by_key=auto_observe_interval_minutes_by_key,
         )
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/freshness_based_auto_materialize.py` & `dagster-1.4.3/dagster/_core/definitions/freshness_based_auto_materialize.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,31 +5,33 @@
     just the current data time of the asset.
 - execution_period: The range of times in which it would be acceptable to materialize this asset,
     i.e. it`s late enough to pull in the required data time, and early enough to not go over the
     maximum lag minutes.
 """
 import datetime
 from collections import defaultdict
-from typing import AbstractSet, Dict, Mapping, Optional, Set, Tuple, cast
+from typing import TYPE_CHECKING, AbstractSet, Dict, Mapping, Optional, Set, Tuple, cast
 
 import pendulum
 
-from dagster._core.definitions.data_time import CachingDataTimeResolver
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._utils.schedules import cron_string_iterator
 
 from .asset_graph import AssetGraph
 from .auto_materialize_condition import (
     AutoMaterializeCondition,
     AutoMaterializeDecisionType,
     DownstreamFreshnessAutoMaterializeCondition,
     FreshnessAutoMaterializeCondition,
 )
 
+if TYPE_CHECKING:
+    from dagster._core.definitions.data_time import CachingDataTimeResolver
+
 
 def get_execution_period_for_policy(
     freshness_policy: FreshnessPolicy,
     effective_data_time: Optional[datetime.datetime],
     current_time: datetime.datetime,
 ) -> pendulum.Period:
     if freshness_policy.cron_schedule:
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/freshness_policy.py` & `dagster-1.4.3/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.4.3/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Callable, Dict, Mapping, NamedTuple, Optional, Set, cast
+from typing import Callable, Dict, Mapping, NamedTuple, Optional, Set, cast
 
 import pendulum
 
 import dagster._check as check
 from dagster._annotations import PublicAttr, experimental
 from dagster._core.definitions.asset_selection import AssetSelection
 from dagster._core.definitions.data_time import CachingDataTimeResolver
@@ -32,17 +32,14 @@
     SensorType,
     SkipReason,
     get_context_param_name,
     get_sensor_context_from_args_or_kwargs,
     validate_and_get_resource_dict,
 )
 
-if TYPE_CHECKING:
-    pass
-
 
 @whitelist_for_serdes
 class FreshnessPolicySensorCursor(
     NamedTuple(
         "_FreshnessPolicySensorCursor",
         [("minutes_late_by_key_str", Mapping[str, Optional[float]])],
     )
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/graph_definition.py` & `dagster-1.4.3/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/hook_definition.py` & `dagster-1.4.3/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/hook_invocation.py` & `dagster-1.4.3/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/inference.py` & `dagster-1.4.3/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/input.py` & `dagster-1.4.3/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/instigation_logger.py` & `dagster-1.4.3/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/job_base.py` & `dagster-1.4.3/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/job_definition.py` & `dagster-1.4.3/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.4.3/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pkgutil
 from importlib import import_module
 from types import ModuleType
 from typing import Dict, Generator, Iterable, List, Optional, Sequence, Set, Tuple, Union
 
 import dagster._check as check
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
+from dagster._core.definitions.backfill_policy import BackfillPolicy
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.errors import DagsterInvalidDefinitionError
 
 from .assets import AssetsDefinition
 from .cacheable_assets import CacheableAssetsDefinition
 from .events import (
     AssetKey,
@@ -98,14 +99,15 @@
 def load_assets_from_modules(
     modules: Iterable[ModuleType],
     group_name: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     *,
     freshness_policy: Optional[FreshnessPolicy] = None,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+    backfill_policy: Optional[BackfillPolicy] = None,
     source_key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
 ) -> Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
     """Constructs a list of assets and source assets from the given modules.
 
     Args:
         modules (Iterable[ModuleType]): The Python modules to look for assets inside.
         group_name (Optional[str]):
@@ -114,27 +116,29 @@
         key_prefix (Optional[Union[str, Sequence[str]]]):
             Prefix to prepend to the keys of the loaded assets. The returned assets will be copies
             of the loaded objects, with the prefix prepended.
         freshness_policy (Optional[FreshnessPolicy]): FreshnessPolicy to apply to all the loaded
             assets.
         auto_materialize_policy (Optional[AutoMaterializePolicy]): AutoMaterializePolicy to apply
             to all the loaded assets.
+        backfill_policy (Optional[AutoMaterializePolicy]): BackfillPolicy to apply to all the loaded assets.
         source_key_prefix (bool): Prefix to prepend to the keys of loaded SourceAssets. The returned
             assets will be copies of the loaded objects, with the prefix prepended.
 
     Returns:
         Sequence[Union[AssetsDefinition, SourceAsset]]:
             A list containing assets and source assets defined in the given modules.
     """
     group_name = check.opt_str_param(group_name, "group_name")
     key_prefix = check_opt_coercible_to_asset_key_prefix_param(key_prefix, "key_prefix")
     freshness_policy = check.opt_inst_param(freshness_policy, "freshness_policy", FreshnessPolicy)
     auto_materialize_policy = check.opt_inst_param(
         auto_materialize_policy, "auto_materialize_policy", AutoMaterializePolicy
     )
+    backfill_policy = check.opt_inst_param(backfill_policy, "backfill_policy", BackfillPolicy)
 
     (
         assets,
         source_assets,
         cacheable_assets,
     ) = assets_from_modules(modules)
 
@@ -142,24 +146,26 @@
         assets,
         source_assets,
         cacheable_assets,
         key_prefix=key_prefix,
         group_name=group_name,
         freshness_policy=freshness_policy,
         auto_materialize_policy=auto_materialize_policy,
+        backfill_policy=backfill_policy,
         source_key_prefix=source_key_prefix,
     )
 
 
 def load_assets_from_current_module(
     group_name: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     *,
     freshness_policy: Optional[FreshnessPolicy] = None,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+    backfill_policy: Optional[BackfillPolicy] = None,
     source_key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
 ) -> Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
     """Constructs a list of assets, source assets, and cacheable assets from the module where
     this function is called.
 
     Args:
         group_name (Optional[str]):
@@ -168,14 +174,15 @@
         key_prefix (Optional[Union[str, Sequence[str]]]):
             Prefix to prepend to the keys of the loaded assets. The returned assets will be copies
             of the loaded objects, with the prefix prepended.
         freshness_policy (Optional[FreshnessPolicy]): FreshnessPolicy to apply to all the loaded
             assets.
         auto_materialize_policy (Optional[AutoMaterializePolicy]): AutoMaterializePolicy to apply
             to all the loaded assets.
+        backfill_policy (Optional[AutoMaterializePolicy]): BackfillPolicy to apply to all the loaded assets.
         source_key_prefix (bool): Prefix to prepend to the keys of loaded SourceAssets. The returned
             assets will be copies of the loaded objects, with the prefix prepended.
 
     Returns:
         Sequence[Union[AssetsDefinition, SourceAsset, CachableAssetsDefinition]]:
             A list containing assets, source assets, and cacheable assets defined in the module.
     """
@@ -186,14 +193,15 @@
 
     return load_assets_from_modules(
         [module],
         group_name=group_name,
         key_prefix=key_prefix,
         freshness_policy=freshness_policy,
         auto_materialize_policy=auto_materialize_policy,
+        backfill_policy=backfill_policy,
     )
 
 
 def assets_from_package_module(
     package_module: ModuleType,
     extra_source_assets: Optional[Sequence[SourceAsset]] = None,
 ) -> Tuple[Sequence[AssetsDefinition], Sequence[SourceAsset], Sequence[CacheableAssetsDefinition]]:
@@ -218,14 +226,15 @@
 def load_assets_from_package_module(
     package_module: ModuleType,
     group_name: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     *,
     freshness_policy: Optional[FreshnessPolicy] = None,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+    backfill_policy: Optional[BackfillPolicy] = None,
     source_key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
 ) -> Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
     """Constructs a list of assets and source assets that includes all asset
     definitions, source assets, and cacheable assets in all sub-modules of the given package module.
 
     A package module is the result of importing a package.
 
@@ -237,52 +246,56 @@
         key_prefix (Optional[Union[str, Sequence[str]]]):
             Prefix to prepend to the keys of the loaded assets. The returned assets will be copies
             of the loaded objects, with the prefix prepended.
         freshness_policy (Optional[FreshnessPolicy]): FreshnessPolicy to apply to all the loaded
             assets.
         auto_materialize_policy (Optional[AutoMaterializePolicy]): AutoMaterializePolicy to apply
             to all the loaded assets.
+        backfill_policy (Optional[AutoMaterializePolicy]): BackfillPolicy to apply to all the loaded assets.
         source_key_prefix (bool): Prefix to prepend to the keys of loaded SourceAssets. The returned
             assets will be copies of the loaded objects, with the prefix prepended.
 
     Returns:
         Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
             A list containing assets, source assets, and cacheable assets defined in the module.
     """
     group_name = check.opt_str_param(group_name, "group_name")
     key_prefix = check_opt_coercible_to_asset_key_prefix_param(key_prefix, "key_prefix")
     freshness_policy = check.opt_inst_param(freshness_policy, "freshness_policy", FreshnessPolicy)
     auto_materialize_policy = check.opt_inst_param(
         auto_materialize_policy, "auto_materialize_policy", AutoMaterializePolicy
     )
+    backfill_policy = check.opt_inst_param(backfill_policy, "backfill_policy", BackfillPolicy)
 
     (
         assets,
         source_assets,
         cacheable_assets,
     ) = assets_from_package_module(package_module)
     return assets_with_attributes(
         assets,
         source_assets,
         cacheable_assets,
         key_prefix=key_prefix,
         group_name=group_name,
         freshness_policy=freshness_policy,
         auto_materialize_policy=auto_materialize_policy,
+        backfill_policy=backfill_policy,
         source_key_prefix=source_key_prefix,
     )
 
 
 def load_assets_from_package_name(
     package_name: str,
     group_name: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     *,
     freshness_policy: Optional[FreshnessPolicy] = None,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+    backfill_policy: Optional[BackfillPolicy] = None,
     source_key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
 ) -> Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
     """Constructs a list of assets, source assets, and cacheable assets that includes all asset
     definitions and source assets in all sub-modules of the given package.
 
     Args:
         package_name (str): The name of a Python package to look for assets inside.
@@ -292,28 +305,30 @@
         key_prefix (Optional[Union[str, Sequence[str]]]):
             Prefix to prepend to the keys of the loaded assets. The returned assets will be copies
             of the loaded objects, with the prefix prepended.
         freshness_policy (Optional[FreshnessPolicy]): FreshnessPolicy to apply to all the loaded
             assets.
         auto_materialize_policy (Optional[AutoMaterializePolicy]): AutoMaterializePolicy to apply
             to all the loaded assets.
+        backfill_policy (Optional[AutoMaterializePolicy]): BackfillPolicy to apply to all the loaded assets.
         source_key_prefix (bool): Prefix to prepend to the keys of loaded SourceAssets. The returned
             assets will be copies of the loaded objects, with the prefix prepended.
 
     Returns:
         Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
             A list containing assets, source assets, and cacheable assets defined in the module.
     """
     package_module = import_module(package_name)
     return load_assets_from_package_module(
         package_module,
         group_name=group_name,
         key_prefix=key_prefix,
         freshness_policy=freshness_policy,
         auto_materialize_policy=auto_materialize_policy,
+        backfill_policy=backfill_policy,
     )
 
 
 def _find_modules_in_package(package_module: ModuleType) -> Iterable[ModuleType]:
     yield package_module
     package_path = package_module.__file__
     if package_path:
@@ -415,47 +430,50 @@
     assets_defs: Sequence[AssetsDefinition],
     source_assets: Sequence[SourceAsset],
     cacheable_assets: Sequence[CacheableAssetsDefinition],
     key_prefix: Optional[Sequence[str]],
     group_name: Optional[str],
     freshness_policy: Optional[FreshnessPolicy],
     auto_materialize_policy: Optional[AutoMaterializePolicy],
+    backfill_policy: Optional[BackfillPolicy],
     source_key_prefix: Optional[Sequence[str]],
 ) -> Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
     # There is a tricky edge case here where if a non-cacheable asset depends on a cacheable asset,
     # and the assets are prefixed, the non-cacheable asset's dependency will not be prefixed since
     # at prefix-time it is not known that its dependency is one of the cacheable assets.
     # https://github.com/dagster-io/dagster/pull/10389#pullrequestreview-1170913271
     if key_prefix:
         assets_defs, source_assets = prefix_assets(
             assets_defs, key_prefix, source_assets, source_key_prefix
         )
         cacheable_assets = [
             cached_asset.with_prefix_for_all(key_prefix) for cached_asset in cacheable_assets
         ]
 
-    if group_name or freshness_policy or auto_materialize_policy:
+    if group_name or freshness_policy or auto_materialize_policy or backfill_policy:
         assets_defs = [
             asset.with_attributes(
                 group_names_by_key={asset_key: group_name for asset_key in asset.keys}
                 if group_name
                 else None,
                 freshness_policy=freshness_policy,
                 auto_materialize_policy=auto_materialize_policy,
+                backfill_policy=backfill_policy,
             )
             for asset in assets_defs
         ]
         if group_name:
             source_assets = [
                 source_asset.with_attributes(group_name=group_name)
                 for source_asset in source_assets
             ]
         cacheable_assets = [
             cached_asset.with_attributes_for_all(
                 group_name,
                 freshness_policy=freshness_policy,
                 auto_materialize_policy=auto_materialize_policy,
+                backfill_policy=backfill_policy,
             )
             for cached_asset in cacheable_assets
         ]
 
     return [*assets_defs, *source_assets, *cacheable_assets]
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/logger_definition.py` & `dagster-1.4.3/dagster/_core/definitions/logger_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from typing import TYPE_CHECKING, Any, Callable, Optional, Union, cast, overload
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.errors import DagsterInvalidInvocationError
 
 from ..decorator_utils import get_function_params
@@ -10,14 +9,16 @@
 from .configurable import AnonymousConfigurableDefinition
 from .definition_config_schema import (
     CoercableToConfigSchema,
     convert_user_facing_definition_config_schema,
 )
 
 if TYPE_CHECKING:
+    import logging
+
     from dagster._core.definitions import JobDefinition
     from dagster._core.execution.context.logger import InitLoggerContext, UnboundInitLoggerContext
 
     InitLoggerFunction = Callable[[InitLoggerContext], logging.Logger]
 
 
 class LoggerDefinition(AnonymousConfigurableDefinition):
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/logger_invocation.py` & `dagster-1.4.3/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/materialize.py` & `dagster-1.4.3/dagster/_core/definitions/materialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import TYPE_CHECKING, Any, Mapping, Optional, Sequence, Set, Union
 
 import dagster._check as check
-from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.unresolved_asset_job_definition import define_asset_job
 from dagster._utils.merger import merge_dicts
 
 from ..errors import DagsterInvariantViolationError
 from ..instance import DagsterInstance
 from ..storage.io_manager import IOManagerDefinition
 from ..storage.mem_io_manager import mem_io_manager
 from .assets import AssetsDefinition
 from .source_asset import SourceAsset
 
 if TYPE_CHECKING:
     from dagster._core.definitions.asset_selection import CoercibleToAssetSelection
+    from dagster._core.definitions.events import AssetKey
 
     from ..execution.execute_in_process_result import ExecuteInProcessResult
 
 
 def materialize(
     assets: Sequence[Union[AssetsDefinition, SourceAsset]],
     run_config: Any = None,
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.4.3/dagster/_core/definitions/metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -846,14 +846,15 @@
         records (TableRecord): The data as a list of records (i.e. rows).
         schema (Optional[TableSchema]): A schema for the table.
     """
 
     @public
     @staticmethod
     def infer_column_type(value: object) -> str:
+        """str: Infer the :py:class:`TableSchema` column type that will be used for a value."""
         if isinstance(value, bool):
             return "bool"
         elif isinstance(value, int):
             return "int"
         elif isinstance(value, float):
             return "float"
         else:
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/metadata/table.py` & `dagster-1.4.3/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.4.3/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,14 @@
         monitored_assets: Union[Sequence[AssetKey], AssetSelection],
         instance: Optional[DagsterInstance] = None,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
         definitions: Optional["Definitions"] = None,
     ):
         from dagster._core.definitions.definitions_class import Definitions
         from dagster._core.definitions.repository_definition import RepositoryDefinition
-        from dagster._core.storage.event_log.base import EventLogRecord
 
         self._repository_def = normalize_to_repository(
             check.opt_inst_param(definitions, "definitions", Definitions),
             check.opt_inst_param(repository_def, "repository_def", RepositoryDefinition),
         )
         self._monitored_asset_keys: Sequence[AssetKey]
         if isinstance(monitored_assets, AssetSelection):
@@ -384,16 +383,14 @@
                 not specified, the latest materialization will be fetched for all assets the
                 multi_asset_sensor monitors.
 
         Returns: Mapping of AssetKey to EventLogRecord where the EventLogRecord is the latest
             materialization event for the asset. If there is no materialization event for the asset,
             the value in the mapping will be None.
         """
-        from dagster._core.storage.event_log.base import EventLogRecord
-
         # Do not evaluate unconsumed events, only events newer than the cursor
         # if there are no new events after the cursor, the cursor points to the most
         # recent event.
 
         if asset_keys is None:
             asset_keys = self._monitored_asset_keys
         else:
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.4.3/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/node_container.py` & `dagster-1.4.3/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/node_definition.py` & `dagster-1.4.3/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/observe.py` & `dagster-1.4.3/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/op_definition.py` & `dagster-1.4.3/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/op_invocation.py` & `dagster-1.4.3/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/op_selection.py` & `dagster-1.4.3/dagster/_core/definitions/op_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import itertools
 from typing import (
+    TYPE_CHECKING,
     AbstractSet,
     Dict,
     Iterable,
     List,
     NamedTuple,
     Optional,
     Sequence,
@@ -21,18 +22,20 @@
     IDependencyDefinition,
     MultiDependencyDefinition,
     NodeHandle,
     NodeInvocation,
     NodeOutput,
 )
 from dagster._core.definitions.graph_definition import GraphDefinition, SubselectedGraphDefinition
-from dagster._core.definitions.node_definition import NodeDefinition
 from dagster._core.errors import DagsterInvalidSubsetError
 from dagster._core.selector.subset_selector import parse_op_queries
 
+if TYPE_CHECKING:
+    from dagster._core.definitions.node_definition import NodeDefinition
+
 
 class OpSelection:
     def __init__(self, query: Iterable[str]):
         self.query = query
 
     def resolve(self, graph_def: GraphDefinition) -> AbstractSet[str]:
         if any(["." in item for item in self.query]):
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/output.py` & `dagster-1.4.3/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/partition.py` & `dagster-1.4.3/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/partition_mapping.py` & `dagster-1.4.3/dagster/_core/definitions/partition_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,21 @@
     def get_downstream_partitions_for_partitions(
         self,
         upstream_partitions_subset: PartitionsSubset,
         downstream_partitions_def: PartitionsDefinition,
         current_time: Optional[datetime] = None,
         dynamic_partitions_store: Optional[DynamicPartitionsStore] = None,
     ) -> PartitionsSubset:
-        raise NotImplementedError()
+        # if any of the partition keys in this partition mapping are contained within the upstream
+        # partitions subset, then all partitions of the downstream asset are dependencies
+        if any(key in upstream_partitions_subset for key in self.partition_keys):
+            return downstream_partitions_def.subset_with_all_partitions(
+                dynamic_partitions_store=dynamic_partitions_store
+            )
+        return downstream_partitions_def.empty_subset()
 
 
 @experimental
 @whitelist_for_serdes
 class MultiToSingleDimensionPartitionMapping(
     PartitionMapping,
     NamedTuple(
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.4.3/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/policy.py` & `dagster-1.4.3/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/reconstruct.py` & `dagster-1.4.3/dagster/_core/definitions/reconstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import inspect
 import json
 import os
 import sys
 from functools import lru_cache
 from typing import (
     TYPE_CHECKING,
@@ -83,15 +81,15 @@
     def __new__(
         cls,
         pointer: CodePointer,
         container_image: Optional[str] = None,
         executable_path: Optional[str] = None,
         entry_point: Optional[Sequence[str]] = None,
         container_context: Optional[Mapping[str, Any]] = None,
-        repository_load_data: Optional[RepositoryLoadData] = None,
+        repository_load_data: Optional["RepositoryLoadData"] = None,
     ):
         from dagster._core.definitions.repository_definition import RepositoryLoadData
 
         return super(ReconstructableRepository, cls).__new__(
             cls,
             pointer=check.inst_param(pointer, "pointer", CodePointer),
             container_image=check.opt_str_param(container_image, "container_image"),
@@ -115,26 +113,26 @@
         self, metadata: Optional["RepositoryLoadData"]
     ) -> "ReconstructableRepository":
         return self._replace(repository_load_data=metadata)
 
     def get_definition(self) -> "RepositoryDefinition":
         return repository_def_from_pointer(self.pointer, self.repository_load_data)
 
-    def get_reconstructable_job(self, name: str) -> ReconstructableJob:
+    def get_reconstructable_job(self, name: str) -> "ReconstructableJob":
         return ReconstructableJob(self, name)
 
     @classmethod
     def for_file(
         cls,
         file: str,
         fn_name: str,
         working_directory: Optional[str] = None,
         container_image: Optional[str] = None,
         container_context: Optional[Mapping[str, Any]] = None,
-    ) -> ReconstructableRepository:
+    ) -> "ReconstructableRepository":
         if not working_directory:
             working_directory = os.getcwd()
         return cls(
             FileCodePointer(file, fn_name, working_directory),
             container_image=container_image,
             container_context=container_context,
         )
@@ -143,15 +141,15 @@
     def for_module(
         cls,
         module: str,
         fn_name: str,
         working_directory: Optional[str] = None,
         container_image: Optional[str] = None,
         container_context: Optional[Mapping[str, Any]] = None,
-    ) -> ReconstructableRepository:
+    ) -> "ReconstructableRepository":
         return cls(
             ModuleCodePointer(module, fn_name, working_directory),
             container_image=container_image,
             container_context=container_context,
         )
 
     def get_python_origin(self) -> RepositoryPythonOrigin:
@@ -243,21 +241,21 @@
             asset_selection=check.opt_nullable_set_param(
                 asset_selection, "asset_selection", AssetKey
             ),
         )
 
     def with_repository_load_data(
         self, metadata: Optional["RepositoryLoadData"]
-    ) -> ReconstructableJob:
+    ) -> "ReconstructableJob":
         return self._replace(repository=self.repository.with_repository_load_data(metadata))
 
     # Keep the most recent 1 definition (globally since this is a NamedTuple method)
     # This allows repeated calls to get_definition in execution paths to not reload the job
     @lru_cache(maxsize=1)
-    def get_definition(self) -> JobDefinition:
+    def get_definition(self) -> "JobDefinition":
         return self.repository.get_definition().get_maybe_subset_job_def(
             self.job_name,
             self.op_selection,
             self.asset_selection,
         )
 
     def get_reconstructable_repository(self) -> ReconstructableRepository:
@@ -283,26 +281,26 @@
 
     def describe(self) -> str:
         return '"{name}" in repository ({repo})'.format(
             repo=self.repository.pointer.describe, name=self.job_name
         )
 
     @staticmethod
-    def for_file(python_file: str, fn_name: str) -> ReconstructableJob:
+    def for_file(python_file: str, fn_name: str) -> "ReconstructableJob":
         return bootstrap_standalone_recon_job(FileCodePointer(python_file, fn_name, os.getcwd()))
 
     @staticmethod
-    def for_module(module: str, fn_name: str) -> ReconstructableJob:
+    def for_module(module: str, fn_name: str) -> "ReconstructableJob":
         return bootstrap_standalone_recon_job(ModuleCodePointer(module, fn_name, os.getcwd()))
 
     def to_dict(self) -> Mapping[str, object]:
         return pack_value(self)
 
     @staticmethod
-    def from_dict(val: Mapping[str, Any]) -> ReconstructableJob:
+    def from_dict(val: Mapping[str, Any]) -> "ReconstructableJob":
         check.mapping_param(val, "val")
 
         inst = unpack_value(val)
         check.invariant(
             isinstance(inst, ReconstructableJob),
             "Deserialized object is not instance of ReconstructableJob, got {type}".format(
                 type=type(inst)
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.4.3/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.4.3/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.4.3/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,46 +139,61 @@
         ]
         if not schedules_with_name:
             raise DagsterInvariantViolationError(
                 f"Could not find schedule {schedule_name} in repository"
             )
         return schedules_with_name[0]
 
+    @public
     def has_schedule(self, schedule_name: str) -> bool:
+        """Check if a schedule with a given name is present in the repository."""
         return schedule_name in self.get_schedule_names()
 
     @public
     def get_all_sensors(self) -> Sequence[SensorDefinition]:
+        """Sequence[SensorDefinition]: Return all sensors in the repository as a list."""
         return []
 
     @public
     def get_sensor_names(self) -> Sequence[str]:
+        """Sequence[str]: Get the names of all sensors in the repository."""
         return [sensor.name for sensor in self.get_all_sensors()]
 
     @public
     def get_sensor(self, sensor_name: str) -> SensorDefinition:
+        """Get a sensor by name.
+
+        Args:
+            sensor_name (str): name of the sensor to retrieve.
+
+        Returns:
+            SensorDefinition: The sensor definition corresponding to the given name.
+        """
         sensors_with_name = [
             sensor for sensor in self.get_all_sensors() if sensor.name == sensor_name
         ]
         if not sensors_with_name:
             raise DagsterInvariantViolationError(
                 f"Could not find sensor {sensor_name} in repository"
             )
         return sensors_with_name[0]
 
     @public
     def has_sensor(self, sensor_name: str) -> bool:
+        """Check if a sensor with a given name is present in the repository."""
         return sensor_name in self.get_sensor_names()
 
     @public
     def get_source_assets_by_key(self) -> Mapping[AssetKey, SourceAsset]:
+        """Mapping[AssetKey, SourceAsset]: Get the source assets for the repository."""
         return {}
 
     @public
     def get_assets_defs_by_key(self) -> Mapping[AssetKey, "AssetsDefinition"]:
+        """Mapping[AssetKey, AssetsDefinition]: Get the asset definitions for the repository."""
         return {}
 
     def load_all_definitions(self):
         # force load of all lazy constructed code artifacts
         self.get_all_jobs()
         self.get_all_schedules()
         self.get_all_sensors()
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.4.3/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from collections import defaultdict
 from inspect import isfunction
 from typing import (
+    TYPE_CHECKING,
     Any,
     Dict,
     List,
     Mapping,
     Optional,
     Sequence,
     Set,
@@ -20,15 +21,14 @@
     ResourceWithKeyMapping,
 )
 from dagster._core.definitions.asset_graph import AssetGraph
 from dagster._core.definitions.assets_job import (
     get_base_asset_jobs,
     is_base_asset_job_name,
 )
-from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.executor_definition import ExecutorDefinition
 from dagster._core.definitions.graph_definition import GraphDefinition
 from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.logger_definition import LoggerDefinition
 from dagster._core.definitions.partitioned_schedule import (
     UnresolvedPartitionedAssetScheduleDefinition,
 )
@@ -38,14 +38,17 @@
 from dagster._core.definitions.source_asset import SourceAsset
 from dagster._core.definitions.unresolved_asset_job_definition import UnresolvedAssetJobDefinition
 from dagster._core.errors import DagsterInvalidDefinitionError
 
 from .repository_data import CachingRepositoryData
 from .valid_definitions import VALID_REPOSITORY_DATA_DICT_KEYS, RepositoryListDefinition
 
+if TYPE_CHECKING:
+    from dagster._core.definitions.events import AssetKey
+
 
 def _find_env_vars(config_entry: Any) -> Set[str]:
     """Given a part of a config dictionary, return a set of environment variables that are used in
     that part of the config.
     """
     # Actual env var entry
     if isinstance(config_entry, Mapping) and set(config_entry.keys()) == {"env"}:
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.4.3/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
+    Dict,
     Iterable,
     List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Type,
@@ -306,14 +307,15 @@
     def load_asset_value(
         self,
         asset_key: CoercibleToAssetKey,
         *,
         python_type: Optional[Type] = None,
         instance: Optional[DagsterInstance] = None,
         partition_key: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
         resource_config: Optional[Any] = None,
     ) -> object:
         """Load the contents of an asset as a Python object.
 
         Invokes `load_input` on the :py:class:`IOManager` associated with the asset.
 
         If you want to load the values of multiple assets, it's more efficient to use
@@ -321,14 +323,16 @@
         resources separately for each asset.
 
         Args:
             asset_key (Union[AssetKey, Sequence[str], str]): The key of the asset to load.
             python_type (Optional[Type]): The python type to load the asset as. This is what will
                 be returned inside `load_input` by `context.dagster_type.typing_type`.
             partition_key (Optional[str]): The partition of the asset to load.
+            metadata (Optional[Dict[str, Any]]): Input metadata to pass to the :py:class:`IOManager`
+                (is equivalent to setting the metadata argument in `In` or `AssetIn`).
             resource_config (Optional[Any]): A dictionary of resource configurations to be passed
                 to the :py:class:`IOManager`.
 
         Returns:
             The contents of an asset as a Python object.
         """
         from dagster._core.storage.asset_value_loader import AssetValueLoader
@@ -336,14 +340,15 @@
         with AssetValueLoader(
             self.assets_defs_by_key, self.source_assets_by_key, instance=instance
         ) as loader:
             return loader.load_asset_value(
                 asset_key,
                 python_type=python_type,
                 partition_key=partition_key,
+                metadata=metadata,
                 resource_config=resource_config,
             )
 
     @public
     def get_asset_value_loader(
         self, instance: Optional[DagsterInstance] = None
     ) -> "AssetValueLoader":
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.4.3/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.4.3/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/resource_annotation.py` & `dagster-1.4.3/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/resource_definition.py` & `dagster-1.4.3/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/resource_invocation.py` & `dagster-1.4.3/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/resource_requirement.py` & `dagster-1.4.3/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/run_config.py` & `dagster-1.4.3/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/run_config_schema.py` & `dagster-1.4.3/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/run_request.py` & `dagster-1.4.3/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.4.3/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/schedule_definition.py` & `dagster-1.4.3/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.4.3/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/selector.py` & `dagster-1.4.3/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/sensor_definition.py` & `dagster-1.4.3/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/source_asset.py` & `dagster-1.4.3/dagster/_core/definitions/source_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,23 +164,29 @@
             Optional[IOManagerDefinition],
             self.resource_defs.get(io_manager_key) if io_manager_key else None,
         )
 
     @public
     @property
     def op(self) -> OpDefinition:
+        """OpDefinition: The OpDefinition associated with the observation function of an observable
+        source asset.
+
+        Throws an error if the asset is not observable.
+        """
         check.invariant(
             isinstance(self.node_def, OpDefinition),
             "The NodeDefinition for this AssetsDefinition is not of type OpDefinition.",
         )
         return cast(OpDefinition, self.node_def)
 
     @public
     @property
     def is_observable(self) -> bool:
+        """bool: Whether the asset is observable."""
         return self.node_def is not None
 
     def _get_op_def_compute_fn(self, observe_fn: SourceAssetObserveFunction):
         from dagster._core.definitions.decorators.op_decorator import (
             DecoratedOpFunction,
             is_context_provided,
         )
```

### Comparing `dagster-1.4.2/dagster/_core/definitions/step_launcher.py` & `dagster-1.4.3/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/target.py` & `dagster-1.4.3/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.4.3/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.4.3/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.4.3/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/utils.py` & `dagster-1.4.3/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/definitions/version_strategy.py` & `dagster-1.4.3/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/errors.py` & `dagster-1.4.3/dagster/_core/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 exceptions, and then reraises them wrapped in a subclass of
 :py:class:`~dagster.DagsterUserCodeExecutionError`.
 
 The wrapped exceptions include additional context for the original exceptions, injected by the
 Dagster runtime.
 """
 
-from __future__ import annotations
-
 import sys
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, Callable, Iterator, Optional, Type
 
 import dagster._check as check
 from dagster._utils.interrupts import raise_interrupts_as
 
@@ -253,17 +251,17 @@
 def raise_execution_interrupts() -> Iterator[None]:
     with raise_interrupts_as(DagsterExecutionInterruptedError):
         yield
 
 
 @contextmanager
 def user_code_error_boundary(
-    error_cls: Type[DagsterUserCodeExecutionError],
+    error_cls: Type["DagsterUserCodeExecutionError"],
     msg_fn: Callable[[], str],
-    log_manager: Optional[DagsterLogManager] = None,
+    log_manager: Optional["DagsterLogManager"] = None,
     **kwargs: object,
 ) -> Iterator[None]:
     """Wraps the execution of user-space code in an error boundary. This places a uniform
     policy around any user code invoked by the framework. This ensures that all user
     errors are wrapped in an exception derived from DagsterUserCodeExecutionError,
     and that the original stack trace of the user error is preserved, so that it
     can be reported without confusing framework code in the stack trace, if a
```

### Comparing `dagster-1.4.2/dagster/_core/event_api.py` & `dagster-1.4.3/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/events/__init__.py` & `dagster-1.4.3/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/events/log.py` & `dagster-1.4.3/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/events/utils.py` & `dagster-1.4.3/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/api.py` & `dagster-1.4.3/dagster/_core/execution/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 from contextlib import contextmanager
 from typing import (
+    TYPE_CHECKING,
     AbstractSet,
     Any,
     Callable,
     Dict,
     Iterator,
     Mapping,
     NamedTuple,
@@ -21,15 +22,14 @@
 from dagster._core.definitions.job_base import InMemoryJob
 from dagster._core.definitions.reconstruct import ReconstructableJob
 from dagster._core.definitions.repository_definition import RepositoryLoadData
 from dagster._core.errors import DagsterExecutionInterruptedError, DagsterInvariantViolationError
 from dagster._core.events import DagsterEvent, EngineEventData
 from dagster._core.execution.context.system import PlanOrchestrationContext
 from dagster._core.execution.plan.execute_plan import inner_plan_execution_iterator
-from dagster._core.execution.plan.outputs import StepOutputHandle
 from dagster._core.execution.plan.plan import ExecutionPlan
 from dagster._core.execution.plan.state import KnownExecutionState
 from dagster._core.execution.retries import RetryMode
 from dagster._core.instance import DagsterInstance, InstanceRef
 from dagster._core.selector import parse_step_selection
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus
 from dagster._core.system_config.objects import ResolvedRunConfig
@@ -43,14 +43,17 @@
     PlanExecutionContextManager,
     PlanOrchestrationContextManager,
     orchestration_context_event_generator,
     scoped_job_context,
 )
 from .job_execution_result import JobExecutionResult
 
+if TYPE_CHECKING:
+    from dagster._core.execution.plan.outputs import StepOutputHandle
+
 ## Brief guide to the execution APIs
 # | function name               | operates over      | sync  | supports    | creates new DagsterRun  |
 # |                             |                    |       | reexecution | in instance             |
 # | --------------------------- | ------------------ | ----- | ----------- | ----------------------- |
 # | execute_job                 | ReconstructableJob | sync  | yes         | yes                     |
 # | execute_run_iterator        | DagsterRun         | async | (1)         | no                      |
 # | execute_run                 | DagsterRun         | sync  | (1)         | no                      |
```

### Comparing `dagster-1.4.2/dagster/_core/execution/asset_backfill.py` & `dagster-1.4.3/dagster/_core/execution/asset_backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,15 @@
     Union,
     cast,
 )
 
 from dagster import _check as check
 from dagster._core.definitions.asset_graph import AssetGraph
 from dagster._core.definitions.asset_graph_subset import AssetGraphSubset
-from dagster._core.definitions.asset_reconciliation_sensor import (
-    build_run_requests,
-    find_parent_materialized_asset_partitions,
-)
+from dagster._core.definitions.asset_reconciliation_sensor import build_run_requests
 from dagster._core.definitions.asset_selection import AssetSelection
 from dagster._core.definitions.assets_job import is_base_asset_job_name
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.partition import PartitionsSubset
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.definitions.selector import JobSubsetSelector
@@ -803,19 +800,17 @@
         }
         target_asset_keys_and_parents = (
             asset_backfill_data.target_subset.asset_keys | target_parent_asset_keys
         )
         (
             parent_materialized_asset_partitions,
             next_latest_storage_id,
-        ) = find_parent_materialized_asset_partitions(
-            asset_graph=asset_graph,
-            instance_queryer=instance_queryer,
-            target_asset_keys=asset_backfill_data.target_subset.asset_keys,
-            target_asset_keys_and_parents=target_asset_keys_and_parents,
+        ) = instance_queryer.asset_partitions_with_newly_updated_parents_and_new_latest_storage_id(
+            target_asset_keys=frozenset(asset_backfill_data.target_subset.asset_keys),
+            target_asset_keys_and_parents=frozenset(target_asset_keys_and_parents),
             latest_storage_id=asset_backfill_data.latest_storage_id,
         )
         initial_candidates.update(parent_materialized_asset_partitions)
 
         yield None
 
         updated_materialized_subset = None
```

### Comparing `dagster-1.4.2/dagster/_core/execution/backfill.py` & `dagster-1.4.3/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/build_resources.py` & `dagster-1.4.3/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/compute_logs.py` & `dagster-1.4.3/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/context/compute.py` & `dagster-1.4.3/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/context/hook.py` & `dagster-1.4.3/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/context/init.py` & `dagster-1.4.3/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/context/input.py` & `dagster-1.4.3/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/context/invocation.py` & `dagster-1.4.3/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/context/logger.py` & `dagster-1.4.3/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/context/output.py` & `dagster-1.4.3/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/context/system.py` & `dagster-1.4.3/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/context_creation_job.py` & `dagster-1.4.3/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/execute_in_process.py` & `dagster-1.4.3/dagster/_core/execution/execute_in_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Any, Dict, FrozenSet, Mapping, Optional, cast
+from typing import TYPE_CHECKING, Any, Dict, FrozenSet, Mapping, Optional, cast
 
 from dagster._core.definitions import GraphDefinition, JobDefinition, Node, NodeHandle, OpDefinition
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.job_base import InMemoryJob
 from dagster._core.errors import DagsterInvalidInvocationError
-from dagster._core.execution.plan.outputs import StepOutputHandle
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.dagster_run import DagsterRun
 from dagster._core.types.dagster_type import DagsterTypeKind
 
 from .api import (
     ExecuteRunWithPlanIterable,
     create_execution_plan,
@@ -17,14 +16,17 @@
 )
 from .context_creation_job import (
     PlanOrchestrationContextManager,
     orchestration_context_event_generator,
 )
 from .execute_in_process_result import ExecuteInProcessResult
 
+if TYPE_CHECKING:
+    from dagster._core.execution.plan.outputs import StepOutputHandle
+
 
 def core_execute_in_process(
     run_config: Mapping[str, object],
     ephemeral_job: JobDefinition,
     instance: Optional[DagsterInstance],
     output_capturing_enabled: bool,
     raise_on_error: bool,
```

### Comparing `dagster-1.4.2/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.4.3/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/execution_result.py` & `dagster-1.4.3/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/host_mode.py` & `dagster-1.4.3/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/job_backfill.py` & `dagster-1.4.3/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/job_execution_result.py` & `dagster-1.4.3/dagster/_core/execution/job_execution_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,29 +40,33 @@
         exit_result = self._reconstruct_context.__exit__(*exc)
         self._context = None
         return exit_result
 
     @public
     @property
     def job_def(self) -> JobDefinition:
+        """JobDefinition: The job definition that was executed."""
         return self._job_def
 
     @public
     @property
     def dagster_run(self) -> DagsterRun:
+        """DagsterRun: The Dagster run that was executed."""
         return self._dagster_run
 
     @public
     @property
     def all_events(self) -> Sequence[DagsterEvent]:
+        """Sequence[DagsterEvent]: List of all events yielded by the job execution."""
         return self._event_list
 
     @public
     @property
     def run_id(self) -> str:
+        """str: The id of the Dagster run that was executed."""
         return self.dagster_run.run_id
 
     @public
     def output_value(self, output_name: str = DEFAULT_OUTPUT) -> Any:
         """Retrieves output of top-level job, if an output is returned.
 
         In order to use this method, the `ExecuteJobResult` object must be opened as a context manager. If this method is used without opening the context manager, it will result in a :py:class:`DagsterInvariantViolationError`. If the top-level job has no output, calling this method will also result in a :py:class:`DagsterInvariantViolationError`.
```

### Comparing `dagster-1.4.2/dagster/_core/execution/memoization.py` & `dagster-1.4.3/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/active.py` & `dagster-1.4.3/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/compute.py` & `dagster-1.4.3/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.4.3/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.4.3/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/execute_step.py` & `dagster-1.4.3/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/external_step.py` & `dagster-1.4.3/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/handle.py` & `dagster-1.4.3/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/inputs.py` & `dagster-1.4.3/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.4.3/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.4.3/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 import pickle
 import sys
-from typing import List
+from typing import TYPE_CHECKING, List
 
-from dagster._core.events.log import EventLogEntry
 from dagster._core.execution.plan.external_step import (
     PICKLED_EVENTS_FILE_NAME,
     external_instance_from_step_run_ref,
     run_step_from_ref,
 )
 from dagster._core.storage.file_manager import LocalFileHandle, LocalFileManager
 from dagster._serdes import serialize_value
 
+if TYPE_CHECKING:
+    from dagster._core.events.log import EventLogEntry
+
 
 def main(step_run_ref_path: str) -> None:
     file_manager = LocalFileManager(".")
     file_handle = LocalFileHandle(step_run_ref_path)
     step_run_ref = pickle.loads(file_manager.read_data(file_handle))
 
     all_events: List[EventLogEntry] = []
```

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/objects.py` & `dagster-1.4.3/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/outputs.py` & `dagster-1.4.3/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/plan.py` & `dagster-1.4.3/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/state.py` & `dagster-1.4.3/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/step.py` & `dagster-1.4.3/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/plan/utils.py` & `dagster-1.4.3/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.4.3/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/resolve_versions.py` & `dagster-1.4.3/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/resources_init.py` & `dagster-1.4.3/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/retries.py` & `dagster-1.4.3/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.4.3/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/stats.py` & `dagster-1.4.3/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/tags.py` & `dagster-1.4.3/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/validate_run_config.py` & `dagster-1.4.3/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/watch_orphans.py` & `dagster-1.4.3/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/execution/with_resources.py` & `dagster-1.4.3/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/executor/base.py` & `dagster-1.4.3/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/executor/child_process_executor.py` & `dagster-1.4.3/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/executor/in_process.py` & `dagster-1.4.3/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/executor/init.py` & `dagster-1.4.3/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/executor/multiprocess.py` & `dagster-1.4.3/dagster/_core/executor/multiprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             )
 
 
 class MultiprocessExecutor(Executor):
     def __init__(
         self,
         retries: RetryMode,
-        max_concurrent: int,
+        max_concurrent: Optional[int],
         tag_concurrency_limits: Optional[List[Dict[str, Any]]] = None,
         start_method: Optional[str] = None,
         explicit_forkserver_preload: Optional[Sequence[str]] = None,
     ):
         self._retries = check.inst_param(retries, "retries", RetryMode)
         if not max_concurrent:
             env_var_default = os.getenv("DAGSTER_MULTIPROCESS_EXECUTOR_MAX_CONCURRENT")
```

### Comparing `dagster-1.4.2/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.4.3/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import os
 import sys
 import time
-from typing import Any, Dict, List, Optional, Sequence, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, cast
 
 import pendulum
 
 import dagster._check as check
 from dagster._core.definitions.metadata import MetadataValue
 from dagster._core.events import DagsterEvent, DagsterEventType, EngineEventData
 from dagster._core.execution.context.system import PlanOrchestrationContext
 from dagster._core.execution.plan.active import ActiveExecution
 from dagster._core.execution.plan.instance_concurrency_context import InstanceConcurrencyContext
 from dagster._core.execution.plan.objects import StepFailureData
 from dagster._core.execution.plan.plan import ExecutionPlan
-from dagster._core.execution.plan.step import ExecutionStep
 from dagster._core.execution.retries import RetryMode
 from dagster._core.executor.step_delegating.step_handler.base import StepHandler, StepHandlerContext
 from dagster._grpc.types import ExecuteStepArgs
 from dagster._utils.error import serializable_error_info_from_exc_info
 
 from ..base import Executor
 
+if TYPE_CHECKING:
+    from dagster._core.execution.plan.step import ExecutionStep
+
 DEFAULT_SLEEP_SECONDS = float(
     os.environ.get("DAGSTER_STEP_DELEGATING_EXECUTOR_SLEEP_SECONDS", "1.0")
 )
 
 
 class StepDelegatingExecutor(Executor):
     """This executor tails the event log for events from the steps that it spins up. It also
```

### Comparing `dagster-1.4.2/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.4.3/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/host_representation/__init__.py` & `dagster-1.4.3/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/host_representation/code_location.py` & `dagster-1.4.3/dagster/_core/host_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/host_representation/external.py` & `dagster-1.4.3/dagster/_core/host_representation/external.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 from datetime import datetime
 from threading import RLock
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Callable,
     Dict,
@@ -41,15 +39,14 @@
     ExternalJobOrigin,
     ExternalPartitionSetOrigin,
     ExternalRepositoryOrigin,
 )
 from dagster._core.instance import DagsterInstance
 from dagster._core.origin import JobPythonOrigin, RepositoryPythonOrigin
 from dagster._core.snap import ExecutionPlanSnapshot
-from dagster._core.snap.execution_plan_snapshot import ExecutionStepSnap
 from dagster._core.utils import toposort
 from dagster._serdes import create_snapshot_id
 from dagster._utils.cached_method import cached_method
 from dagster._utils.schedules import schedule_execution_time_iterator
 
 from .external_data import (
     DEFAULT_MODE_NAME,
@@ -71,14 +68,15 @@
 )
 from .handle import InstigatorHandle, JobHandle, PartitionSetHandle, RepositoryHandle
 from .job_index import JobIndex
 from .represented import RepresentedJob
 
 if TYPE_CHECKING:
     from dagster._core.scheduler.instigation import InstigatorState
+    from dagster._core.snap.execution_plan_snapshot import ExecutionStepSnap
 
 
 class ExternalRepository:
     """ExternalRepository is a object that represents a loaded repository definition that
     is resident in another process or container. Host processes such as dagster-webserver use
     objects such as these to interact with user-defined artifacts.
     """
@@ -128,95 +126,95 @@
 
     @property
     def name(self) -> str:
         return self.external_repository_data.name
 
     @property
     @cached_method
-    def _external_schedules(self) -> Dict[str, ExternalSchedule]:
+    def _external_schedules(self) -> Dict[str, "ExternalSchedule"]:
         return {
             external_schedule_data.name: ExternalSchedule(external_schedule_data, self._handle)
             for external_schedule_data in self.external_repository_data.external_schedule_datas
         }
 
     def has_external_schedule(self, schedule_name: str) -> bool:
         return schedule_name in self._external_schedules
 
-    def get_external_schedule(self, schedule_name: str) -> ExternalSchedule:
+    def get_external_schedule(self, schedule_name: str) -> "ExternalSchedule":
         return self._external_schedules[schedule_name]
 
-    def get_external_schedules(self) -> Sequence[ExternalSchedule]:
+    def get_external_schedules(self) -> Sequence["ExternalSchedule"]:
         return list(self._external_schedules.values())
 
     @property
     @cached_method
-    def _external_resources(self) -> Dict[str, ExternalResource]:
+    def _external_resources(self) -> Dict[str, "ExternalResource"]:
         return {
             external_resource_data.name: ExternalResource(external_resource_data, self._handle)
             for external_resource_data in (
                 self.external_repository_data.external_resource_data or []
             )
         }
 
     def has_external_resource(self, resource_name: str) -> bool:
         return resource_name in self._external_resources
 
-    def get_external_resource(self, resource_name: str) -> ExternalResource:
+    def get_external_resource(self, resource_name: str) -> "ExternalResource":
         return self._external_resources[resource_name]
 
-    def get_external_resources(self) -> Iterable[ExternalResource]:
+    def get_external_resources(self) -> Iterable["ExternalResource"]:
         return self._external_resources.values()
 
     @property
     def _utilized_env_vars(self) -> Mapping[str, Sequence[EnvVarConsumer]]:
         return self.external_repository_data.utilized_env_vars or {}
 
     def get_utilized_env_vars(self) -> Mapping[str, Sequence[EnvVarConsumer]]:
         return self._utilized_env_vars
 
     @property
     @cached_method
-    def _external_sensors(self) -> Dict[str, ExternalSensor]:
+    def _external_sensors(self) -> Dict[str, "ExternalSensor"]:
         return {
             external_sensor_data.name: ExternalSensor(external_sensor_data, self._handle)
             for external_sensor_data in self.external_repository_data.external_sensor_datas
         }
 
     def has_external_sensor(self, sensor_name: str) -> bool:
         return sensor_name in self._external_sensors
 
-    def get_external_sensor(self, sensor_name: str) -> ExternalSensor:
+    def get_external_sensor(self, sensor_name: str) -> "ExternalSensor":
         return self._external_sensors[sensor_name]
 
-    def get_external_sensors(self) -> Sequence[ExternalSensor]:
+    def get_external_sensors(self) -> Sequence["ExternalSensor"]:
         return list(self._external_sensors.values())
 
     @property
     @cached_method
-    def _external_partition_sets(self) -> Dict[str, ExternalPartitionSet]:
+    def _external_partition_sets(self) -> Dict[str, "ExternalPartitionSet"]:
         return {
             external_partition_set_data.name: ExternalPartitionSet(
                 external_partition_set_data, self._handle
             )
             for external_partition_set_data in self.external_repository_data.external_partition_set_datas
         }
 
     def has_external_partition_set(self, partition_set_name: str) -> bool:
         return partition_set_name in self._external_partition_sets
 
-    def get_external_partition_set(self, partition_set_name: str) -> ExternalPartitionSet:
+    def get_external_partition_set(self, partition_set_name: str) -> "ExternalPartitionSet":
         return self._external_partition_sets[partition_set_name]
 
-    def get_external_partition_sets(self) -> Sequence[ExternalPartitionSet]:
+    def get_external_partition_sets(self) -> Sequence["ExternalPartitionSet"]:
         return list(self._external_partition_sets.values())
 
     def has_external_job(self, job_name: str) -> bool:
         return job_name in self._job_map
 
-    def get_full_external_job(self, job_name: str) -> ExternalJob:
+    def get_full_external_job(self, job_name: str) -> "ExternalJob":
         check.str_param(job_name, "job_name")
         check.invariant(
             self.has_external_job(job_name), f'No external job named "{job_name}" found'
         )
         with self._memo_lock:
             if job_name not in self._cached_jobs:
                 job_item = self._job_map[job_name]
@@ -236,15 +234,15 @@
                     repository_handle=self.handle,
                     external_job_ref=external_ref,
                     ref_to_data_fn=self._ref_to_data_fn,
                 )
 
             return self._cached_jobs[job_name]
 
-    def get_all_external_jobs(self) -> Sequence[ExternalJob]:
+    def get_all_external_jobs(self) -> Sequence["ExternalJob"]:
         return [self.get_full_external_job(pn) for pn in self._job_map]
 
     @property
     def handle(self) -> RepositoryHandle:
         return self._handle
 
     @property
@@ -671,15 +669,15 @@
             self._external_schedule_data.default_status
             if self._external_schedule_data.default_status
             else DefaultScheduleStatus.STOPPED
         )
 
     def get_current_instigator_state(
         self, stored_state: Optional["InstigatorState"]
-    ) -> InstigatorState:
+    ) -> "InstigatorState":
         from dagster._core.scheduler.instigation import (
             InstigatorState,
             InstigatorStatus,
             ScheduleInstigatorData,
         )
 
         if self.default_status == DefaultScheduleStatus.RUNNING:
@@ -803,15 +801,15 @@
 
     @property
     def sensor_type(self) -> SensorType:
         return self._external_sensor_data.sensor_type or SensorType.UNKNOWN
 
     def get_current_instigator_state(
         self, stored_state: Optional["InstigatorState"]
-    ) -> InstigatorState:
+    ) -> "InstigatorState":
         from dagster._core.scheduler.instigation import (
             InstigatorState,
             InstigatorStatus,
             SensorInstigatorData,
         )
 
         if self.default_status == DefaultSensorStatus.RUNNING:
```

### Comparing `dagster-1.4.2/dagster/_core/host_representation/external_data.py` & `dagster-1.4.3/dagster/_core/host_representation/external_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 import inspect
 import json
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from enum import Enum
 from typing import (
+    TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Mapping,
     NamedTuple,
     Optional,
@@ -40,18 +41,18 @@
 from dagster._core.definitions import (
     JobDefinition,
     PartitionsDefinition,
     RepositoryDefinition,
     ScheduleDefinition,
     SourceAsset,
 )
-from dagster._core.definitions.asset_layer import AssetOutputInfo
 from dagster._core.definitions.asset_sensor_definition import AssetSensorDefinition
 from dagster._core.definitions.assets_job import is_base_asset_job_name
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
+from dagster._core.definitions.backfill_policy import BackfillPolicy
 from dagster._core.definitions.definition_config_schema import ConfiguredDefinitionConfigSchema
 from dagster._core.definitions.dependency import (
     GraphNode,
     Node,
     NodeHandle,
     NodeOutputHandle,
     OpNode,
@@ -83,14 +84,17 @@
 from dagster._core.errors import DagsterInvalidDefinitionError
 from dagster._core.snap import JobSnapshot
 from dagster._core.snap.mode import ResourceDefSnap, build_resource_def_snap
 from dagster._core.storage.io_manager import IOManagerDefinition
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils.error import SerializableErrorInfo
 
+if TYPE_CHECKING:
+    from dagster._core.definitions.asset_layer import AssetOutputInfo
+
 DEFAULT_MODE_NAME = "default"
 DEFAULT_PRESET_NAME = "default"
 
 
 @whitelist_for_serdes(storage_field_names={"external_job_datas": "external_pipeline_datas"})
 class ExternalRepositoryData(
     NamedTuple(
@@ -675,26 +679,42 @@
                 end=pendulum.from_timestamp(self.end, tz=self.timezone) if self.end else None,
                 minute_offset=self.minute_offset,
                 hour_offset=self.hour_offset,
                 day_offset=self.day_offset,
             )
 
 
+def _dedup_partition_keys(keys: Sequence[str]):
+    # Use both a set and a list here to preserve lookup performance in case of large inputs. (We
+    # can't just use a set because we need to preserve ordering.)
+    seen_keys: Set[str] = set()
+    new_keys: List[str] = []
+    for key in keys:
+        if key not in seen_keys:
+            new_keys.append(key)
+            seen_keys.add(key)
+    return new_keys
+
+
 @whitelist_for_serdes
 class ExternalStaticPartitionsDefinitionData(
     ExternalPartitionsDefinitionData,
     NamedTuple("_ExternalStaticPartitionsDefinitionData", [("partition_keys", Sequence[str])]),
 ):
     def __new__(cls, partition_keys: Sequence[str]):
         return super(ExternalStaticPartitionsDefinitionData, cls).__new__(
             cls, partition_keys=check.sequence_param(partition_keys, "partition_keys", str)
         )
 
     def get_partitions_definition(self):
-        return StaticPartitionsDefinition(self.partition_keys)
+        # v1.4 made `StaticPartitionsDefinition` error if given duplicate keys. This caused
+        # host process errors for users who had not upgraded their user code to 1.4 and had dup
+        # keys, since the host process `StaticPartitionsDefinition` would throw an error.
+        keys = _dedup_partition_keys(self.partition_keys)
+        return StaticPartitionsDefinition(keys)
 
 
 @whitelist_for_serdes
 class ExternalPartitionDimensionDefinition(
     NamedTuple(
         "_ExternalPartitionDimensionDefinition",
         [
@@ -1070,14 +1090,15 @@
             ("is_observable", bool),
             # If a set of assets can't be materialized independently from each other, they will all
             # have the same atomic_execution_unit_id. This ID should be stable across reloads and
             # unique deployment-wide.
             ("atomic_execution_unit_id", Optional[str]),
             ("required_top_level_resources", Optional[Sequence[str]]),
             ("auto_materialize_policy", Optional[AutoMaterializePolicy]),
+            ("backfill_policy", Optional[BackfillPolicy]),
             ("auto_observe_interval_minutes", Optional[float]),
         ],
     )
 ):
     """A definition of a node in the logical asset graph.
 
     A function for computing the asset and an identifier for that asset.
@@ -1103,14 +1124,15 @@
         group_name: Optional[str] = None,
         freshness_policy: Optional[FreshnessPolicy] = None,
         is_source: Optional[bool] = None,
         is_observable: bool = False,
         atomic_execution_unit_id: Optional[str] = None,
         required_top_level_resources: Optional[Sequence[str]] = None,
         auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
         auto_observe_interval_minutes: Optional[float] = None,
     ):
         # backcompat logic to handle ExternalAssetNodes serialized without op_names/graph_name
         if not op_names:
             op_names = list(filter(None, [op_name]))
 
         # backcompat logic to handle ExternalAssetNodes serialzied without is_source
@@ -1159,14 +1181,17 @@
                 required_top_level_resources, "required_top_level_resources", of_type=str
             ),
             auto_materialize_policy=check.opt_inst_param(
                 auto_materialize_policy,
                 "auto_materialize_policy",
                 AutoMaterializePolicy,
             ),
+            backfill_policy=check.opt_inst_param(
+                backfill_policy, "backfill_policy", BackfillPolicy
+            ),
             auto_observe_interval_minutes=check.opt_numeric_param(
                 auto_observe_interval_minutes, "auto_observe_interval_minutes"
             ),
         )
 
 
 ResourceJobUsageMap = Dict[str, List[ResourceJobUsageEntry]]
@@ -1316,14 +1341,15 @@
     node_defs_by_asset_key: Dict[
         AssetKey, List[Tuple[NodeOutputHandle, JobDefinition]]
     ] = defaultdict(list)
     asset_info_by_asset_key: Dict[AssetKey, AssetOutputInfo] = dict()
     freshness_policy_by_asset_key: Dict[AssetKey, FreshnessPolicy] = dict()
     metadata_by_asset_key: Dict[AssetKey, MetadataUserInput] = dict()
     auto_materialize_policy_by_asset_key: Dict[AssetKey, AutoMaterializePolicy] = dict()
+    backfill_policy_by_asset_key: Dict[AssetKey, Optional[BackfillPolicy]] = dict()
 
     deps: Dict[AssetKey, Dict[AssetKey, ExternalAssetDependency]] = defaultdict(dict)
     dep_by: Dict[AssetKey, Dict[AssetKey, ExternalAssetDependedBy]] = defaultdict(dict)
     all_upstream_asset_keys: Set[AssetKey] = set()
     op_names_by_asset_key: Dict[AssetKey, Sequence[str]] = {}
     code_version_by_asset_key: Dict[AssetKey, Optional[str]] = dict()
     group_name_by_asset_key: Dict[AssetKey, str] = {}
@@ -1366,14 +1392,17 @@
                     downstream_asset_key=output_key
                 )
 
         for assets_def in asset_layer.assets_defs_by_key.values():
             metadata_by_asset_key.update(assets_def.metadata_by_key)
             freshness_policy_by_asset_key.update(assets_def.freshness_policies_by_key)
             auto_materialize_policy_by_asset_key.update(assets_def.auto_materialize_policies_by_key)
+            backfill_policy_by_asset_key.update(
+                {key: assets_def.backfill_policy for key in assets_def.keys}
+            )
             descriptions_by_asset_key.update(assets_def.descriptions_by_key)
             if len(assets_def.keys) > 1 and not assets_def.can_subset:
                 atomic_execution_unit_id = assets_def.unique_id
 
                 for asset_key in assets_def.keys:
                     atomic_execution_unit_ids_by_asset_key[asset_key] = atomic_execution_unit_id
 
@@ -1493,14 +1522,15 @@
                 metadata=asset_metadata,
                 # assets defined by Out(asset_key="k") do not have any group
                 # name specified we default to DEFAULT_GROUP_NAME here to ensure
                 # such assets are part of the default group
                 group_name=group_name_by_asset_key.get(asset_key, DEFAULT_GROUP_NAME),
                 freshness_policy=freshness_policy_by_asset_key.get(asset_key),
                 auto_materialize_policy=auto_materialize_policy_by_asset_key.get(asset_key),
+                backfill_policy=backfill_policy_by_asset_key.get(asset_key),
                 atomic_execution_unit_id=atomic_execution_unit_ids_by_asset_key.get(asset_key),
                 required_top_level_resources=required_top_level_resources,
             )
         )
 
     return asset_nodes
```

### Comparing `dagster-1.4.2/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.4.3/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import sys
 import threading
 import uuid
 from contextlib import AbstractContextManager
 from typing import (
     TYPE_CHECKING,
     Any,
```

### Comparing `dagster-1.4.2/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.4.3/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/host_representation/handle.py` & `dagster-1.4.3/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/host_representation/historical.py` & `dagster-1.4.3/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/host_representation/job_index.py` & `dagster-1.4.3/dagster/_core/host_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/host_representation/origin.py` & `dagster-1.4.3/dagster/_core/host_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/host_representation/represented.py` & `dagster-1.4.3/dagster/_core/host_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/instance/__init__.py` & `dagster-1.4.3/dagster/_core/instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import logging
 import logging.config
 import os
 import sys
 import time
 import weakref
 from abc import abstractmethod
@@ -229,15 +227,15 @@
 
 T_DagsterInstance = TypeVar("T_DagsterInstance", bound="DagsterInstance", default="DagsterInstance")
 
 
 class MayHaveInstanceWeakref(Generic[T_DagsterInstance]):
     """Mixin for classes that can have a weakref back to a Dagster instance."""
 
-    _instance_weakref: Optional[weakref.ReferenceType[T_DagsterInstance]]
+    _instance_weakref: "Optional[weakref.ReferenceType[T_DagsterInstance]]"
 
     def __init__(self):
         self._instance_weakref = None
 
     @property
     def has_instance(self) -> bool:
         return hasattr(self, "_instance_weakref") and (self._instance_weakref is not None)
@@ -330,17 +328,17 @@
             keys.
         ref (Optional[InstanceRef]): Used by internal machinery to pass instances across process
             boundaries.
     """
 
     # Stores TemporaryDirectory instances that were created for DagsterInstance.local_temp() calls
     # to be removed once the instance is garbage collected.
-    _TEMP_DIRS: weakref.WeakKeyDictionary[
-        DagsterInstance, TemporaryDirectory
-    ] = weakref.WeakKeyDictionary()
+    _TEMP_DIRS: "weakref.WeakKeyDictionary[DagsterInstance, TemporaryDirectory]" = (
+        weakref.WeakKeyDictionary()
+    )
 
     def __init__(
         self,
         instance_type: InstanceType,
         local_artifact_storage: "LocalArtifactStorage",
         run_storage: "RunStorage",
         event_storage: "EventLogStorage",
@@ -348,14 +346,15 @@
         compute_log_manager: Optional["ComputeLogManager"],
         run_launcher: Optional["RunLauncher"],
         scheduler: Optional["Scheduler"] = None,
         schedule_storage: Optional["ScheduleStorage"] = None,
         settings: Optional[Mapping[str, Any]] = None,
         secrets_loader: Optional["SecretsLoader"] = None,
         ref: Optional[InstanceRef] = None,
+        **_kwargs: Any,  # we accept kwargs for forward-compat of custom instances
     ):
         from dagster._core.launcher import RunLauncher
         from dagster._core.run_coordinator import RunCoordinator
         from dagster._core.scheduler import Scheduler
         from dagster._core.secrets import SecretsLoader
         from dagster._core.storage.captured_log_manager import CapturedLogManager
         from dagster._core.storage.compute_log_manager import ComputeLogManager
@@ -1132,17 +1131,17 @@
         run_config: Optional[Mapping[str, object]],
         resolved_op_selection: Optional[AbstractSet[str]],
         step_keys_to_execute: Optional[Sequence[str]],
         status: Optional[DagsterRunStatus],
         tags: Mapping[str, str],
         root_run_id: Optional[str],
         parent_run_id: Optional[str],
-        job_snapshot: Optional[JobSnapshot],
-        execution_plan_snapshot: Optional[ExecutionPlanSnapshot],
-        parent_job_snapshot: Optional[JobSnapshot],
+        job_snapshot: Optional["JobSnapshot"],
+        execution_plan_snapshot: Optional["ExecutionPlanSnapshot"],
+        parent_job_snapshot: Optional["JobSnapshot"],
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
         op_selection: Optional[Sequence[str]] = None,
         external_job_origin: Optional["ExternalJobOrigin"] = None,
         job_code_origin: Optional[JobPythonOrigin] = None,
     ) -> DagsterRun:
         # https://github.com/dagster-io/dagster/issues/2403
         if tags and IS_AIRFLOW_INGEST_PIPELINE_STR in tags:
@@ -1330,17 +1329,17 @@
         run_id: Optional[str],
         run_config: Optional[Mapping[str, object]],
         status: Optional[DagsterRunStatus],
         tags: Optional[Mapping[str, Any]],
         root_run_id: Optional[str],
         parent_run_id: Optional[str],
         step_keys_to_execute: Optional[Sequence[str]],
-        execution_plan_snapshot: Optional[ExecutionPlanSnapshot],
-        job_snapshot: Optional[JobSnapshot],
-        parent_job_snapshot: Optional[JobSnapshot],
+        execution_plan_snapshot: Optional["ExecutionPlanSnapshot"],
+        job_snapshot: Optional["JobSnapshot"],
+        parent_job_snapshot: Optional["JobSnapshot"],
         asset_selection: Optional[AbstractSet[AssetKey]],
         resolved_op_selection: Optional[AbstractSet[str]],
         op_selection: Optional[Sequence[str]],
         external_job_origin: Optional["ExternalJobOrigin"],
         job_code_origin: Optional[JobPythonOrigin],
     ) -> DagsterRun:
         from dagster._core.definitions.utils import validate_tags
@@ -1560,17 +1559,17 @@
         run_id: str,
         run_config: Optional[Mapping[str, object]],
         resolved_op_selection: Optional[AbstractSet[str]],
         step_keys_to_execute: Optional[Sequence[str]],
         tags: Mapping[str, str],
         root_run_id: Optional[str],
         parent_run_id: Optional[str],
-        job_snapshot: Optional[JobSnapshot],
-        execution_plan_snapshot: Optional[ExecutionPlanSnapshot],
-        parent_job_snapshot: Optional[JobSnapshot],
+        job_snapshot: Optional["JobSnapshot"],
+        execution_plan_snapshot: Optional["ExecutionPlanSnapshot"],
+        parent_job_snapshot: Optional["JobSnapshot"],
         op_selection: Optional[Sequence[str]] = None,
         job_code_origin: Optional[JobPythonOrigin] = None,
     ) -> DagsterRun:
         # The usage of this method is limited to dagster-airflow, specifically in Dagster
         # Operators that are executed in Airflow. Because a common workflow in Airflow is to
         # retry dags from arbitrary tasks, we need any node to be capable of creating a
         # DagsterRun.
@@ -1723,28 +1722,28 @@
     @traced
     def logs_after(
         self,
         run_id: str,
         cursor: Optional[int] = None,
         of_type: Optional["DagsterEventType"] = None,
         limit: Optional[int] = None,
-    ) -> Sequence[EventLogEntry]:
+    ) -> Sequence["EventLogEntry"]:
         return self._event_storage.get_logs_for_run(
             run_id,
             cursor=cursor,
             of_type=of_type,
             limit=limit,
         )
 
     @traced
     def all_logs(
         self,
         run_id: str,
         of_type: Optional[Union["DagsterEventType", Set["DagsterEventType"]]] = None,
-    ) -> Sequence[EventLogEntry]:
+    ) -> Sequence["EventLogEntry"]:
         return self._event_storage.get_logs_for_run(run_id, of_type=of_type)
 
     @traced
     def get_records_for_run(
         self,
         run_id: str,
         cursor: Optional[str] = None,
@@ -1856,16 +1855,16 @@
 
     @public
     @traced
     def get_status_by_partition(
         self,
         asset_key: AssetKey,
         partition_keys: Sequence[str],
-        partitions_def: PartitionsDefinition,
-    ) -> Optional[Mapping[str, AssetPartitionStatus]]:
+        partitions_def: "PartitionsDefinition",
+    ) -> Optional[Mapping[str, "AssetPartitionStatus"]]:
         """Get the current status of provided partition_keys for the provided asset.
 
         Args:
             asset_key (AssetKey): The asset to get per-partition status for.
             partition_keys (Sequence[str]): The partitions to get status for.
             partitions_def (PartitionsDefinition): The PartitionsDefinition of the asset to get
                 per-partition status for.
@@ -1962,15 +1961,15 @@
     def get_materialization_count_by_partition(
         self, asset_keys: Sequence[AssetKey], after_cursor: Optional[int] = None
     ) -> Mapping[AssetKey, Mapping[str, int]]:
         return self._event_storage.get_materialization_count_by_partition(asset_keys, after_cursor)
 
     @traced
     def get_latest_storage_id_by_partition(
-        self, asset_key: AssetKey, event_type: DagsterEventType
+        self, asset_key: AssetKey, event_type: "DagsterEventType"
     ) -> Mapping[str, int]:
         """Fetch the latest materialzation storage id for each partition for a given asset key.
 
         Returns a mapping of partition to storage id.
         """
         return self._event_storage.get_latest_storage_id_by_partition(asset_key, event_type)
 
@@ -2071,18 +2070,18 @@
         return event_log_handler
 
     def get_handlers(self) -> Sequence[logging.Handler]:
         handlers: List[logging.Handler] = [self._get_event_log_handler()]
         handlers.extend(self._get_yaml_python_handlers())
         return handlers
 
-    def store_event(self, event: EventLogEntry) -> None:
+    def store_event(self, event: "EventLogEntry") -> None:
         self._event_storage.store_event(event)
 
-    def handle_new_event(self, event: EventLogEntry) -> None:
+    def handle_new_event(self, event: "EventLogEntry") -> None:
         run_id = event.run_id
 
         self._event_storage.store_event(event)
 
         if event.is_dagster_event and event.get_dagster_event().is_job_event:
             self._run_storage.handle_run_event(run_id, event.get_dagster_event())
 
@@ -2092,20 +2091,20 @@
     def add_event_listener(self, run_id: str, cb) -> None:
         self._subscribers[run_id].append(cb)
 
     def report_engine_event(
         self,
         message: str,
         dagster_run: Optional[DagsterRun] = None,
-        engine_event_data: Optional[EngineEventData] = None,
+        engine_event_data: Optional["EngineEventData"] = None,
         cls: Optional[Type[object]] = None,
         step_key: Optional[str] = None,
         job_name: Optional[str] = None,
         run_id: Optional[str] = None,
-    ) -> DagsterEvent:
+    ) -> "DagsterEvent":
         """Report a EngineEvent that occurred outside of a job execution context."""
         from dagster._core.events import DagsterEvent, DagsterEventType, EngineEventData
 
         check.opt_class_param(cls, "cls")
         check.str_param(message, "message")
         check.opt_inst_param(dagster_run, "dagster_run", DagsterRun)
         check.opt_str_param(run_id, "run_id")
@@ -2181,15 +2180,15 @@
         )
         self.report_dagster_event(canceling_event, run_id=run.run_id)
 
     def report_run_canceled(
         self,
         dagster_run: DagsterRun,
         message: Optional[str] = None,
-    ) -> DagsterEvent:
+    ) -> "DagsterEvent":
         from dagster._core.events import DagsterEvent, DagsterEventType
 
         check.inst_param(dagster_run, "dagster_run", DagsterRun)
 
         message = check.opt_str_param(
             message,
             "mesage",
@@ -2202,15 +2201,15 @@
             message=message,
         )
         self.report_dagster_event(dagster_event, run_id=dagster_run.run_id, log_level=logging.ERROR)
         return dagster_event
 
     def report_run_failed(
         self, dagster_run: DagsterRun, message: Optional[str] = None
-    ) -> DagsterEvent:
+    ) -> "DagsterEvent":
         from dagster._core.events import DagsterEvent, DagsterEventType
 
         check.inst_param(dagster_run, "dagster_run", DagsterRun)
 
         message = check.opt_str_param(
             message,
             "message",
@@ -2393,23 +2392,23 @@
     def run_will_resume(self, run_id: str) -> bool:
         if not self.run_monitoring_enabled:
             return False
         return self.count_resume_run_attempts(run_id) < self.run_monitoring_max_resume_run_attempts
 
     # Scheduler
 
-    def start_schedule(self, external_schedule: "ExternalSchedule") -> InstigatorState:
+    def start_schedule(self, external_schedule: "ExternalSchedule") -> "InstigatorState":
         return self._scheduler.start_schedule(self, external_schedule)  # type: ignore
 
     def stop_schedule(
         self,
         schedule_origin_id: str,
         schedule_selector_id: str,
         external_schedule: Optional["ExternalSchedule"],
-    ) -> InstigatorState:
+    ) -> "InstigatorState":
         return self._scheduler.stop_schedule(  # type: ignore
             self, schedule_origin_id, schedule_selector_id, external_schedule
         )
 
     def scheduler_debug_info(self) -> "SchedulerDebugInfo":
         from dagster._core.definitions.run_request import InstigatorType
         from dagster._core.scheduler import SchedulerDebugInfo
@@ -2434,15 +2433,15 @@
             scheduler_info=self.scheduler.debug_info(),  # type: ignore
             schedule_storage=schedules,
             errors=errors,
         )
 
     # Schedule / Sensor Storage
 
-    def start_sensor(self, external_sensor: "ExternalSensor") -> InstigatorState:
+    def start_sensor(self, external_sensor: "ExternalSensor") -> "InstigatorState":
         from dagster._core.definitions.run_request import InstigatorType
         from dagster._core.scheduler.instigation import (
             InstigatorState,
             InstigatorStatus,
             SensorInstigatorData,
         )
 
@@ -2467,15 +2466,15 @@
             return self.update_instigator_state(stored_state.with_status(InstigatorStatus.RUNNING))
 
     def stop_sensor(
         self,
         instigator_origin_id: str,
         selector_id: str,
         external_sensor: Optional["ExternalSensor"],
-    ) -> InstigatorState:
+    ) -> "InstigatorState":
         from dagster._core.definitions.run_request import InstigatorType
         from dagster._core.scheduler.instigation import (
             InstigatorState,
             InstigatorStatus,
             SensorInstigatorData,
         )
 
@@ -2503,16 +2502,16 @@
             return self.update_instigator_state(stored_state.with_status(InstigatorStatus.STOPPED))
 
     @traced
     def all_instigator_state(
         self,
         repository_origin_id: Optional[str] = None,
         repository_selector_id: Optional[str] = None,
-        instigator_type: Optional[InstigatorType] = None,
-        instigator_statuses: Optional[Set[InstigatorStatus]] = None,
+        instigator_type: Optional["InstigatorType"] = None,
+        instigator_statuses: Optional[Set["InstigatorStatus"]] = None,
     ):
         if not self._schedule_storage:
             check.failed("Schedule storage not available")
         return self._schedule_storage.all_instigator_state(
             repository_origin_id, repository_selector_id, instigator_type, instigator_statuses
         )
 
@@ -2549,30 +2548,30 @@
         if not self._schedule_storage:
             return {}
         return self._schedule_storage.get_batch_ticks(selector_ids, limit, statuses)
 
     @traced
     def get_tick(
         self, origin_id: str, selector_id: str, timestamp: float
-    ) -> Optional[InstigatorTick]:
+    ) -> Optional["InstigatorTick"]:
         matches = self._schedule_storage.get_ticks(  # type: ignore  # (possible none)
             origin_id, selector_id, before=timestamp + 1, after=timestamp - 1, limit=1
         )
         return matches[0] if len(matches) else None
 
     @traced
     def get_ticks(
         self,
         origin_id: str,
         selector_id: str,
         before: Optional[float] = None,
         after: Optional[float] = None,
         limit: Optional[int] = None,
-        statuses: Optional[Sequence[TickStatus]] = None,
-    ) -> Sequence[InstigatorTick]:
+        statuses: Optional[Sequence["TickStatus"]] = None,
+    ) -> Sequence["InstigatorTick"]:
         return self._schedule_storage.get_ticks(  # type: ignore  # (possible none)
             origin_id, selector_id, before=before, after=after, limit=limit, statuses=statuses
         )
 
     def create_tick(self, tick_data: "TickData") -> "InstigatorTick":
         return check.not_none(self._schedule_storage).create_tick(tick_data)
 
@@ -2580,15 +2579,15 @@
         return check.not_none(self._schedule_storage).update_tick(tick)
 
     def purge_ticks(
         self,
         origin_id: str,
         selector_id: str,
         before: float,
-        tick_statuses: Optional[Sequence[TickStatus]] = None,
+        tick_statuses: Optional[Sequence["TickStatus"]] = None,
     ) -> None:
         self._schedule_storage.purge_ticks(origin_id, selector_id, before, tick_statuses)  # type: ignore  # (possible none)
 
     def wipe_all_schedules(self) -> None:
         if self._scheduler:
             self._scheduler.wipe(self)  # type: ignore  # (possible none)
 
@@ -2717,15 +2716,15 @@
         for k, v in new_env.items():
             os.environ[k] = v
 
     def get_latest_data_version_record(
         self,
         key: AssetKey,
         is_source: Optional[bool] = None,
-    ) -> Optional[EventLogRecord]:
+    ) -> Optional["EventLogRecord"]:
         from dagster._core.event_api import EventRecordsFilter
         from dagster._core.events import DagsterEventType
 
         # When we cant don't know whether the requested key corresponds to a source or regular
         # asset, we need to retrieve both the latest observation and materialization for all assets.
         # If there is a materialization, it's a regular asset and we can ignore the observation.
```

### Comparing `dagster-1.4.2/dagster/_core/instance/config.py` & `dagster-1.4.3/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/instance/ref.py` & `dagster-1.4.3/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/instance_for_test.py` & `dagster-1.4.3/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/launcher/base.py` & `dagster-1.4.3/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.4.3/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.4.3/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/log_manager.py` & `dagster-1.4.3/dagster/_core/log_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from __future__ import annotations
-
 import datetime
 import logging
 from typing import TYPE_CHECKING, Any, Mapping, NamedTuple, Optional, Sequence, Union, cast
 
 from typing_extensions import Protocol
 
 import dagster._check as check
-from dagster._core.storage.dagster_run import DagsterRun
 from dagster._core.utils import coerce_valid_log_level, make_new_run_id
 from dagster._utils.log import get_dagster_logger
 
 if TYPE_CHECKING:
     from dagster import DagsterInstance
     from dagster._core.events import DagsterEvent
+    from dagster._core.storage.dagster_run import DagsterRun
 
 DAGSTER_META_KEY = "dagster_meta"
 
 
 class IDagsterMeta(Protocol):
     @property
-    def dagster_meta(self) -> DagsterLoggingMetadata:
+    def dagster_meta(self) -> "DagsterLoggingMetadata":
         ...
 
 
 # The type-checker complains here that DagsterLogRecord does not implement the `dagster_meta`
 # property of `IDagsterMeta`. We ignore this error because we don't need to implement this method--
 # `DagsterLogRecord` is a stub class that is never instantiated. We only ever cast
 # `logging.LogRecord` objects to `DagsterLogRecord`, because it gives us typed access to the
@@ -220,15 +218,15 @@
         self._should_capture = True
         super().__init__()
 
     @property
     def logging_metadata(self) -> DagsterLoggingMetadata:
         return self._logging_metadata
 
-    def with_tags(self, **new_tags: str) -> DagsterLogHandler:
+    def with_tags(self, **new_tags: str) -> "DagsterLogHandler":
         return DagsterLogHandler(
             logging_metadata=self.logging_metadata._replace(**new_tags),
             loggers=self._loggers,
             handlers=self._handlers,
         )
 
     def _extract_extra(self, record: logging.LogRecord) -> Mapping[str, Any]:
@@ -419,15 +417,15 @@
             *args: the logged message will be msg % args
         """
         level = coerce_valid_log_level(level)
         # log DagsterEvents regardless of level
         if self.isEnabledFor(level) or ("extra" in kwargs and DAGSTER_META_KEY in kwargs["extra"]):
             self._log(level, msg, args, **kwargs)
 
-    def with_tags(self, **new_tags: str) -> DagsterLogManager:
+    def with_tags(self, **new_tags: str) -> "DagsterLogManager":
         """Add new tags in "new_tags" to the set of tags attached to this log manager instance, and
         return a new DagsterLogManager with the merged set of tags.
 
         Args:
             new_tags (Dict[str,str]): Dictionary of tags
 
         Returns:
```

### Comparing `dagster-1.4.2/dagster/_core/nux.py` & `dagster-1.4.3/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/origin.py` & `dagster-1.4.3/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/run_coordinator/base.py` & `dagster-1.4.3/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.4.3/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.4.3/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/scheduler/__init__.py` & `dagster-1.4.3/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/scheduler/execution.py` & `dagster-1.4.3/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/scheduler/instigation.py` & `dagster-1.4.3/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/scheduler/scheduler.py` & `dagster-1.4.3/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/secrets/env_file.py` & `dagster-1.4.3/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/selector/subset_selector.py` & `dagster-1.4.3/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/snap/__init__.py` & `dagster-1.4.3/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/snap/dagster_types.py` & `dagster-1.4.3/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/snap/dep_snapshot.py` & `dagster-1.4.3/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.4.3/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/snap/job_snapshot.py` & `dagster-1.4.3/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/snap/mode.py` & `dagster-1.4.3/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/snap/node.py` & `dagster-1.4.3/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.4.3/dagster/_core/snap/snap_to_yaml.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,30 +23,14 @@
         return {k: v for k, v in filtered_dict.items() if v is not None and v != {}}
 
 
 def _cleanup_run_config_dict(run_config_dict: Any) -> Any:
     """Performs cleanup of the run config dict to remove empty dicts and strip the default executor
     config if it has not been overridden, to make the output more readable.
     """
-    # We manually strip the default executor config because
-    # the max_concurrent default value is a sentinel and can be confusing
-    # if presented to the user:
-    # execution:
-    #   config:
-    #     multiprocess:
-    #       max_concurrent: 0
-    if (
-        run_config_dict.get("execution", {})
-        .get("config", {})
-        .get("multiprocess", {})
-        .get("max_concurrent", None)
-        == 0
-    ):
-        del run_config_dict["execution"]["config"]["multiprocess"]["max_concurrent"]
-
     return _filter_empty_dicts(run_config_dict)
 
 
 def default_values_yaml_from_type_snap(
     snapshot: ConfigSchemaSnapshot,
     type_snap: ConfigTypeSnap,
 ) -> str:
```

### Comparing `dagster-1.4.2/dagster/_core/storage/DEVELOPING.md` & `dagster-1.4.3/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/README.md` & `dagster-1.4.3/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/env.py` & `dagster-1.4.3/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.4.3/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/asset_value_loader.py` & `dagster-1.4.3/dagster/_core/storage/asset_value_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,58 +71,62 @@
     @public
     def load_asset_value(
         self,
         asset_key: CoercibleToAssetKey,
         *,
         python_type: Optional[Type[object]] = None,
         partition_key: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
         resource_config: Optional[Any] = None,
     ) -> object:
         """Loads the contents of an asset as a Python object.
 
         Invokes `load_input` on the :py:class:`IOManager` associated with the asset.
 
         Args:
             asset_key (Union[AssetKey, Sequence[str], str]): The key of the asset to load.
             python_type (Optional[Type]): The python type to load the asset as. This is what will
                 be returned inside `load_input` by `context.dagster_type.typing_type`.
             partition_key (Optional[str]): The partition of the asset to load.
+            metadata (Optional[Dict[str, Any]]): Input metadata to pass to the :py:class:`IOManager`
+                (is equivalent to setting the metadata argument in `In` or `AssetIn`).
             resource_config (Optional[Any]): A dictionary of resource configurations to be passed
                 to the :py:class:`IOManager`.
 
         Returns:
             The contents of an asset as a Python object.
         """
         asset_key = AssetKey.from_coercible(asset_key)
         resource_config = resource_config or {}
+        output_metadata = {}
 
         if asset_key in self._assets_defs_by_key:
             assets_def = self._assets_defs_by_key[asset_key]
 
             resource_defs = merge_dicts(
                 {DEFAULT_IO_MANAGER_KEY: default_job_io_manager_with_fs_io_manager_schema},
                 assets_def.resource_defs,
             )
             io_manager_key = assets_def.get_io_manager_key_for_asset_key(asset_key)
             io_manager_def = resource_defs[io_manager_key]
             name = assets_def.get_output_name_for_asset_key(asset_key)
-            metadata = assets_def.metadata_by_key[asset_key]
+            output_metadata = assets_def.metadata_by_key[asset_key]
             op_def = assets_def.get_op_def_for_asset_key(asset_key)
             asset_partitions_def = assets_def.partitions_def
         elif asset_key in self._source_assets_by_key:
             source_asset = self._source_assets_by_key[asset_key]
 
             resource_defs = merge_dicts(
                 {DEFAULT_IO_MANAGER_KEY: default_job_io_manager_with_fs_io_manager_schema},
                 source_asset.resource_defs,
             )
             io_manager_key = source_asset.get_io_manager_key()
             io_manager_def = resource_defs[io_manager_key]
             name = asset_key.path[-1]
-            metadata = source_asset.raw_metadata
+            output_metadata = source_asset.raw_metadata
             op_def = None
             asset_partitions_def = source_asset.partitions_def
         else:
             check.failed(f"Asset key {asset_key} not found")
 
         required_resource_keys = get_transitive_required_resource_keys(
             io_manager_def.required_resource_keys, resource_defs
@@ -143,27 +147,28 @@
 
         input_context = build_input_context(
             name=None,
             asset_key=asset_key,
             dagster_type=resolve_dagster_type(python_type),
             upstream_output=build_output_context(
                 name=name,
-                metadata=metadata,
+                metadata=output_metadata,
                 asset_key=asset_key,
                 op_def=op_def,
                 resource_config=resource_config,
             ),
             resources=self._resource_instance_cache,
             resource_config=io_manager_config[io_manager_key].config,
             partition_key=partition_key,
             asset_partition_key_range=PartitionKeyRange(partition_key, partition_key)
             if partition_key is not None
             else None,
             asset_partitions_def=asset_partitions_def,
             instance=self._instance,
+            metadata=metadata,
         )
 
         return io_manager.load_input(input_context)
 
     def __enter__(self):
         return self
```

### Comparing `dagster-1.4.2/dagster/_core/storage/base_storage.py` & `dagster-1.4.3/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.4.3/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/captured_log_manager.py` & `dagster-1.4.3/dagster/_core/storage/captured_log_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from typing import IO, Callable, Generator, Iterator, NamedTuple, Optional, Sequence
 
 from typing_extensions import Final, Self
 
 import dagster._check as check
@@ -103,15 +101,17 @@
             stderr_location=stderr_location,
             stdout_download_url=stdout_download_url,
             stderr_download_url=stderr_download_url,
         )
 
 
 class CapturedLogSubscription:
-    def __init__(self, manager: CapturedLogManager, log_key: Sequence[str], cursor: Optional[str]):
+    def __init__(
+        self, manager: "CapturedLogManager", log_key: Sequence[str], cursor: Optional[str]
+    ):
         self._manager = manager
         self._log_key = log_key
         self._cursor = cursor
         self._observer: Optional[Callable[[CapturedLogData], None]] = None
         self.is_complete = False
 
     def __call__(self, observer: Optional[Callable[[CapturedLogData], None]]) -> Self:
```

### Comparing `dagster-1.4.2/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.4.3/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/compute_log_manager.py` & `dagster-1.4.3/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/config.py` & `dagster-1.4.3/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/dagster_run.py` & `dagster-1.4.3/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/db_io_manager.py` & `dagster-1.4.3/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/event_log/__init__.py` & `dagster-1.4.3/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/event_log/base.py` & `dagster-1.4.3/dagster/_core/storage/event_log/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 )
 
 import dagster._check as check
 from dagster._core.assets import AssetDetails
 from dagster._core.definitions.events import AssetKey
 from dagster._core.event_api import EventHandlerFn, EventLogRecord, EventRecordsFilter
 from dagster._core.events import DagsterEventType
-from dagster._core.events.log import EventLogEntry
 from dagster._core.execution.stats import (
     RunStepKeyStatsSnapshot,
     build_run_stats_from_events,
     build_run_step_stats_from_events,
 )
 from dagster._core.instance import MayHaveInstanceWeakref, T_DagsterInstance
 from dagster._core.storage.dagster_run import DagsterRunStatsSnapshot
 from dagster._core.storage.sql import AlembicVersion
 from dagster._seven import json
 from dagster._utils import PrintFn
 from dagster._utils.concurrency import ConcurrencyClaimStatus, ConcurrencyKeyInfo
 
 if TYPE_CHECKING:
+    from dagster._core.events.log import EventLogEntry
     from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
 
 
 class EventLogConnection(NamedTuple):
     records: Sequence[EventLogRecord]
     cursor: str
     has_more: bool
```

### Comparing `dagster-1.4.2/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.4.3/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/event_log/migration.py` & `dagster-1.4.3/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.4.3/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/event_log/schema.py` & `dagster-1.4.3/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.4.3/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from dagster._core.errors import (
     DagsterEventLogInvalidForRun,
     DagsterInvalidInvocationError,
     DagsterInvariantViolationError,
 )
 from dagster._core.event_api import RunShardedEventsCursor
 from dagster._core.events import ASSET_EVENTS, MARKER_EVENTS, DagsterEventType
+from dagster._core.events.log import EventLogEntry
 from dagster._core.execution.stats import RunStepKeyStatsSnapshot, build_run_step_stats_from_events
 from dagster._core.storage.sql import SqlAlchemyQuery, SqlAlchemyRow
 from dagster._core.storage.sqlalchemy_compat import (
     db_case,
     db_fetch_mappings,
     db_select,
     db_subquery,
@@ -63,15 +64,14 @@
 
 from ..dagster_run import DagsterRunStatsSnapshot
 from .base import (
     AssetEntry,
     AssetRecord,
     EventLogConnection,
     EventLogCursor,
-    EventLogEntry,
     EventLogRecord,
     EventLogStorage,
     EventRecordsFilter,
 )
 from .migration import ASSET_DATA_MIGRATIONS, ASSET_KEY_INDEX_COLS, EVENT_LOG_DATA_MIGRATIONS
 from .schema import (
     AssetEventTagsTable,
```

### Comparing `dagster-1.4.2/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.4.3/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.4.3/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.4.3/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/file_manager.py` & `dagster-1.4.3/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/fs_io_manager.py` & `dagster-1.4.3/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/input_manager.py` & `dagster-1.4.3/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/io_manager.py` & `dagster-1.4.3/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/legacy_storage.py` & `dagster-1.4.3/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.4.3/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/mem_io_manager.py` & `dagster-1.4.3/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.4.3/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/migration/utils.py` & `dagster-1.4.3/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.4.3/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/output_manager.py` & `dagster-1.4.3/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/partition_status_cache.py` & `dagster-1.4.3/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/root.py` & `dagster-1.4.3/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/runs/base.py` & `dagster-1.4.3/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/runs/in_memory.py` & `dagster-1.4.3/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/runs/migration.py` & `dagster-1.4.3/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/runs/schema.py` & `dagster-1.4.3/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.4.3/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.4.3/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.4.3/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/schedules/base.py` & `dagster-1.4.3/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/schedules/migration.py` & `dagster-1.4.3/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/schedules/schema.py` & `dagster-1.4.3/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.4.3/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.4.3/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.4.3/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/sql.py` & `dagster-1.4.3/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.4.3/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/sqlite.py` & `dagster-1.4.3/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/sqlite_storage.py` & `dagster-1.4.3/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/tags.py` & `dagster-1.4.3/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/temp_file_manager.py` & `dagster-1.4.3/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/storage/upath_io_manager.py` & `dagster-1.4.3/dagster/_core/storage/upath_io_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,29 +251,34 @@
             else:
                 raise e
 
         context.add_input_metadata({"path": MetadataValue.path(str(path))})
         return obj
 
     def _load_partition_from_path(
-        self, context: InputContext, path: "UPath", backcompat_path: Optional["UPath"] = None
+        self,
+        context: InputContext,
+        partition_key: str,
+        path: "UPath",
+        backcompat_path: Optional["UPath"] = None,
     ) -> Any:
         """1. Try to load the partition from the normal path.
         2. If it was not found, try to load it from the backcompat path.
         3. If allow_missing_partitions metadata is True, skip the partition if it was not found in any of the paths.
         Otherwise, raise an error.
 
         Args:
+            context (InputContext): IOManager Input context
+            partition_key (str): the partition key corresponding to the partition being loaded
             path (UPath): The path to the partition.
             backcompat_path (Optional[UPath]): The path to the partition in the backcompat location.
 
         Returns:
             Any: The object loaded from the partition.
         """
-        partition_key = context.partition_key
         allow_missing_partitions = (
             context.metadata.get("allow_missing_partitions", False)
             if context.metadata is not None
             else False
         )
 
         try:
@@ -311,15 +316,18 @@
         context.log.debug(f"Loading {len(paths)} partitions...")
 
         objs = {}
 
         if not inspect.iscoroutinefunction(self.load_from_path):
             for partition_key in context.asset_partition_keys:
                 obj = self._load_partition_from_path(
-                    context, paths[partition_key], backcompat_paths.get(partition_key)
+                    context,
+                    partition_key,
+                    paths[partition_key],
+                    backcompat_paths.get(partition_key),
                 )
                 if obj is not None:  # in case some partitions were skipped
                     objs[partition_key] = obj
             return objs
         else:
             # load_from_path returns a coroutine, so we need to await the results
 
@@ -328,15 +336,18 @@
 
                 tasks = []
 
                 for partition_key in context.asset_partition_keys:
                     tasks.append(
                         loop.create_task(
                             self._load_partition_from_path(
-                                context, paths[partition_key], backcompat_paths.get(partition_key)
+                                context,
+                                partition_key,
+                                paths[partition_key],
+                                backcompat_paths.get(partition_key),
                             )
                         )
                     )
 
                 results = await asyncio.gather(*tasks, return_exceptions=True)
 
                 # need to handle missing partitions here because exceptions don't get propagated from async calls
```

### Comparing `dagster-1.4.2/dagster/_core/system_config/composite_descent.py` & `dagster-1.4.3/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/system_config/objects.py` & `dagster-1.4.3/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/telemetry.py` & `dagster-1.4.3/dagster/_core/telemetry.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 import click
 import yaml
 from typing_extensions import ParamSpec
 
 import dagster._check as check
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicyType
+from dagster._core.definitions.backfill_policy import BackfillPolicyType
 from dagster._core.definitions.job_base import IJob
 from dagster._core.definitions.reconstruct import (
     ReconstructableJob,
     ReconstructableRepository,
     get_ephemeral_repository_name,
 )
 from dagster._core.errors import DagsterInvariantViolationError
@@ -473,14 +474,16 @@
 
     num_partitioned_assets_in_repo = 0
     num_multi_partitioned_assets_in_repo = 0
     num_dynamic_partitioned_assets_in_repo = 0
     num_assets_with_freshness_policies_in_repo = 0
     num_assets_with_eager_auto_materialize_policies_in_repo = 0
     num_assets_with_lazy_auto_materialize_policies_in_repo = 0
+    num_assets_with_single_run_backfill_policies_in_repo = 0
+    num_assets_with_multi_run_backfill_policies_in_repo = 0
     num_source_assets_in_repo = 0
     num_observable_source_assets_in_repo = 0
     num_dbt_assets_in_repo = 0
     num_assets_with_code_versions_in_repo = 0
 
     for asset in external_asset_nodes:
         if asset.partitions_def_data:
@@ -497,14 +500,20 @@
 
         if asset.auto_materialize_policy is not None:
             if asset.auto_materialize_policy.policy_type == AutoMaterializePolicyType.EAGER:
                 num_assets_with_eager_auto_materialize_policies_in_repo += 1
             else:
                 num_assets_with_lazy_auto_materialize_policies_in_repo += 1
 
+        if asset.backfill_policy is not None:
+            if asset.backfill_policy.policy_type == BackfillPolicyType.SINGLE_RUN:
+                num_assets_with_single_run_backfill_policies_in_repo += 1
+            else:
+                num_assets_with_multi_run_backfill_policies_in_repo += 1
+
         if asset.is_source:
             num_source_assets_in_repo += 1
 
             if asset.is_observable:
                 num_observable_source_assets_in_repo += 1
 
         if asset.code_version is not None:
@@ -534,14 +543,20 @@
         ),
         "num_assets_with_eager_auto_materialize_policies_in_repo": str(
             num_assets_with_eager_auto_materialize_policies_in_repo
         ),
         "num_assets_with_lazy_auto_materialize_policies_in_repo": str(
             num_assets_with_lazy_auto_materialize_policies_in_repo
         ),
+        "num_assets_with_single_run_backfill_policies_in_repo": str(
+            num_assets_with_single_run_backfill_policies_in_repo
+        ),
+        "num_assets_with_multi_run_backfill_policies_in_repo": str(
+            num_assets_with_multi_run_backfill_policies_in_repo
+        ),
         "num_observable_source_assets_in_repo": str(num_observable_source_assets_in_repo),
         "num_dbt_assets_in_repo": str(num_dbt_assets_in_repo),
         "num_assets_with_code_versions_in_repo": str(num_assets_with_code_versions_in_repo),
         "num_asset_reconciliation_sensors_in_repo": str(num_asset_reconciliation_sensors_in_repo),
     }
```

### Comparing `dagster-1.4.2/dagster/_core/telemetry_upload.py` & `dagster-1.4.3/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/test_utils.py` & `dagster-1.4.3/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.4.3/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/types/config_schema.py` & `dagster-1.4.3/dagster/_core/types/config_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import hashlib
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, AbstractSet, Any, Callable, Iterator, Optional, cast
 
 from typing_extensions import TypeAlias
 
 import dagster._check as check
```

### Comparing `dagster-1.4.2/dagster/_core/types/dagster_type.py` & `dagster-1.4.3/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/types/decorator.py` & `dagster-1.4.3/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/types/loadable_target_origin.py` & `dagster-1.4.3/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/types/primitive_mapping.py` & `dagster-1.4.3/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/types/python_dict.py` & `dagster-1.4.3/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/types/python_set.py` & `dagster-1.4.3/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/types/python_tuple.py` & `dagster-1.4.3/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/types/transform_typing.py` & `dagster-1.4.3/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/utility_ops.py` & `dagster-1.4.3/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/utils.py` & `dagster-1.4.3/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/workspace/autodiscovery.py` & `dagster-1.4.3/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/workspace/config_schema.py` & `dagster-1.4.3/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/workspace/context.py` & `dagster-1.4.3/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/workspace/load.py` & `dagster-1.4.3/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/workspace/load_target.py` & `dagster-1.4.3/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/workspace/permissions.py` & `dagster-1.4.3/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_core/workspace/workspace.py` & `dagster-1.4.3/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/__init__.py` & `dagster-1.4.3/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/asset_daemon.py` & `dagster-1.4.3/dagster/_daemon/asset_daemon.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import Optional
 
 import pendulum
 
 import dagster._check as check
-from dagster._core.definitions.asset_reconciliation_sensor import (
-    AssetReconciliationCursor,
-    reconcile,
-)
+from dagster._core.definitions.asset_daemon_cursor import AssetDaemonCursor
+from dagster._core.definitions.asset_reconciliation_sensor import reconcile
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.definitions.selector import JobSubsetSelector
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus
 from dagster._core.storage.tags import (
     ASSET_EVALUATION_ID_TAG,
@@ -44,19 +42,15 @@
 
 def _get_raw_cursor(instance: DagsterInstance) -> Optional[str]:
     return instance.daemon_cursor_storage.get_cursor_values({CURSOR_KEY}).get(CURSOR_KEY)
 
 
 def get_current_evaluation_id(instance: DagsterInstance) -> Optional[int]:
     raw_cursor = _get_raw_cursor(instance)
-    return (
-        AssetReconciliationCursor.get_evaluation_id_from_serialized(raw_cursor)
-        if raw_cursor
-        else None
-    )
+    return AssetDaemonCursor.get_evaluation_id_from_serialized(raw_cursor) if raw_cursor else None
 
 
 class AssetDaemon(IntervalDaemon):
     def __init__(self, interval_seconds: int):
         super().__init__(interval_seconds=interval_seconds)
 
     @classmethod
@@ -99,17 +93,17 @@
 
         if not target_asset_keys and not has_auto_observe_assets:
             yield
             return
 
         raw_cursor = _get_raw_cursor(instance)
         cursor = (
-            AssetReconciliationCursor.from_serialized(raw_cursor, asset_graph)
+            AssetDaemonCursor.from_serialized(raw_cursor, asset_graph)
             if raw_cursor
-            else AssetReconciliationCursor.empty()
+            else AssetDaemonCursor.empty()
         )
 
         run_requests, new_cursor, evaluations = reconcile(
             asset_graph=asset_graph,
             target_asset_keys=target_asset_keys,
             instance=instance,
             cursor=cursor,
```

### Comparing `dagster-1.4.2/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.4.3/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.4.3/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
 import os
-from typing import Callable, Dict, Iterator, List, Mapping, Optional, Sequence
+from typing import TYPE_CHECKING, Callable, Dict, Iterator, List, Mapping, Optional, Sequence
 
 import dagster._check as check
 from dagster import DagsterEventType
-from dagster._core.events.log import EventLogEntry
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.dagster_run import RunRecord, RunsFilter
 from dagster._core.workspace.context import IWorkspaceProcessContext
 
 from ..daemon import IntervalDaemon
 from .auto_run_reexecution import consume_new_runs_for_automatic_reexecution
 
+if TYPE_CHECKING:
+    from dagster._core.events.log import EventLogEntry
+
 _INTERVAL_SECONDS = int(os.environ.get("DAGSTER_EVENT_LOG_CONSUMER_DAEMON_INTERVAL_SECONDS", 5))
 _EVENT_LOG_FETCH_LIMIT = int(os.environ.get("DAGSTER_EVENT_LOG_CONSUMER_DAEMON_FETCH_LIMIT", 500))
 
 DAGSTER_EVENT_TYPES = [DagsterEventType.RUN_FAILURE, DagsterEventType.RUN_SUCCESS]
 
 
 class EventLogConsumerDaemon(IntervalDaemon):
```

### Comparing `dagster-1.4.2/dagster/_daemon/backfill.py` & `dagster-1.4.3/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/cli/__init__.py` & `dagster-1.4.3/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/controller.py` & `dagster-1.4.3/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/daemon.py` & `dagster-1.4.3/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.4.3/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.4.3/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.4.3/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/sensor.py` & `dagster-1.4.3/dagster/_daemon/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -895,16 +895,23 @@
 ):
     run_keys = [run_request.run_key for run_request in run_requests if run_request.run_key]
 
     if not run_keys:
         return {}
 
     # fetch runs from the DB with only the run key tag
-    # note: while possible to filter more at DB level with tags - it is avoided here due to observed perf problems
-    runs_with_run_keys = instance.get_runs(filters=RunsFilter(tags={RUN_KEY_TAG: run_keys}))
+    # note: while possible to filter more at DB level with tags - it is avoided here due to observed
+    # perf problems
+    runs_with_run_keys = []
+    for run_key in run_keys:
+        # do serial fetching, which has better perf than a single query with an IN clause, due to
+        # how the query planner does the runs/run_tags join
+        runs_with_run_keys.extend(
+            instance.get_runs(filters=RunsFilter(tags={RUN_KEY_TAG: run_key}))
+        )
 
     # filter down to runs with run_key that match the sensor name and its namespace (repository)
     valid_runs: List[DagsterRun] = []
     for run in runs_with_run_keys:
         # if the run doesn't have a set origin, just match on sensor name
         if (
             run.external_job_origin is None
```

### Comparing `dagster-1.4.2/dagster/_daemon/types.py` & `dagster-1.4.3/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_daemon/workspace.py` & `dagster-1.4.3/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_generate/download.py` & `dagster-1.4.3/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_generate/generate.py` & `dagster-1.4.3/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.4.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.4.3/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.4.3/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_grpc/__init__.py` & `dagster-1.4.3/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_grpc/client.py` & `dagster-1.4.3/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_grpc/compile.py` & `dagster-1.4.3/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_grpc/impl.py` & `dagster-1.4.3/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_grpc/protos/api.proto` & `dagster-1.4.3/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_grpc/proxy_server.py` & `dagster-1.4.3/dagster/_grpc/proxy_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from __future__ import annotations
-
 import logging
 import sys
 import threading
 from contextlib import ExitStack
-from typing import Dict, Optional
+from typing import TYPE_CHECKING, Dict, Optional
 
 import dagster._check as check
 from dagster._core.host_representation.grpc_server_registry import GrpcServerRegistry
 from dagster._core.host_representation.origin import (
     ManagedGrpcPythonEnvCodeLocationOrigin,
 )
 from dagster._core.instance import InstanceRef
 from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
-from dagster._grpc.client import DagsterGrpcClient
 from dagster._serdes import deserialize_value, serialize_value
 from dagster._utils.error import serializable_error_info_from_exc_info
 
 from .__generated__ import api_pb2
 from .__generated__.api_pb2_grpc import DagsterApiServicer
 from .types import (
     CancelExecutionRequest,
     CancelExecutionResult,
     ExecuteExternalJobArgs,
     ShutdownServerResult,
     StartRunResult,
 )
 
+if TYPE_CHECKING:
+    from dagster._grpc.client import DagsterGrpcClient
+
 CLEANUP_TICK = 1
 
 
 class DagsterProxyApiServicer(DagsterApiServicer):
     """Service that implements the dagster gRPC API by opening up a "dagster api grpc" subprocess, and proxying
     all gRPC calls to the server running in that subprocess. This allows us to reload code by
     restarting the subprocess without needing to restart the parent process.
```

### Comparing `dagster-1.4.2/dagster/_grpc/server.py` & `dagster-1.4.3/dagster/_grpc/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-from __future__ import annotations
-
 import json
 import logging
 import math
 import multiprocessing
 import os
 import queue
 import sys
 import threading
 import time
 import uuid
 import warnings
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import ExitStack
-from multiprocessing.synchronize import Event as MPEvent
-from subprocess import Popen
 from threading import Event as ThreadingEventType
 from time import sleep
-from typing import Any, Dict, Iterable, Iterator, List, Mapping, Optional, Sequence, Tuple, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    cast,
+)
 
 import grpc
 from grpc_health.v1 import health, health_pb2, health_pb2_grpc
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._core.code_pointer import CodePointer
@@ -86,14 +94,18 @@
     PartitionSetExecutionParamArgs,
     SensorExecutionArgs,
     ShutdownServerResult,
     StartRunResult,
 )
 from .utils import get_loadable_targets, max_rx_bytes, max_send_bytes
 
+if TYPE_CHECKING:
+    from multiprocessing.synchronize import Event as MPEvent
+    from subprocess import Popen
+
 EVENT_QUEUE_POLL_INTERVAL = 0.1
 
 CLEANUP_TICK = 0.5
 
 STREAMING_CHUNK_SIZE = 4000000
 
 
@@ -1066,15 +1078,15 @@
     fixed_server_id: Optional[str] = None,
     startup_timeout: int = 20,
     cwd: Optional[str] = None,
     log_level: str = "INFO",
     env: Optional[Dict[str, str]] = None,
     inject_env_vars_from_instance: bool = True,
     container_image: Optional[str] = None,
-    container_context: Optional[dict[str, Any]] = None,
+    container_context: Optional[Dict[str, Any]] = None,
 ):
     check.invariant((port or socket) and not (port and socket), "Set only port or socket")
     check.opt_inst_param(loadable_target_origin, "loadable_target_origin", LoadableTargetOrigin)
     check.opt_int_param(max_workers, "max_workers")
 
     executable_path = loadable_target_origin.executable_path if loadable_target_origin else None
 
@@ -1120,15 +1132,15 @@
 
     return server_process
 
 
 def _open_server_process_on_dynamic_port(
     max_retries: int = 10,
     **kwargs,
-) -> Tuple[Optional[Popen[str]], Optional[int]]:
+) -> Tuple[Optional["Popen[str]"], Optional[int]]:
     server_process = None
     retries = 0
     port = None
     while server_process is None and retries < max_retries:
         port = find_free_port()
         try:
             server_process = open_server_process(port=port, socket=None, **kwargs)
```

### Comparing `dagster-1.4.2/dagster/_grpc/server_watcher.py` & `dagster-1.4.3/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_grpc/types.py` & `dagster-1.4.3/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_grpc/utils.py` & `dagster-1.4.3/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_loggers/__init__.py` & `dagster-1.4.3/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_module_alias_map.py` & `dagster-1.4.3/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_scheduler/scheduler.py` & `dagster-1.4.3/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_scheduler/stale.py` & `dagster-1.4.3/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_serdes/__init__.py` & `dagster-1.4.3/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_serdes/config_class.py` & `dagster-1.4.3/dagster/_serdes/config_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,36 @@
 import importlib
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Mapping, NamedTuple, Optional, Type, TypeVar, Union, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Mapping,
+    NamedTuple,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+    overload,
+)
 
 from typing_extensions import Self
 
 import dagster._check as check
-from dagster._config.config_schema import UserConfigSchema
 from dagster._utils import convert_dagster_submodule_name
 from dagster._utils.yaml_utils import load_run_config_yaml
 
 from .serdes import (
     NamedTupleSerializer,
     whitelist_for_serdes,
 )
 
+if TYPE_CHECKING:
+    from dagster._config.config_schema import UserConfigSchema
+
 T_ConfigurableClass = TypeVar("T_ConfigurableClass")
 
 
 class ConfigurableClassDataSerializer(NamedTupleSerializer["ConfigurableClassData"]):
     def after_pack(self, **packed: Any) -> Dict[str, Any]:
         packed["module_name"] = convert_dagster_submodule_name(packed["module_name"], "public")
         return packed
```

### Comparing `dagster-1.4.2/dagster/_serdes/ipc.py` & `dagster-1.4.3/dagster/_serdes/ipc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import os
 import signal
 import subprocess
 import sys
 from contextlib import contextmanager
 from io import TextIOWrapper
 from subprocess import Popen
@@ -40,15 +38,15 @@
 def ipc_write_unary_response(output_file: str, obj: NamedTuple) -> None:
     check.not_none_param(obj, "obj")
     with ipc_write_stream(output_file) as stream:
         stream.send(obj)
 
 
 def read_unary_response(
-    output_file: str, timeout: int = 30, ipc_process: Optional[Popen[bytes]] = None
+    output_file: str, timeout: int = 30, ipc_process: "Optional[Popen[bytes]]" = None
 ) -> Optional[NamedTuple]:
     messages = list(ipc_read_event_stream(output_file, timeout=timeout, ipc_process=ipc_process))
     check.invariant(len(messages) == 1)
     return messages[0]
 
 
 @whitelist_for_serdes
@@ -137,27 +135,27 @@
     while True:
         line = file_pointer.readline()
         if line:
             return deserialize_value(line.rstrip(), NamedTuple)
         sleep(sleep_interval)
 
 
-def _poll_process(ipc_process: Optional[Popen[bytes]]) -> None:
+def _poll_process(ipc_process: "Optional[Popen[bytes]]") -> None:
     if not ipc_process:
         return
     if ipc_process.poll() is not None:
         raise DagsterIPCProtocolError(
             "Process exited with return code {return_code} while waiting for events".format(
                 return_code=ipc_process.returncode
             )
         )
 
 
 def ipc_read_event_stream(
-    file_path: str, timeout: int = 30, ipc_process: Optional[Popen[bytes]] = None
+    file_path: str, timeout: int = 30, ipc_process: "Optional[Popen[bytes]]" = None
 ) -> Iterator[Optional[NamedTuple]]:
     # Wait for file to be ready
     sleep_interval = 0.1
     elapsed_time = 0
     while elapsed_time < timeout and not os.path.exists(file_path):
         _poll_process(ipc_process)
         elapsed_time += sleep_interval
@@ -193,30 +191,30 @@
             message = _process_line(file_pointer)
 
 
 # Windows subprocess termination utilities
 # https://stefan.sofa-rockers.org/2013/08/15/handling-sub-process-hierarchies-python-linux-os-x/
 
 
-def open_ipc_subprocess(parts: Sequence[str], **kwargs: Any) -> Popen[bytes]:
+def open_ipc_subprocess(parts: Sequence[str], **kwargs: Any) -> "Popen[bytes]":
     """Sets the correct flags to support graceful termination."""
     check.list_param(parts, "parts", str)
 
     creationflags = 0
     if sys.platform == "win32":
         creationflags = subprocess.CREATE_NEW_PROCESS_GROUP
 
     return subprocess.Popen(  # type: ignore  # (unclear whether this is actually guaranteed to return Popen[bytes])
         parts,
         creationflags=creationflags,
         **kwargs,
     )
 
 
-def interrupt_ipc_subprocess(proc: Popen[bytes]) -> None:
+def interrupt_ipc_subprocess(proc: "Popen[bytes]") -> None:
     """Send CTRL_BREAK on Windows, SIGINT on other platforms."""
     if sys.platform == "win32":
         proc.send_signal(signal.CTRL_BREAK_EVENT)
     else:
         proc.send_signal(signal.SIGINT)
```

### Comparing `dagster-1.4.2/dagster/_serdes/serdes.py` & `dagster-1.4.3/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_serdes/utils.py` & `dagster-1.4.3/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_seven/__init__.py` & `dagster-1.4.3/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_seven/abc.py` & `dagster-1.4.3/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_seven/compat/pendulum.py` & `dagster-1.4.3/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/__init__.py` & `dagster-1.4.3/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/alert.py` & `dagster-1.4.3/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/backcompat.py` & `dagster-1.4.3/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/backoff.py` & `dagster-1.4.3/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/cached_method.py` & `dagster-1.4.3/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/caching_instance_queryer.py` & `dagster-1.4.3/dagster/_utils/caching_instance_queryer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from collections import defaultdict
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
+    Callable,
     Dict,
+    FrozenSet,
     Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
+    Set,
+    Tuple,
     Union,
     cast,
 )
 
 import pendulum
 
 import dagster._check as check
@@ -510,14 +514,155 @@
                 partitions_def_name
             ] = self.instance.get_dynamic_partitions(partitions_def_name)
         return self._dynamic_partitions_cache[partitions_def_name]
 
     def has_dynamic_partition(self, partitions_def_name: str, partition_key: str) -> bool:
         return partition_key in self.get_dynamic_partitions(partitions_def_name)
 
+    @cached_method
+    def asset_partitions_with_newly_updated_parents_and_new_latest_storage_id(
+        self,
+        *,
+        latest_storage_id: Optional[int],
+        target_asset_keys: FrozenSet[AssetKey],
+        target_asset_keys_and_parents: FrozenSet[AssetKey],
+        can_reconcile_fn: Callable[[AssetKeyPartitionKey], bool] = lambda _: True,
+        map_old_time_partitions: bool = True,
+    ) -> Tuple[AbstractSet[AssetKeyPartitionKey], Optional[int]]:
+        """Finds asset partitions in the given selection whose parents have been materialized since
+        latest_storage_id.
+
+        Returns:
+            - A set of asset partitions.
+            - The latest observed storage_id across all relevant assets. Can be used to avoid scanning
+                the same events the next time this function is called.
+        """
+        result_asset_partitions: Set[AssetKeyPartitionKey] = set()
+        result_latest_storage_id = latest_storage_id
+
+        for asset_key in target_asset_keys_and_parents:
+            if self.asset_graph.is_source(asset_key) and not self.asset_graph.is_observable(
+                asset_key
+            ):
+                continue
+
+            # the set of asset partitions which have been updated since the latest storage id
+            new_asset_partitions = self.get_asset_partitions_updated_after_cursor(
+                asset_key=asset_key,
+                asset_partitions=None,
+                after_cursor=latest_storage_id,
+            )
+            if not new_asset_partitions:
+                continue
+
+            partitions_def = self.asset_graph.get_partitions_def(asset_key)
+            if partitions_def is None:
+                latest_record = check.not_none(
+                    self.get_latest_materialization_or_observation_record(
+                        AssetKeyPartitionKey(asset_key)
+                    )
+                )
+                for child in self.asset_graph.get_children_partitions(
+                    dynamic_partitions_store=self,
+                    current_time=self.evaluation_time,
+                    asset_key=asset_key,
+                ):
+                    child_partitions_def = self.asset_graph.get_partitions_def(child.asset_key)
+                    if (
+                        child.asset_key in target_asset_keys
+                        # when mapping from unpartitioned assets to time partitioned assets, we ignore
+                        # historical time partitions
+                        and (
+                            map_old_time_partitions
+                            or not isinstance(child_partitions_def, TimeWindowPartitionsDefinition)
+                            or child.partition_key
+                            == child_partitions_def.get_last_partition_key(
+                                current_time=self.evaluation_time
+                            )
+                        )
+                        and not self.is_asset_planned_for_run(latest_record.run_id, child)
+                    ):
+                        result_asset_partitions.add(child)
+            else:
+                partitions_subset = partitions_def.empty_subset().with_partition_keys(
+                    [
+                        asset_partition.partition_key
+                        for asset_partition in new_asset_partitions
+                        if asset_partition.partition_key is not None
+                        and partitions_def.has_partition_key(
+                            asset_partition.partition_key,
+                            dynamic_partitions_store=self,
+                            current_time=self.evaluation_time,
+                        )
+                    ]
+                )
+                for child in self.asset_graph.get_children(asset_key):
+                    child_partitions_def = self.asset_graph.get_partitions_def(child)
+                    if child not in target_asset_keys:
+                        continue
+                    elif not child_partitions_def:
+                        result_asset_partitions.add(AssetKeyPartitionKey(child, None))
+                    else:
+                        # we are mapping from the partitions of the parent asset to the partitions of
+                        # the child asset
+                        partition_mapping = self.asset_graph.get_partition_mapping(child, asset_key)
+                        child_partitions_subset = (
+                            partition_mapping.get_downstream_partitions_for_partitions(
+                                partitions_subset,
+                                downstream_partitions_def=child_partitions_def,
+                                dynamic_partitions_store=self,
+                                current_time=self.evaluation_time,
+                            )
+                        )
+                        for child_partition in child_partitions_subset.get_partition_keys():
+                            # we need to see if the child is planned for the same run, but this is
+                            # expensive, so we try to avoid doing so in as many situations as possible
+                            child_asset_partition = AssetKeyPartitionKey(child, child_partition)
+                            if not can_reconcile_fn(child_asset_partition):
+                                continue
+                            elif (
+                                # if child has a different partitions def than the parent, then it must
+                                # have been executed in a different run, so it's a valid candidate
+                                child_partitions_def != partitions_def
+                                # if child partition key is not the same as any newly materialized
+                                # parent key, then it could not have been executed in the same run as
+                                # its parent
+                                or child_partition not in partitions_subset
+                                # if child partition is not failed or in progress, then even if it was
+                                # executed in the same run, we can filter it out later with an is_reconciled
+                                # check (cheaper than the below logic)
+                                or child_partition
+                                not in self.get_failed_or_in_progress_subset(asset_key=child)
+                            ):
+                                result_asset_partitions.add(child_asset_partition)
+                            else:
+                                # manually query to see if this asset partition was intended to be
+                                # executed in the same run as its parent
+                                latest_partition_record = check.not_none(
+                                    self.get_latest_materialization_or_observation_record(
+                                        AssetKeyPartitionKey(asset_key, child_partition),
+                                        after_cursor=latest_storage_id,
+                                    )
+                                )
+                                if not self.is_asset_planned_for_run(
+                                    latest_partition_record.run_id, child
+                                ):
+                                    result_asset_partitions.add(child_asset_partition)
+
+            asset_latest_storage_id = self.get_latest_materialization_or_observation_storage_id(
+                AssetKeyPartitionKey(asset_key)
+            )
+            if (
+                result_latest_storage_id is None
+                or (asset_latest_storage_id or 0) > result_latest_storage_id
+            ):
+                result_latest_storage_id = asset_latest_storage_id
+
+        return (result_asset_partitions, result_latest_storage_id)
+
     ####################
     # RECONCILIATION
     ####################
 
     def _asset_partitions_data_versions(
         self,
         asset_key: AssetKey,
@@ -603,82 +748,88 @@
         )
         return {
             asset_partition
             for asset_partition, version in latest_versions.items()
             if previous_versions.get(asset_partition) != version
         }
 
+    def get_updated_and_missing_parent_asset_partitions(
+        self,
+        asset_partition: AssetKeyPartitionKey,
+        parent_asset_partitions: AbstractSet[AssetKeyPartitionKey],
+    ) -> Tuple[AbstractSet[AssetKeyPartitionKey], AbstractSet[AssetKeyPartitionKey]]:
+        parent_asset_partitions_by_key: Dict[AssetKey, List[AssetKeyPartitionKey]] = defaultdict(
+            list
+        )
+        for parent in parent_asset_partitions:
+            parent_asset_partitions_by_key[parent.asset_key].append(parent)
+
+        time_or_dynamic_partitioned = isinstance(
+            self.asset_graph.get_partitions_def(asset_partition.asset_key),
+            (TimeWindowPartitionsDefinition, DynamicPartitionsDefinition),
+        )
+        updated_parents = set()
+        missing_parents = set()
+        for parent_key, asset_partitions in parent_asset_partitions_by_key.items():
+            # ignore non-observable source parents
+            if self.asset_graph.is_source(parent_key) and not self.asset_graph.is_observable(
+                parent_key
+            ):
+                continue
+
+            # find missing parents
+            for parent in asset_partitions:
+                if not self.asset_partition_has_materialization_or_observation(parent):
+                    missing_parents.add(parent)
+
+            # when mapping from time or dynamic downstream to unpartitioned upstream, only check
+            # for existence of upstream materialization, do not worry about updates
+            if time_or_dynamic_partitioned and not self.asset_graph.is_partitioned(parent_key):
+                continue
+
+            updated_parents.update(
+                self.get_asset_partitions_updated_after_cursor(
+                    asset_key=parent_key,
+                    asset_partitions=asset_partitions,
+                    after_cursor=self.get_latest_materialization_or_observation_storage_id(
+                        asset_partition
+                    ),
+                )
+            )
+        return updated_parents, missing_parents
+
     @cached_method
     def get_root_unreconciled_ancestors(
         self, *, asset_partition: AssetKeyPartitionKey
     ) -> AbstractSet[AssetKey]:
         """Return the set of root unreconciled ancestors of the given asset partition, i.e. the set
         of ancestors of this asset partition which are unreconciled for a reason other than that
         one of their ancestors is unreconciled.
         """
         # always treat source assets as reconciled
         if self.asset_graph.is_source(asset_partition.asset_key):
             return set()
         elif not self.asset_partition_has_materialization_or_observation(asset_partition):
             return {asset_partition.asset_key}
 
-        time_or_dynamic_partitioned = isinstance(
-            self.asset_graph.get_partitions_def(asset_partition.asset_key),
-            (TimeWindowPartitionsDefinition, DynamicPartitionsDefinition),
-        )
-
-        parent_asset_partitions_by_key: Dict[AssetKey, List[AssetKeyPartitionKey]] = defaultdict(
-            list
-        )
-
-        for parent in self.asset_graph.get_parents_partitions(
+        parent_asset_partitions = self.asset_graph.get_parents_partitions(
             dynamic_partitions_store=self,
             current_time=self._evaluation_time,
             asset_key=asset_partition.asset_key,
             partition_key=asset_partition.partition_key,
-        ).parent_partitions:
-            parent_asset_partitions_by_key[parent.asset_key].append(parent)
+        ).parent_partitions
 
-        root_unreconciled_ancestors = set()
-        for parent_key, parent_asset_partitions in parent_asset_partitions_by_key.items():
-            # ignore non-observable source parents
-            if self.asset_graph.is_source(parent_key) and not self.asset_graph.is_observable(
-                parent_key
-            ):
-                continue
-
-            # when mapping from time or dynamic downstream to unpartitioned upstream, only check
-            # for existence of upstream materialization, do not worry about timestamps
-            if time_or_dynamic_partitioned and not self.asset_graph.is_partitioned(parent_key):
-                if not all(
-                    self.asset_partition_has_materialization_or_observation(parent)
-                    for parent in parent_asset_partitions
-                ):
-                    root_unreconciled_ancestors.add(parent_key)
-                continue
+        updated_parents, missing_parents = self.get_updated_and_missing_parent_asset_partitions(
+            asset_partition, parent_asset_partitions
+        )
+        updated_or_missing_parent_asset_partitions = updated_parents | missing_parents
 
-            updated_parent_asset_partitions = self.get_asset_partitions_updated_after_cursor(
-                asset_key=parent_key,
-                asset_partitions=parent_asset_partitions,
-                after_cursor=self.get_latest_materialization_or_observation_storage_id(
-                    asset_partition
-                ),
-            )
-            if updated_parent_asset_partitions:
-                # this asset has updated parents, so it must be materialized before it is reconciled
-                root_unreconciled_ancestors.add(asset_partition.asset_key)
-            # recurse over parents
-            for parent in set(parent_asset_partitions) - updated_parent_asset_partitions:
-                root_unreconciled_ancestors.update(
-                    self.get_root_unreconciled_ancestors(asset_partition=parent)
-                )
+        root_unreconciled_ancestors = (
+            {asset_partition.asset_key} if updated_or_missing_parent_asset_partitions else set()
+        )
 
+        # recurse over parents
+        for parent in set(parent_asset_partitions) - updated_or_missing_parent_asset_partitions:
+            root_unreconciled_ancestors.update(
+                self.get_root_unreconciled_ancestors(asset_partition=parent)
+            )
         return root_unreconciled_ancestors
-
-    def is_reconciled(self, asset_partition: AssetKeyPartitionKey) -> bool:
-        """Returns a boolean representing if the given `asset_partition` is currently reconciled.
-        An asset (partition) is considered unreconciled if any of:
-        - It has never been materialized
-        - One of its parents has been updated more recently than it has
-        - One of its parents is unreconciled.
-        """
-        return len(self.get_root_unreconciled_ancestors(asset_partition=asset_partition)) == 0
```

### Comparing `dagster-1.4.2/dagster/_utils/concurrency.py` & `dagster-1.4.3/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/dagster_type.py` & `dagster-1.4.3/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/env.py` & `dagster-1.4.3/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/error.py` & `dagster-1.4.3/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/external.py` & `dagster-1.4.3/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/forked_pdb.py` & `dagster-1.4.3/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/hosted_user_process.py` & `dagster-1.4.3/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/indenting_printer.py` & `dagster-1.4.3/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/interrupts.py` & `dagster-1.4.3/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/log.py` & `dagster-1.4.3/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/merger.py` & `dagster-1.4.3/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/net.py` & `dagster-1.4.3/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/schedules.py` & `dagster-1.4.3/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/tags.py` & `dagster-1.4.3/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/temp_file.py` & `dagster-1.4.3/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/test/__init__.py` & `dagster-1.4.3/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/test/mysql_instance.py` & `dagster-1.4.3/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/test/postgres_instance.py` & `dagster-1.4.3/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/test/schedule_storage.py` & `dagster-1.4.3/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/timing.py` & `dagster-1.4.3/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/typing_api.py` & `dagster-1.4.3/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster/_utils/yaml_utils.py` & `dagster-1.4.3/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.4.2/dagster.egg-info/PKG-INFO` & `dagster-1.4.3/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.4.2
+Version: 1.4.3
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.4.2/dagster.egg-info/SOURCES.txt` & `dagster-1.4.3/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -81,26 +81,28 @@
 dagster/_core/telemetry_upload.py
 dagster/_core/test_utils.py
 dagster/_core/utility_ops.py
 dagster/_core/utils.py
 dagster/_core/container_context/__init__.py
 dagster/_core/container_context/config.py
 dagster/_core/definitions/__init__.py
+dagster/_core/definitions/asset_daemon_cursor.py
 dagster/_core/definitions/asset_graph.py
 dagster/_core/definitions/asset_graph_subset.py
 dagster/_core/definitions/asset_in.py
 dagster/_core/definitions/asset_layer.py
 dagster/_core/definitions/asset_out.py
 dagster/_core/definitions/asset_reconciliation_sensor.py
 dagster/_core/definitions/asset_selection.py
 dagster/_core/definitions/asset_sensor_definition.py
 dagster/_core/definitions/assets.py
 dagster/_core/definitions/assets_job.py
 dagster/_core/definitions/auto_materialize_condition.py
 dagster/_core/definitions/auto_materialize_policy.py
+dagster/_core/definitions/backfill_policy.py
 dagster/_core/definitions/cacheable_assets.py
 dagster/_core/definitions/composition.py
 dagster/_core/definitions/config.py
 dagster/_core/definitions/configurable.py
 dagster/_core/definitions/data_time.py
 dagster/_core/definitions/data_version.py
 dagster/_core/definitions/definition_config_schema.py
```

### Comparing `dagster-1.4.2/dagster.egg-info/requires.txt` & `dagster-1.4.3/dagster.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 pytest-cov==2.10.1
 pytest-dependency==0.5.1
 pytest-mock==3.3.1
 pytest-rerunfailures==10.0
 pytest-runner==5.2
 pytest-xdist==2.1.0
 pytest==7.0.1
-responses
+responses<=0.23.1
 syrupy<4
 tox==3.25.0
 yamllint
 
 [test:python_version >= "3.8"]
 buildkite-test-collector
 morefs[asynclocal]
```

### Comparing `dagster-1.4.2/setup.py` & `dagster-1.4.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             "pytest-cov==2.10.1",
             "pytest-dependency==0.5.1",
             "pytest-mock==3.3.1",
             "pytest-rerunfailures==10.0",
             "pytest-runner==5.2",
             "pytest-xdist==2.1.0",
             "pytest==7.0.1",  # last version supporting python 3.6
-            "responses",
+            "responses<=0.23.1",  # https://github.com/getsentry/responses/issues/654
             "syrupy<4",  # 3.7 compatible,
             "tox==3.25.0",
             "yamllint",
             "morefs[asynclocal]; python_version>='3.8'",
         ],
         "black": [
             "black[jupyter]==22.12.0",
```

