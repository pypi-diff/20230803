# Comparing `tmp/datapackage-pipelines-2.2.6.tar.gz` & `tmp/datapackage-pipelines-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datapackage-pipelines-2.2.6.tar", last modified: Fri Apr 16 17:13:48 2021, max compression
+gzip compressed data, was "dist/datapackage-pipelines-2.2.9.tar", last modified: Fri Jun 25 13:33:57 2021, max compression
```

## Comparing `datapackage-pipelines-2.2.6.tar` & `datapackage-pipelines-2.2.9.tar`

### file list

```diff
@@ -1,137 +1,158 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2911 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2228 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)    87581 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    72855 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/VERSION
--rw-rw-r--   0 travis    (2000) travis    (2000)      253 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      114 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/celery_tasks/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/celery_tasks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1520 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/celery_tasks/celery_app.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1313 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/celery_tasks/celery_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6341 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/celery_tasks/celery_tasks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2759 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/celery_tasks/dependency_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5019 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/cli.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/generators/
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/generators/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      942 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/generators/generator_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/generators/schedules.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      217 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/generators/utilities.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      439 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/add_computed_field.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      426 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/add_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      863 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/add_resource.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/cache_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      707 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/concatenate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      383 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/deduplicate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      522 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/delete_fields.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12186 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/dumper_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/file_formats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/to_path.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      419 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/to_sql.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      772 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/to_zip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      668 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump_to_path.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      561 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump_to_sql.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      427 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump_to_zip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      620 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/duplicate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/filter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      426 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/find_replace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      451 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/flow.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/internal/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/internal/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      646 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/internal/sink.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      935 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/join.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1152 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/load.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      579 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/load_metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3655 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/load_resource.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      316 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/printer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      826 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/set_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      529 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/sort.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8678 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/stream_remote_resources.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      506 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/unpivot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      341 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/update_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      449 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/lib/update_resource.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/manager/
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/manager/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      191 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/manager/logging_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10383 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/manager/runner.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/manager/runners/
--rw-rw-r--   0 travis    (2000) travis    (2000)       86 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/manager/runners/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      218 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/manager/runners/base_runner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1127 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/manager/runners/local_python.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      875 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/manager/runners/runner_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11556 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/manager/tasks.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      200 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/errors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/hashers/
--rw-rw-r--   0 travis    (2000) travis    (2000)      126 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/hashers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3072 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/hashers/dependency_resolver.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1473 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/hashers/hash_calculator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/parsers/
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/parsers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/parsers/base_parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      776 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/parsers/basic_pipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3089 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/parsers/source_spec_pipeline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3770 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/resolver.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/schemas/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/schemas/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/schemas/pipeline-spec.schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/schemas/validator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4535 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/specs/specs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/status/
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/status/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1879 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/status/backend_filesystem.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2021 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/status/backend_redis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2738 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/status/backend_sqlite.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      805 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/status/hook_sender.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3812 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/status/pipeline_execution.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7313 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/status/pipeline_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1483 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/status/status_manager.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12830 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/dirtools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/execution_id.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4595 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/extended_json.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1442 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/flow_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      983 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/lazy_dict.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7128 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/lib_test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      816 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/resources.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/stat_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1442 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/tabulator_txt_parser.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/web/
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/web/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11760 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/web/server.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/web/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15588 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/web/templates/dashboard.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/wrapper/
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/wrapper/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4028 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/wrapper/input_processor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7185 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/datapackage_pipelines/wrapper/wrapper.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    87581 2021-04-16 17:13:47.000000 datapackage-pipelines-2.2.6/datapackage_pipelines.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4705 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/datapackage_pipelines.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-16 17:13:47.000000 datapackage-pipelines-2.2.6/datapackage_pipelines.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2021-04-16 17:13:47.000000 datapackage-pipelines-2.2.6/datapackage_pipelines.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-16 17:13:47.000000 datapackage-pipelines-2.2.6/datapackage_pipelines.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      355 2021-04-16 17:13:47.000000 datapackage-pipelines-2.2.6/datapackage_pipelines.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-04-16 17:13:47.000000 datapackage-pipelines-2.2.6/datapackage_pipelines.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2290 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/tests/data/datapackage.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1052 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/tests/data/datapackage2.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/tests/data/datapackage3.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/tests/data/sample.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-16 17:13:48.000000 datapackage-pipelines-2.2.6/tests/stdlib/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/tests/stdlib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1605 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/tests/stdlib/test_stdlib.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      612 2021-04-16 17:07:13.000000 datapackage-pipelines-2.2.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1146 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1081 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (116)      208 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2416 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)    87581 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    72855 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (116)        5 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/VERSION
+-rw-r--r--   0 runner    (1001) docker     (116)      253 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      114 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/app.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/celery_tasks/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/celery_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1520 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/celery_tasks/celery_app.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1313 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/celery_tasks/celery_common.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6341 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/celery_tasks/celery_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2759 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/celery_tasks/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5019 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/generators/
+-rw-r--r--   0 runner    (1001) docker     (116)      132 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      942 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/generators/generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)      171 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/generators/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (116)      217 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/generators/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      439 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/add_computed_field.py
+-rw-r--r--   0 runner    (1001) docker     (116)      426 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (116)      863 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/add_resource.py
+-rw-r--r--   0 runner    (1001) docker     (116)      205 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/cache_loader.py
+-rw-r--r--   0 runner    (1001) docker     (116)      707 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      383 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      522 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/delete_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12186 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/dumper_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4472 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/file_formats.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1062 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/to_path.py
+-rw-r--r--   0 runner    (1001) docker     (116)      419 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/to_sql.py
+-rw-r--r--   0 runner    (1001) docker     (116)      772 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/to_zip.py
+-rw-r--r--   0 runner    (1001) docker     (116)      668 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump_to_path.py
+-rw-r--r--   0 runner    (1001) docker     (116)      561 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump_to_sql.py
+-rw-r--r--   0 runner    (1001) docker     (116)      427 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump_to_zip.py
+-rw-r--r--   0 runner    (1001) docker     (116)      620 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      478 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/filter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      426 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/find_replace.py
+-rw-r--r--   0 runner    (1001) docker     (116)      451 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/internal/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      646 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/internal/sink.py
+-rw-r--r--   0 runner    (1001) docker     (116)      935 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/join.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1152 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/load.py
+-rw-r--r--   0 runner    (1001) docker     (116)      579 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/load_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3655 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/load_resource.py
+-rw-r--r--   0 runner    (1001) docker     (116)      316 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/printer.py
+-rw-r--r--   0 runner    (1001) docker     (116)      826 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/set_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)      529 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/sort.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8777 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/stream_remote_resources.py
+-rw-r--r--   0 runner    (1001) docker     (116)      506 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/unpivot.py
+-rw-r--r--   0 runner    (1001) docker     (116)      341 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/update_package.py
+-rw-r--r--   0 runner    (1001) docker     (116)      449 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/lib/update_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/manager/
+-rw-r--r--   0 runner    (1001) docker     (116)      113 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      191 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/manager/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10383 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/manager/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/manager/runners/
+-rw-r--r--   0 runner    (1001) docker     (116)       86 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/manager/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      218 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/manager/runners/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1127 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/manager/runners/local_python.py
+-rw-r--r--   0 runner    (1001) docker     (116)      875 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/manager/runners/runner_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11556 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/manager/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/
+-rw-r--r--   0 runner    (1001) docker     (116)       99 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      200 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/hashers/
+-rw-r--r--   0 runner    (1001) docker     (116)      126 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/hashers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3072 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/hashers/dependency_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1473 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/hashers/hash_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/parsers/
+-rw-r--r--   0 runner    (1001) docker     (116)      107 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1721 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/parsers/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (116)      776 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/parsers/basic_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3089 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/parsers/source_spec_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3770 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/schemas/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1363 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/schemas/pipeline-spec.schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)      595 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/schemas/validator.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4535 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/specs/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/status/
+-rw-r--r--   0 runner    (1001) docker     (116)       76 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1879 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/status/backend_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2021 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/status/backend_redis.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2738 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/status/backend_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (116)      805 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/status/hook_sender.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3812 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/status/pipeline_execution.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7313 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/status/pipeline_status.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1483 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/status/status_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12830 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/dirtools.py
+-rw-r--r--   0 runner    (1001) docker     (116)       67 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/execution_id.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4595 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/extended_json.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1442 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/flow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      983 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/lazy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7128 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/lib_test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)      816 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/resources.py
+-rw-r--r--   0 runner    (1001) docker     (116)      246 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/stat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1442 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/tabulator_txt_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/web/
+-rw-r--r--   0 runner    (1001) docker     (116)       24 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11760 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/web/server.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/web/templates/
+-rw-r--r--   0 runner    (1001) docker     (116)    15588 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/web/templates/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (116)       99 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4028 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/wrapper/input_processor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7185 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/datapackage_pipelines/wrapper/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    87581 2021-06-25 13:33:56.000000 datapackage-pipelines-2.2.9/datapackage_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5152 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/datapackage_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-06-25 13:33:56.000000 datapackage-pipelines-2.2.9/datapackage_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       55 2021-06-25 13:33:56.000000 datapackage-pipelines-2.2.9/datapackage_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-06-25 13:24:36.000000 datapackage-pipelines-2.2.9/datapackage_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      355 2021-06-25 13:33:56.000000 datapackage-pipelines-2.2.9/datapackage_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       28 2021-06-25 13:33:56.000000 datapackage-pipelines-2.2.9/datapackage_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       67 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2290 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/cli/dpp_tests_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      219 2021-06-25 13:31:35.000000 datapackage-pipelines-2.2.9/tests/cli/dpp_tests_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-06-25 13:31:35.000000 datapackage-pipelines-2.2.9/tests/cli/dpp_tests_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2021-06-25 13:31:35.000000 datapackage-pipelines-2.2.9/tests/cli/dpp_tests_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/cli/test_flow_data/
+-rw-------   0 runner    (1001) docker     (116)     1259 2021-06-25 13:31:48.000000 datapackage-pipelines-2.2.9/tests/cli/test_flow_data/datapackage.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (116)      490 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/tests/data/datapackage.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1052 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/tests/data/datapackage2.json
+-rw-r--r--   0 runner    (1001) docker     (116)      495 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/tests/data/datapackage3.json
+-rw-r--r--   0 runner    (1001) docker     (116)      159 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/tests/data/sample.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/env/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/env/dummy/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/env/dummy/code-test-output/
+-rw-------   0 runner    (1001) docker     (116)     2290 2021-06-25 13:30:26.000000 datapackage-pipelines-2.2.9/tests/env/dummy/code-test-output/datapackage.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/env/dummy/hooks-outputs/
+-rw-------   0 runner    (1001) docker     (116)     2039 2021-06-25 13:30:17.000000 datapackage-pipelines-2.2.9/tests/env/dummy/hooks-outputs/datapackage.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/env/dummy/nulls-test/
+-rw-------   0 runner    (1001) docker     (116)     3726 2021-06-25 13:30:07.000000 datapackage-pipelines-2.2.9/tests/env/dummy/nulls-test/datapackage.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/env/dummy/type-tests-output/
+-rw-------   0 runner    (1001) docker     (116)     2171 2021-06-25 13:31:23.000000 datapackage-pipelines-2.2.9/tests/env/dummy/type-tests-output/datapackage.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/env/dummy/type-tests-output2/
+-rw-------   0 runner    (1001) docker     (116)     2299 2021-06-25 13:31:25.000000 datapackage-pipelines-2.2.9/tests/env/dummy/type-tests-output2/datapackage.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-06-25 13:33:57.000000 datapackage-pipelines-2.2.9/tests/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/tests/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1605 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/tests/stdlib/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (116)      612 2021-06-25 13:24:05.000000 datapackage-pipelines-2.2.9/tox.ini
```

### Comparing `datapackage-pipelines-2.2.6/LICENSE.md` & `datapackage-pipelines-2.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/Makefile` & `datapackage-pipelines-2.2.9/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 	tests/cli/test_exclude_dirnames.sh &&\
 	tests/cli/test_flow.sh
 
 version:
 	@echo $(VERSION)
 
 build:
+	docker login -u "${DOCKER_USERNAME}" -p "${DOCKER_PASSWORD}"
 	docker pull frictionlessdata/datapackage-pipelines:latest &&\
 	docker build -t frictionlessdata/datapackage-pipelines:latest --cache-from frictionlessdata/datapackage-pipelines . &&\
 	docker build -t frictionlessdata/datapackage-pipelines:latest-alpine --cache-from frictionlessdata/datapackage-pipelines . &&\
 	docker build -t frictionlessdata/datapackage-pipelines:${VERSION} --cache-from frictionlessdata/datapackage-pipelines . &&\
 	docker build -t frictionlessdata/datapackage-pipelines:${VERSION}-alpine --cache-from frictionlessdata/datapackage-pipelines . &&\
 	docker pull frictionlessdata/datapackage-pipelines:latest-slim &&\
 	docker build -t frictionlessdata/datapackage-pipelines:latest-slim -f Dockerfile.slim --cache-from frictionlessdata/datapackage-pipelines:latest-slim . &&\
@@ -52,8 +53,14 @@
 	docker push frictionlessdata/datapackage-pipelines:latest-alpine &&\
 	docker push frictionlessdata/datapackage-pipelines:latest-slim
 
 deploy-tags:
 	docker login -u "${DOCKER_USERNAME}" -p "${DOCKER_PASSWORD}" &&\
 	docker push frictionlessdata/datapackage-pipelines:${VERSION} &&\
 	docker push frictionlessdata/datapackage-pipelines:${VERSION}-alpine &&\
-	docker push frictionlessdata/datapackage-pipelines:${VERSION}-slim
+	docker push frictionlessdata/datapackage-pipelines:${VERSION}-slim
+
+deploy-pip:
+	rm -rf dist/ || true
+	pip install wheel twine
+	python setup.py sdist bdist_wheel
+	python -m twine upload dist/*
```

### Comparing `datapackage-pipelines-2.2.6/PKG-INFO` & `datapackage-pipelines-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapackage-pipelines
-Version: 2.2.6
+Version: 2.2.9
 Summary: {{ DESCRIPTION }}
 Home-page: https://github.com/frictionlessdata/datapackage-pipelines
 Author: Open Knowledge Foundation
 Author-email: info@okfn.org
 License: MIT
 Description: # Datapackage Pipelines
```

### Comparing `datapackage-pipelines-2.2.6/README.md` & `datapackage-pipelines-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/celery_tasks/celery_app.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/celery_tasks/celery_app.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/celery_tasks/celery_common.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/celery_tasks/celery_common.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/celery_tasks/celery_tasks.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/celery_tasks/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/celery_tasks/dependency_manager.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/celery_tasks/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/cli.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/cli.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/generators/generator_base.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/generators/generator_base.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/add_resource.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/add_resource.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/concatenate.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/concatenate.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/delete_fields.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/delete_fields.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/dumper_base.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/dumper_base.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/file_formats.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/file_formats.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/to_path.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/to_path.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump/to_zip.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump/to_zip.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump_to_path.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump_to_path.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/dump_to_sql.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/dump_to_sql.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/duplicate.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/duplicate.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/internal/sink.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/internal/sink.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/join.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/join.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/load.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/load.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/load_metadata.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/load_metadata.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/load_resource.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/load_resource.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/set_types.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/set_types.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/sort.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/sort.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/lib/stream_remote_resources.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/lib/stream_remote_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import logging
 import time
-from datetime import date
+from datetime import date, time as datetime_time
 import itertools
 from decimal import Decimal
 import requests
 
 import tabulator
 
 from tableschema import Schema
@@ -24,14 +24,16 @@
         return value
     elif value is None:
         return ''
     elif isinstance(value, (int, float, bool, Decimal)):
         return str(value)
     elif isinstance(value, date):
         return value.isoformat()
+    elif isinstance(value, datetime_time):
+        return value.isoformat()
     elif isinstance(value, (list, dict)):
         return json.dumps(value)
 
     assert False, "Internal error - don't know how to handle %r of type %r" % (value, type(value))
 
 
 def _reader(opener, _url, max_row=-1):
```

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/manager/runner.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/manager/runner.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/manager/runners/local_python.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/manager/runners/local_python.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/manager/runners/runner_config.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/manager/runners/runner_config.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/manager/tasks.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/manager/tasks.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/specs/hashers/dependency_resolver.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/specs/hashers/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/specs/hashers/hash_calculator.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/specs/hashers/hash_calculator.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/specs/parsers/base_parser.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/specs/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/specs/parsers/basic_pipeline.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/specs/parsers/basic_pipeline.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/specs/parsers/source_spec_pipeline.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/specs/parsers/source_spec_pipeline.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/specs/resolver.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/specs/resolver.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/specs/schemas/pipeline-spec.schema.json` & `datapackage-pipelines-2.2.9/datapackage_pipelines/specs/schemas/pipeline-spec.schema.json`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/specs/schemas/validator.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/specs/schemas/validator.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/specs/specs.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/specs/specs.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/status/backend_filesystem.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/status/backend_filesystem.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/status/backend_redis.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/status/backend_redis.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/status/backend_sqlite.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/status/backend_sqlite.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/status/hook_sender.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/status/hook_sender.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/status/pipeline_execution.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/status/pipeline_execution.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/status/pipeline_status.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/status/pipeline_status.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/status/status_manager.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/status/status_manager.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/dirtools.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/dirtools.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/extended_json.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/extended_json.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/flow_utils.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/flow_utils.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/lazy_dict.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/lib_test_helpers.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/lib_test_helpers.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/resources.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/resources.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/utilities/tabulator_txt_parser.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/utilities/tabulator_txt_parser.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/web/server.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/web/server.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/web/templates/dashboard.html` & `datapackage-pipelines-2.2.9/datapackage_pipelines/web/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/wrapper/input_processor.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/wrapper/input_processor.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines/wrapper/wrapper.py` & `datapackage-pipelines-2.2.9/datapackage_pipelines/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines.egg-info/PKG-INFO` & `datapackage-pipelines-2.2.9/datapackage_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapackage-pipelines
-Version: 2.2.6
+Version: 2.2.9
 Summary: {{ DESCRIPTION }}
 Home-page: https://github.com/frictionlessdata/datapackage-pipelines
 Author: Open Knowledge Foundation
 Author-email: info@okfn.org
 License: MIT
 Description: # Datapackage Pipelines
```

### Comparing `datapackage-pipelines-2.2.6/datapackage_pipelines.egg-info/SOURCES.txt` & `datapackage-pipelines-2.2.9/datapackage_pipelines.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-.travis.yml
 LICENSE.md
 MANIFEST.in
 Makefile
 README.md
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/main.yml
 datapackage_pipelines/VERSION
 datapackage_pipelines/__init__.py
 datapackage_pipelines/app.py
 datapackage_pipelines/cli.py
 datapackage_pipelines.egg-info/PKG-INFO
 datapackage_pipelines.egg-info/SOURCES.txt
 datapackage_pipelines.egg-info/dependency_links.txt
@@ -102,13 +102,22 @@
 datapackage_pipelines/utilities/tabulator_txt_parser.py
 datapackage_pipelines/web/__init__.py
 datapackage_pipelines/web/server.py
 datapackage_pipelines/web/templates/dashboard.html
 datapackage_pipelines/wrapper/__init__.py
 datapackage_pipelines/wrapper/input_processor.py
 datapackage_pipelines/wrapper/wrapper.py
+tests/cli/dpp_tests_cli.egg-info/SOURCES.txt
+tests/cli/dpp_tests_cli.egg-info/dependency_links.txt
+tests/cli/dpp_tests_cli.egg-info/top_level.txt
+tests/cli/test_flow_data/datapackage.json
 tests/data/datapackage.json
 tests/data/datapackage2.json
 tests/data/datapackage3.json
 tests/data/sample.txt
+tests/env/dummy/code-test-output/datapackage.json
+tests/env/dummy/hooks-outputs/datapackage.json
+tests/env/dummy/nulls-test/datapackage.json
+tests/env/dummy/type-tests-output/datapackage.json
+tests/env/dummy/type-tests-output2/datapackage.json
 tests/stdlib/__init__.py
 tests/stdlib/test_stdlib.py
```

### Comparing `datapackage-pipelines-2.2.6/setup.py` & `datapackage-pipelines-2.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/tests/data/datapackage2.json` & `datapackage-pipelines-2.2.9/tests/data/datapackage2.json`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/tests/stdlib/test_stdlib.py` & `datapackage-pipelines-2.2.9/tests/stdlib/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `datapackage-pipelines-2.2.6/tox.ini` & `datapackage-pipelines-2.2.9/tox.ini`

 * *Files identical despite different names*

